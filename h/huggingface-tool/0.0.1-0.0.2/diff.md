# Comparing `tmp/huggingface_tool-0.0.1.tar.gz` & `tmp/huggingface_tool-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huggingface_tool-0.0.1.tar", last modified: Wed Jul  5 07:55:02 2023, max compression
+gzip compressed data, was "huggingface_tool-0.0.2.tar", last modified: Wed Jul 12 05:31:38 2023, max compression
```

## Comparing `huggingface_tool-0.0.1.tar` & `huggingface_tool-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-05 07:55:02.976752 huggingface_tool-0.0.1/
--rw-r--r--   0 4paradigm   (501) staff       (20)    11357 2023-07-05 05:15:55.000000 huggingface_tool-0.0.1/LICENSE
--rw-r--r--   0 4paradigm   (501) staff       (20)     1979 2023-07-05 07:55:02.976600 huggingface_tool-0.0.1/PKG-INFO
--rw-r--r--   0 4paradigm   (501) staff       (20)      882 2023-07-05 07:53:10.000000 huggingface_tool-0.0.1/README.md
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-05 07:55:02.967675 huggingface_tool-0.0.1/huggingface_tool/
--rw-r--r--   0 4paradigm   (501) staff       (20)     1113 2023-07-05 05:19:24.000000 huggingface_tool-0.0.1/huggingface_tool/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-05 07:55:02.970856 huggingface_tool-0.0.1/huggingface_tool/cli/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-06-26 08:37:33.000000 huggingface_tool-0.0.1/huggingface_tool/cli/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3131 2023-07-05 07:47:39.000000 huggingface_tool-0.0.1/huggingface_tool/cli/cli.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-05 07:55:02.973395 huggingface_tool-0.0.1/huggingface_tool/savers/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-07-05 05:24:38.000000 huggingface_tool-0.0.1/huggingface_tool/savers/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1273 2023-07-05 07:43:36.000000 huggingface_tool-0.0.1/huggingface_tool/savers/base_saver.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1025 2023-07-05 07:49:11.000000 huggingface_tool-0.0.1/huggingface_tool/savers/dataset_saver.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      918 2023-07-05 07:40:41.000000 huggingface_tool-0.0.1/huggingface_tool/savers/diffusion_model_saver.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      957 2023-07-05 07:46:38.000000 huggingface_tool-0.0.1/huggingface_tool/savers/model_saver.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      848 2023-07-05 07:38:00.000000 huggingface_tool-0.0.1/huggingface_tool/savers/tokenizer_saver.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-05 07:55:02.976166 huggingface_tool-0.0.1/huggingface_tool/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-06-26 08:58:04.000000 huggingface_tool-0.0.1/huggingface_tool/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1290 2023-07-05 05:32:09.000000 huggingface_tool-0.0.1/huggingface_tool/utils/logger.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1370 2023-07-05 05:21:26.000000 huggingface_tool-0.0.1/huggingface_tool/utils/util.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-05 07:55:02.970410 huggingface_tool-0.0.1/huggingface_tool.egg-info/
--rw-r--r--   0 4paradigm   (501) staff       (20)     1979 2023-07-05 07:55:02.000000 huggingface_tool-0.0.1/huggingface_tool.egg-info/PKG-INFO
--rw-r--r--   0 4paradigm   (501) staff       (20)      703 2023-07-05 07:55:02.000000 huggingface_tool-0.0.1/huggingface_tool.egg-info/SOURCES.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)        1 2023-07-05 07:55:02.000000 huggingface_tool-0.0.1/huggingface_tool.egg-info/dependency_links.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       55 2023-07-05 07:55:02.000000 huggingface_tool-0.0.1/huggingface_tool.egg-info/entry_points.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)      197 2023-07-05 07:55:02.000000 huggingface_tool-0.0.1/huggingface_tool.egg-info/requires.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       17 2023-07-05 07:55:02.000000 huggingface_tool-0.0.1/huggingface_tool.egg-info/top_level.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       38 2023-07-05 07:55:02.977899 huggingface_tool-0.0.1/setup.cfg
--rw-r--r--   0 4paradigm   (501) staff       (20)     2951 2023-07-05 06:23:52.000000 huggingface_tool-0.0.1/setup.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-12 05:31:38.321753 huggingface_tool-0.0.2/
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11357 2023-07-05 08:02:03.000000 huggingface_tool-0.0.2/LICENSE
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2500 2023-07-12 05:31:38.321630 huggingface_tool-0.0.2/PKG-INFO
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1403 2023-07-12 05:28:23.000000 huggingface_tool-0.0.2/README.md
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-12 05:31:38.318002 huggingface_tool-0.0.2/huggingface_tool/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1113 2023-07-12 05:31:28.000000 huggingface_tool-0.0.2/huggingface_tool/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-12 05:31:38.319132 huggingface_tool-0.0.2/huggingface_tool/cli/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-06-26 08:37:33.000000 huggingface_tool-0.0.2/huggingface_tool/cli/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3534 2023-07-12 05:25:10.000000 huggingface_tool-0.0.2/huggingface_tool/cli/cli.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-12 05:31:38.320757 huggingface_tool-0.0.2/huggingface_tool/savers/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-07-05 05:24:38.000000 huggingface_tool-0.0.2/huggingface_tool/savers/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      961 2023-07-12 05:17:52.000000 huggingface_tool-0.0.2/huggingface_tool/savers/base_model_saver.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1277 2023-07-12 05:19:30.000000 huggingface_tool-0.0.2/huggingface_tool/savers/base_saver.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1025 2023-07-05 07:49:11.000000 huggingface_tool-0.0.2/huggingface_tool/savers/dataset_saver.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      931 2023-07-12 05:17:52.000000 huggingface_tool-0.0.2/huggingface_tool/savers/diffusion_model_saver.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1779 2023-07-12 05:23:51.000000 huggingface_tool-0.0.2/huggingface_tool/savers/model_saver.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      861 2023-07-12 05:18:18.000000 huggingface_tool-0.0.2/huggingface_tool/savers/tokenizer_saver.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-12 05:31:38.321351 huggingface_tool-0.0.2/huggingface_tool/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-06-26 08:58:04.000000 huggingface_tool-0.0.2/huggingface_tool/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1290 2023-07-05 05:32:09.000000 huggingface_tool-0.0.2/huggingface_tool/utils/logger.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1370 2023-07-05 05:21:26.000000 huggingface_tool-0.0.2/huggingface_tool/utils/util.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-12 05:31:38.318774 huggingface_tool-0.0.2/huggingface_tool.egg-info/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2500 2023-07-12 05:31:38.000000 huggingface_tool-0.0.2/huggingface_tool.egg-info/PKG-INFO
+-rw-r--r--   0 4paradigm   (501) staff       (20)      747 2023-07-12 05:31:38.000000 huggingface_tool-0.0.2/huggingface_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)        1 2023-07-12 05:31:38.000000 huggingface_tool-0.0.2/huggingface_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       55 2023-07-12 05:31:38.000000 huggingface_tool-0.0.2/huggingface_tool.egg-info/entry_points.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)      197 2023-07-12 05:31:38.000000 huggingface_tool-0.0.2/huggingface_tool.egg-info/requires.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       17 2023-07-12 05:31:38.000000 huggingface_tool-0.0.2/huggingface_tool.egg-info/top_level.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       38 2023-07-12 05:31:38.321793 huggingface_tool-0.0.2/setup.cfg
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2951 2023-07-05 06:23:52.000000 huggingface_tool-0.0.2/setup.py
```

### Comparing `huggingface_tool-0.0.1/LICENSE` & `huggingface_tool-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `huggingface_tool-0.0.1/PKG-INFO` & `huggingface_tool-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huggingface_tool
-Version: 0.0.1
+Version: 0.0.2
 Summary: Toolkit for managing huggingface models and datasets
 Home-page: https://github.com/OpenRL-Lab/huggingface_tool
 Author: openrl contributors
 Author-email: huangsy1314@163.com
 Project-URL: Code, https://github.com/OpenRL-Lab/huggingface_tool
 Project-URL: Documentation, https://huggingface_tool.readthedocs.io/
 Keywords: huggingface toolkit
@@ -22,23 +22,29 @@
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
 
 # huggingface_tool
 
+[![PyPI](https://img.shields.io/pypi/v/huggingface-tool)](https://pypi.org/project/huggingface-tool/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/huggingface-tool)
+[![Hits-of-Code](https://hitsofcode.com/github/OpenRL-Lab/huggingface_tool?branch=main)](https://hitsofcode.com/github/OpenRL-Lab/huggingface_tool/view?branch=main)
+
 Tools for loading, upload, managing huggingface models and datasets
 
 
 ## Installation
 
-`pip install huggingface_tool`
+`pip install huggingface-tool`
 
 ## Usage
 
+- Download and save transformer models with: `htool save-model <model_class> <model_name> <save_dir>`
+  - For example: `htool save-model AutoModelForCausalLM gpt2 ./gpt2`
 - Download and save tokenizer with: `htool save-tk <tokenizer_name> <save_dir>`
   - For example: `htool save-tk gpt2 ./gpt2 `
 - Download and save dataset with: `htool save-data <dataset_name> <save_dir>`
   - For example: `htool save-data daily_dialog ./daily_dialog`
 - Download and save diffusion models with: `htool save-dm <model_name> <save_dir>`
   - For example: `htool save-dm google/ddpm-cat-256 ./google/`
```

### Comparing `huggingface_tool-0.0.1/huggingface_tool/__init__.py` & `huggingface_tool-0.0.2/huggingface_tool/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 
 
 __TITLE__ = "huggingface_tool"
-__VERSION__ = "v0.0.1"
+__VERSION__ = "v0.0.2"
 __DESCRIPTION__ = "Toolkit for managing huggingface models and datasets"
 __AUTHOR__ = "OpenRL Contributors"
 __EMAIL__ = "huangshiyu@4paradigm.com"
 __version__ = __VERSION__
 
 import platform
```

### Comparing `huggingface_tool-0.0.1/huggingface_tool/cli/__init__.py` & `huggingface_tool-0.0.2/huggingface_tool/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `huggingface_tool-0.0.1/huggingface_tool/cli/cli.py` & `huggingface_tool-0.0.2/huggingface_tool/cli/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,34 +20,35 @@
 import click
 from click.core import Context, Option
 from termcolor import colored
 
 from huggingface_tool import __AUTHOR__, __EMAIL__, __TITLE__, __VERSION__
 from huggingface_tool.utils.util import get_system_info
 
+
 def red(text: str):
     return colored(text, "red")
 
 
 def print_version(
-    ctx: Context,
-    param: Option,
-    value: bool,
+        ctx: Context,
+        param: Option,
+        value: bool,
 ) -> None:
     if not value or ctx.resilient_parsing:
         return
     click.secho(f"{__TITLE__.upper()} version: {red(__VERSION__)}")
     click.secho(f"Developed by {__AUTHOR__}, Email: {red(__EMAIL__)}")
     ctx.exit()
 
 
 def print_system_info(
-    ctx: Context,
-    param: Option,
-    value: bool,
+        ctx: Context,
+        param: Option,
+        value: bool,
 ) -> None:
     if not value or ctx.resilient_parsing:
         return
     info_dict = get_system_info()
     for key, value in info_dict.items():
         click.secho(f"- {key}: {red(value)}")
     ctx.exit()
@@ -89,28 +90,43 @@
     from huggingface_tool.savers.diffusion_model_saver import DiffusionModelSaver
     saver = DiffusionModelSaver(model_name)
     if saver.load():
         saver.save(save_dir)
     else:
         saver.logger.info("Model not found")
 
+
 @cli.command()
 @click.argument("tokenizer_name")
 @click.argument("save_dir")
 def save_tk(tokenizer_name, save_dir):
     from huggingface_tool.savers.tokenizer_saver import TokenizerSaver
     saver = TokenizerSaver(tokenizer_name)
     if saver.load():
         saver.save(save_dir)
     else:
         saver.logger.info("Tokenizer not found")
 
+
 @cli.command()
 @click.argument("dataset_name")
 @click.argument("save_dir")
 def save_data(dataset_name, save_dir):
     from huggingface_tool.savers.dataset_saver import DatasetSaver
     saver = DatasetSaver(dataset_name)
     if saver.load():
         saver.save(save_dir)
     else:
-        saver.logger.info("Dataset not found")
+        saver.logger.info("Dataset not found")
+
+
+@cli.command()
+@click.argument("model_class")
+@click.argument("model_name")
+@click.argument("save_dir")
+def save_model(model_class, model_name, save_dir):
+    from huggingface_tool.savers.model_saver import ModelSaver
+    saver = ModelSaver(model_class, model_name)
+    if saver.load():
+        saver.save(save_dir)
+    else:
+        saver.logger.info("Dataset not found")
```

### Comparing `huggingface_tool-0.0.1/huggingface_tool/savers/__init__.py` & `huggingface_tool-0.0.2/huggingface_tool/savers/__init__.py`

 * *Files identical despite different names*

### Comparing `huggingface_tool-0.0.1/huggingface_tool/savers/base_saver.py` & `huggingface_tool-0.0.2/huggingface_tool/savers/base_saver.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 """"""
 
 from abc import ABC, abstractmethod
 
 from huggingface_tool.utils.logger import Logger
 
 class BaseSaver(ABC):
-    def __init__(self, name):
+    def __init__(self, name:str):
         self.logger = Logger()
         self.name = name
         self.loaded_object = None
 
 
 
     def load(self) -> bool:
```

### Comparing `huggingface_tool-0.0.1/huggingface_tool/savers/dataset_saver.py` & `huggingface_tool-0.0.2/huggingface_tool/savers/dataset_saver.py`

 * *Files identical despite different names*

### Comparing `huggingface_tool-0.0.1/huggingface_tool/savers/diffusion_model_saver.py` & `huggingface_tool-0.0.2/huggingface_tool/savers/diffusion_model_saver.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
-from huggingface_tool.savers.model_saver import ModelSaver
+from huggingface_tool.savers.base_model_saver import BaseModelSaver
 
 import torch
 from diffusers import StableDiffusionPipeline
 
-class DiffusionModelSaver(ModelSaver):
+class DiffusionModelSaver(BaseModelSaver):
     def _load(self, name)->bool:
         return StableDiffusionPipeline.from_pretrained(name, torch_dtype=torch.float16)
```

### Comparing `huggingface_tool-0.0.1/huggingface_tool/savers/model_saver.py` & `huggingface_tool-0.0.2/huggingface_tool/savers/base_model_saver.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 from abc import ABC
 from huggingface_tool.savers.base_saver import BaseSaver
 
-class ModelSaver(BaseSaver,ABC):
+class BaseModelSaver(BaseSaver,ABC):
     def save(self, save_dir: str):
         if self.loaded_object is None:
             self.logger.info("No model loaded, cannot save")
             return
         self.loaded_object.save_pretrained(save_dir)
```

### Comparing `huggingface_tool-0.0.1/huggingface_tool/savers/tokenizer_saver.py` & `huggingface_tool-0.0.2/huggingface_tool/utils/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,14 +11,7 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
-from transformers import AutoTokenizer
-
-from huggingface_tool.savers.model_saver import ModelSaver
-
-class TokenizerSaver(ModelSaver):
-    def _load(self,name):
-        return AutoTokenizer.from_pretrained(name)
```

### Comparing `huggingface_tool-0.0.1/huggingface_tool/utils/logger.py` & `huggingface_tool-0.0.2/huggingface_tool/utils/logger.py`

 * *Files identical despite different names*

### Comparing `huggingface_tool-0.0.1/huggingface_tool/utils/util.py` & `huggingface_tool-0.0.2/huggingface_tool/utils/util.py`

 * *Files identical despite different names*

### Comparing `huggingface_tool-0.0.1/huggingface_tool.egg-info/PKG-INFO` & `huggingface_tool-0.0.2/huggingface_tool.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huggingface-tool
-Version: 0.0.1
+Version: 0.0.2
 Summary: Toolkit for managing huggingface models and datasets
 Home-page: https://github.com/OpenRL-Lab/huggingface_tool
 Author: openrl contributors
 Author-email: huangsy1314@163.com
 Project-URL: Code, https://github.com/OpenRL-Lab/huggingface_tool
 Project-URL: Documentation, https://huggingface_tool.readthedocs.io/
 Keywords: huggingface toolkit
@@ -22,23 +22,29 @@
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
 
 # huggingface_tool
 
+[![PyPI](https://img.shields.io/pypi/v/huggingface-tool)](https://pypi.org/project/huggingface-tool/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/huggingface-tool)
+[![Hits-of-Code](https://hitsofcode.com/github/OpenRL-Lab/huggingface_tool?branch=main)](https://hitsofcode.com/github/OpenRL-Lab/huggingface_tool/view?branch=main)
+
 Tools for loading, upload, managing huggingface models and datasets
 
 
 ## Installation
 
-`pip install huggingface_tool`
+`pip install huggingface-tool`
 
 ## Usage
 
+- Download and save transformer models with: `htool save-model <model_class> <model_name> <save_dir>`
+  - For example: `htool save-model AutoModelForCausalLM gpt2 ./gpt2`
 - Download and save tokenizer with: `htool save-tk <tokenizer_name> <save_dir>`
   - For example: `htool save-tk gpt2 ./gpt2 `
 - Download and save dataset with: `htool save-data <dataset_name> <save_dir>`
   - For example: `htool save-data daily_dialog ./daily_dialog`
 - Download and save diffusion models with: `htool save-dm <model_name> <save_dir>`
   - For example: `htool save-dm google/ddpm-cat-256 ./google/`
```

### Comparing `huggingface_tool-0.0.1/huggingface_tool.egg-info/SOURCES.txt` & `huggingface_tool-0.0.2/huggingface_tool.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 huggingface_tool.egg-info/dependency_links.txt
 huggingface_tool.egg-info/entry_points.txt
 huggingface_tool.egg-info/requires.txt
 huggingface_tool.egg-info/top_level.txt
 huggingface_tool/cli/__init__.py
 huggingface_tool/cli/cli.py
 huggingface_tool/savers/__init__.py
+huggingface_tool/savers/base_model_saver.py
 huggingface_tool/savers/base_saver.py
 huggingface_tool/savers/dataset_saver.py
 huggingface_tool/savers/diffusion_model_saver.py
 huggingface_tool/savers/model_saver.py
 huggingface_tool/savers/tokenizer_saver.py
 huggingface_tool/utils/__init__.py
 huggingface_tool/utils/logger.py
```

### Comparing `huggingface_tool-0.0.1/setup.py` & `huggingface_tool-0.0.2/setup.py`

 * *Files identical despite different names*


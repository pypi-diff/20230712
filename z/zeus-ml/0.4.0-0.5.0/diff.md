# Comparing `tmp/zeus-ml-0.4.0.tar.gz` & `tmp/zeus-ml-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeus-ml-0.4.0.tar", last modified: Wed Jun 21 01:27:37 2023, max compression
+gzip compressed data, was "zeus-ml-0.5.0.tar", last modified: Wed Jul 12 03:12:38 2023, max compression
```

## Comparing `zeus-ml-0.4.0.tar` & `zeus-ml-0.5.0.tar`

### file list

```diff
@@ -1,35 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:27:37.155956 zeus-ml-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-21 01:27:34.000000 zeus-ml-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-21 01:27:37.155956 zeus-ml-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-06-21 01:27:34.000000 zeus-ml-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-21 01:27:34.000000 zeus-ml-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 01:27:37.155956 zeus-ml-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-21 01:27:34.000000 zeus-ml-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:27:37.155956 zeus-ml-0.4.0/zeus/
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-21 01:27:34.000000 zeus-ml-0.4.0/zeus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-06-21 01:27:34.000000 zeus-ml-0.4.0/zeus/analyze.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-06-21 01:27:34.000000 zeus-ml-0.4.0/zeus/job.py
--rw-r--r--   0 runner    (1001) docker     (123)    11966 2023-06-21 01:27:34.000000 zeus-ml-0.4.0/zeus/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:27:37.155956 zeus-ml-0.4.0/zeus/policy/
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-21 01:27:34.000000 zeus-ml-0.4.0/zeus/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-06-21 01:27:34.000000 zeus-ml-0.4.0/zeus/policy/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-06-21 01:27:34.000000 zeus-ml-0.4.0/zeus/policy/mab.py
--rw-r--r--   0 runner    (1001) docker     (123)    19970 2023-06-21 01:27:34.000000 zeus-ml-0.4.0/zeus/policy/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:27:37.155956 zeus-ml-0.4.0/zeus/run/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-21 01:27:34.000000 zeus-ml-0.4.0/zeus/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48890 2023-06-21 01:27:34.000000 zeus-ml-0.4.0/zeus/run/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    15157 2023-06-21 01:27:34.000000 zeus-ml-0.4.0/zeus/run/master.py
--rw-r--r--   0 runner    (1001) docker     (123)    36515 2023-06-21 01:27:34.000000 zeus-ml-0.4.0/zeus/simulate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:27:37.155956 zeus-ml-0.4.0/zeus/util/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-21 01:27:34.000000 zeus-ml-0.4.0/zeus/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-21 01:27:34.000000 zeus-ml-0.4.0/zeus/util/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-21 01:27:34.000000 zeus-ml-0.4.0/zeus/util/framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-06-21 01:27:34.000000 zeus-ml-0.4.0/zeus/util/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-21 01:27:34.000000 zeus-ml-0.4.0/zeus/util/lr_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-06-21 01:27:34.000000 zeus-ml-0.4.0/zeus/util/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:27:37.155956 zeus-ml-0.4.0/zeus_ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-21 01:27:37.000000 zeus-ml-0.4.0/zeus_ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-21 01:27:37.000000 zeus-ml-0.4.0/zeus_ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 01:27:37.000000 zeus-ml-0.4.0/zeus_ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-21 01:27:37.000000 zeus-ml-0.4.0/zeus_ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-21 01:27:37.000000 zeus-ml-0.4.0/zeus_ml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:12:38.956215 zeus-ml-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-07-12 03:12:38.956215 zeus-ml-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 03:12:38.956215 zeus-ml-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:12:38.948215 zeus-ml-0.5.0/zeus/
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15356 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:12:38.952216 zeus-ml-0.5.0/zeus/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14092 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/optimizer/power_limit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:12:38.952216 zeus-ml-0.5.0/zeus/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/policy/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/policy/mab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19970 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/policy/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:12:38.952216 zeus-ml-0.5.0/zeus/run/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49008 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/run/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15157 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/run/master.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36532 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/simulate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:12:38.952216 zeus-ml-0.5.0/zeus/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/util/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/util/framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/util/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/util/lr_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/util/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-07-12 03:12:35.000000 zeus-ml-0.5.0/zeus/util/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 03:12:38.956215 zeus-ml-0.5.0/zeus_ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-07-12 03:12:38.000000 zeus-ml-0.5.0/zeus_ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-12 03:12:38.000000 zeus-ml-0.5.0/zeus_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 03:12:38.000000 zeus-ml-0.5.0/zeus_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-12 03:12:38.000000 zeus-ml-0.5.0/zeus_ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-12 03:12:38.000000 zeus-ml-0.5.0/zeus_ml.egg-info/top_level.txt
```

### Comparing `zeus-ml-0.4.0/LICENSE` & `zeus-ml-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.4.0/README.md` & `zeus-ml-0.5.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,94 @@
 <div align="center">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="docs/assets/img/logo_dark.svg">
   <source media="(prefers-color-scheme: light)" srcset="docs/assets/img/logo_light.svg">
   <img alt="Zeus logo" width="55%" src="docs/assets/img/logo_dark.svg">
 </picture>
-<h1>An Energy Optimization Framework for DNN Training</h1>
+<h1>A Framework for Deep Learning Energy Measurement and Optimization</h1>
 </div>
 
 [![NSDI23 paper](https://custom-icon-badges.herokuapp.com/badge/NSDI'23-paper-b31b1b.svg)](https://www.usenix.org/conference/nsdi23/presentation/you)
 [![Docker Hub](https://badgen.net/docker/pulls/symbioticlab/zeus?icon=docker&label=Docker%20pulls)](https://hub.docker.com/r/symbioticlab/zeus)
 [![Slack workspace](https://badgen.net/badge/icon/Join%20workspace/611f69?icon=slack&label=Slack)](https://join.slack.com/t/zeus-ml/shared_invite/zt-1najba5mb-WExy7zoNTyaZZfTlUWoLLg)
 [![Homepage build](https://github.com/SymbioticLab/Zeus/actions/workflows/deploy_homepage.yaml/badge.svg)](https://github.com/SymbioticLab/Zeus/actions/workflows/deploy_homepage.yaml)
 [![Apache-2.0 License](https://custom-icon-badges.herokuapp.com/github/license/SymbioticLab/Zeus?logo=law)](/LICENSE)
 
-Zeus automatically optimizes the **energy and time** of training a DNN to a target validation metric by finding the optimal **batch size** and **GPU power limit**.
+---
+**Latest News** ⚡ 
+
+- \[2023/07\] [`ZeusMonitor`](https://ml.energy/zeus/reference/monitor/#zeus.monitor.ZeusMonitor) was used to profile GPU time and energy consumption for the [ML.ENERGY leaderboard](https://ml.energy/leaderboard).
+- \[2023/03\] [Chase](https://symbioticlab.org/publications/files/chase:ccai23/chase-ccai23.pdf), an automatic carbon optimization framework for DNN training, will appear at ICLR'23 workshop.
+- \[2022/11\] [Carbon-Aware Zeus](https://taikai.network/gsf/hackathons/carbonhack22/projects/cl95qxjpa70555701uhg96r0ek6/idea) won the **second overall best solution award** at Carbon Hack 22.
+---
+
+Zeus is a general framework for (1) measuring GPU energy consumption and (2) optimizing energy and time for DNN training.
+
+### Measuring GPU energy
+
+```python
+from zeus.monitor import ZeusMonitor
+
+monitor = ZeusMonitor(gpu_indices=[0,1,2,3])
+
+monitor.begin_window("heavy computation")
+# Four GPUs consuming energy like crazy!
+measurement = monitor.end_window("heavy computation")
+
+print(f"Energy: {measurement.total_energy} J")
+print(f"Time  : {measurement.time} s")
+```
+
+### Finding the optimal GPU power limit
+
+Zeus silently profiles different power limits during training and converges to the optimal one.
+
+```python
+from zeus.monitor import ZeusMonitor
+from zeus.optimizer import GlobalPowerLimitOptimizer
+
+monitor = ZeusMonitor(gpu_indices=[0,1,2,3])
+plo = GlobalPowerLimitOptimizer(monitor)
+
+plo.on_epoch_begin()
+
+for x, y in train_dataloader:
+    plo.on_step_begin()
+    # Learn from x and y!
+    plo.on_step_end()
+
+plo.on_epoch_end()
+```
 
 Please refer to our NSDI’23 [paper](https://www.usenix.org/conference/nsdi23/presentation/you) and [slides](https://www.usenix.org/system/files/nsdi23_slides_chung.pdf) for details.
 Checkout [Overview](https://ml.energy/zeus/overview/) for a summary.
 
 Zeus is part of [The ML.ENERGY Initiative](https://ml.energy).
 
 ## Repository Organization
 
 ```
 .
 ├── zeus/                # ⚡ Zeus Python package
+│   ├── optimizer/       #    - GPU energy and time optimizers
 │   ├── run/             #    - Tools for running Zeus on real training jobs
 │   ├── policy/          #    - Optimization policies and extension interfaces
 │   ├── util/            #    - Utility functions and classes
-│   ├── simulate.py      #    - Tools for trace-driven simulation
 │   ├── monitor.py       #    - `ZeusMonitor`: Measure GPU time and energy of any code block
+│   ├── controller.py    #    - Tools for controlling the flow of training
+│   ├── callback.py      #    - Base class for Hugging Face-like training callbacks.
+│   ├── simulate.py      #    - Tools for trace-driven simulation
 │   ├── analyze.py       #    - Analysis functions for power logs
 │   └── job.py           #    - Class for job specification
 │
 ├── zeus_monitor/        # 🔌 GPU power monitor
 │   ├── zemo/            #    -  A header-only library for querying NVML
 │   └── main.cpp         #    -  Source code of the power monitor
 │
 ├── examples/            # 🛠️ Examples of integrating Zeus
-│   ├── capriccio/       #    - Integrating with Huggingface and Capriccio
-│   ├── imagenet/        #    - Integrating with torchvision and ImageNet
-│   ├── cifar100/        #    - Integrating with torchvision and CIFAR100
-│   └── trace_driven/    #    - Using the Zeus trace-driven simulator
 │
 ├── capriccio/           # 🌊 A drifting sentiment analysis dataset
 │
 └── trace/               # 🗃️ Train and power traces for various GPUs and DNNs
 ```
 
 ## Getting Started
@@ -66,38 +109,31 @@
     bash
 ```
 
 Refer to [Environment setup](https://ml.energy/zeus/getting_started/environment/) for details.
 
 ### Examples
 
-We provide working examples for integrating and running Zeus:
-
-- Integrating Zeus with Computer Vision
-    - [ImageNet](examples/imagenet)
-    - [CIFAR100](examples/cifar100)
-- [Integrating Zeus with Natural Language Processing](examples/capriccio)
-- [Running trace-driven simulation on single recurring jobs and the Alibaba GPU cluster trace](examples/trace_driven)
+We provide working examples for integrating and running Zeus in the `examples/` directory.
 
 
 ## Extending Zeus
 
 You can easily implement custom policies for batch size and power limit optimization and plug it into Zeus.
 
 Refer to [Extending Zeus](https://ml.energy/zeus/extend/) for details.
 
+
 ## Carbon-Aware Zeus
 
-The use of GPUs for training DNNs results in high carbon emissions and energy consumption. Building on top of Zeus, we introduce *Chase* -- a carbon-aware solution. *Chase* dynamically controls the energy consumption of GPUs; adapts to shifts in carbon intensity during DNN training, reducing carbon footprint with minimal compromises on training performance. To proactively adapt to shifting carbon intensity, a lightweight machine learning algorithm is used to forecast the carbon intensity of the upcoming time frame. For more details on Chase, please refer to our [paper](https://www.usenix.org/conference/nsdi23/presentation/you) and the [chase branch](https://github.com/SymbioticLab/Zeus/tree/chase). 
+The use of GPUs for training DNNs results in high carbon emissions and energy consumption. Building on top of Zeus, we introduce *Chase* -- a carbon-aware solution. *Chase* dynamically controls the energy consumption of GPUs; adapts to shifts in carbon intensity during DNN training, reducing carbon footprint with minimal compromises on training performance. To proactively adapt to shifting carbon intensity, a lightweight machine learning algorithm is used to forecast the carbon intensity of the upcoming time frame. For more details on Chase, please refer to our [paper](https://symbioticlab.org/publications/files/chase:ccai23/chase-ccai23.pdf) and the [chase branch](https://github.com/SymbioticLab/Zeus/tree/chase). 
 
 
 ## Citation
 
-Please consider citing our NSDI’23 paper if you find Zeus to be related to your research project.
-
 ```bibtex
 @inproceedings{zeus-nsdi23,
     title     = {Zeus: Understanding and Optimizing {GPU} Energy Consumption of {DNN} Training},
     author    = {Jie You and Jae-Won Chung and Mosharaf Chowdhury},
     booktitle = {USENIX NSDI},
     year      = {2023}
 }
```

### Comparing `zeus-ml-0.4.0/pyproject.toml` & `zeus-ml-0.5.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -12,14 +12,15 @@
   "RUF", # Ruff-introduced misc rules
 ]
 ignore = [
   "PLW0603",  # Global statement
   "B019",     # Usage of functools.lru_cache
   "PLR0913",  # Too many function arguments
   "B905",     # zip strict argument
+  "PLR0915",  # Too many statements
 ]
 line-length = 120
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
 [tool.ruff.per-file-ignores]
```

### Comparing `zeus-ml-0.4.0/setup.py` & `zeus-ml-0.5.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,42 +13,43 @@
 # limitations under the License.
 
 from setuptools import setup, find_packages
 
 extras_require={
     "lint": ["ruff", "black==22.6.0"],
     "test": ["pytest==7.3.2", "pytest-mock==3.10.0", "pytest-xdist==3.3.1"],
+    "torch": ["torch==2.0.1"],
 }
-extras_require["dev"] = extras_require["lint"] + extras_require["test"]
+extras_require["dev"] = extras_require["lint"] + extras_require["test"] + extras_require["torch"]
 
 setup(
     name="zeus-ml",
-    version="0.4.0",
-    description="An Energy Optimization Framework for DNN Training",
-    long_description="# Zeus: An Energy Optimization Framework for DNN Training\n",
+    version="0.5.0",
+    description="A framework for deep learning energy measurement and optimization.",
+    long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SymbioticLab/Zeus",
     author="Jae-Won Chung",
     author_email="jwnchung@umich.edu",
     license="Apache-2.0",
     classifiers=[
         "Environment :: GPU :: NVIDIA CUDA",
         "License :: OSI Approved :: Apache Software License",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
-    keywords=["deep-learning", "power", "energy", "mlsys"],
+    keywords=["deep-learning", "power", "energy", "sustainability", "mlsys"],
     project_urls={
         "Documentation": "https://ml.energy/zeus",
     },
     packages=find_packages("."),
     install_requires=[
         "numpy",
-        "pandas==1.4.2",
+        "pandas",
         "scikit-learn",
         "pynvml",
     ],
     python_requires=">=3.8",
     extras_require=extras_require,
 )
```

### Comparing `zeus-ml-0.4.0/zeus/__init__.py` & `zeus-ml-0.5.0/zeus/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,21 +8,22 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Zeus is an energy optimization framework for DNN training.
+"""Zeus is a framework for deep learning energy measurement and optimization.
 
 Modules:
 
+- [`run`][zeus.run]: Machinery for actually running Zeus.
+- [`monitor`][zeus.monitor]: Class for profiling energy inside training scripts.
+- [`optimizer`][zeus.optimizer]: A collection of optimizers for various knobs.
+- [`callback`][zeus.callback]: Callback definition.
+- [`controller`][zeus.controller]: A collection of controllers that influence training flow.
 - [`analyze`][zeus.analyze]: Functions for analyzing log files.
-- [`profile`][zeus.profile]: Tools for profiling energy and time. Will be deprecated.
-- [`profiling`][zeus.profiling]: Tools for profiling energy for an arbitrary profilng window inside training scripts
 - [`job`][zeus.job]: Job specification.
-- [`run`][zeus.run]: Machinery for actually running Zeus.
 - [`simulate`][zeus.simulate]: Machinery for trace-driven Zeus.
 - [`policy`][zeus.policy]: Collection of optimization policies.
-- [`monitor`][zeus.monitor]: Class for profiling energy inside training scripts.
 - [`util`][zeus.util]: Utility functions and classes.
 """
```

### Comparing `zeus-ml-0.4.0/zeus/analyze.py` & `zeus-ml-0.5.0/zeus/analyze.py`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.4.0/zeus/job.py` & `zeus-ml-0.5.0/zeus/job.py`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.4.0/zeus/monitor.py` & `zeus-ml-0.5.0/zeus/monitor.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,22 +20,23 @@
 import time
 import shutil
 import signal
 import atexit
 import logging
 import tempfile
 import subprocess
-from functools import cached_property, lru_cache
+from pathlib import Path
 from dataclasses import dataclass
+from functools import cached_property, lru_cache
 
 import pynvml
 
 from zeus import analyze
-from zeus.util.framework import cuda_sync
 from zeus.util.logging import get_logger
+from zeus.util.framework import cuda_sync
 
 
 @dataclass
 class Measurement:
     """Measurement result of one window.
 
     Attributes:
@@ -52,21 +53,21 @@
         """Total energy consumed (in Joules) during the measurement window."""
         return sum(self.energy.values())
 
 
 class ZeusMonitor:
     """Measure the GPU energy and time consumption of a block of code.
 
-    Works for multi-GPU, heterogeneous GPU types, and any DL framework.
+    Works for multi-GPU and heterogeneous GPU types. Aware of `CUDA_VISIBLE_DEVICES`.
 
     You can mark the beginning and end of a measurement window, during which the GPU
     energy and time consumed will be recorded. Multiple concurrent measurement windows
     are supported.
 
-    ## Integrated Example
+    ## Integration Example
 
     ```python
     from zeus.monitor import ZeusMontior
 
     # Time/Energy measurements for four GPUs will begin and end at the same time.
     gpu_indices = [0, 1, 2, 3]
     monitor = ZeusMonitor(gpu_indices)
@@ -83,71 +84,109 @@
 
     # Print the measurement result.
     time_consumed, energy_consumed = prof_result.time, prof_result.energy
     print(f"Training took {time_consumed} seconds.")
     for gpu_idx, gpu_energy in zip(gpu_indices, energy_consumed):
         print(f"GPU {gpu_idx} consumed {gpu_energy} Joules.")
     ```
+
+    Attributes:
+        gpu_indices (`list[int]`): Indices of all the CUDA devices to monitor, from the
+            DL framework's perspective after applying `CUDA_VISIBLE_DEVICES`.
+        nvml_gpu_indices (`list[int]`): Indices of all the CUDA devices to monitor, from
+            NVML/system's perspective.
     """
 
     def __init__(
         self,
         gpu_indices: list[int] | None = None,
         monitor_exec: str = "zeus_monitor",
+        log_file: str | Path | None = None,
     ) -> None:
         """Instantiate the monitor.
 
         For Volta or newer GPUs, energy consumption is measured very cheaply with the
-        `nvmlDeviceGetTotalEnergyConsumption` API. Otherwise, the energy API is not
-        supported. Thus, the Zeus monitor binary is used to poll `nvmlDeviceGetPowerUsage`
+        `nvmlDeviceGetTotalEnergyConsumption` API. The API is not supported on older
+        architectures, so the `zeus_monitor` binary is used to poll `nvmlDeviceGetPowerUsage`
         and write to a temporary CSV file, which is then integrated over time to compute
         energy consumption.
 
         Args:
-            gpu_indices: Indices of all the CUDA devices to monitor. Time/Energy measurement
+            gpu_indices: Indices of all the CUDA devices to monitor. Time/Energy measurements
                 will begin and end at the same time for these GPUs (i.e., synchronized).
-                If None, all the GPUs available will be used (while respecting the
-                `CUDA_VISIBLE_DEVICES` environment variable). (Default: `None`)
+                If None, all the GPUs available will be used. `CUDA_VISIBLE_DEVICES`
+                is respected if set, e.g., GPU index `1` passed into `gpu_indices` when
+                `CUDA_VISIBLE_DEVICES=2,3` will be interpreted as CUDA device `3`.
+                `CUDA_VISIBLE_DEVICES`s formatted with comma-separated indices are supported.
+                (Default: `None`)
             monitor_exec: Zeus monitor executable. (Default: `"zeus_monitor"`)
+            log_file: Path to the log CSV file. If `None`, logging will be disabled.
         """
         # Initialize NVML.
         pynvml.nvmlInit()
 
-        # Initialize logger.
-        self.logger = get_logger(type(self).__name__)
-
-        # If `gpu_indices` is None, use all the GPUs available.
+        # Sanity check.
+        if gpu_indices is not None and not gpu_indices:
+            raise ValueError("`gpu_indices` must be None or non-empty.")
+
+        # Find the NVML GPU indices visible to PyTorch, respecting `CUDA_VISIBLE_DEVICES`.
+        if (cuda_visible_device := os.environ.get("CUDA_VISIBLE_DEVICES")) is not None:
+            nvml_visible_indices = [int(idx) for idx in cuda_visible_device.split(",")]
+        else:
+            nvml_visible_indices = list(range(pynvml.nvmlDeviceGetCount()))
+
+        # NVML GPU indices and PyTorch GPU indices should be different.
+        # We always use PyTorch GPU indices when communicating with the outside world,
+        # but when dealing with NVML, we use the NVML GPU indices.
         if gpu_indices is None:
-            # NVML is not aware of the `CUDA_VISIBLE_DEVICES` environment variable,
-            # so we need to manually check whether it's set.
-            cuda_visible_devices = os.environ.get("CUDA_VISIBLE_DEVICES")
-            if cuda_visible_devices is not None:
-                gpu_indices = [int(idx) for idx in cuda_visible_devices.split(",")]
-            else:
-                gpu_indices = list(range(pynvml.nvmlDeviceGetCount()))
+            nvml_gpu_indices = nvml_visible_indices
+            torch_gpu_indices = list(range(len(nvml_visible_indices)))
+        else:
+            nvml_gpu_indices = [nvml_visible_indices[idx] for idx in gpu_indices]
+            torch_gpu_indices = gpu_indices
+        self.gpu_indices = torch_gpu_indices
+        self.nvml_gpu_indices = nvml_gpu_indices
 
-        # Save all the GPU handles.
+        # Save all the NVML GPU handles. These should be called with system-level GPU indices.
         self.gpu_handles: dict[int, pynvml.c_nvmlDevice_t] = {}
-        for gpu_index in gpu_indices:
-            handle = pynvml.nvmlDeviceGetHandleByIndex(gpu_index)
-            self.gpu_handles[gpu_index] = handle
+        for nvml_gpu_index, torch_gpu_index in zip(nvml_gpu_indices, torch_gpu_indices):
+            handle = pynvml.nvmlDeviceGetHandleByIndex(nvml_gpu_index)
+            self.gpu_handles[torch_gpu_index] = handle
+
+        # Initialize loggers.
+        self.logger = get_logger(type(self).__name__)
+        if log_file is None:
+            self.log_file = None
+        else:
+            if dir := os.path.dirname(log_file):
+                os.makedirs(dir, exist_ok=True)
+            self.log_file = open(log_file, "w")  # ruff: noqa: SIM115
+            self.logger.info("Writing measurement logs to %s.", log_file)
+            self.log_file.write(
+                f"start_time,window_name,elapsed_time,{','.join(map(lambda i: f'gpu{i}_energy', self.gpu_indices))}\n",
+            )
+            self.log_file.flush()
+
+        self.logger.info("Monitoring GPU %s.", self.gpu_indices)
 
         # A dictionary that maps the string keys of active measurement windows to
         # the state of the measurement window. Each element in the dictionary is a tuple of:
         #     1) Time elapsed at the beginning of this window.
         #     2) Total energy consumed by each >= Volta GPU at the beginning of this window.
         self.measurement_states: dict[str, tuple[float, dict[int, float]]] = {}
 
         # Shutdown NVML and kill the monitors when the training script exits.
         # The exit hook is a no-op when no monitors are running, so we can register it
         # before starting any monitors.
         def exit_hook():
             # Shutdown NVML.
             pynvml.nvmlShutdown()
             self._stop_monitors()
+            if self.log_file is not None:
+                self.log_file.close()
 
         atexit.register(exit_hook)
 
         # Start monitors that poll power for older architecture GPUs.
         self.monitors: dict[int, subprocess.Popen] = {}
         self._start_monitors(monitor_exec)
 
@@ -171,28 +210,35 @@
         if any(old_arch_flags):
             # Check whether the monitor path is good.
             if not shutil.which(monitor_exec):
                 raise ValueError(f"'{monitor_exec}' is not executable")
             # Create a temporary directory.
             self.monitor_log_dir = tempfile.mkdtemp()
 
-        # Capture the time when we started the monitors.
-        self.monitor_start_time = time.monotonic()
-
         # Spawn monitor process when GPU has older architecture.
-        for gpu_index, arch_is_old in zip(self.gpu_handles, old_arch_flags):
+        # The monitor should be spawned with NVML GPU indices.
+        # However, we still use the PyTorch GPU indices to construct the log path because
+        # `end_window` accesses the power log path with PyTorch GPU indices.
+        for torch_gpu_index, nvml_gpu_index, arch_is_old in zip(
+            self.gpu_indices,
+            self.nvml_gpu_indices,
+            old_arch_flags,
+        ):
             if arch_is_old:
-                log_path = self._monitor_log_path(gpu_index)
+                log_path = self._monitor_log_path(torch_gpu_index)
                 # 10 Hz (100 ms sleep) polling should be enough.
                 monitor = subprocess.Popen(
-                    [monitor_exec, log_path, "0", "100", str(gpu_index)],
+                    [monitor_exec, log_path, "0", "100", str(nvml_gpu_index)],
                 )
                 # Save the mapping from `gpu_index` to monitor.
-                self.monitors[gpu_index] = monitor
-                self._log("Zeus monitor started.", gpu_index)
+                self.monitors[torch_gpu_index] = monitor
+                self._log("Zeus monitor started.", nvml_gpu_index)
+
+        # Capture the time when we started the monitors.
+        self.monitor_start_time = time.monotonic()
 
     def _stop_monitors(self) -> None:
         """Kill the power monitor subprocess."""
         for monitor in self.monitors.values():
             monitor.send_signal(signal.SIGINT)
         for gpu_index, monitor in self.monitors.items():
             monitor.wait(timeout=1.0)
@@ -210,14 +256,15 @@
 
     def begin_window(self, key: str, sync_cuda: bool = True) -> None:
         """Begin a new measurement window.
 
         Args:
             key: Unique name of the measurement window.
             sync_cuda: Whether to synchronize CUDA before starting the measurement window.
+                (Default: `True`)
         """
         # Make sure the key is unique.
         if key in self.measurement_states:
             raise ValueError(f"Measurement window '{key}' already exists")
 
         # Call cudaSynchronize to make sure we freeze at the right time.
         if sync_cuda:
@@ -236,33 +283,44 @@
                     pynvml.nvmlDeviceGetTotalEnergyConsumption(gpu_handle) / 1000.0
                 )
 
         # Add measurement state to dictionary.
         self.measurement_states[key] = (timestamp, energy_state)
         self._log(f"Measurement window '{key}' started.")
 
-    def end_window(self, key: str, sync_cuda: bool = True) -> Measurement:
+    def end_window(
+        self, key: str, sync_cuda: bool = True, cancel: bool = False
+    ) -> Measurement:
         """End a measurement window and return the time and energy consumption.
 
         Args:
             key: Name of an active measurement window.
             sync_cuda: Whether to synchronize CUDA before ending the measurement window.
                 (default: `True`)
+            cancel: Whether to cancel the measurement window. If `True`, the measurement
+                window is assumed to be cancelled and discarded. Thus, an empty Measurement
+                object will be returned and the measurement window will not be recorded in
+                the log file either. `sync_cuda` is still respected.
         """
         # Retrieve the start time and energy consumption of this window.
         try:
             start_time, start_energy = self.measurement_states.pop(key)
         except KeyError:
             raise ValueError(f"Measurement window '{key}' does not exist") from None
 
         # Call cudaSynchronize to make sure we freeze at the right time.
         if sync_cuda:
             for gpu_index in self.gpu_handles:
                 cuda_sync(gpu_index)
 
+        # If the measurement window is cancelled, return an empty Measurement object.
+        if cancel:
+            self._log(f"Measurement window '{key}' cancelled.")
+            return Measurement(time=0.0, energy={gpu: 0.0 for gpu in self.gpu_handles})
+
         end_time: float = time.monotonic()
         time_consumption: float = end_time - start_time
         energy_consumption: dict[int, float] = {}
         for gpu_index, gpu_handle in self.gpu_handles.items():
             # Query energy directly if the GPU has newer architecture.
             if self._is_new_arch(gpu_index):
                 end_energy = (
@@ -274,14 +332,24 @@
                 energy_consumption[gpu_index] = analyze.energy(
                     self._monitor_log_path(gpu_index),
                     start_time - self.monitor_start_time,
                     end_time - self.monitor_start_time,
                 )
 
         self._log(f"Measurement window '{key}' ended.")
+
+        # Add to log file.
+        if self.log_file is not None:
+            self.log_file.write(
+                f"{start_time},{key},{time_consumption},"
+                + ",".join(map(str, energy_consumption.values()))
+                + "\n"
+            )
+            self.log_file.flush()
+
         return Measurement(time_consumption, energy_consumption)
 
     def _log(
         self, message: str, gpu_index: int | None = None, level: int = logging.INFO
     ) -> None:
         """Print out message with prefix.
```

### Comparing `zeus-ml-0.4.0/zeus/policy/__init__.py` & `zeus-ml-0.5.0/zeus/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.4.0/zeus/policy/interface.py` & `zeus-ml-0.5.0/zeus/policy/interface.py`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.4.0/zeus/policy/mab.py` & `zeus-ml-0.5.0/zeus/policy/mab.py`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.4.0/zeus/policy/optimizer.py` & `zeus-ml-0.5.0/zeus/policy/optimizer.py`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.4.0/zeus/run/__init__.py` & `zeus-ml-0.5.0/zeus/run/__init__.py`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.4.0/zeus/run/dataloader.py` & `zeus-ml-0.5.0/zeus/run/dataloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -796,15 +796,17 @@
             f"end_of_this_profile_window {self.sample_num + self.profile_iter} "
             f"< end_of_this_epoch {self.num_samples}"
         )
 
         if self.rank == 0:
             # Push profiling window for the current power limit value.
             # This window will profile for `self.profile_iter` iterations.
-            self._begin_measurement("__ZeusDataLoader_power_limit")
+            self._begin_measurement(
+                f"__ZeusDataLoader_power_limit_{self.current_gpu_pl//1000}"
+            )
 
         # Set the sample number when we started profiling.
         self.prof_start_sample = self.sample_num
 
         # Set profiling state.
         self.prof_state = PROFILING
 
@@ -836,15 +838,17 @@
         torch.cuda.synchronize()
 
         # Advance to the next power limit. Affects self.power_limits_left.
         self.prof_pl_index += 1
 
         if self.rank == 0:
             # Pop profiling window for the current power limit and fetch profiling results.
-            profiling_result = self._end_measurement("__ZeusDataLoader_power_limit")
+            profiling_result = self._end_measurement(
+                f"__ZeusDataLoader_power_limit_{self.current_gpu_pl//1000}"
+            )
             time_consumed, energy_consumed = (
                 profiling_result.time,
                 profiling_result.energy,
             )
             # Summing up the average power on all GPUs.
             sum_avg_power = sum(energy_consumed.values()) / time_consumed
             self.train_power_result[self.current_gpu_pl] = sum_avg_power
```

### Comparing `zeus-ml-0.4.0/zeus/run/master.py` & `zeus-ml-0.5.0/zeus/run/master.py`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.4.0/zeus/simulate.py` & `zeus-ml-0.5.0/zeus/simulate.py`

 * *Files 0% similar despite different names*

```diff
@@ -790,15 +790,15 @@
         """
         # Filter by job spec and BS.
         df = job.filter_df(self.df)
         df = df.loc[(df.batch_size == batch_size)]
 
         # Compute the epoch cost of each power limit (Equation 7).
         max_pl = df.power_limit.max().item()
-        df = df.groupby(["power_limit"], as_index=False).mean()
+        df = df.groupby(["power_limit"], as_index=False).mean(numeric_only=True)
         df["epoch_cost"] = (
             eta_knob * df["average_power"] + (1 - eta_knob) * max_pl
         ) * df["time_per_epoch"]
 
         # We'll be profiling energy from larger to smaller power limits.
         df = df.sort_values(by="power_limit", ascending=False)
         result = {rec.power_limit: rec.epoch_cost for rec in df.to_records(index=False)}
```

### Comparing `zeus-ml-0.4.0/zeus/util/__init__.py` & `zeus-ml-0.5.0/zeus/util/__init__.py`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.4.0/zeus/util/check.py` & `zeus-ml-0.5.0/zeus/util/check.py`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.4.0/zeus/util/framework.py` & `zeus-ml-0.5.0/zeus/util/framework.py`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.4.0/zeus/util/logging.py` & `zeus-ml-0.5.0/zeus/util/logging.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,14 +38,17 @@
         """Flush both log file and stdout."""
         self.file.flush()
         self.stdout.flush()
 
 
 def get_logger(name: str, level: int = logging.INFO) -> logging.Logger:
     """Get a logger with the given name with some formatting configs."""
+    if name in logging.Logger.manager.loggerDict:
+        return logging.getLogger(name)
+
     logger = logging.getLogger(name)
     logger.propagate = False
     logger.setLevel(level)
     formatter = logging.Formatter(
         "[%(asctime)s] [%(name)s](%(filename)s:%(lineno)d) %(message)s"
     )
     handler = logging.StreamHandler(sys.stdout)
```

### Comparing `zeus-ml-0.4.0/zeus/util/lr_scaler.py` & `zeus-ml-0.5.0/zeus/util/lr_scaler.py`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.4.0/zeus/util/metric.py` & `zeus-ml-0.5.0/zeus/util/metric.py`

 * *Files identical despite different names*

### Comparing `zeus-ml-0.4.0/zeus_ml.egg-info/SOURCES.txt` & `zeus-ml-0.5.0/zeus_ml.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 zeus/__init__.py
 zeus/analyze.py
+zeus/callback.py
+zeus/controller.py
 zeus/job.py
 zeus/monitor.py
 zeus/simulate.py
+zeus/optimizer/__init__.py
+zeus/optimizer/power_limit.py
 zeus/policy/__init__.py
 zeus/policy/interface.py
 zeus/policy/mab.py
 zeus/policy/optimizer.py
 zeus/run/__init__.py
 zeus/run/dataloader.py
 zeus/run/master.py
 zeus/util/__init__.py
 zeus/util/check.py
 zeus/util/framework.py
 zeus/util/logging.py
 zeus/util/lr_scaler.py
 zeus/util/metric.py
+zeus/util/testing.py
 zeus_ml.egg-info/PKG-INFO
 zeus_ml.egg-info/SOURCES.txt
 zeus_ml.egg-info/dependency_links.txt
 zeus_ml.egg-info/requires.txt
 zeus_ml.egg-info/top_level.txt
```


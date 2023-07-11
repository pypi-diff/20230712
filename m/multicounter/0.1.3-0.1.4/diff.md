# Comparing `tmp/multicounter-0.1.3.tar.gz` & `tmp/multicounter-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multicounter-0.1.3.tar", max compression
+gzip compressed data, was "multicounter-0.1.4.tar", max compression
```

## Comparing `multicounter-0.1.3.tar` & `multicounter-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0    16725 2022-05-27 18:37:44.451690 multicounter-0.1.3/LICENSE
--rw-r--r--   0        0        0     2588 2022-05-27 18:37:44.451690 multicounter-0.1.3/README.md
--rw-r--r--   0        0        0      273 2022-05-27 18:37:44.451690 multicounter-0.1.3/multicounter/__init__.py
--rw-r--r--   0        0        0      826 2022-05-27 18:37:44.455690 multicounter-0.1.3/multicounter/multicounter.py
--rw-r--r--   0        0        0      429 2022-05-27 18:37:44.455690 multicounter-0.1.3/multicounter/py.typed
--rw-r--r--   0        0        0      665 2022-05-27 18:37:44.455690 multicounter-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3286 2022-05-27 18:38:03.247376 multicounter-0.1.3/setup.py
--rw-r--r--   0        0        0     3318 2022-05-27 18:38:03.247602 multicounter-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    16725 2023-07-11 22:21:56.633995 multicounter-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2969 2023-07-11 22:21:56.633995 multicounter-0.1.4/README.md
+-rw-r--r--   0        0        0      273 2023-07-11 22:21:56.633995 multicounter-0.1.4/multicounter/__init__.py
+-rw-r--r--   0        0        0      826 2023-07-11 22:21:56.633995 multicounter-0.1.4/multicounter/multicounter.py
+-rw-r--r--   0        0        0      429 2023-07-11 22:21:56.633995 multicounter-0.1.4/multicounter/py.typed
+-rw-r--r--   0        0        0      659 2023-07-11 22:21:56.633995 multicounter-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3794 1970-01-01 00:00:00.000000 multicounter-0.1.4/PKG-INFO
```

### Comparing `multicounter-0.1.3/LICENSE` & `multicounter-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `multicounter-0.1.3/README.md` & `multicounter-0.1.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,19 @@
  file, You can obtain one at http://mozilla.org/MPL/2.0/.
 -->
 
 # MultiCounter
 
 A simple, elegant counter with support for counting multiple things at once.
 
+<!-- BADGES -->
+[![](https://badgen.net/github/license/thehale/multicounter)](https://github.com/thehale/multicounter/blob/master/LICENSE)
+[![](https://badgen.net/badge/icon/Sponsor/pink?icon=github&label)](https://github.com/sponsors/thehale)
+[![](https://badgen.net/badge/icon/Follow%20@jhaledev/1DA1F2?icon=twitter&label)](https://twitter.com/intent/user?screen_name=jhaledev)
+
 ## Installation
 
 ### Pip
 ```bash
 pip install multicounter
 ```
```

### Comparing `multicounter-0.1.3/multicounter/multicounter.py` & `multicounter-0.1.4/multicounter/multicounter.py`

 * *Files identical despite different names*

### Comparing `multicounter-0.1.3/pyproject.toml` & `multicounter-0.1.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "multicounter"
-version = "0.1.3"
+version = "0.1.4"
 description = "A simple, elegant counter with support for counting multiple things at once."
 authors = ["Joseph Hale <me@jhale.dev>"]
 license = "MPL-2.0"
 readme = "README.md"
-homepage = "https://github.com/jhale1805/multicounter"
-repository = "https://github.com/jhale1805/multicounter"
-documentation = "https://github.com/jhale1805/multicounter"
+homepage = "https://github.com/thehale/multicounter"
+repository = "https://github.com/thehale/multicounter"
+documentation = "https://github.com/thehale/multicounter"
 keywords = [ "counter", "statistics" ]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.7"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.1"
-pre-commit = "^2.19.0"
-black = "^22.3.0"
+pytest = "^7.4"
+pre-commit = "^2.21.0"
+black = "^23.3.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `multicounter-0.1.3/setup.py` & `multicounter-0.1.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,116 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: multicounter
+Version: 0.1.4
+Summary: A simple, elegant counter with support for counting multiple things at once.
+Home-page: https://github.com/thehale/multicounter
+License: MPL-2.0
+Keywords: counter,statistics
+Author: Joseph Hale
+Author-email: me@jhale.dev
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Project-URL: Documentation, https://github.com/thehale/multicounter
+Project-URL: Repository, https://github.com/thehale/multicounter
+Description-Content-Type: text/markdown
 
-packages = \
-['multicounter']
+<!--
+ Copyright (c) 2022 Joseph Hale
 
-package_data = \
-{'': ['*']}
+ This Source Code Form is subject to the terms of the Mozilla Public
+ License, v. 2.0. If a copy of the MPL was not distributed with this
+ file, You can obtain one at http://mozilla.org/MPL/2.0/.
+-->
 
-setup_kwargs = {
-    'name': 'multicounter',
-    'version': '0.1.3',
-    'description': 'A simple, elegant counter with support for counting multiple things at once.',
-    'long_description': "<!--\n Copyright (c) 2022 Joseph Hale\n\n This Source Code Form is subject to the terms of the Mozilla Public\n License, v. 2.0. If a copy of the MPL was not distributed with this\n file, You can obtain one at http://mozilla.org/MPL/2.0/.\n-->\n\n# MultiCounter\n\nA simple, elegant counter with support for counting multiple things at once.\n\n## Installation\n\n### Pip\n```bash\npip install multicounter\n```\n\n### Poetry\n```bash\npoetry add multicounter\n```\n\n## Usage\n```python\nfrom multicounter import MultiCounter\nmc = MultiCounter()\n\n# Choose a name for your counter and start counting!\nmc.foo += 1\n\n# You can choose an initial value for a counter ...\nmc.bar = 42\n# ... and increment or decrement it however you like.\nmc.bar -= 4\n\nprint(mc.get_counters())\n# {'foo': 1, 'bar': 38}\n```\n\n## Contributing\nSee [CONTRIBUTING.md](CONTRIBUTING.md)\n\n## The Legal Stuff\n\n```\n`MultiCounter` by Joseph Hale is licensed under the terms of the Mozilla\nPublic License, v 2.0, which are available at https://mozilla.org/MPL/2.0/.\n\nYou can download the source code for `MultiCounter` for free from\nhttps://github.com/jhale1805/multicounter.\n```\n\n### TL;DR\n\nYou can use files from this project in both open source and proprietary\napplications, provided you include the above attribution. However, if\nyou modify any code in this project, or copy blocks of it into your own\ncode, you must publicly share the resulting files (note, not your whole\nprogram) under the MPL-2.0. The best way to do this is via a Pull\nRequest back into this project.\n\nIf you have any other questions, you may also find Mozilla's [official\nFAQ](https://www.mozilla.org/en-US/MPL/2.0/FAQ/) for the MPL-2.0\nlicense insightful.\n\nIf you dislike this license, you can contact me about negotiating a\npaid contract with different terms.\n\n**Disclaimer:** This TL;DR is just a summary. All legal questions\nregarding usage of this project must be handled according to the\nofficial terms specified in the `LICENSE` file.\n\n### Why the MPL-2.0 license?\n\nI believe that an open-source software license should ensure that code\ncan be used everywhere.\n\nStrict copyleft licenses, like the GPL family of licenses, fail to\nfulfill that vision because they only permit code to be used in other\nGPL-licensed projects. Permissive licenses, like the MIT and Apache\nlicenses, allow code to be used everywhere but fail to prevent\nproprietary or GPL-licensed projects from limiting access to any\nimprovements they make.\n\nIn contrast, the MPL-2.0 license allows code to be used in any software\nproject, while ensuring that any improvements remain available for\neveryone.\n",
-    'author': 'Joseph Hale',
-    'author_email': 'me@jhale.dev',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/jhale1805/multicounter',
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.8,<4.0',
-}
+# MultiCounter
 
+A simple, elegant counter with support for counting multiple things at once.
+
+<!-- BADGES -->
+[![](https://badgen.net/github/license/thehale/multicounter)](https://github.com/thehale/multicounter/blob/master/LICENSE)
+[![](https://badgen.net/badge/icon/Sponsor/pink?icon=github&label)](https://github.com/sponsors/thehale)
+[![](https://badgen.net/badge/icon/Follow%20@jhaledev/1DA1F2?icon=twitter&label)](https://twitter.com/intent/user?screen_name=jhaledev)
+
+## Installation
+
+### Pip
+```bash
+pip install multicounter
+```
+
+### Poetry
+```bash
+poetry add multicounter
+```
+
+## Usage
+```python
+from multicounter import MultiCounter
+mc = MultiCounter()
+
+# Choose a name for your counter and start counting!
+mc.foo += 1
+
+# You can choose an initial value for a counter ...
+mc.bar = 42
+# ... and increment or decrement it however you like.
+mc.bar -= 4
+
+print(mc.get_counters())
+# {'foo': 1, 'bar': 38}
+```
+
+## Contributing
+See [CONTRIBUTING.md](CONTRIBUTING.md)
+
+## The Legal Stuff
+
+```
+`MultiCounter` by Joseph Hale is licensed under the terms of the Mozilla
+Public License, v 2.0, which are available at https://mozilla.org/MPL/2.0/.
+
+You can download the source code for `MultiCounter` for free from
+https://github.com/jhale1805/multicounter.
+```
+
+### TL;DR
+
+You can use files from this project in both open source and proprietary
+applications, provided you include the above attribution. However, if
+you modify any code in this project, or copy blocks of it into your own
+code, you must publicly share the resulting files (note, not your whole
+program) under the MPL-2.0. The best way to do this is via a Pull
+Request back into this project.
+
+If you have any other questions, you may also find Mozilla's [official
+FAQ](https://www.mozilla.org/en-US/MPL/2.0/FAQ/) for the MPL-2.0
+license insightful.
+
+If you dislike this license, you can contact me about negotiating a
+paid contract with different terms.
+
+**Disclaimer:** This TL;DR is just a summary. All legal questions
+regarding usage of this project must be handled according to the
+official terms specified in the `LICENSE` file.
+
+### Why the MPL-2.0 license?
+
+I believe that an open-source software license should ensure that code
+can be used everywhere.
+
+Strict copyleft licenses, like the GPL family of licenses, fail to
+fulfill that vision because they only permit code to be used in other
+GPL-licensed projects. Permissive licenses, like the MIT and Apache
+licenses, allow code to be used everywhere but fail to prevent
+proprietary or GPL-licensed projects from limiting access to any
+improvements they make.
+
+In contrast, the MPL-2.0 license allows code to be used in any software
+project, while ensuring that any improvements remain available for
+everyone.
 
-setup(**setup_kwargs)
```


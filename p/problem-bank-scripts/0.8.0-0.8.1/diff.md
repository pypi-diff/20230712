# Comparing `tmp/problem_bank_scripts-0.8.0.tar.gz` & `tmp/problem_bank_scripts-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "problem_bank_scripts-0.8.0.tar", max compression
+gzip compressed data, was "problem_bank_scripts-0.8.1.tar", max compression
```

## Comparing `problem_bank_scripts-0.8.0.tar` & `problem_bank_scripts-0.8.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rwxr-xr-x   0        0        0        1 2021-05-16 14:07:02.985176 problem_bank_scripts-0.8.0/LICENSE
--rw-r--r--   0        0        0     1605 2023-06-15 01:42:11.784217 problem_bank_scripts-0.8.0/README.md
--rw-r--r--   0        0        0     1075 2023-07-12 05:18:16.217091 problem_bank_scripts-0.8.0/pyproject.toml
--rw-r--r--   0        0        0       59 2023-07-12 05:18:25.250411 problem_bank_scripts-0.8.0/src/problem_bank_scripts/__init__.py
--rw-r--r--   0        0        0     1757 2023-06-15 17:31:34.807559 problem_bank_scripts-0.8.0/src/problem_bank_scripts/attributions.json
--rw-r--r--   0        0        0    13614 2023-07-07 00:02:47.412321 problem_bank_scripts-0.8.0/src/problem_bank_scripts/prairielearn.py
--rw-r--r--   0        0        0    47688 2023-07-12 05:17:41.713889 problem_bank_scripts-0.8.0/src/problem_bank_scripts/problem_bank_scripts.py
--rw-r--r--   0        0        0      129 2022-06-24 05:48:29.289246 problem_bank_scripts-0.8.0/src/problem_bank_scripts/qti_export.py
--rw-r--r--   0        0        0    19225 2022-06-24 07:32:56.504377 problem_bank_scripts-0.8.0/src/problem_bank_scripts/webwork_to_md.py
--rw-r--r--   0        0        0     2644 2023-07-12 05:18:59.681901 problem_bank_scripts-0.8.0/setup.py
--rw-r--r--   0        0        0     2576 2023-07-12 05:18:59.682100 problem_bank_scripts-0.8.0/PKG-INFO
+-rwxr-xr-x   0        0        0        1 2021-05-16 14:07:02.985176 problem_bank_scripts-0.8.1/LICENSE
+-rw-r--r--   0        0        0     1605 2023-06-15 01:42:11.784217 problem_bank_scripts-0.8.1/README.md
+-rw-r--r--   0        0        0     1075 2023-07-12 05:37:37.250067 problem_bank_scripts-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0       59 2023-07-12 05:37:43.547248 problem_bank_scripts-0.8.1/src/problem_bank_scripts/__init__.py
+-rw-r--r--   0        0        0     1757 2023-06-15 17:31:34.807559 problem_bank_scripts-0.8.1/src/problem_bank_scripts/attributions.json
+-rw-r--r--   0        0        0    13614 2023-07-07 00:02:47.412321 problem_bank_scripts-0.8.1/src/problem_bank_scripts/prairielearn.py
+-rw-r--r--   0        0        0    47690 2023-07-12 05:37:04.899030 problem_bank_scripts-0.8.1/src/problem_bank_scripts/problem_bank_scripts.py
+-rw-r--r--   0        0        0      129 2022-06-24 05:48:29.289246 problem_bank_scripts-0.8.1/src/problem_bank_scripts/qti_export.py
+-rw-r--r--   0        0        0    19225 2022-06-24 07:32:56.504377 problem_bank_scripts-0.8.1/src/problem_bank_scripts/webwork_to_md.py
+-rw-r--r--   0        0        0     2644 2023-07-12 05:38:06.055988 problem_bank_scripts-0.8.1/setup.py
+-rw-r--r--   0        0        0     2576 2023-07-12 05:38:06.056204 problem_bank_scripts-0.8.1/PKG-INFO
```

### Comparing `problem_bank_scripts-0.8.0/README.md` & `problem_bank_scripts-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `problem_bank_scripts-0.8.0/pyproject.toml` & `problem_bank_scripts-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "problem_bank_scripts"
-version = "0.8.0"
+version = "0.8.1"
 description = "A package with useful functions to convert between different problem bank formats."
 authors = ["Open Problem Bank Team"]
 license = "MIT"
 readme = "README.md"
 documentation = "https://problem_bank_scripts.readthedocs.io/en/latest/"
 homepage = "https://github.com/open-resources/problem_bank_scripts"
 repository = "https://github.com/open-resources/problem_bank_scripts"
```

### Comparing `problem_bank_scripts-0.8.0/src/problem_bank_scripts/attributions.json` & `problem_bank_scripts-0.8.1/src/problem_bank_scripts/attributions.json`

 * *Files identical despite different names*

### Comparing `problem_bank_scripts-0.8.0/src/problem_bank_scripts/prairielearn.py` & `problem_bank_scripts-0.8.1/src/problem_bank_scripts/prairielearn.py`

 * *Files identical despite different names*

### Comparing `problem_bank_scripts-0.8.0/src/problem_bank_scripts/problem_bank_scripts.py` & `problem_bank_scripts-0.8.1/src/problem_bank_scripts/problem_bank_scripts.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 path = pathlib.Path().resolve().as_posix()
 topics = {"Template": "000.Template"}  # Start with special cased topics
 
 try:
     subjects = [path.split('instructor_')[1].split('_bank')[0]]
 except:
-    warnings.warn(f"\na subject could not be found from the path:\n'{path}'\ntopics from all subjects have been loaded.")
+    # warnings.warn(f"\na subject could not be found from the path:\n'{path}'\ntopics from all subjects have been loaded.")
     subjects = ["physics", "datascience", "stats"]
 
 for subject in subjects:
     url = f"https://raw.githubusercontent.com/open-resources/learning_outcomes/main/outputs_csv/LO_{subject}.csv"
     learning_outcomes = pd.read_csv(url)
     topics |= {topic: f"{i:03}.{topic}" for i, topic in enumerate(learning_outcomes["Topic"].unique(), start=1)}
```

### Comparing `problem_bank_scripts-0.8.0/src/problem_bank_scripts/webwork_to_md.py` & `problem_bank_scripts-0.8.1/src/problem_bank_scripts/webwork_to_md.py`

 * *Files identical despite different names*

### Comparing `problem_bank_scripts-0.8.0/setup.py` & `problem_bank_scripts-0.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'numpy>=1.22,<2.0',
  'pandas>=2.0,<3.0',
  'problem-bank-helpers>=0.1.14,<0.2.0',
  'sympy>=1.8,<2.0']
 
 setup_kwargs = {
     'name': 'problem-bank-scripts',
-    'version': '0.8.0',
+    'version': '0.8.1',
     'description': 'A package with useful functions to convert between different problem bank formats.',
     'long_description': '# Problem Bank Scripts \n\n[![Python](https://img.shields.io/badge/python-3.9-blue)]()\n[![codecov](https://codecov.io/gh/open-resources/problem_bank_scripts/branch/main/graph/badge.svg)](https://codecov.io/gh/open-resources/problem_bank_scripts)\n[![Documentation Status](https://readthedocs.org/projects/problem_bank_scripts/badge/?version=latest)](https://problem_bank_scripts.readthedocs.io/en/latest/?badge=latest)\n\n\n## Installation\n\n```bash\n$ pip install -i https://test.pypi.org/simple/ problem_bank_scripts\n```\n\n## Update version\n\nHere are the steps to increment the version (replace patch with major/minor/patch)\n\n```\npoetry version patch\n\npico src/problem_bank_scripts/__init__.py\n\npico tests/test_problem_bank_scripts.py\n\npoetry run pytest\n\ncd docs; poetry run make html; cd ..\n\ngit add .; git commit -m "increment version"; git push\n\npoetry build\n\npoetry publish\n```\n\n\n## Features\n\n- TODO\n\n## Dependencies\n\n- TODO\n\n## Usage\n\n- TODO\n\n## Documentation\n\nThe official documentation is hosted on Read the Docs: https://problem_bank_scripts.readthedocs.io/en/latest/\n\n## Contributors\n\nWe welcome and recognize all contributions. You can see a list of current contributors in the [contributors tab](https://github.com/open-resources/problem_bank_scripts/graphs/contributors).\n\n### Credits\n\nThis package was created with Cookiecutter and the UBC-MDS/cookiecutter-ubc-mds project template, modified from the [pyOpenSci/cookiecutter-pyopensci](https://github.com/pyOpenSci/cookiecutter-pyopensci) project template and the [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage).\n',
     'author': 'Open Problem Bank Team',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/open-resources/problem_bank_scripts',
```

### Comparing `problem_bank_scripts-0.8.0/PKG-INFO` & `problem_bank_scripts-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: problem-bank-scripts
-Version: 0.8.0
+Version: 0.8.1
 Summary: A package with useful functions to convert between different problem bank formats.
 Home-page: https://github.com/open-resources/problem_bank_scripts
 License: MIT
 Author: Open Problem Bank Team
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


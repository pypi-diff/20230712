# Comparing `tmp/problem_bank_scripts-0.7.1.tar.gz` & `tmp/problem_bank_scripts-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "problem_bank_scripts-0.7.1.tar", max compression
+gzip compressed data, was "problem_bank_scripts-0.8.0.tar", max compression
```

## Comparing `problem_bank_scripts-0.7.1.tar` & `problem_bank_scripts-0.8.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rwxr-xr-x   0        0        0        1 2021-05-16 14:07:02.985176 problem_bank_scripts-0.7.1/LICENSE
--rw-r--r--   0        0        0     1605 2023-06-15 01:42:11.784217 problem_bank_scripts-0.7.1/README.md
--rw-r--r--   0        0        0     1052 2023-07-10 22:54:12.853113 problem_bank_scripts-0.7.1/pyproject.toml
--rw-r--r--   0        0        0       59 2023-07-10 22:46:01.404559 problem_bank_scripts-0.7.1/src/problem_bank_scripts/__init__.py
--rw-r--r--   0        0        0     1757 2023-06-15 17:31:34.807559 problem_bank_scripts-0.7.1/src/problem_bank_scripts/attributions.json
--rw-r--r--   0        0        0    13614 2023-07-07 00:02:47.412321 problem_bank_scripts-0.7.1/src/problem_bank_scripts/prairielearn.py
--rw-r--r--   0        0        0    47476 2023-07-10 22:57:58.740430 problem_bank_scripts-0.7.1/src/problem_bank_scripts/problem_bank_scripts.py
--rw-r--r--   0        0        0      129 2022-06-24 05:48:29.289246 problem_bank_scripts-0.7.1/src/problem_bank_scripts/qti_export.py
--rw-r--r--   0        0        0    19225 2022-06-24 07:32:56.504377 problem_bank_scripts-0.7.1/src/problem_bank_scripts/webwork_to_md.py
--rw-r--r--   0        0        0     2644 2023-07-10 22:58:44.071882 problem_bank_scripts-0.7.1/setup.py
--rw-r--r--   0        0        0     2576 2023-07-10 22:58:44.072101 problem_bank_scripts-0.7.1/PKG-INFO
+-rwxr-xr-x   0        0        0        1 2021-05-16 14:07:02.985176 problem_bank_scripts-0.8.0/LICENSE
+-rw-r--r--   0        0        0     1605 2023-06-15 01:42:11.784217 problem_bank_scripts-0.8.0/README.md
+-rw-r--r--   0        0        0     1075 2023-07-12 05:18:16.217091 problem_bank_scripts-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0       59 2023-07-12 05:18:25.250411 problem_bank_scripts-0.8.0/src/problem_bank_scripts/__init__.py
+-rw-r--r--   0        0        0     1757 2023-06-15 17:31:34.807559 problem_bank_scripts-0.8.0/src/problem_bank_scripts/attributions.json
+-rw-r--r--   0        0        0    13614 2023-07-07 00:02:47.412321 problem_bank_scripts-0.8.0/src/problem_bank_scripts/prairielearn.py
+-rw-r--r--   0        0        0    47688 2023-07-12 05:17:41.713889 problem_bank_scripts-0.8.0/src/problem_bank_scripts/problem_bank_scripts.py
+-rw-r--r--   0        0        0      129 2022-06-24 05:48:29.289246 problem_bank_scripts-0.8.0/src/problem_bank_scripts/qti_export.py
+-rw-r--r--   0        0        0    19225 2022-06-24 07:32:56.504377 problem_bank_scripts-0.8.0/src/problem_bank_scripts/webwork_to_md.py
+-rw-r--r--   0        0        0     2644 2023-07-12 05:18:59.681901 problem_bank_scripts-0.8.0/setup.py
+-rw-r--r--   0        0        0     2576 2023-07-12 05:18:59.682100 problem_bank_scripts-0.8.0/PKG-INFO
```

### Comparing `problem_bank_scripts-0.7.1/README.md` & `problem_bank_scripts-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `problem_bank_scripts-0.7.1/pyproject.toml` & `problem_bank_scripts-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "problem_bank_scripts"
-version = "0.7.1"
+version = "0.8.0"
 description = "A package with useful functions to convert between different problem bank formats."
 authors = ["Open Problem Bank Team"]
 license = "MIT"
 readme = "README.md"
 documentation = "https://problem_bank_scripts.readthedocs.io/en/latest/"
 homepage = "https://github.com/open-resources/problem_bank_scripts"
 repository = "https://github.com/open-resources/problem_bank_scripts"
@@ -32,8 +32,8 @@
 myst-parser = "^0.17"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
-filterwarnings = ["ignore::DeprecationWarning"]
+filterwarnings = ["ignore::DeprecationWarning", "ignore::UserWarning"]
```

### Comparing `problem_bank_scripts-0.7.1/src/problem_bank_scripts/attributions.json` & `problem_bank_scripts-0.8.0/src/problem_bank_scripts/attributions.json`

 * *Files identical despite different names*

### Comparing `problem_bank_scripts-0.7.1/src/problem_bank_scripts/prairielearn.py` & `problem_bank_scripts-0.8.0/src/problem_bank_scripts/prairielearn.py`

 * *Files identical despite different names*

### Comparing `problem_bank_scripts-0.7.1/src/problem_bank_scripts/problem_bank_scripts.py` & `problem_bank_scripts-0.8.0/src/problem_bank_scripts/problem_bank_scripts.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,26 +28,28 @@
 ## Dealing with YAML
 import yaml
 
 ## Loading files : https://stackoverflow.com/a/60687710
 import importlib.resources
 
 ## Topic Validation
-topic_list = set()
-path = pathlib.Path().resolve()
+
+path = pathlib.Path().resolve().as_posix()
+topics = {"Template": "000.Template"}  # Start with special cased topics
+
 try:
     subjects = [path.split('instructor_')[1].split('_bank')[0]]
 except:
     warnings.warn(f"\na subject could not be found from the path:\n'{path}'\ntopics from all subjects have been loaded.")
     subjects = ["physics", "datascience", "stats"]
 
 for subject in subjects:
     url = f"https://raw.githubusercontent.com/open-resources/learning_outcomes/main/outputs_csv/LO_{subject}.csv"
     learning_outcomes = pd.read_csv(url)
-    topic_list |= set(learning_outcomes["Topic"])
+    topics |= {topic: f"{i:03}.{topic}" for i, topic in enumerate(learning_outcomes["Topic"].unique(), start=1)}
 
 # Start of reading/parsing functions
 
 
 def defdict_to_dict(defdict, finaldict):
     """Convert a defaultdict (nested) to a regular dictionary.
         - Answer copied from: https://stackoverflow.com/a/61133504/2217577
@@ -101,15 +103,15 @@
     nested_dict[part]["title"] = tokens[level2_headers[0] + 1].content
 
     # Store the content of the level 2 header
     try:
         content = mdformat.renderer.MDRenderer().render(
                 tokens[3 : get_next_headerloc(3, tokens, 3)], mdit.options, env
             )  # Note the 3 is there to exclude header start,header content,header end tokens
-        nested_dict[part]["content"] = content
+        nested_dict[part]["content"] = content.replace(r"\\", "\\")
     except IndexError:
         print("It looks like there is an empty section of header level 2 in your md file.")
         raise
 
     # Get all Level 3 headers
     level3_headers = [i for i, j in enumerate(tokens) if j.tag == "h3" if j.nesting == 1]
 
@@ -343,15 +345,15 @@
     body_parts = {}
     parts_dict = {}
 
     part_counter = 0
 
     for k, v in blocks.items():
 
-        rendered_part = mdformat.renderer.MDRenderer().render(tokens[v[0] : v[1]], mdit.options, env)
+        rendered_part = mdformat.renderer.MDRenderer().render(tokens[v[0] : v[1]], mdit.options, env).replace(r"\\", "\\")
 
         if k == "title":
             body_parts["title"] = rendered_part
 
         elif k == "preamble":
             body_parts["preamble"] = rendered_part
 
@@ -698,21 +700,21 @@
 
     options = ''
     statements = ''
     ## Note: `|@`` gets converted into `{{` and `@|`` gets converted to `}}` by `replace_tags()`
     for a in data_dict["params"][f"{part_name}"].keys():
 
         if "option" in a:
-            value = f"|@ params.{part_name}.{a}.value @|"
+            value = f"|@|@ params.{part_name}.{a}.value @|@|"
 
-            options += f"\t<pl-option name= '{a}' > {value} </pl-option>\n"
+            options += f"\t<pl-option> {value} </pl-option>\n"
 
         if "statement" in a:
             matches_with = f"|@ params.{part_name}.{a}.matches @|"
-            value = f"|@ params.{part_name}.{a}.value @|"
+            value = f"|@|@ params.{part_name}.{a}.value @|@|"
 
             statements += f"\t<pl-statement match= '{matches_with}' > {value} </pl-statement>\n"
 
     html += statements
     html += options
 
     html += "</pl-matching>\n"
@@ -948,15 +950,15 @@
 
         # Write the YAML to a file
         output_path.parent.mkdir(parents=True, exist_ok=True)
         output_path.write_text(
             "---\n"
             + header_yml
             + "---\n"
-            + text.replace(r"\\", "\\")
+            + text
             + "\n## Attribution\n\n"
             + process_attribution(header.get("attribution")),
             encoding="utf8",
         )
 
         ####################################################
         #### End Temporary Fix for issue of myst no longer permitting nested dicts
@@ -1002,17 +1004,15 @@
 
         # Write the YAML to a file
         output_path.parent.mkdir(parents=True, exist_ok=True)
         output_path.write_text(
             "---\n"
             + header_yml
             + "\n---\n"
-            + dict_to_md(
-                body_parts,
-            ).replace(r"\\", "\\")
+            + dict_to_md(body_parts)
             + "\n## Attribution\n\n"
             + process_attribution(header.get("attribution")),
             encoding="utf8",
         )
 
     # Move image assets
     files_to_copy = header.get("assets")
@@ -1044,14 +1044,15 @@
             raise NotImplementedError("Check the source filepath; it does not have 'source' in it!! ")
     else:
         ## TODO: It's annoying that here output_path.parent is used, but for md problems, it's just output_path
         output_path = pathlib.Path(output_path).parent
 
     # Parse the MD file
     parsed_q = read_md_problem(source_filepath)
+    parsed_q["header"]["topic"] = topics[parsed_q["header"]["topic"]] # Add integer topic id, this is safe because we validated the header in read_md_problem
 
     # Create output dir if it doesn't exist
     output_path.mkdir(parents=True, exist_ok=True)
 
     #################################################################################
     # Run the python code; this improved way was suggested by Phil Austin of UBC EOAS
 
@@ -1243,10 +1244,10 @@
     )  # Remove empty highlight-lines attributes
     html = re.sub(r"(?<!\\)`(?P<Code>[^`]+)`", r"<code>\g<Code></code>", html)
     html = html.replace("\\`", "`")  # Replace escaped backticks
     return html
 
 def validate_header(header_dict):
     # check if topic is valid (i.e. from the list of topics in the learning_outcomes repo for this subject)
-    if header_dict["topic"] not in topic_list and header_dict["topic"] != "Template":
-        raise ValueError(f"topic '{header_dict['topic']}' is not listed in the learning outcomes")
-        
+    
+    if topics.get(topic := header_dict["topic"], None) is None:
+        raise ValueError(f"topic '{topic}' is not listed in the learning outcomes")
```

### Comparing `problem_bank_scripts-0.7.1/src/problem_bank_scripts/webwork_to_md.py` & `problem_bank_scripts-0.8.0/src/problem_bank_scripts/webwork_to_md.py`

 * *Files identical despite different names*

### Comparing `problem_bank_scripts-0.7.1/setup.py` & `problem_bank_scripts-0.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'numpy>=1.22,<2.0',
  'pandas>=2.0,<3.0',
  'problem-bank-helpers>=0.1.14,<0.2.0',
  'sympy>=1.8,<2.0']
 
 setup_kwargs = {
     'name': 'problem-bank-scripts',
-    'version': '0.7.1',
+    'version': '0.8.0',
     'description': 'A package with useful functions to convert between different problem bank formats.',
     'long_description': '# Problem Bank Scripts \n\n[![Python](https://img.shields.io/badge/python-3.9-blue)]()\n[![codecov](https://codecov.io/gh/open-resources/problem_bank_scripts/branch/main/graph/badge.svg)](https://codecov.io/gh/open-resources/problem_bank_scripts)\n[![Documentation Status](https://readthedocs.org/projects/problem_bank_scripts/badge/?version=latest)](https://problem_bank_scripts.readthedocs.io/en/latest/?badge=latest)\n\n\n## Installation\n\n```bash\n$ pip install -i https://test.pypi.org/simple/ problem_bank_scripts\n```\n\n## Update version\n\nHere are the steps to increment the version (replace patch with major/minor/patch)\n\n```\npoetry version patch\n\npico src/problem_bank_scripts/__init__.py\n\npico tests/test_problem_bank_scripts.py\n\npoetry run pytest\n\ncd docs; poetry run make html; cd ..\n\ngit add .; git commit -m "increment version"; git push\n\npoetry build\n\npoetry publish\n```\n\n\n## Features\n\n- TODO\n\n## Dependencies\n\n- TODO\n\n## Usage\n\n- TODO\n\n## Documentation\n\nThe official documentation is hosted on Read the Docs: https://problem_bank_scripts.readthedocs.io/en/latest/\n\n## Contributors\n\nWe welcome and recognize all contributions. You can see a list of current contributors in the [contributors tab](https://github.com/open-resources/problem_bank_scripts/graphs/contributors).\n\n### Credits\n\nThis package was created with Cookiecutter and the UBC-MDS/cookiecutter-ubc-mds project template, modified from the [pyOpenSci/cookiecutter-pyopensci](https://github.com/pyOpenSci/cookiecutter-pyopensci) project template and the [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage).\n',
     'author': 'Open Problem Bank Team',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/open-resources/problem_bank_scripts',
```

### Comparing `problem_bank_scripts-0.7.1/PKG-INFO` & `problem_bank_scripts-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: problem-bank-scripts
-Version: 0.7.1
+Version: 0.8.0
 Summary: A package with useful functions to convert between different problem bank formats.
 Home-page: https://github.com/open-resources/problem_bank_scripts
 License: MIT
 Author: Open Problem Bank Team
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


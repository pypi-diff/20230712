# Comparing `tmp/virtue-2023.5.3.tar.gz` & `tmp/virtue-2023.7.2.tar.gz`

## Comparing `virtue-2023.5.3.tar` & `virtue-2023.7.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 virtue-2023.5.3/.coveragerc
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 virtue-2023.5.3/.flake8
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 virtue-2023.5.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 virtue-2023.5.3/.readthedocs.yml
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 virtue-2023.5.3/.testr.conf
--rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 virtue-2023.5.3/noxfile.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 virtue-2023.5.3/.github/FUNDING.yml
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 virtue-2023.5.3/.github/SECURITY.md
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 virtue-2023.5.3/.github/dependabot.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 virtue-2023.5.3/.github/release.yml
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 virtue-2023.5.3/.github/workflows/ci.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 virtue-2023.5.3/docs/Makefile
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 virtue-2023.5.3/docs/api.rst
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 virtue-2023.5.3/docs/conf.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 virtue-2023.5.3/docs/index.rst
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 virtue-2023.5.3/docs/requirements.in
--rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 virtue-2023.5.3/docs/requirements.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 virtue-2023.5.3/docs/spelling-wordlist.txt
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/__init__.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/__main__.py
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/_cli.py
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/loaders.py
--rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/locators.py
--rw-r--r--   0        0        0    15025 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/reporters.py
--rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/__init__.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/test_cli.py
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/test_loaders.py
--rw-r--r--   0        0        0     7246 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/test_locators.py
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/test_reporters.py
--rw-r--r--   0        0        0    12351 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/test_runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/samples/__init__.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/samples/dynamic_test.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/samples/failures_and_errors.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/samples/failures_and_unexpected_passes.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/samples/mixin.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/samples/module_for_TestLoaders.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/samples/module_for_TestObjectLocator.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/samples/module_with_exception.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/samples/no_tests.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/samples/one_expected_failure.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/samples/one_expected_failure_mispassing.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/samples/one_successful_test.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/samples/one_unsuccessful_test.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/samples/repeated_similar_output.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/samples/subtests.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/samples/success_and_warning.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/samples/two_unsuccessful_tests.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 virtue-2023.5.3/COPYING
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 virtue-2023.5.3/README.rst
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 virtue-2023.5.3/pyproject.toml
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 virtue-2023.5.3/PKG-INFO
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 virtue-2023.7.2/.coveragerc
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 virtue-2023.7.2/.flake8
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 virtue-2023.7.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 virtue-2023.7.2/.readthedocs.yml
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 virtue-2023.7.2/.testr.conf
+-rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 virtue-2023.7.2/noxfile.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 virtue-2023.7.2/.github/FUNDING.yml
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 virtue-2023.7.2/.github/SECURITY.md
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 virtue-2023.7.2/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 virtue-2023.7.2/.github/release.yml
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 virtue-2023.7.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 virtue-2023.7.2/docs/Makefile
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 virtue-2023.7.2/docs/api.rst
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 virtue-2023.7.2/docs/conf.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 virtue-2023.7.2/docs/index.rst
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 virtue-2023.7.2/docs/requirements.in
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 virtue-2023.7.2/docs/requirements.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 virtue-2023.7.2/docs/spelling-wordlist.txt
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/__init__.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/__main__.py
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/_cli.py
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/loaders.py
+-rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/locators.py
+-rw-r--r--   0        0        0    15025 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/reporters.py
+-rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/__init__.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/test_cli.py
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/test_loaders.py
+-rw-r--r--   0        0        0     7246 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/test_locators.py
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/test_reporters.py
+-rw-r--r--   0        0        0    12351 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/test_runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/samples/__init__.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/samples/dynamic_test.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/samples/failures_and_errors.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/samples/failures_and_unexpected_passes.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/samples/mixin.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/samples/module_for_TestLoaders.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/samples/module_for_TestObjectLocator.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/samples/module_with_exception.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/samples/no_tests.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/samples/one_expected_failure.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/samples/one_expected_failure_mispassing.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/samples/one_successful_test.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/samples/one_unsuccessful_test.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/samples/repeated_similar_output.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/samples/subtests.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/samples/success_and_warning.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 virtue-2023.7.2/virtue/tests/samples/two_unsuccessful_tests.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 virtue-2023.7.2/COPYING
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 virtue-2023.7.2/README.rst
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 virtue-2023.7.2/pyproject.toml
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 virtue-2023.7.2/PKG-INFO
```

### Comparing `virtue-2023.5.3/.flake8` & `virtue-2023.7.2/.flake8`

 * *Files identical despite different names*

### Comparing `virtue-2023.5.3/.pre-commit-config.yaml` & `virtue-2023.7.2/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -7,25 +7,25 @@
       - id: check-vcs-permalinks
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
         args: [--fix, lf]
       - id: trailing-whitespace
-  - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: "v0.0.270"
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: "v0.0.277"
     hooks:
       - id: ruff
   - repo: https://github.com/PyCQA/isort
     rev: 5.12.0
     hooks:
       - id: isort
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - name: black
         id: black
         args: ["--line-length", "79"]
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: "v3.0.0-alpha.9-for-vscode"
+    rev: "v3.0.0"
     hooks:
       - id: prettier
```

### Comparing `virtue-2023.5.3/noxfile.py` & `virtue-2023.7.2/noxfile.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from pathlib import Path
+from tempfile import TemporaryDirectory
 import os
 
 import nox
 
 ROOT = Path(__file__).parent
 PYPROJECT = ROOT / "pyproject.toml"
 DOCS = ROOT / "docs"
@@ -54,25 +55,18 @@
 def audit(session):
     session.install("pip_audit", ROOT)
     session.run("python", "-m", "pip_audit")
 
 
 @session(tags=["build"])
 def build(session):
-    session.install("build")
-    tmpdir = session.create_tmp()
-    session.run("python", "-m", "build", ROOT, "--outdir", tmpdir)
-
-
-@session(tags=["style"])
-def readme(session):
     session.install("build", "twine")
-    tmpdir = session.create_tmp()
-    session.run("python", "-m", "build", ROOT, "--outdir", tmpdir)
-    session.run("python", "-m", "twine", "check", "--strict", tmpdir + "/*")
+    with TemporaryDirectory() as tmpdir:
+        session.run("python", "-m", "build", ROOT, "--outdir", tmpdir)
+        session.run("twine", "check", "--strict", tmpdir + "/*")
 
 
 @session()
 def secrets(session):
     session.install("detect-secrets")
     session.run("detect-secrets", "scan", ROOT)
 
@@ -101,28 +95,29 @@
             "man",
             "spelling",
         ]
     ],
 )
 def docs(session, builder):
     session.install("-r", DOCS / "requirements.txt")
-    tmpdir = Path(session.create_tmp())
-    argv = ["-n", "-T", "-W"]
-    if builder != "spelling":
-        argv += ["-q"]
-    session.run(
-        "python",
-        "-m",
-        "sphinx",
-        "-b",
-        builder,
-        DOCS,
-        tmpdir / builder,
-        *argv,
-    )
+    with TemporaryDirectory() as tmpdir_str:
+        tmpdir = Path(tmpdir_str)
+        argv = ["-n", "-T", "-W"]
+        if builder != "spelling":
+            argv += ["-q"]
+        session.run(
+            "python",
+            "-m",
+            "sphinx",
+            "-b",
+            builder,
+            DOCS,
+            tmpdir / builder,
+            *argv,
+        )
 
 
 @session(tags=["docs", "style"], name="docs(style)")
 def docs_style(session):
     session.install(
         "doc8",
         "pygments",
```

### Comparing `virtue-2023.5.3/.github/SECURITY.md` & `virtue-2023.7.2/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `virtue-2023.5.3/.github/workflows/ci.yml` & `virtue-2023.7.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `virtue-2023.5.3/docs/Makefile` & `virtue-2023.7.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `virtue-2023.5.3/docs/conf.py` & `virtue-2023.7.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.5.3/docs/requirements.txt` & `virtue-2023.7.2/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `virtue-2023.5.3/virtue/_cli.py` & `virtue-2023.7.2/virtue/_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                 Reporter = resolve_name(value)
             except (ValueError, ImportError, AttributeError):
                 raise click.BadParameter(f"{value!r} is not a known reporter")
 
         return Reporter()
 
 
-@click.command(context_settings=dict(help_option_names=["-h", "--help"]))
+@click.command(context_settings=dict(help_option_names=["-h", "--help"]))  # type: ignore[arg-type]  # noqa: E501
 @click.version_option(prog_name="virtue")
 @click.option(
     "--reporter",
     default="default",
     help=dedent(
         """
         the name of a reporter to use for outputting test results.
```

### Comparing `virtue-2023.5.3/virtue/loaders.py` & `virtue-2023.7.2/virtue/loaders.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.5.3/virtue/locators.py` & `virtue-2023.7.2/virtue/locators.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.5.3/virtue/reporters.py` & `virtue-2023.7.2/virtue/reporters.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.5.3/virtue/runner.py` & `virtue-2023.7.2/virtue/runner.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.5.3/virtue/tests/test_cli.py` & `virtue-2023.7.2/virtue/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.5.3/virtue/tests/test_loaders.py` & `virtue-2023.7.2/virtue/tests/test_loaders.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.5.3/virtue/tests/test_locators.py` & `virtue-2023.7.2/virtue/tests/test_locators.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.5.3/virtue/tests/test_reporters.py` & `virtue-2023.7.2/virtue/tests/test_reporters.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.5.3/virtue/tests/test_runner.py` & `virtue-2023.7.2/virtue/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.5.3/virtue/tests/samples/subtests.py` & `virtue-2023.7.2/virtue/tests/samples/subtests.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.5.3/COPYING` & `virtue-2023.7.2/COPYING`

 * *Files identical despite different names*

### Comparing `virtue-2023.5.3/README.rst` & `virtue-2023.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `virtue-2023.5.3/pyproject.toml` & `virtue-2023.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `virtue-2023.5.3/PKG-INFO` & `virtue-2023.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virtue
-Version: 2023.5.3
+Version: 2023.7.2
 Summary: After trial comes virtue. A test runner for good.
 Project-URL: Homepage, https://github.com/Julian/Virtue
 Project-URL: Documentation, https://virtue.readthedocs.io/
 Project-URL: Issues, https://github.com/Julian/Virtue/issues/
 Project-URL: Funding, https://github.com/sponsors/Julian
 Project-URL: Source, https://github.com/Julian/Virtue
 Author: Julian Berman
```


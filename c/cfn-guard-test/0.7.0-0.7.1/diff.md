# Comparing `tmp/cfn_guard_test-0.7.0.tar.gz` & `tmp/cfn_guard_test-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfn_guard_test-0.7.0.tar", max compression
+gzip compressed data, was "cfn_guard_test-0.7.1.tar", max compression
```

## Comparing `cfn_guard_test-0.7.0.tar` & `cfn_guard_test-0.7.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1052 2023-06-15 14:00:59.241530 cfn_guard_test-0.7.0/LICENSE.md
--rw-r--r--   0        0        0     3144 2023-06-15 14:01:00.009542 cfn_guard_test-0.7.0/cfn_guard_test/__init__.py
--rw-r--r--   0        0        0     2379 2023-06-15 14:00:59.241530 cfn_guard_test-0.7.0/cfn_guard_test/case.py
--rw-r--r--   0        0        0     2781 2023-06-15 14:00:59.241530 cfn_guard_test-0.7.0/cfn_guard_test/reader.py
--rw-r--r--   0        0        0     2412 2023-06-15 14:00:59.241530 cfn_guard_test-0.7.0/cfn_guard_test/report.py
--rw-r--r--   0        0        0     1135 2023-06-15 14:00:59.241530 cfn_guard_test-0.7.0/cfn_guard_test/rule.py
--rw-r--r--   0        0        0     1962 2023-06-15 14:00:59.241530 cfn_guard_test-0.7.0/cfn_guard_test/runner.py
--rw-r--r--   0        0        0     2317 2023-06-15 14:00:59.241530 cfn_guard_test-0.7.0/cfn_guard_test/suite.py
--rw-r--r--   0        0        0     1835 2023-06-15 14:00:59.241530 cfn_guard_test-0.7.0/cfn_guard_test/suites.py
--rw-r--r--   0        0        0      950 2023-06-15 14:01:00.009542 cfn_guard_test-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      644 1970-01-01 00:00:00.000000 cfn_guard_test-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1052 2023-07-12 13:21:10.956774 cfn_guard_test-0.7.1/LICENSE.md
+-rw-r--r--   0        0        0     3118 2023-07-12 13:21:11.744785 cfn_guard_test-0.7.1/cfn_guard_test/__init__.py
+-rw-r--r--   0        0        0     2379 2023-07-12 13:21:10.956774 cfn_guard_test-0.7.1/cfn_guard_test/case.py
+-rw-r--r--   0        0        0     2781 2023-07-12 13:21:10.956774 cfn_guard_test-0.7.1/cfn_guard_test/reader.py
+-rw-r--r--   0        0        0     2411 2023-07-12 13:21:10.956774 cfn_guard_test-0.7.1/cfn_guard_test/report.py
+-rw-r--r--   0        0        0     1135 2023-07-12 13:21:10.956774 cfn_guard_test-0.7.1/cfn_guard_test/rule.py
+-rw-r--r--   0        0        0     1962 2023-07-12 13:21:10.956774 cfn_guard_test-0.7.1/cfn_guard_test/runner.py
+-rw-r--r--   0        0        0     2317 2023-07-12 13:21:10.956774 cfn_guard_test-0.7.1/cfn_guard_test/suite.py
+-rw-r--r--   0        0        0     1835 2023-07-12 13:21:10.956774 cfn_guard_test-0.7.1/cfn_guard_test/suites.py
+-rw-r--r--   0        0        0      950 2023-07-12 13:21:11.744785 cfn_guard_test-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      644 1970-01-01 00:00:00.000000 cfn_guard_test-0.7.1/PKG-INFO
```

### Comparing `cfn_guard_test-0.7.0/LICENSE.md` & `cfn_guard_test-0.7.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cfn_guard_test-0.7.0/cfn_guard_test/__init__.py` & `cfn_guard_test-0.7.1/cfn_guard_test/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from cfn_guard_test.rule import CfnGuardRule
 from cfn_guard_test.runner import CfnGuardRunner
 from cfn_guard_test.suite import CfnGuardTestSuite
 from cfn_guard_test.suites import CfnGuardTestSuites
 from cfn_guard_test.reader import CfnGuardReader
 
 
-__version__ = "0.7.0"
+__version__ = "0.7.1"
 
 
 def validate_cfn_guard_path(
     ctx: click.Context, _: click.Option, value: Optional[str]
 ) -> str:
     if not value or ctx.resilient_parsing:
         return "cfn-guard"
@@ -34,29 +34,28 @@
 
     return value
 
 
 def validate_writable_path(
     ctx: click.Context, _: click.Option, value: Optional[str]
 ) -> Optional[str]:
-
     try:
         if value:
             with open(value, "w") as fh:
                 if not fh.writable():
                     raise Exception()
     except FileNotFoundError:
         raise click.ClickException(f"The given path is not writable: {value}")
     except Exception:
         raise click.ClickException(f"The given path is not writable: {value}")
 
     return value
 
 
-@click.command()
+@click.command()  # type: ignore
 @click.option("-r", "--rules-path", callback=resolve_paths)
 @click.option("-t", "--test-path", callback=resolve_paths)
 @click.option("--cfn-guard-path", callback=validate_cfn_guard_path)
 @click.option("--junit-path", callback=validate_writable_path)
 @click.option("-v", "--verbose", count=True)
 def main(
     rules_path: str,
@@ -88,15 +87,14 @@
     click.echo(f"Failed {suites.failed}")
     click.echo(f"Passed {suites.passed}")
     click.echo()
     display_failures_errors(suites)
 
 
 def display_failures_errors(suites: CfnGuardTestSuites) -> None:
-
     if suites.errors:
         click.echo(click.style("Errors:", bold=True))
         list(map(click.echo, suites.error_messages))
         click.echo()
 
     if suites.failed:
         click.echo(click.style("Failures:", bold=True))
@@ -105,11 +103,7 @@
 
     if suites.errors or suites.failed:
         exit(1)
 
 
 def resolve_output_callback(verbose) -> Optional[Callable[[str], None]]:
     return click.echo if verbose else None
-
-
-if __name__ == "__main__":
-    main()
```

### Comparing `cfn_guard_test-0.7.0/cfn_guard_test/case.py` & `cfn_guard_test-0.7.1/cfn_guard_test/case.py`

 * *Files identical despite different names*

### Comparing `cfn_guard_test-0.7.0/cfn_guard_test/reader.py` & `cfn_guard_test-0.7.1/cfn_guard_test/reader.py`

 * *Files identical despite different names*

### Comparing `cfn_guard_test-0.7.0/cfn_guard_test/report.py` & `cfn_guard_test-0.7.1/cfn_guard_test/report.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
     """
     Understands how to create reports
     """
 
     __suites: List[TestSuite]
 
     def __init__(self, suites: CfnGuardTestSuites):
-
         self.__suites = []
 
         for suite in suites.all_suites:
             self.__timestamp = suite.duration
 
             self.__suites.append(
                 TestSuite(
```

### Comparing `cfn_guard_test-0.7.0/cfn_guard_test/rule.py` & `cfn_guard_test-0.7.1/cfn_guard_test/rule.py`

 * *Files identical despite different names*

### Comparing `cfn_guard_test-0.7.0/cfn_guard_test/runner.py` & `cfn_guard_test-0.7.1/cfn_guard_test/runner.py`

 * *Files identical despite different names*

### Comparing `cfn_guard_test-0.7.0/cfn_guard_test/suite.py` & `cfn_guard_test-0.7.1/cfn_guard_test/suite.py`

 * *Files identical despite different names*

### Comparing `cfn_guard_test-0.7.0/cfn_guard_test/suites.py` & `cfn_guard_test-0.7.1/cfn_guard_test/suites.py`

 * *Files identical despite different names*

### Comparing `cfn_guard_test-0.7.0/pyproject.toml` & `cfn_guard_test-0.7.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [tool.poetry]
 name = "cfn-guard-test"
-version = "0.7.0"
+version = "0.7.1"
 description = "cfn-guard-test is a wrapper for cfn-guard that allows you to run unit tests for your cfn-guard rules."
 authors = ["Joris Conijn <joris@conijnonline.nl>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 junit-xml = "^1.9"
 click = "^8.0.3"
 
 [tool.poetry.dev-dependencies]
-black = "^23.3"
-mypy = "^1.3"
-pytest = "^7.3.2"
+black = "^23.7"
+mypy = "^1.4"
+pytest = "^7.4.0"
 pytest-cov = "^4.1.0"
 pytest-mypy = "^0.10.3"
 toml = "^0.10.2"
 types-toml = "^0.10.8"
 xenon = "^0.9.0"
 radon = "^5.1.0"
-python-semantic-release = "^7.34.4"
+python-semantic-release = "^7.34.6"
 
 [tool.poetry.scripts]
 cfn-guard-test = "cfn_guard_test:main"
 
 [tool.semantic_release]
 version_variable = [
     "cfn_guard_test/__init__.py:__version__",
```

### Comparing `cfn_guard_test-0.7.0/PKG-INFO` & `cfn_guard_test-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfn-guard-test
-Version: 0.7.0
+Version: 0.7.1
 Summary: cfn-guard-test is a wrapper for cfn-guard that allows you to run unit tests for your cfn-guard rules.
 License: MIT
 Author: Joris Conijn
 Author-email: joris@conijnonline.nl
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


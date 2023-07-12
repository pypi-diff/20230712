# Comparing `tmp/fastchecks-0.2.1rc2.tar.gz` & `tmp/fastchecks-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastchecks-0.2.1rc2.tar", max compression
+gzip compressed data, was "fastchecks-0.2.2.tar", max compression
```

## Comparing `fastchecks-0.2.1rc2.tar` & `fastchecks-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    11357 2023-07-11 10:41:01.033771 fastchecks-0.2.1rc2/LICENSE
--rw-r--r--   0        0        0     5033 2023-07-11 11:48:52.604708 fastchecks-0.2.1rc2/README.md
--rw-r--r--   0        0        0      569 2023-07-11 10:41:01.034019 fastchecks-0.2.1rc2/fastchecks/NOTICE
--rw-r--r--   0        0        0      707 2023-07-11 07:04:21.284270 fastchecks-0.2.1rc2/fastchecks/__init__.py
--rw-r--r--   0        0        0     4718 2023-07-11 09:12:31.872942 fastchecks-0.2.1rc2/fastchecks/check.py
--rw-r--r--   0        0        0    12259 2023-07-11 11:48:52.605005 fastchecks-0.2.1rc2/fastchecks/cli.py
--rw-r--r--   0        0        0     3165 2023-07-11 11:48:52.605178 fastchecks-0.2.1rc2/fastchecks/conf.py
--rw-r--r--   0        0        0      874 2023-07-11 09:12:31.873625 fastchecks-0.2.1rc2/fastchecks/log.py
--rw-r--r--   0        0        0      892 2023-07-11 10:41:00.994931 fastchecks-0.2.1rc2/fastchecks/meta.py
--rw-r--r--   0        0        0     6992 2023-07-11 11:36:08.255245 fastchecks-0.2.1rc2/fastchecks/runner.py
--rw-r--r--   0        0        0     3166 2023-07-11 09:12:31.874127 fastchecks-0.2.1rc2/fastchecks/sockets/__init__.py
--rw-r--r--   0        0        0     6330 2023-07-11 09:12:31.874318 fastchecks-0.2.1rc2/fastchecks/sockets/postgres/__init__.py
--rw-r--r--   0        0        0      539 2023-07-11 09:12:31.874566 fastchecks-0.2.1rc2/fastchecks/sockets/postgres/schema/down.sql
--rw-r--r--   0        0        0     2122 2023-07-09 17:17:25.645446 fastchecks-0.2.1rc2/fastchecks/sockets/postgres/schema/up.sql
--rw-r--r--   0        0        0     6174 2023-07-11 09:12:31.874817 fastchecks-0.2.1rc2/fastchecks/types.py
--rw-r--r--   0        0        0     3264 2023-07-10 18:11:32.678072 fastchecks-0.2.1rc2/fastchecks/util.py
--rw-r--r--   0        0        0     3866 2023-07-11 09:12:31.875063 fastchecks-0.2.1rc2/fastchecks/vutil.py
--rw-r--r--   0        0        0     1978 2023-07-11 11:49:32.742553 fastchecks-0.2.1rc2/pyproject.toml
--rw-r--r--   0        0        0     5707 1970-01-01 00:00:00.000000 fastchecks-0.2.1rc2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-11 10:41:01.033771 fastchecks-0.2.2/LICENSE
+-rw-r--r--   0        0        0      569 2023-07-12 12:48:59.063130 fastchecks-0.2.2/NOTICE
+-rw-r--r--   0        0        0     5355 2023-07-12 12:48:59.063381 fastchecks-0.2.2/README.md
+-rw-r--r--   0        0        0      707 2023-07-11 07:04:21.284270 fastchecks-0.2.2/fastchecks/__init__.py
+-rw-r--r--   0        0        0     4718 2023-07-11 09:12:31.872942 fastchecks-0.2.2/fastchecks/check.py
+-rw-r--r--   0        0        0    12259 2023-07-11 12:00:38.514751 fastchecks-0.2.2/fastchecks/cli.py
+-rw-r--r--   0        0        0     3165 2023-07-11 12:00:38.515268 fastchecks-0.2.2/fastchecks/conf.py
+-rw-r--r--   0        0        0      874 2023-07-11 09:12:31.873625 fastchecks-0.2.2/fastchecks/log.py
+-rw-r--r--   0        0        0      995 2023-07-12 12:48:59.063620 fastchecks-0.2.2/fastchecks/meta.py
+-rw-r--r--   0        0        0     6992 2023-07-11 11:36:08.255245 fastchecks-0.2.2/fastchecks/runner.py
+-rw-r--r--   0        0        0     3166 2023-07-11 09:12:31.874127 fastchecks-0.2.2/fastchecks/sockets/__init__.py
+-rw-r--r--   0        0        0     6330 2023-07-11 09:12:31.874318 fastchecks-0.2.2/fastchecks/sockets/postgres/__init__.py
+-rw-r--r--   0        0        0      539 2023-07-11 09:12:31.874566 fastchecks-0.2.2/fastchecks/sockets/postgres/schema/down.sql
+-rw-r--r--   0        0        0     2122 2023-07-09 17:17:25.645446 fastchecks-0.2.2/fastchecks/sockets/postgres/schema/up.sql
+-rw-r--r--   0        0        0     6174 2023-07-11 09:12:31.874817 fastchecks-0.2.2/fastchecks/types.py
+-rw-r--r--   0        0        0     3264 2023-07-10 18:11:32.678072 fastchecks-0.2.2/fastchecks/util.py
+-rw-r--r--   0        0        0     4706 2023-07-12 12:48:59.063886 fastchecks-0.2.2/fastchecks/vutil.py
+-rw-r--r--   0        0        0     2114 2023-07-12 12:48:59.103408 fastchecks-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     6109 1970-01-01 00:00:00.000000 fastchecks-0.2.2/PKG-INFO
```

### Comparing `fastchecks-0.2.1rc2/LICENSE` & `fastchecks-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastchecks-0.2.1rc2/README.md` & `fastchecks-0.2.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -6,19 +6,25 @@
 [![Snyk](https://img.shields.io/badge/%20Snyk_security-monitored-8742B8?logo=snyk&logoColor=white)](https://github.com/juanmirocks/fastchecks/actions)
 
 
 
 ## Features
 
 **🍀 Feature-rich**
+* Each check tracks:
+  * timestamp
+  * response time
+  * HTTP response status code
+  * optionally, given regex is (safely) tested if it matches the response body or not
+  * info about possible connection errors, like timeouts and/or unreachable host
 * Websites to check & their results are stored in postgres by default 🐘 (the library is ready for other data stores / sockets).
   * You can use postgres locally installed, running on docker, or with a DBaaS, e.g. Aiven.
-* Run stored all websites once, at configurable-scheduled intervals, or even with your system's cron.
-* The scheduling keeps running even if the computer goes to sleep!
-* Nice, configurable logging
+* Monitor stored websites once, at configurable-scheduled intervals (each website check can use an independent interval or use a default), or even with your system's cron.
+* The scheduling keeps running even if the computer goes to sleep.
+* Nice, configurable logging.
 * CLI API & Python's (Python >= 3.11).
   * A [webserver](https://github.com/juanmirocks/fastchecks/issues/3) is planned.
 * ...and more!
 
 
 **🚀 Speed**
 * All operations are asynchronous. This app sits on 3 giants:
@@ -39,23 +45,23 @@
 * Further type checking with Pydantic (v2).
 * Further static analysis with pyflakes.
 
 
 
 ## Install
 
-### With pip
+### Via pip
 
 ```shell
 # You need to run this with a Python 3.11 environment -- You can manage different python versions for instance with `pyenv`
 pip install -U fastchecks
 ```
 
 
-### From source
+### or via source
 
 You need to have [python poetry](https://python-poetry.org/docs/) installed. Then:
 
 ```shell
 # clone this repository
 _reponame="fastchecks";
 _branch="main";
```

### Comparing `fastchecks-0.2.1rc2/fastchecks/NOTICE` & `fastchecks-0.2.2/NOTICE`

 * *Files identical despite different names*

### Comparing `fastchecks-0.2.1rc2/fastchecks/__init__.py` & `fastchecks-0.2.2/fastchecks/__init__.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.2.1rc2/fastchecks/check.py` & `fastchecks-0.2.2/fastchecks/check.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.2.1rc2/fastchecks/cli.py` & `fastchecks-0.2.2/fastchecks/cli.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.2.1rc2/fastchecks/conf.py` & `fastchecks-0.2.2/fastchecks/conf.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.2.1rc2/fastchecks/log.py` & `fastchecks-0.2.2/fastchecks/log.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.2.1rc2/fastchecks/meta.py` & `fastchecks-0.2.2/fastchecks/meta.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from importlib import metadata
 import tomllib
 
+# Defines constants with package's (meta) information
+
 _MODULE_NAME = "fastchecks"
 
 try:
-    # TODO: the file is not available when installed as a package
+    # TODO: the file depends on the path and is also not available when installed as a package
     with open("pyproject.toml", "rb") as f:
         _META = tomllib.load(f)
 
         NAME = _META["tool"]["poetry"]["name"]
         VERSION = _META["tool"]["poetry"]["version"]
         DESCRIPTION = _META["tool"]["poetry"]["description"]
         WEBSITE = _META["tool"]["poetry"].get("homepage", _META["tool"]["poetry"]["repository"])
 
-except FileNotFoundError:
+except:  # In particular: FileNotFoundError:
     # Back up option for now for reading the package information
     # See: https://github.com/python-poetry/poetry/issues/273
     _META = {}
 
     NAME = _MODULE_NAME
 
     try:
```

### Comparing `fastchecks-0.2.1rc2/fastchecks/runner.py` & `fastchecks-0.2.2/fastchecks/runner.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.2.1rc2/fastchecks/sockets/__init__.py` & `fastchecks-0.2.2/fastchecks/sockets/__init__.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.2.1rc2/fastchecks/sockets/postgres/__init__.py` & `fastchecks-0.2.2/fastchecks/sockets/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.2.1rc2/fastchecks/sockets/postgres/schema/down.sql` & `fastchecks-0.2.2/fastchecks/sockets/postgres/schema/down.sql`

 * *Files identical despite different names*

### Comparing `fastchecks-0.2.1rc2/fastchecks/sockets/postgres/schema/up.sql` & `fastchecks-0.2.2/fastchecks/sockets/postgres/schema/up.sql`

 * *Files identical despite different names*

### Comparing `fastchecks-0.2.1rc2/fastchecks/types.py` & `fastchecks-0.2.2/fastchecks/types.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.2.1rc2/fastchecks/util.py` & `fastchecks-0.2.2/fastchecks/util.py`

 * *Files identical despite different names*

### Comparing `fastchecks-0.2.1rc2/fastchecks/vutil.py` & `fastchecks-0.2.2/fastchecks/vutil.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 #
 # Utils for validating data values, specifically user inputs.
-# - Further validation functions are defined conf module (which depend on configuration values).
+# - Further validation functions are defined in the conf module (i.e., those that depend on configuration values).
 #
 # Conventions:
 # * Unless otherwise specified, validators must raise ValueError if the value is invalid.
 # * Functions that validate a value and (if valid) return it, are prefixed with "validated_".
 # * Functions that validate a value and (if valid) return an optionally computed value, are prefixed with "validate_".
 #
 
 from numbers import Number
 from urllib.parse import ParseResult, urlparse
 import re2
 
 from fastchecks import meta, require
 
+# Note: currently these values are the same as those defined in the postgres DB schema. But they could be smaller, i.e. stricter.
+# MAYBE: reuse these values for the schema.
+URL_MAX_LEN = 2048
+REGEX_MAX_LEN = 2048
+
+
+def validate_max_len(x: str, max_len: int, varname: str = "string") -> None:
+    require(len(x) <= max_len, f"The {varname} cannot have length greater than: {max_len}")
+
 
 __FALSE = ["false", "f", "0", "no", "n"]
 __TRUE = ["true", "t", "1", "yes", "y"]
 
 
 def validated_parsed_bool_answer(val: str) -> bool:
     val_low = val.lower()
@@ -48,34 +57,39 @@
     )
     return val
 
 
 ACCEPTED_WEB_URL_SCHEMES = {"http", "https"}
 
 
-def validate_url(url: str, accepted_schemes: set[str], raise_error: bool = True) -> ParseResult | None:
+def validate_url(
+    url: str, accepted_schemes: set[str], raise_error: bool = True, max_len: int = URL_MAX_LEN
+) -> ParseResult | None:
     """
     Validate that the given string is a valid URL and has one of the accepted schemes.
     * If the URL is valid, return the urlparse's parsed result.
     * Else:
         * if raise_error is True, raise ValueError.
         * else, return None.
     """
     # See: https://snyk.io/blog/secure-python-url-validation/
 
     try:
+        validate_max_len(url, max_len=max_len, varname="url")
         ret = urlparse(url)
-        accept: bool = bool(ret.scheme) and bool(ret.netloc) and ret.scheme in accepted_schemes
+        accept = bool(ret.scheme) and bool(ret.netloc) and ret.scheme in accepted_schemes
     except:
-        return None
+        accept = False
 
     if accept:
         return ret
     elif raise_error:
-        raise ValueError(f"Invalid URL (also it must start with a scheme in: {accepted_schemes}): {url}")
+        raise ValueError(
+            f"Invalid URL (also, it must start with a scheme in {accepted_schemes}, and have max size {max_len}): {url}"
+        )
     else:
         return None
 
 
 def validated_web_url(url: str) -> str:
     validate_url(url, accepted_schemes=ACCEPTED_WEB_URL_SCHEMES, raise_error=True)
     return url
@@ -96,22 +110,28 @@
     """
     Validate regex string: the regex must be compilable with google's re2 library.
 
     If the regex is valid, return its re2._Regexp for possible later use.
     Else if raise_error is True, raise ValueError.
     """
     try:
+        validate_max_len(regex, max_len=REGEX_MAX_LEN, varname="regex")
         return re2.compile(regex)
-    except re2.error:
-        if raise_error:
-            raise ValueError(
-                f"Invalid regex (cannot compile it with google-re2 regex syntax https://github.com/google/re2/wiki/Syntax): {regex}"
-            )
-        else:
+    except Exception as e:
+        if not raise_error:
             return None
+        else:
+            match e:
+                case ValueError():
+                    # return early validation error for max_len for expressivity
+                    raise
+                case _:
+                    raise ValueError(
+                        f"Invalid regex (cannot compile it with google-re2 regex syntax https://github.com/google/re2/wiki/Syntax): {regex}"
+                    )
 
 
 def validated_regex(regex: str) -> str:
     validate_regex(regex, raise_error=True)
     return regex
```

### Comparing `fastchecks-0.2.1rc2/pyproject.toml` & `fastchecks-0.2.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 [tool.poetry]
 name = "fastchecks"
-version = "0.2.1-rc2"
+version = "0.2.2"
 description = "🚥 Fast website monitoring backend service"
 authors = ["Dr. Juan Miguel Cejuela <i@juanmi.rocks>"]
+license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/juanmirocks/fastchecks"
 packages = [{ include = "fastchecks" }]
+include = ["NOTICE"]
 
 
 [tool.poetry.scripts]
 fastchecks = 'fastchecks.cli:main'
 
 
 [tool.poetry.dependencies]
@@ -53,22 +55,25 @@
 [tool.poe.tasks]
 # format code
 fmt = "black ."
 
 # run tests with coverage -- for now do not use xdist's `-n auto` option
 test = "pytest --cov=fastchecks --cov-report=term-missing --cov-report=lcov:.cov/coverage.lcov" # HTML possible too: --cov-report=html:.cov/html"
 
+# Checks the validity of the pyproject.toml file
+lint_package = "poetry check"
+
 lint_errors = "pyflakes ."
 
 # For now ignore possible non 0 exit code; but at least report warnings & errors
 lint_types.shell = "mypy || true"
 lint_types_strict.shell = "mypy --strict || true"
 
 lint_bandit = "bandit -c pyproject.toml -r ."
 # snyk is not installed as a python dependency, but as a shell command (see how to install Snyk CLI: https://docs.snyk.io/snyk-cli/install-the-snyk-cli)
 lint_snyk.shell = "snyk code test; snyk test"
 lint_sec = ["lint_bandit", "lint_snyk"]
 
 # Snyk not added here since it might not be installed in the system
-lint_all = ["lint_errors", "lint_types", "lint_bandit"]
+lint_all = ["lint_package", "lint_errors", "lint_types", "lint_bandit"]
 
 test_n_lint = ["test", "lint_all"]
```

### Comparing `fastchecks-0.2.1rc2/PKG-INFO` & `fastchecks-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: fastchecks
-Version: 0.2.1rc2
+Version: 0.2.2
 Summary: 🚥 Fast website monitoring backend service
 Home-page: https://github.com/juanmirocks/fastchecks
+License: Apache-2.0
 Author: Dr. Juan Miguel Cejuela
 Author-email: i@juanmi.rocks
 Requires-Python: >=3.11,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: apscheduler (==4.0.0a2)
 Requires-Dist: google-re2 (>=1.0,<2.0)
 Requires-Dist: psycopg[binary,pool] (>=3.1.9,<4.0.0)
 Requires-Dist: pydantic (>=2.0.1,<3.0.0)
@@ -24,19 +26,25 @@
 [![Snyk](https://img.shields.io/badge/%20Snyk_security-monitored-8742B8?logo=snyk&logoColor=white)](https://github.com/juanmirocks/fastchecks/actions)
 
 
 
 ## Features
 
 **🍀 Feature-rich**
+* Each check tracks:
+  * timestamp
+  * response time
+  * HTTP response status code
+  * optionally, given regex is (safely) tested if it matches the response body or not
+  * info about possible connection errors, like timeouts and/or unreachable host
 * Websites to check & their results are stored in postgres by default 🐘 (the library is ready for other data stores / sockets).
   * You can use postgres locally installed, running on docker, or with a DBaaS, e.g. Aiven.
-* Run stored all websites once, at configurable-scheduled intervals, or even with your system's cron.
-* The scheduling keeps running even if the computer goes to sleep!
-* Nice, configurable logging
+* Monitor stored websites once, at configurable-scheduled intervals (each website check can use an independent interval or use a default), or even with your system's cron.
+* The scheduling keeps running even if the computer goes to sleep.
+* Nice, configurable logging.
 * CLI API & Python's (Python >= 3.11).
   * A [webserver](https://github.com/juanmirocks/fastchecks/issues/3) is planned.
 * ...and more!
 
 
 **🚀 Speed**
 * All operations are asynchronous. This app sits on 3 giants:
@@ -57,23 +65,23 @@
 * Further type checking with Pydantic (v2).
 * Further static analysis with pyflakes.
 
 
 
 ## Install
 
-### With pip
+### Via pip
 
 ```shell
 # You need to run this with a Python 3.11 environment -- You can manage different python versions for instance with `pyenv`
 pip install -U fastchecks
 ```
 
 
-### From source
+### or via source
 
 You need to have [python poetry](https://python-poetry.org/docs/) installed. Then:
 
 ```shell
 # clone this repository
 _reponame="fastchecks";
 _branch="main";
```


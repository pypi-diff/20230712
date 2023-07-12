# Comparing `tmp/docformatter-1.7.4.tar.gz` & `tmp/docformatter-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docformatter-1.7.4.tar", max compression
+gzip compressed data, was "docformatter-1.7.5.tar", max compression
```

## Comparing `docformatter-1.7.4.tar` & `docformatter-1.7.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1061 2022-07-29 13:50:28.414095 docformatter-1.7.4/LICENSE
--rw-r--r--   0        0        0     6864 2023-06-06 14:28:12.772135 docformatter-1.7.4/README.rst
--rw-r--r--   0        0        0     6352 2023-07-10 13:44:42.178415 docformatter-1.7.4/pyproject.toml
--rw-r--r--   0        0        0     1614 2023-06-06 14:28:12.798136 docformatter-1.7.4/src/docformatter/__init__.py
--rwxr-xr-x   0        0        0     6417 2023-06-23 16:31:57.338250 docformatter-1.7.4/src/docformatter/__main__.py
--rw-r--r--   0        0        0     1191 2023-07-10 13:44:42.178415 docformatter-1.7.4/src/docformatter/__pkginfo__.py
--rw-r--r--   0        0        0    13592 2023-06-07 03:06:35.282648 docformatter-1.7.4/src/docformatter/configuration.py
--rw-r--r--   0        0        0     3717 2023-06-23 17:25:42.338248 docformatter-1.7.4/src/docformatter/encode.py
--rw-r--r--   0        0        0    21006 2023-07-07 02:43:16.864063 docformatter-1.7.4/src/docformatter/format.py
--rw-r--r--   0        0        0     6998 2023-06-06 14:28:12.821136 docformatter-1.7.4/src/docformatter/strings.py
--rw-r--r--   0        0        0    28451 2023-07-10 13:44:42.178415 docformatter-1.7.4/src/docformatter/syntax.py
--rw-r--r--   0        0        0     4573 2023-04-28 16:27:48.980570 docformatter-1.7.4/src/docformatter/util.py
--rw-r--r--   0        0        0     8266 1970-01-01 00:00:00.000000 docformatter-1.7.4/PKG-INFO
+-rw-r--r--   0        0        0     1061 2022-07-29 13:50:28.414095 docformatter-1.7.5/LICENSE
+-rw-r--r--   0        0        0     6864 2023-06-06 14:28:12.772135 docformatter-1.7.5/README.rst
+-rw-r--r--   0        0        0     6352 2023-07-12 01:39:28.815373 docformatter-1.7.5/pyproject.toml
+-rw-r--r--   0        0        0     1614 2023-06-06 14:28:12.798136 docformatter-1.7.5/src/docformatter/__init__.py
+-rwxr-xr-x   0        0        0     6417 2023-06-23 16:31:57.338250 docformatter-1.7.5/src/docformatter/__main__.py
+-rw-r--r--   0        0        0     1191 2023-07-12 01:39:28.815373 docformatter-1.7.5/src/docformatter/__pkginfo__.py
+-rw-r--r--   0        0        0    13592 2023-06-07 03:06:35.282648 docformatter-1.7.5/src/docformatter/configuration.py
+-rw-r--r--   0        0        0     3717 2023-06-23 17:25:42.338248 docformatter-1.7.5/src/docformatter/encode.py
+-rw-r--r--   0        0        0    21006 2023-07-11 01:39:14.908939 docformatter-1.7.5/src/docformatter/format.py
+-rw-r--r--   0        0        0     6998 2023-06-06 14:28:12.821136 docformatter-1.7.5/src/docformatter/strings.py
+-rw-r--r--   0        0        0    28457 2023-07-12 01:33:57.285166 docformatter-1.7.5/src/docformatter/syntax.py
+-rw-r--r--   0        0        0     4573 2023-04-28 16:27:48.980570 docformatter-1.7.5/src/docformatter/util.py
+-rw-r--r--   0        0        0     8266 1970-01-01 00:00:00.000000 docformatter-1.7.5/PKG-INFO
```

### Comparing `docformatter-1.7.4/LICENSE` & `docformatter-1.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `docformatter-1.7.4/README.rst` & `docformatter-1.7.5/README.rst`

 * *Files identical despite different names*

### Comparing `docformatter-1.7.4/pyproject.toml` & `docformatter-1.7.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docformatter"
-version = "1.7.4"
+version = "1.7.5"
 description = "Formats docstrings to follow PEP 257"
 authors = ["Steven Myint"]
 maintainers = [
     "Doyle Rowland <doyle.rowland@reliaqual.com>",
 ]
 license = "Expat"
 readme = "README.rst"
```

### Comparing `docformatter-1.7.4/src/docformatter/__init__.py` & `docformatter-1.7.5/src/docformatter/__init__.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.7.4/src/docformatter/__main__.py` & `docformatter-1.7.5/src/docformatter/__main__.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.7.4/src/docformatter/__pkginfo__.py` & `docformatter-1.7.5/src/docformatter/__pkginfo__.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 # NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS
 # BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN
 # ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """Package information for docformatter."""
 
-__version__ = "1.7.4"
+__version__ = "1.7.5"
```

### Comparing `docformatter-1.7.4/src/docformatter/configuration.py` & `docformatter-1.7.5/src/docformatter/configuration.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.7.4/src/docformatter/encode.py` & `docformatter-1.7.5/src/docformatter/encode.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.7.4/src/docformatter/format.py` & `docformatter-1.7.5/src/docformatter/format.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.7.4/src/docformatter/strings.py` & `docformatter-1.7.5/src/docformatter/strings.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.7.4/src/docformatter/syntax.py` & `docformatter-1.7.5/src/docformatter/syntax.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
 OPTION_REGEX = r"^-{1,2}[\S ]+ {2}\S+"
 """Regular expression to use for finding option lists."""
 
 REST_REGEX = r"((\.{2}|`{2}) ?[\w.~-]+(:{2}|`{2})?[\w ]*?|`[\w.~]+`)"
 """Regular expression to use for finding reST directives."""
 
-SPHINX_REGEX = r":(param|raises|return|rtype|type)[a-zA-Z0-9_\-.() ]*:"
+SPHINX_REGEX = r":(param|raises|return|rtype|type|yield)[a-zA-Z0-9_\-.() ]*:"
 """Regular expression to use for finding Sphinx-style field lists."""
 
 URL_PATTERNS = (
     "afp|"
     "apt|"
     "bitcoin|"
     "chrome|"
```

### Comparing `docformatter-1.7.4/src/docformatter/util.py` & `docformatter-1.7.5/src/docformatter/util.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.7.4/PKG-INFO` & `docformatter-1.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docformatter
-Version: 1.7.4
+Version: 1.7.5
 Summary: Formats docstrings to follow PEP 257
 Home-page: https://github.com/PyCQA/docformatter
 License: Expat
 Keywords: PEP 257,pep257,style,formatter,docstrings
 Author: Steven Myint
 Maintainer: Doyle Rowland
 Maintainer-email: doyle.rowland@reliaqual.com
```


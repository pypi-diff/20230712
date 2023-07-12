# Comparing `tmp/LbProdRun-1.5.0.tar.gz` & `tmp/LbProdRun-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LbProdRun-1.5.0.tar", last modified: Tue Jun  6 06:44:27 2023, max compression
+gzip compressed data, was "LbProdRun-1.5.1.tar", last modified: Wed Jul 12 09:43:49 2023, max compression
```

## Comparing `LbProdRun-1.5.0.tar` & `LbProdRun-1.5.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 06:44:27.900000 LbProdRun-1.5.0/
--rw-r--r--   0 root         (0) root         (0)     2055 2023-06-06 06:44:13.000000 LbProdRun-1.5.0/.gitignore
--rw-r--r--   0 root         (0) root         (0)     2482 2023-06-06 06:44:13.000000 LbProdRun-1.5.0/.gitlab-ci.yml
--rw-r--r--   0 root         (0) root         (0)     1071 2023-06-06 06:44:13.000000 LbProdRun-1.5.0/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)    16310 2023-06-06 06:44:13.000000 LbProdRun-1.5.0/.pylintrc
--rw-r--r--   0 root         (0) root         (0)      388 2023-06-06 06:44:13.000000 LbProdRun-1.5.0/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)    35149 2023-06-06 06:44:13.000000 LbProdRun-1.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2655 2023-06-06 06:44:27.900000 LbProdRun-1.5.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2233 2023-06-06 06:44:13.000000 LbProdRun-1.5.0/README.md
--rw-r--r--   0 root         (0) root         (0)      304 2023-06-06 06:44:13.000000 LbProdRun-1.5.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1103 2023-06-06 06:44:27.900000 LbProdRun-1.5.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 06:44:27.896000 LbProdRun-1.5.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 06:44:27.900000 LbProdRun-1.5.0/src/LbProdRun/
--rw-r--r--   0 root         (0) root         (0)    12272 2023-06-06 06:44:13.000000 LbProdRun-1.5.0/src/LbProdRun/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1333 2023-06-06 06:44:13.000000 LbProdRun-1.5.0/src/LbProdRun/__main__.py
--rw-r--r--   0 root         (0) root         (0)     4715 2023-06-06 06:44:13.000000 LbProdRun-1.5.0/src/LbProdRun/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 06:44:27.900000 LbProdRun-1.5.0/src/LbProdRun.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2655 2023-06-06 06:44:27.000000 LbProdRun-1.5.0/src/LbProdRun.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      458 2023-06-06 06:44:27.000000 LbProdRun-1.5.0/src/LbProdRun.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 06:44:27.000000 LbProdRun-1.5.0/src/LbProdRun.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-06-06 06:44:27.000000 LbProdRun-1.5.0/src/LbProdRun.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      154 2023-06-06 06:44:27.000000 LbProdRun-1.5.0/src/LbProdRun.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-06 06:44:27.000000 LbProdRun-1.5.0/src/LbProdRun.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 06:44:27.900000 LbProdRun-1.5.0/tests/
--rw-r--r--   0 root         (0) root         (0)     4704 2023-06-06 06:44:13.000000 LbProdRun-1.5.0/tests/test_cli.py
--rw-r--r--   0 root         (0) root         (0)     3028 2023-06-06 06:44:13.000000 LbProdRun-1.5.0/tests/test_options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:43:49.096000 LbProdRun-1.5.1/
+-rw-r--r--   0 root         (0) root         (0)     2055 2023-07-12 09:43:34.000000 LbProdRun-1.5.1/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     2482 2023-07-12 09:43:34.000000 LbProdRun-1.5.1/.gitlab-ci.yml
+-rw-r--r--   0 root         (0) root         (0)     1071 2023-07-12 09:43:34.000000 LbProdRun-1.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)    16310 2023-07-12 09:43:34.000000 LbProdRun-1.5.1/.pylintrc
+-rw-r--r--   0 root         (0) root         (0)      388 2023-07-12 09:43:34.000000 LbProdRun-1.5.1/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-07-12 09:43:34.000000 LbProdRun-1.5.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2655 2023-07-12 09:43:49.096000 LbProdRun-1.5.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2233 2023-07-12 09:43:34.000000 LbProdRun-1.5.1/README.md
+-rw-r--r--   0 root         (0) root         (0)      304 2023-07-12 09:43:34.000000 LbProdRun-1.5.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-07-12 09:43:49.096000 LbProdRun-1.5.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:43:49.092000 LbProdRun-1.5.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:43:49.092000 LbProdRun-1.5.1/src/LbProdRun/
+-rw-r--r--   0 root         (0) root         (0)    12272 2023-07-12 09:43:34.000000 LbProdRun-1.5.1/src/LbProdRun/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1333 2023-07-12 09:43:34.000000 LbProdRun-1.5.1/src/LbProdRun/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     4764 2023-07-12 09:43:34.000000 LbProdRun-1.5.1/src/LbProdRun/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:43:49.096000 LbProdRun-1.5.1/src/LbProdRun.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2655 2023-07-12 09:43:49.000000 LbProdRun-1.5.1/src/LbProdRun.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      458 2023-07-12 09:43:49.000000 LbProdRun-1.5.1/src/LbProdRun.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 09:43:49.000000 LbProdRun-1.5.1/src/LbProdRun.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-12 09:43:49.000000 LbProdRun-1.5.1/src/LbProdRun.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      154 2023-07-12 09:43:49.000000 LbProdRun-1.5.1/src/LbProdRun.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-12 09:43:49.000000 LbProdRun-1.5.1/src/LbProdRun.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 09:43:49.096000 LbProdRun-1.5.1/tests/
+-rw-r--r--   0 root         (0) root         (0)     4772 2023-07-12 09:43:34.000000 LbProdRun-1.5.1/tests/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)     3028 2023-07-12 09:43:34.000000 LbProdRun-1.5.1/tests/test_options.py
```

### Comparing `LbProdRun-1.5.0/.gitignore` & `LbProdRun-1.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `LbProdRun-1.5.0/.gitlab-ci.yml` & `LbProdRun-1.5.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `LbProdRun-1.5.0/.pre-commit-config.yaml` & `LbProdRun-1.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `LbProdRun-1.5.0/.pylintrc` & `LbProdRun-1.5.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `LbProdRun-1.5.0/LICENSE` & `LbProdRun-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `LbProdRun-1.5.0/PKG-INFO` & `LbProdRun-1.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LbProdRun
-Version: 1.5.0
+Version: 1.5.1
 Summary: CLI for running LHCb applications from LHCbDIRAC
 Home-page: https://gitlab.cern.ch/lhcb-core/lbprodrun
 License: GPL-3.0-only
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `LbProdRun-1.5.0/README.md` & `LbProdRun-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `LbProdRun-1.5.0/setup.cfg` & `LbProdRun-1.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `LbProdRun-1.5.0/src/LbProdRun/__init__.py` & `LbProdRun-1.5.1/src/LbProdRun/__init__.py`

 * *Files identical despite different names*

### Comparing `LbProdRun-1.5.0/src/LbProdRun/__main__.py` & `LbProdRun-1.5.1/src/LbProdRun/__main__.py`

 * *Files identical despite different names*

### Comparing `LbProdRun-1.5.0/src/LbProdRun/models.py` & `LbProdRun-1.5.1/src/LbProdRun/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,23 +21,23 @@
 class BaseModel(_BaseModel, extra=Extra.forbid, validate_assignment=True):
     pass
 
 
 class BaseApplication(BaseModel):
     name: str
     version: str
-    event_timeout: Optional[float]
+    event_timeout: Optional[float] = None
     number_of_processors: int = 1
 
 
 class JobSpecV1(BaseModel):
     class ReleaseApplication(BaseApplication):
         data_pkgs: list[str] = []
         binary_tag: str = "best"
-        nightly: Optional[str]
+        nightly: Optional[str] = None
 
     class LbDevApplication(BaseApplication):
         project_base: Path
         binary_tag: str
 
     class FullDevApplication(BaseApplication):
         run_script: Path
@@ -48,17 +48,17 @@
     application: Union[ReleaseApplication, LbDevApplication, FullDevApplication]
 
     class LegacyOptions(BaseModel):
         command: Annotated[list[str], Field(min_length=1)] = []
         # FIXME: Ideally this should be annotated however there are too many buggy steps
         # files: Annotated[list[str], Field(min_length=1)]
         files: list[str]
-        format: Optional[str]
-        gaudi_extra_options: Optional[str]
-        processing_pass: Optional[str]
+        format: Optional[str] = None
+        gaudi_extra_options: Optional[str] = None
+        processing_pass: Optional[str] = None
 
         @validator("command", pre=True, always=True)
         def set_command(cls, command):  # noqa: B902  # pylint: disable=no-self-argument
             return command or ["gaudirun.py", "-T"]
 
     class LbExecOptions(BaseModel):
         entrypoint: str
@@ -77,16 +77,16 @@
         first_event_number: Optional[int] = None
 
     input: Input = Input()
 
     class Output(BaseModel):
         prefix: str
         types: list[str]
-        histogram_file: Optional[str]
-        compression: Optional[str]
+        histogram_file: Optional[str] = None
+        compression: Optional[str] = None
 
     output: Output
 
     class DBTags(BaseModel):
         dddb_tag: Optional[str] = None
         conddb_tag: Optional[str] = None
         dq_tag: Optional[str] = None
```

### Comparing `LbProdRun-1.5.0/src/LbProdRun.egg-info/PKG-INFO` & `LbProdRun-1.5.1/src/LbProdRun.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LbProdRun
-Version: 1.5.0
+Version: 1.5.1
 Summary: CLI for running LHCb applications from LHCbDIRAC
 Home-page: https://gitlab.cern.ch/lhcb-core/lbprodrun
 License: GPL-3.0-only
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `LbProdRun-1.5.0/tests/test_cli.py` & `LbProdRun-1.5.1/tests/test_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,8 +115,11 @@
                     "types": ["d02hhll.strip.mdst"],
                 },
             }
         )
     )
     result = runner.invoke(app, str(tmp_path))
     assert result.exit_code >= 64
-    assert "not a valid integer" in result.stdout
+    assert (
+        "should be a valid integer, unable to parse string as an integer"
+        in result.stdout
+    )
```

### Comparing `LbProdRun-1.5.0/tests/test_options.py` & `LbProdRun-1.5.1/tests/test_options.py`

 * *Files identical despite different names*


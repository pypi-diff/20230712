# Comparing `tmp/adsctl-0.3.0.tar.gz` & `tmp/adsctl-0.4.0.tar.gz`

## Comparing `adsctl-0.3.0.tar` & `adsctl-0.4.0.tar`

### file list

```diff
@@ -1,53 +1,56 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 adsctl-0.3.0/.DS_Store
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 adsctl-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 adsctl-0.3.0/.python-version
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 adsctl-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 adsctl-0.3.0/RELEASE.md
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 adsctl-0.3.0/TESTING.md
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 adsctl-0.3.0/Taskfile.yml
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 adsctl-0.3.0/requirements-dev.lock
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 adsctl-0.3.0/requirements.lock
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 adsctl-0.3.0/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 adsctl-0.3.0/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/__about__.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/__init__.py
--rw-r--r--   0        0        0     3063 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/application.py
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/client.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/parse.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/queries.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/api/__init__.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/api/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/api/campaign/__init__.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/api/campaign/budget.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/api/campaign/main.py
--rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/api/campaign/status.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/cli/__init__.py
--rw-r--r--   0        0        0     7362 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/cli/auth.py
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/cli/cli.py
--rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/cli/config.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/cli/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/cli/edit/__init__.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/cli/edit/campaign.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/cli/edit/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/config/__init__.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/config/config_file.py
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/config/model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/prompt/__init__.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/prompt/cli.py
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/prompt/completer.py
--rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/prompt/key_bindings.py
--rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/prompt/prompt.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/utils/__init__.py
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 adsctl-0.3.0/src/adsctl/utils/fs.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 adsctl-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 adsctl-0.3.0/tests/conftest.py
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 adsctl-0.3.0/tests/test_config_file.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 adsctl-0.3.0/tests/test_parse.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 adsctl-0.3.0/tests/test_pkg.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 adsctl-0.3.0/tests/templates/config_1.toml
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 adsctl-0.3.0/tests/templates/config_invalid_id.toml
--rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 adsctl-0.3.0/.gitignore
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 adsctl-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0     6720 2020-02-02 00:00:00.000000 adsctl-0.3.0/README.md
--rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 adsctl-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     7842 2020-02-02 00:00:00.000000 adsctl-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 adsctl-0.4.0/.DS_Store
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 adsctl-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 adsctl-0.4.0/.python-version
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 adsctl-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 adsctl-0.4.0/RELEASE.md
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 adsctl-0.4.0/TESTING.md
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 adsctl-0.4.0/Taskfile.yml
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 adsctl-0.4.0/requirements-dev.lock
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 adsctl-0.4.0/requirements.lock
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/__about__.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/__init__.py
+-rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/application.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/client.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/parse.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/queries.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/api/__init__.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/api/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/api/asset/__init__.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/api/asset/image.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/api/campaign/__init__.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/api/campaign/budget.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/api/campaign/main.py
+-rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/api/campaign/status.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/cli/__init__.py
+-rw-r--r--   0        0        0     7393 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/cli/auth.py
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/cli/cli.py
+-rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/cli/config.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/cli/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/cli/create/__init__.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/cli/create/asset.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/cli/create/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/cli/edit/__init__.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/cli/edit/campaign.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/cli/edit/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/config/__init__.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/config/config_file.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/config/model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/prompt/__init__.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/prompt/cli.py
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/prompt/completer.py
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/prompt/key_bindings.py
+-rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/prompt/prompt.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/utils/__init__.py
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 adsctl-0.4.0/src/adsctl/utils/fs.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 adsctl-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 adsctl-0.4.0/tests/conftest.py
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 adsctl-0.4.0/tests/test_config_file.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 adsctl-0.4.0/tests/test_parse.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 adsctl-0.4.0/tests/test_pkg.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 adsctl-0.4.0/tests/templates/config_1.toml
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 adsctl-0.4.0/tests/templates/config_invalid_id.toml
+-rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 adsctl-0.4.0/.gitignore
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 adsctl-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     6720 2020-02-02 00:00:00.000000 adsctl-0.4.0/README.md
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 adsctl-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 adsctl-0.4.0/PKG-INFO
```

### Comparing `adsctl-0.3.0/.pre-commit-config.yaml` & `adsctl-0.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adsctl-0.3.0/requirements-dev.lock` & `adsctl-0.4.0/requirements-dev.lock`

 * *Files 17% similar despite different names*

```diff
@@ -1,96 +1,110 @@
--e file:///Users/danielfrg/google/adsctl
-anyio==3.6.2
+# generated by rye
+# use `rye lock` or `rye sync` to update this lockfile
+#
+# last locked with the following flags:
+#   pre: false
+#   features: []
+#   all-features: true
+
+-e file:.
+anyio==3.7.1
 appnope==0.1.3
 asttokens==2.2.1
 backcall==0.2.0
 black==23.3.0
-cachetools==5.3.0
-certifi==2022.12.7
-charset-normalizer==3.1.0
-click==8.1.3
-coverage==7.2.3
+build==0.10.0
+cachetools==5.3.1
+certifi==2023.5.7
+charset-normalizer==3.2.0
+click==8.1.4
+coverage==7.2.7
 decorator==5.1.1
 distlib==0.3.6
-editables==0.3
-exceptiongroup==1.1.1
+editables==0.4
+exceptiongroup==1.1.2
 executing==1.2.0
-filelock==3.12.0
-google-ads==21.0.0
+filelock==3.12.2
+google-ads==21.2.0
 google-api-core==2.11.0
-google-auth==2.17.3
+google-auth==2.22.0
 google-auth-oauthlib==1.0.0
-googleapis-common-protos==1.59.0
-grpcio==1.54.0
-grpcio-status==1.54.0
+googleapis-common-protos==1.59.1
+grpcio==1.56.0
+grpcio-status==1.56.0
 h11==0.14.0
 hatch==1.7.0
-hatchling==1.14.1
-httpcore==0.17.0
-httpx==0.24.0
+hatchling==1.18.0
+httpcore==0.17.3
+httpx==0.24.1
 hyperlink==21.0.0
 idna==3.4
-importlib-metadata==6.6.0
+importlib-metadata==6.8.0
+importlib-resources==6.0.0
 iniconfig==2.0.0
-ipython==8.12.0
-isort==6.0.0b2
-jaraco-classes==3.2.3
+ipython==8.12.2
+isort==5.12.0
+jaraco-classes==3.3.0
 jedi==0.18.2
 jinja2==3.1.2
-keyring==23.13.1
-markdown-it-py==2.2.0
-markupsafe==2.1.2
+keyring==24.2.0
+markdown-it-py==3.0.0
+markupsafe==2.1.3
 matplotlib-inline==0.1.6
 mdurl==0.1.2
 more-itertools==9.1.0
 mypy==1.2.0
 mypy-extensions==1.0.0
-numpy==1.24.3
+numpy==1.24.4
 oauthlib==3.2.2
 packaging==23.1
-pandas==2.0.0
+pandas==2.0.3
 parso==0.8.3
 pathspec==0.11.1
 pexpect==4.8.0
 pickleshare==0.7.5
-platformdirs==3.2.0
-pluggy==1.0.0
-prompt-toolkit==3.0.38
-proto-plus==1.22.2
-protobuf==4.22.3
+pillow==10.0.0
+pip-tools==6.14.0
+platformdirs==3.8.1
+pluggy==1.2.0
+prompt-toolkit==3.0.39
+proto-plus==1.22.3
+protobuf==4.23.4
 ptyprocess==0.7.0
 pure-eval==0.2.2
 pyasn1==0.5.0
 pyasn1-modules==0.3.0
-pydantic==1.10.7
+pydantic==1.10.11
 pygments==2.15.1
 pyperclip==1.8.2
-pytest==7.3.1
-pytest-cov==4.0.0
+pyproject-hooks==1.0.0
+pytest==7.4.0
+pytest-cov==4.1.0
 python-dateutil==2.8.2
 pytz==2023.3
 pyyaml==6.0
-requests==2.28.2
+requests==2.31.0
 requests-oauthlib==1.3.1
-rich==13.3.4
+rich==13.4.2
 rsa==4.9
-ruff==0.0.262
+ruff==0.0.277
 shellingham==1.5.0.post1
 six==1.16.0
 sniffio==1.3.0
 stack-data==0.6.2
 tabulate==0.9.0
 tomli==2.0.1
 tomli-w==1.0.0
-tomlkit==0.11.7
+tomlkit==0.11.8
 traitlets==5.9.0
-trove-classifiers==2023.4.22
-typing-extensions==4.5.0
+trove-classifiers==2023.7.6
+typing-extensions==4.7.1
 tzdata==2023.3
-urllib3==1.26.15
+urllib3==1.26.16
 userpath==1.8.0
-virtualenv==20.22.0
+virtualenv==20.23.1
 wcwidth==0.2.6
-zipp==3.15.0
-
+wheel==0.40.0
+zipp==3.16.0
 # The following packages are considered to be unsafe in a requirements file:
-setuptools==67.7.1
+pip==23.1.2
+setuptools==68.0.0
```

### Comparing `adsctl-0.3.0/src/adsctl/application.py` & `adsctl-0.4.0/src/adsctl/application.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,33 @@
+from typing import Union
+
 from google.ads.googleads.client import GoogleAdsClient
 
 from adsctl import client as client_utils
 from adsctl.config.config_file import ConfigFile
 from adsctl.config.model import AccountConfig, RootConfig
 from adsctl.parse import parseStream
 from adsctl.utils.fs import Path
 
 
 class Application:
-    config_file_path: Path | None
+    config_file_path: Union[Path, None]
     config_file: ConfigFile
-    client: GoogleAdsClient | None
-    _customer_id: str | None
+    client: Union[GoogleAdsClient, None]
+    _customer_id: Union[str, None]
     params: dict = {}
+    api_version: str = "v13"
 
     def __init__(
         self,
-        config_file: str | None = None,  # Path to config file
-        account: str | None = None,
-        customer_id: str | None = None,
+        config_file: Union[str, None] = None,  # Path to config file
+        account: Union[str, None] = None,
+        customer_id: Union[str, None] = None,
         load_config=True,
     ):
-
         self._customer_id = customer_id
         if config_file is None:
             self.config_file_path = ConfigFile.get_default_location()
             self.config_file = ConfigFile(account=account)
         else:
             self.config_file_path = Path(config_file)
             path_ = None if config_file is None else Path(config_file)
@@ -39,49 +41,49 @@
         return self.config_file.model
 
     @property
     def account(self) -> AccountConfig:
         return self.config_file.account
 
     @property
-    def customer_id(self) -> str | None:
+    def customer_id(self) -> Union[str, None]:
         if self._customer_id:
             return self._customer_id.replace("-", "")
         else:
             return self.account.customer_id.replace("-", "")
 
     def load_config(self):
         self.config_file.load()
 
     def create_client(self):
         gads_config = self.config_file.account.clientSettings()
-        client_ = client_utils.get_client(gads_config)
+        client_ = client_utils.get_client(gads_config, version=self.api_version)
         self.client = client_
         return client_
 
-    def query(self, query, customer_id=None, params: dict | None = None):
+    def query(self, query, customer_id=None, params: Union[dict, None] = None):
         if params is None:
             params = {}
         customer_id = customer_id or self.config_file.account.customer_id
         myclient = self.create_client()
         stream = self.search_stream(query=query, client=myclient, params=params)
         tables = parseStream(stream)
         return tables
 
-    def search(self, query, client, customer_id=None, params: dict | None = None):
+    def search(self, query, client, customer_id=None, params: Union[dict, None] = None):
         if params is None:
             params = {}
         customer_id = customer_id or self.customer_id or self.account.customer_id
         query_ = client_utils.render_template(query.strip(), **params)
 
         ga_service = client.get_service("GoogleAdsService")
         return ga_service.search(query=query_, customer_id=customer_id)
 
     def search_stream(
-        self, query, client, customer_id=None, params: dict | None = None
+        self, query, client, customer_id=None, params: Union[dict, None] = None
     ):
         if params is None:
             params = {}
         customer_id = customer_id or self.customer_id or self.account.customer_id
         query_ = client_utils.render_template(query.strip(), **params)
 
         ga_service = client.get_service("GoogleAdsService")
```

### Comparing `adsctl-0.3.0/src/adsctl/parse.py` & `adsctl-0.4.0/src/adsctl/parse.py`

 * *Files identical despite different names*

### Comparing `adsctl-0.3.0/src/adsctl/queries.py` & `adsctl-0.4.0/src/adsctl/queries.py`

 * *Files identical despite different names*

### Comparing `adsctl-0.3.0/src/adsctl/api/campaign/budget.py` & `adsctl-0.4.0/src/adsctl/api/campaign/budget.py`

 * *Files identical despite different names*

### Comparing `adsctl-0.3.0/src/adsctl/api/campaign/status.py` & `adsctl-0.4.0/src/adsctl/api/campaign/status.py`

 * *Files identical despite different names*

### Comparing `adsctl-0.3.0/src/adsctl/cli/auth.py` & `adsctl-0.4.0/src/adsctl/cli/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import hashlib
 import os
 import re
 import socket
 import sys
+from typing import Union
 from urllib.parse import unquote
 
 import click
 from google_auth_oauthlib.flow import Flow
 
 from adsctl.application import Application
 
@@ -91,15 +92,15 @@
                 sys.exit(1)
 
         f.write(new_content)
 
     click.echo("Done! You can now run adsctl commands.")
 
 
-def oauth_flow(secrets_file: str) -> str | None:
+def oauth_flow(secrets_file: str) -> Union[str, None]:
     """Do the OAuth flow to get a refresh token."""
 
     # if args.additional_scopes:
     #     configured_scopes.extend(args.additional_scopes)
 
     configured_scopes = [_SCOPE]
```

### Comparing `adsctl-0.3.0/src/adsctl/cli/cli.py` & `adsctl-0.4.0/src/adsctl/cli/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 
 import click
 
 from adsctl.__about__ import __version__
 from adsctl.cli.auth import auth
 from adsctl.cli.config import config
+from adsctl.cli.create.main import create
 from adsctl.cli.edit.main import edit
 from adsctl.cli.utils import create_app
 
 
 @click.group()
 @click.option(
     "--config-file",
@@ -41,12 +42,13 @@
         ctx.obj = app
     except Exception as e:
         click.echo(f"Error loading config: {e}")
 
 
 main.add_command(auth)
 main.add_command(edit)
+main.add_command(create)
 main.add_command(config)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `adsctl-0.3.0/src/adsctl/cli/config.py` & `adsctl-0.4.0/src/adsctl/cli/config.py`

 * *Files identical despite different names*

### Comparing `adsctl-0.3.0/src/adsctl/cli/utils.py` & `adsctl-0.4.0/src/adsctl/cli/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import sys
+from typing import Union
 
 import click
 
 from adsctl.application import Application
 from adsctl.utils.fs import Path
 
 
 def create_app(
-    config_file_path: str | None = None,
-    customer_id: str | None = None,
-    account: str | None = None,
+    config_file_path: Union[str, None] = None,
+    customer_id: Union[str, None] = None,
+    account: Union[str, None] = None,
 ) -> Application:
 
     if config_file_path:
         used_config_file = Path(config_file_path).resolve()
         if not used_config_file.is_file():
             click.echo(
                 f"The selected config file `{str(config_file_path)}` does not exist."
```

### Comparing `adsctl-0.3.0/src/adsctl/cli/edit/campaign.py` & `adsctl-0.4.0/src/adsctl/cli/edit/campaign.py`

 * *Files identical despite different names*

### Comparing `adsctl-0.3.0/src/adsctl/config/config_file.py` & `adsctl-0.4.0/src/adsctl/config/config_file.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-from typing import cast
+from typing import Union, cast
 
 from adsctl.config.model import AccountConfig, RootConfig
 from adsctl.utils.fs import Path, load_toml_data
 
 
 class ConfigFile:
     model: RootConfig
-    account_name: str | None
+    account_name: Union[str, None]
 
-    def __init__(self, path: Path | None = None, account: str | None = None):
-        self._path: Path | None = path
+    def __init__(
+        self, path: Union[Path, None] = None, account: Union[str, None] = None
+    ):
+        self._path: Union[Path, None] = path
         self.model = cast(RootConfig, None)
         self.account_name = account
 
     @property
     def path(self):
         if self._path is None:
             self._path = self.get_default_location()
```

### Comparing `adsctl-0.3.0/src/adsctl/config/model.py` & `adsctl-0.4.0/src/adsctl/config/model.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import re
+from typing import Dict, Union
 
 from pydantic import BaseModel, BaseSettings, validator
 
 
 class OAuth(BaseModel):
     client_id: str = ""
     client_secret: str = ""
-    refresh_token: str | None = None
+    refresh_token: Union[str, None] = None
 
 
 class AccountConfig(BaseModel):
     developer_token: str = ""
     customer_id: str = ""
     login_customer_id: str = ""
     oauth: OAuth = OAuth()
@@ -33,13 +34,13 @@
         if self.login_customer_id:
             base["login_customer_id"] = self.login_customer_id
         return base
 
 
 class RootConfig(BaseSettings):
     current_account: str = "default"
-    accounts: dict[str, AccountConfig] = {
+    accounts: Dict[str, AccountConfig] = {
         "default": AccountConfig(),
     }
 
     class Config:
         env_prefix = "adsctl_"
```

### Comparing `adsctl-0.3.0/src/adsctl/prompt/cli.py` & `adsctl-0.4.0/src/adsctl/prompt/cli.py`

 * *Files identical despite different names*

### Comparing `adsctl-0.3.0/src/adsctl/prompt/completer.py` & `adsctl-0.4.0/src/adsctl/prompt/completer.py`

 * *Files identical despite different names*

### Comparing `adsctl-0.3.0/src/adsctl/prompt/key_bindings.py` & `adsctl-0.4.0/src/adsctl/prompt/key_bindings.py`

 * *Files identical despite different names*

### Comparing `adsctl-0.3.0/src/adsctl/prompt/prompt.py` & `adsctl-0.4.0/src/adsctl/prompt/prompt.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 import sys
+from typing import Union
 
 import click
 from google.ads.googleads.errors import GoogleAdsException
 from prompt_toolkit import PromptSession
 from prompt_toolkit.completion import FuzzyCompleter, ThreadedCompleter
 from prompt_toolkit.history import FileHistory
 from tabulate import tabulate
 
 from adsctl.application import Application
 from adsctl.parse import parseStream
 from adsctl.prompt.completer import MyCustomCompleter
 from adsctl.prompt.key_bindings import adsctl_bindings
 
 
-def prompt_loop(app: Application, output="table", params: dict | None = None):
+def prompt_loop(app: Application, output="table", params: Union[dict, None] = None):
     if app.config_file_path is None:
         my_history = None
     else:
         history_file = app.config_file_path.parent / "history.txt"
         my_history = FileHistory(str(history_file))
 
     key_bindings = adsctl_bindings()
-    completer = ThreadedCompleter(FuzzyCompleter(MyCustomCompleter()))
+    ThreadedCompleter(FuzzyCompleter(MyCustomCompleter()))
     session = PromptSession(
         history=my_history,
-        completer=completer,
-        complete_while_typing=True,
+        # completer=completer,
+        # complete_while_typing=True,
         key_bindings=key_bindings,
         multiline=True,
     )
 
     while True:
         try:
             query = session.prompt(">>> ").strip()
@@ -55,15 +56,15 @@
             pass
         except EOFError:
             # Control-D pressed
             sys.exit()
 
 
 def make_query(
-    app: Application, query, output="table", params: dict | None = None
+    app: Application, query, output="table", params: Union[dict, None] = None
 ) -> None | list | dict:
     results = None
     stream = app.search_stream(query, params=params)
 
     if output == "plain":
         results = []
         for batch in stream:
```

### Comparing `adsctl-0.3.0/src/adsctl/utils/fs.py` & `adsctl-0.4.0/src/adsctl/utils/fs.py`

 * *Files identical despite different names*

### Comparing `adsctl-0.3.0/tests/conftest.py` & `adsctl-0.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `adsctl-0.3.0/tests/test_config_file.py` & `adsctl-0.4.0/tests/test_config_file.py`

 * *Files identical despite different names*

### Comparing `adsctl-0.3.0/tests/test_parse.py` & `adsctl-0.4.0/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `adsctl-0.3.0/.gitignore` & `adsctl-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `adsctl-0.3.0/LICENSE.txt` & `adsctl-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `adsctl-0.3.0/README.md` & `adsctl-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `adsctl-0.3.0/pyproject.toml` & `adsctl-0.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 [project]
 name = "adsctl"
 description = "Google Ads Control CLI and Prompt"
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.8"
 license = "Apache-2.0"
 keywords = ["google ads", "google ads api", "cli", "prompt"]
 authors = [{ name = "Daniel Rodriguez", email = "daniel@danielfrg.com" }]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "google-ads>=20.0.0",
@@ -20,33 +22,35 @@
   "jinja2>=3.1.0",
   "pandas>=2.0.0",
   "pydantic>=1.10.0,<2.0.0",
   "tabulate>=0.9.0",
   "prompt_toolkit>=3.0.38",
   "tomli-w>=1.0",
   "tomlkit>=0.11.1",
+  "Pillow>=9.5.0",
 ]
 dynamic = ["version"]
 
-# [project.optional-dependencies]
-# test = []
+[project.optional-dependencies]
+test = ["coverage[toml]", "pytest", "pytest-cov"]
 
 [project.scripts]
 gaql = "adsctl.prompt.cli:main"
 adsctl = "adsctl.cli.cli:main"
 
 [tool.rye]
 dev-dependencies = [
   "black~=23.3.0",
   "hatch~=1.7.0",
-  "isort~=6.0.0b2",
+  "ipython~=8.12.0",
+  "isort~=5.12.0",
   "mypy~=1.2.0",
   "ruff~=0.0.262",
-  "coverage[toml]", "pytest", "pytest-cov"
-, "ipython~=8.12.0"]
+  "pip-tools",
+]
 
 [tool.rye.scripts]
 test = "pytest --no-cov"
 testall = "pytest --no-cov --ads-api"
 cov = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=src/adsctl --cov=tests"
 
 [tool.pytest.ini_options]
@@ -65,19 +69,19 @@
 omit = ["tests/*"]
 
 [tool.coverage.report]
 exclude_lines = ["no cov", "if __name__ == .__main__.:", "if TYPE_CHECKING:"]
 
 [tool.ruff]
 select = [
-    "E",  # pycodestyle errors
-    "W",  # pycodestyle warnings
-    "F",  # pyflakes
-    # "I",  # isort
-    "B",  # flake8-bugbear
+  "E", # pycodestyle errors
+  "W", # pycodestyle warnings
+  "F", # pyflakes
+  # "I",  # isort
+  "B", # flake8-bugbear
 ]
 
 [tool.isort]
 profile = "black"
 
 [tool.mypy]
 strict = true
```

### Comparing `adsctl-0.3.0/PKG-INFO` & `adsctl-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 Metadata-Version: 2.1
 Name: adsctl
-Version: 0.3.0
+Version: 0.4.0
 Summary: Google Ads Control CLI and Prompt
 Project-URL: Documentation, https://github.com/danielfrg/adsctl#readme
 Project-URL: Issues, https://github.com/danielfrg/adsctl/issues
 Project-URL: Source, https://github.com/danielfrg/adsctl
 Author-email: Daniel Rodriguez <daniel@danielfrg.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
 Keywords: cli,google ads,google ads api,prompt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Requires-Dist: click>=8.1
 Requires-Dist: google-ads>=20.0.0
 Requires-Dist: jinja2>=3.1.0
 Requires-Dist: pandas>=2.0.0
+Requires-Dist: pillow>=9.5.0
 Requires-Dist: prompt-toolkit>=3.0.38
 Requires-Dist: pydantic<2.0.0,>=1.10.0
 Requires-Dist: tabulate>=0.9.0
 Requires-Dist: tomli-w>=1.0
 Requires-Dist: tomlkit>=0.11.1
+Provides-Extra: test
+Requires-Dist: coverage[toml]; extra == 'test'
+Requires-Dist: pytest; extra == 'test'
+Requires-Dist: pytest-cov; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Google Ads API CLI and Prompt
 
 <p align="center">
     <a href="https://pypi.org/project/adsctl/">
         <img src="https://img.shields.io/pypi/v/adsctl.svg">
```

#### html2text {}

```diff
@@ -1,22 +1,26 @@
-Metadata-Version: 2.1 Name: adsctl Version: 0.3.0 Summary: Google Ads Control
+Metadata-Version: 2.1 Name: adsctl Version: 0.4.0 Summary: Google Ads Control
 CLI and Prompt Project-URL: Documentation, https://github.com/danielfrg/
 adsctl#readme Project-URL: Issues, https://github.com/danielfrg/adsctl/issues
 Project-URL: Source, https://github.com/danielfrg/adsctl Author-email: Daniel
 Rodriguez
 danielfrg.com> License-Expression: Apache-2.0 License-File: LICENSE.txt
 Keywords: cli,google ads,google ads api,prompt Classifier: Development Status
 :: 4 - Beta Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy Requires-
-Python: >=3.10 Requires-Dist: click>=8.1 Requires-Dist: google-ads>=20.0.0
-Requires-Dist: jinja2>=3.1.0 Requires-Dist: pandas>=2.0.0 Requires-Dist:
-prompt-toolkit>=3.0.38 Requires-Dist: pydantic<2.0.0,>=1.10.0 Requires-Dist:
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python ::
+Implementation :: CPython Classifier: Programming Language :: Python ::
+Implementation :: PyPy Requires-Python: >=3.8 Requires-Dist: click>=8.1
+Requires-Dist: google-ads>=20.0.0 Requires-Dist: jinja2>=3.1.0 Requires-Dist:
+pandas>=2.0.0 Requires-Dist: pillow>=9.5.0 Requires-Dist: prompt-
+toolkit>=3.0.38 Requires-Dist: pydantic<2.0.0,>=1.10.0 Requires-Dist:
 tabulate>=0.9.0 Requires-Dist: tomli-w>=1.0 Requires-Dist: tomlkit>=0.11.1
+Provides-Extra: test Requires-Dist: coverage[toml]; extra == 'test' Requires-
+Dist: pytest; extra == 'test' Requires-Dist: pytest-cov; extra == 'test'
 Description-Content-Type: text/markdown # Google Ads API CLI and Prompt
    [https://img.shields.io/pypi/v/adsctl.svg] [https://img.shields.io/pypi/
   pyversions/adsctl.svg] [https://github.com/danielfrg/adsctl/workflows/test/
                                   badge.svg]
  [https://img.shields.io/:license-Apache%202-blue.svg]
 Google Ads Interface for humans. _This is a work in progress, please open an
 issue if you find any bugs or have any suggestions._ Features: - A command line
```


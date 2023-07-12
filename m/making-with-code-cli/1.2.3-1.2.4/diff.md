# Comparing `tmp/making_with_code_cli-1.2.3.tar.gz` & `tmp/making_with_code_cli-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "making_with_code_cli-1.2.3.tar", max compression
+gzip compressed data, was "making_with_code_cli-1.2.4.tar", max compression
```

## Comparing `making_with_code_cli-1.2.3.tar` & `making_with_code_cli-1.2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1342 2023-05-30 14:14:06.604035 making_with_code_cli-1.2.3/README.md
--rw-r--r--   0        0        0     8199 2023-07-11 21:54:46.877560 making_with_code_cli-1.2.3/making_with_code_cli/cli.py
--rw-r--r--   0        0        0    15465 2023-07-12 13:42:10.964095 making_with_code_cli-1.2.3/making_with_code_cli/cli_setup.py
--rw-r--r--   0        0        0      551 2023-07-10 19:39:26.763192 making_with_code_cli-1.2.3/making_with_code_cli/curriculum.py
--rw-r--r--   0        0        0      658 2023-07-10 20:30:48.777211 making_with_code_cli-1.2.3/making_with_code_cli/errors.py
--rw-r--r--   0        0        0      276 2023-06-05 20:21:54.165003 making_with_code_cli-1.2.3/making_with_code_cli/git_backend/__init__.py
--rw-r--r--   0        0        0     1613 2023-07-02 18:57:59.595603 making_with_code_cli-1.2.3/making_with_code_cli/git_backend/base_backend.py
--rw-r--r--   0        0        0     3461 2023-06-05 20:20:21.178737 making_with_code_cli-1.2.3/making_with_code_cli/git_backend/github_backend.py
--rw-r--r--   0        0        0     3845 2023-06-05 20:21:08.636148 making_with_code_cli-1.2.3/making_with_code_cli/git_backend/github_org_backend.py
--rw-r--r--   0        0        0     4048 2023-07-11 16:15:54.845783 making_with_code_cli-1.2.3/making_with_code_cli/git_backend/mwc_backend.py
--rw-r--r--   0        0        0      309 2023-07-10 21:24:34.798346 making_with_code_cli-1.2.3/making_with_code_cli/git_wrapper.py
--rw-r--r--   0        0        0      266 2023-05-30 14:14:06.615290 making_with_code_cli-1.2.3/making_with_code_cli/helpers.py
--rw-r--r--   0        0        0     1526 2023-07-10 20:12:17.374391 making_with_code_cli-1.2.3/making_with_code_cli/mwc_accounts_api.py
--rw-r--r--   0        0        0     1629 2023-05-30 14:14:06.616770 making_with_code_cli-1.2.3/making_with_code_cli/settings.py
--rw-r--r--   0        0        0     1682 2023-05-30 14:14:06.617319 making_with_code_cli-1.2.3/making_with_code_cli/styles.py
--rw-r--r--   0        0        0      663 2023-07-12 13:42:18.916945 making_with_code_cli-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     2096 1970-01-01 00:00:00.000000 making_with_code_cli-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1342 2023-05-30 14:14:06.604035 making_with_code_cli-1.2.4/README.md
+-rw-r--r--   0        0        0     8199 2023-07-11 21:54:46.877560 making_with_code_cli-1.2.4/making_with_code_cli/cli.py
+-rw-r--r--   0        0        0    15436 2023-07-12 14:04:10.315780 making_with_code_cli-1.2.4/making_with_code_cli/cli_setup.py
+-rw-r--r--   0        0        0      551 2023-07-10 19:39:26.763192 making_with_code_cli-1.2.4/making_with_code_cli/curriculum.py
+-rw-r--r--   0        0        0      658 2023-07-10 20:30:48.777211 making_with_code_cli-1.2.4/making_with_code_cli/errors.py
+-rw-r--r--   0        0        0      276 2023-06-05 20:21:54.165003 making_with_code_cli-1.2.4/making_with_code_cli/git_backend/__init__.py
+-rw-r--r--   0        0        0     1613 2023-07-02 18:57:59.595603 making_with_code_cli-1.2.4/making_with_code_cli/git_backend/base_backend.py
+-rw-r--r--   0        0        0     3461 2023-06-05 20:20:21.178737 making_with_code_cli-1.2.4/making_with_code_cli/git_backend/github_backend.py
+-rw-r--r--   0        0        0     3845 2023-06-05 20:21:08.636148 making_with_code_cli-1.2.4/making_with_code_cli/git_backend/github_org_backend.py
+-rw-r--r--   0        0        0     4048 2023-07-11 16:15:54.845783 making_with_code_cli-1.2.4/making_with_code_cli/git_backend/mwc_backend.py
+-rw-r--r--   0        0        0      309 2023-07-10 21:24:34.798346 making_with_code_cli-1.2.4/making_with_code_cli/git_wrapper.py
+-rw-r--r--   0        0        0      266 2023-05-30 14:14:06.615290 making_with_code_cli-1.2.4/making_with_code_cli/helpers.py
+-rw-r--r--   0        0        0     1526 2023-07-10 20:12:17.374391 making_with_code_cli-1.2.4/making_with_code_cli/mwc_accounts_api.py
+-rw-r--r--   0        0        0     1629 2023-05-30 14:14:06.616770 making_with_code_cli-1.2.4/making_with_code_cli/settings.py
+-rw-r--r--   0        0        0     1682 2023-05-30 14:14:06.617319 making_with_code_cli-1.2.4/making_with_code_cli/styles.py
+-rw-r--r--   0        0        0      663 2023-07-12 14:08:32.551795 making_with_code_cli-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2096 1970-01-01 00:00:00.000000 making_with_code_cli-1.2.4/PKG-INFO
```

### Comparing `making_with_code_cli-1.2.3/README.md` & `making_with_code_cli-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.3/making_with_code_cli/cli.py` & `making_with_code_cli-1.2.4/making_with_code_cli/cli.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.3/making_with_code_cli/cli_setup.py` & `making_with_code_cli-1.2.4/making_with_code_cli/cli_setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,15 +225,15 @@
         return f"source {get_mwc_rc_path()}" in platform_rc_file().read_text()
 
     def run_task(self):
         with platform_rc_file().open('a') as fh:
             result = run("which mwc", shell=True, check=True, text=True, capture_output=True)
             mwcpath = Path(result.stdout).parent
             fh.write(f"\n# MAKING WITH CODE\n")
-            fh.write(f'export PATH="{mwcpath}:$PATH"\n')
+            fh.write(f'export PATH="$PATH:{mwcpath}"\n')
             fh.write(f"source {get_mwc_rc_path()}\n")
 
 class InstallHomebrew(SetupTask):
     description = "Install homebrew"
     platform = Platform.MAC
 
     def is_complete(self):
@@ -417,16 +417,15 @@
     def run_task(self):
         (Path.home() / ".gitconfig").touch()
         for key, val in self.get_expected_git_config().items():
             run(f'git config --global --replace-all {key} {val}', shell=True, check=True)
 
     def read_git_config(self, setting):
         "Reads current git config setting"
-        result = run(f"git config --get {setting}", shell=True, check=True, 
-                capture_output=True, text=True)
+        result = run(f"git config --get {setting}", shell=True, capture_output=True, text=True)
         return result.stdout.strip()
 
     def get_expected_git_config(self):
         """Returns a dict containing expected git configuration settings.
         """
         git_config = {"init.defaultBranch": "main"}
         if self.settings.get('editor') in self.editorcmds:
```

### Comparing `making_with_code_cli-1.2.3/making_with_code_cli/curriculum.py` & `making_with_code_cli-1.2.4/making_with_code_cli/curriculum.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.3/making_with_code_cli/errors.py` & `making_with_code_cli-1.2.4/making_with_code_cli/errors.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.3/making_with_code_cli/git_backend/base_backend.py` & `making_with_code_cli-1.2.4/making_with_code_cli/git_backend/base_backend.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.3/making_with_code_cli/git_backend/github_backend.py` & `making_with_code_cli-1.2.4/making_with_code_cli/git_backend/github_backend.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.3/making_with_code_cli/git_backend/github_org_backend.py` & `making_with_code_cli-1.2.4/making_with_code_cli/git_backend/github_org_backend.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.3/making_with_code_cli/git_backend/mwc_backend.py` & `making_with_code_cli-1.2.4/making_with_code_cli/git_backend/mwc_backend.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.3/making_with_code_cli/mwc_accounts_api.py` & `making_with_code_cli-1.2.4/making_with_code_cli/mwc_accounts_api.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.3/making_with_code_cli/settings.py` & `making_with_code_cli-1.2.4/making_with_code_cli/settings.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.3/making_with_code_cli/styles.py` & `making_with_code_cli-1.2.4/making_with_code_cli/styles.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.3/pyproject.toml` & `making_with_code_cli-1.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "making-with-code-cli"
-version = "1.2.3"
+version = "1.2.4"
 description = "Courseware for Making With Code"
 authors = ["Chris Proctor <chris@chrisproctor.net>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/cproctor/making-with-code-courseware"
 
 [tool.poetry.dependencies]
```

### Comparing `making_with_code_cli-1.2.3/PKG-INFO` & `making_with_code_cli-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: making-with-code-cli
-Version: 1.2.3
+Version: 1.2.4
 Summary: Courseware for Making With Code
 Home-page: https://github.com/cproctor/making-with-code-courseware
 License: MIT
 Author: Chris Proctor
 Author-email: chris@chrisproctor.net
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```


# Comparing `tmp/making_with_code_cli-1.2.2.tar.gz` & `tmp/making_with_code_cli-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "making_with_code_cli-1.2.2.tar", max compression
+gzip compressed data, was "making_with_code_cli-1.2.3.tar", max compression
```

## Comparing `making_with_code_cli-1.2.2.tar` & `making_with_code_cli-1.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1342 2023-05-30 14:14:06.604035 making_with_code_cli-1.2.2/README.md
--rw-r--r--   0        0        0     8199 2023-07-10 22:17:59.387044 making_with_code_cli-1.2.2/making_with_code_cli/cli.py
--rw-r--r--   0        0        0    15392 2023-07-10 20:16:58.660240 making_with_code_cli-1.2.2/making_with_code_cli/cli_setup.py
--rw-r--r--   0        0        0      551 2023-07-10 19:39:26.763192 making_with_code_cli-1.2.2/making_with_code_cli/curriculum.py
--rw-r--r--   0        0        0      658 2023-07-10 20:30:48.777211 making_with_code_cli-1.2.2/making_with_code_cli/errors.py
--rw-r--r--   0        0        0      276 2023-06-05 20:21:54.165003 making_with_code_cli-1.2.2/making_with_code_cli/git_backend/__init__.py
--rw-r--r--   0        0        0     1613 2023-07-02 18:57:59.595603 making_with_code_cli-1.2.2/making_with_code_cli/git_backend/base_backend.py
--rw-r--r--   0        0        0     3461 2023-06-05 20:20:21.178737 making_with_code_cli-1.2.2/making_with_code_cli/git_backend/github_backend.py
--rw-r--r--   0        0        0     3845 2023-06-05 20:21:08.636148 making_with_code_cli-1.2.2/making_with_code_cli/git_backend/github_org_backend.py
--rw-r--r--   0        0        0     4048 2023-07-11 16:15:54.845783 making_with_code_cli-1.2.2/making_with_code_cli/git_backend/mwc_backend.py
--rw-r--r--   0        0        0      309 2023-07-10 21:24:34.798346 making_with_code_cli-1.2.2/making_with_code_cli/git_wrapper.py
--rw-r--r--   0        0        0      266 2023-05-30 14:14:06.615290 making_with_code_cli-1.2.2/making_with_code_cli/helpers.py
--rw-r--r--   0        0        0     1526 2023-07-10 20:12:17.374391 making_with_code_cli-1.2.2/making_with_code_cli/mwc_accounts_api.py
--rw-r--r--   0        0        0     1629 2023-05-30 14:14:06.616770 making_with_code_cli-1.2.2/making_with_code_cli/settings.py
--rw-r--r--   0        0        0     1682 2023-05-30 14:14:06.617319 making_with_code_cli-1.2.2/making_with_code_cli/styles.py
--rw-r--r--   0        0        0      663 2023-07-11 16:16:07.656393 making_with_code_cli-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     2096 1970-01-01 00:00:00.000000 making_with_code_cli-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1342 2023-05-30 14:14:06.604035 making_with_code_cli-1.2.3/README.md
+-rw-r--r--   0        0        0     8199 2023-07-11 21:54:46.877560 making_with_code_cli-1.2.3/making_with_code_cli/cli.py
+-rw-r--r--   0        0        0    15465 2023-07-12 13:42:10.964095 making_with_code_cli-1.2.3/making_with_code_cli/cli_setup.py
+-rw-r--r--   0        0        0      551 2023-07-10 19:39:26.763192 making_with_code_cli-1.2.3/making_with_code_cli/curriculum.py
+-rw-r--r--   0        0        0      658 2023-07-10 20:30:48.777211 making_with_code_cli-1.2.3/making_with_code_cli/errors.py
+-rw-r--r--   0        0        0      276 2023-06-05 20:21:54.165003 making_with_code_cli-1.2.3/making_with_code_cli/git_backend/__init__.py
+-rw-r--r--   0        0        0     1613 2023-07-02 18:57:59.595603 making_with_code_cli-1.2.3/making_with_code_cli/git_backend/base_backend.py
+-rw-r--r--   0        0        0     3461 2023-06-05 20:20:21.178737 making_with_code_cli-1.2.3/making_with_code_cli/git_backend/github_backend.py
+-rw-r--r--   0        0        0     3845 2023-06-05 20:21:08.636148 making_with_code_cli-1.2.3/making_with_code_cli/git_backend/github_org_backend.py
+-rw-r--r--   0        0        0     4048 2023-07-11 16:15:54.845783 making_with_code_cli-1.2.3/making_with_code_cli/git_backend/mwc_backend.py
+-rw-r--r--   0        0        0      309 2023-07-10 21:24:34.798346 making_with_code_cli-1.2.3/making_with_code_cli/git_wrapper.py
+-rw-r--r--   0        0        0      266 2023-05-30 14:14:06.615290 making_with_code_cli-1.2.3/making_with_code_cli/helpers.py
+-rw-r--r--   0        0        0     1526 2023-07-10 20:12:17.374391 making_with_code_cli-1.2.3/making_with_code_cli/mwc_accounts_api.py
+-rw-r--r--   0        0        0     1629 2023-05-30 14:14:06.616770 making_with_code_cli-1.2.3/making_with_code_cli/settings.py
+-rw-r--r--   0        0        0     1682 2023-05-30 14:14:06.617319 making_with_code_cli-1.2.3/making_with_code_cli/styles.py
+-rw-r--r--   0        0        0      663 2023-07-12 13:42:18.916945 making_with_code_cli-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2096 1970-01-01 00:00:00.000000 making_with_code_cli-1.2.3/PKG-INFO
```

### Comparing `making_with_code_cli-1.2.2/README.md` & `making_with_code_cli-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.2/making_with_code_cli/cli.py` & `making_with_code_cli-1.2.3/making_with_code_cli/cli.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.2/making_with_code_cli/cli_setup.py` & `making_with_code_cli-1.2.3/making_with_code_cli/cli_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,14 +166,28 @@
 def get_shell_name():
     shellpath = run("echo $SHELL", shell=True, capture_output=True, text=True)
     return shellpath.stdout.split('/')[-1].strip()
 
 def get_mwc_rc_path():
     return (Path.home() / ".mwc_rc").resolve()
 
+def platform_rc_file():
+    shell = get_shell_name()
+    candidates = [
+        ("bash", Path.home() / ".bash_profile"),
+        ("bash", Path.home() / ".bash_rc"),
+        ("bash", Path.home() / ".bashrc"),
+        ("zsh", Path.home() / ".zprofile"),
+        ("zsh", Path.home() / ".zshrc"),
+    ]
+    for sh, rc in candidates:
+        if shell == sh and rc.exists():
+            return rc
+    raise IOError("Can't find an rc file.")
+
 class SetupTask:
     "An idempotent task"
     platform = Platform.SUPPORTED
     description = "A task"
 
     def __init__(self, settings):
         self.settings = settings
@@ -204,49 +218,38 @@
 
 class MWCShellConfig(SetupTask):
     """Writes a line in the rc shell config file sourcing ~/.mwc_rc.
     """
     description = "Link main shell config file to ~/.mwc_rc"
 
     def is_complete(self):
-        return f"source {get_mwc_rc_path()}" in self.platform_rc_file().read_text()
+        return f"source {get_mwc_rc_path()}" in platform_rc_file().read_text()
 
     def run_task(self):
-        with self.platform_rc_file().open('a') as fh:
+        with platform_rc_file().open('a') as fh:
             result = run("which mwc", shell=True, check=True, text=True, capture_output=True)
             mwcpath = Path(result.stdout).parent
             fh.write(f"\n# MAKING WITH CODE\n")
             fh.write(f'export PATH="{mwcpath}:$PATH"\n')
             fh.write(f"source {get_mwc_rc_path()}\n")
-        
-    def platform_rc_file(self):
-        shell = get_shell_name()
-        candidates = [
-            ("bash", Path.home() / ".bash_profile"),
-            ("bash", Path.home() / ".bash_rc"),
-            ("bash", Path.home() / ".bashrc"),
-            ("zsh", Path.home() / ".zprofile"),
-            ("zsh", Path.home() / ".zshrc"),
-        ]
-        for sh, rc in candidates:
-            if shell == sh and rc.exists():
-                return rc
-        raise IOError("Can't find an rc file.")
 
 class InstallHomebrew(SetupTask):
     description = "Install homebrew"
     platform = Platform.MAC
 
     def is_complete(self):
         return self.executable_on_path("brew")
 
     def run_task(self):
         click.echo(address("Installing homebrew... (this may take a while)"))
         cmd = '/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"'
         run(cmd, shell=True, check=True)
+        with platform_rc_file().open('a') as fh:
+            fh.write('\nPATH="/usr/local/bin:$PATH"\n')
+        sys.path.append("/usr/local/bin")
 
 class InstallXCode(SetupTask):
     description = "Install XCode"
     platform = Platform.MAC
 
     def is_complete(self):
         return bool(run("xcode-select -p", shell=True, capture_output=True, check=True).stdout)
```

### Comparing `making_with_code_cli-1.2.2/making_with_code_cli/curriculum.py` & `making_with_code_cli-1.2.3/making_with_code_cli/curriculum.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.2/making_with_code_cli/errors.py` & `making_with_code_cli-1.2.3/making_with_code_cli/errors.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.2/making_with_code_cli/git_backend/base_backend.py` & `making_with_code_cli-1.2.3/making_with_code_cli/git_backend/base_backend.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.2/making_with_code_cli/git_backend/github_backend.py` & `making_with_code_cli-1.2.3/making_with_code_cli/git_backend/github_backend.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.2/making_with_code_cli/git_backend/github_org_backend.py` & `making_with_code_cli-1.2.3/making_with_code_cli/git_backend/github_org_backend.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.2/making_with_code_cli/git_backend/mwc_backend.py` & `making_with_code_cli-1.2.3/making_with_code_cli/git_backend/mwc_backend.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.2/making_with_code_cli/mwc_accounts_api.py` & `making_with_code_cli-1.2.3/making_with_code_cli/mwc_accounts_api.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.2/making_with_code_cli/settings.py` & `making_with_code_cli-1.2.3/making_with_code_cli/settings.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.2/making_with_code_cli/styles.py` & `making_with_code_cli-1.2.3/making_with_code_cli/styles.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.2/pyproject.toml` & `making_with_code_cli-1.2.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "making-with-code-cli"
-version = "1.2.2"
+version = "1.2.3"
 description = "Courseware for Making With Code"
 authors = ["Chris Proctor <chris@chrisproctor.net>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/cproctor/making-with-code-courseware"
 
 [tool.poetry.dependencies]
```

### Comparing `making_with_code_cli-1.2.2/PKG-INFO` & `making_with_code_cli-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: making-with-code-cli
-Version: 1.2.2
+Version: 1.2.3
 Summary: Courseware for Making With Code
 Home-page: https://github.com/cproctor/making-with-code-courseware
 License: MIT
 Author: Chris Proctor
 Author-email: chris@chrisproctor.net
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```


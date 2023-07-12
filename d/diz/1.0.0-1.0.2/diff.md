# Comparing `tmp/diz-1.0.0.tar.gz` & `tmp/diz-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diz-1.0.0.tar", last modified: Mon Jul 10 12:10:09 2023, max compression
+gzip compressed data, was "diz-1.0.2.tar", last modified: Wed Jul 12 11:59:23 2023, max compression
```

## Comparing `diz-1.0.0.tar` & `diz-1.0.2.tar`

### file list

```diff
@@ -1,28 +1,37 @@
-drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 12:10:09.751318 diz-1.0.0/
--rw-r--r--   0 mj         (501) staff       (20)     2242 2023-07-10 12:10:09.751213 diz-1.0.0/PKG-INFO
--rw-r--r--   0 mj         (501) staff       (20)     2092 2023-07-10 12:09:27.000000 diz-1.0.0/README.md
-drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 12:10:09.747994 diz-1.0.0/diz/
--rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-10 03:55:54.000000 diz-1.0.0/diz/__init__.py
-drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 12:10:09.749364 diz-1.0.0/diz/commands/
--rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-09 04:12:43.000000 diz-1.0.0/diz/commands/__init__.py
--rw-r--r--   0 mj         (501) staff       (20)      480 2023-07-10 07:28:31.000000 diz-1.0.0/diz/commands/install.py
--rw-r--r--   0 mj         (501) staff       (20)     2146 2023-07-10 07:31:06.000000 diz-1.0.0/diz/commands/setup.py
--rw-r--r--   0 mj         (501) staff       (20)     1069 2023-07-10 12:08:33.000000 diz-1.0.0/diz/commands/shell.py
--rw-r--r--   0 mj         (501) staff       (20)     1979 2023-07-10 12:06:10.000000 diz-1.0.0/diz/main.py
-drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 12:10:09.750932 diz-1.0.0/diz/utils/
--rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-09 03:48:51.000000 diz-1.0.0/diz/utils/__init__.py
--rw-r--r--   0 mj         (501) staff       (20)      237 2023-07-09 05:10:52.000000 diz-1.0.0/diz/utils/dir.py
--rw-r--r--   0 mj         (501) staff       (20)      161 2023-07-09 05:15:30.000000 diz-1.0.0/diz/utils/download.py
--rw-r--r--   0 mj         (501) staff       (20)      831 2023-07-10 08:31:21.000000 diz-1.0.0/diz/utils/pip.py
--rw-r--r--   0 mj         (501) staff       (20)      144 2023-07-09 14:45:55.000000 diz-1.0.0/diz/utils/validators.py
--rw-r--r--   0 mj         (501) staff       (20)     1226 2023-07-10 07:57:15.000000 diz-1.0.0/diz/utils/venv.py
--rw-r--r--   0 mj         (501) staff       (20)      308 2023-07-10 04:14:09.000000 diz-1.0.0/diz/utils/yaml.py
-drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-10 12:10:09.748633 diz-1.0.0/diz.egg-info/
--rw-r--r--   0 mj         (501) staff       (20)     2242 2023-07-10 12:10:09.000000 diz-1.0.0/diz.egg-info/PKG-INFO
--rw-r--r--   0 mj         (501) staff       (20)      441 2023-07-10 12:10:09.000000 diz-1.0.0/diz.egg-info/SOURCES.txt
--rw-r--r--   0 mj         (501) staff       (20)        1 2023-07-10 12:10:09.000000 diz-1.0.0/diz.egg-info/dependency_links.txt
--rw-r--r--   0 mj         (501) staff       (20)       38 2023-07-10 12:10:09.000000 diz-1.0.0/diz.egg-info/entry_points.txt
--rw-r--r--   0 mj         (501) staff       (20)      129 2023-07-10 12:10:09.000000 diz-1.0.0/diz.egg-info/requires.txt
--rw-r--r--   0 mj         (501) staff       (20)        4 2023-07-10 12:10:09.000000 diz-1.0.0/diz.egg-info/top_level.txt
--rw-r--r--   0 mj         (501) staff       (20)       38 2023-07-10 12:10:09.751355 diz-1.0.0/setup.cfg
--rw-r--r--   0 mj         (501) staff       (20)      703 2023-07-10 12:09:52.000000 diz-1.0.0/setup.py
+drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-12 11:59:23.763490 diz-1.0.2/
+-rw-r--r--   0 mj         (501) staff       (20)     2242 2023-07-12 11:59:23.763376 diz-1.0.2/PKG-INFO
+-rw-r--r--   0 mj         (501) staff       (20)     2092 2023-07-10 12:09:27.000000 diz-1.0.2/README.md
+drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-12 11:59:23.758509 diz-1.0.2/diz/
+-rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-10 03:55:54.000000 diz-1.0.2/diz/__init__.py
+drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-12 11:59:23.760082 diz-1.0.2/diz/commands/
+-rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-09 04:12:43.000000 diz-1.0.2/diz/commands/__init__.py
+-rw-r--r--   0 mj         (501) staff       (20)      480 2023-07-10 07:28:31.000000 diz-1.0.2/diz/commands/install.py
+-rw-r--r--   0 mj         (501) staff       (20)     2153 2023-07-12 07:28:11.000000 diz-1.0.2/diz/commands/setup.py
+-rw-r--r--   0 mj         (501) staff       (20)     1069 2023-07-10 12:08:33.000000 diz-1.0.2/diz/commands/shell.py
+-rw-r--r--   0 mj         (501) staff       (20)     1979 2023-07-10 12:06:10.000000 diz-1.0.2/diz/main.py
+drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-12 11:59:23.761704 diz-1.0.2/diz/utils/
+-rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-09 03:48:51.000000 diz-1.0.2/diz/utils/__init__.py
+-rw-r--r--   0 mj         (501) staff       (20)      302 2023-07-12 07:12:36.000000 diz-1.0.2/diz/utils/dir.py
+-rw-r--r--   0 mj         (501) staff       (20)      161 2023-07-09 05:15:30.000000 diz-1.0.2/diz/utils/download.py
+-rw-r--r--   0 mj         (501) staff       (20)      831 2023-07-10 08:31:21.000000 diz-1.0.2/diz/utils/pip.py
+-rw-r--r--   0 mj         (501) staff       (20)      305 2023-07-12 07:24:42.000000 diz-1.0.2/diz/utils/shell.py
+-rw-r--r--   0 mj         (501) staff       (20)      144 2023-07-09 14:45:55.000000 diz-1.0.2/diz/utils/validators.py
+-rw-r--r--   0 mj         (501) staff       (20)      927 2023-07-11 02:44:28.000000 diz-1.0.2/diz/utils/venv.py
+-rw-r--r--   0 mj         (501) staff       (20)      308 2023-07-10 04:14:09.000000 diz-1.0.2/diz/utils/yaml.py
+drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-12 11:59:23.759393 diz-1.0.2/diz.egg-info/
+-rw-r--r--   0 mj         (501) staff       (20)     2242 2023-07-12 11:59:23.000000 diz-1.0.2/diz.egg-info/PKG-INFO
+-rw-r--r--   0 mj         (501) staff       (20)      608 2023-07-12 11:59:23.000000 diz-1.0.2/diz.egg-info/SOURCES.txt
+-rw-r--r--   0 mj         (501) staff       (20)        1 2023-07-12 11:59:23.000000 diz-1.0.2/diz.egg-info/dependency_links.txt
+-rw-r--r--   0 mj         (501) staff       (20)       38 2023-07-12 11:59:23.000000 diz-1.0.2/diz.egg-info/entry_points.txt
+-rw-r--r--   0 mj         (501) staff       (20)      129 2023-07-12 11:59:23.000000 diz-1.0.2/diz.egg-info/requires.txt
+-rw-r--r--   0 mj         (501) staff       (20)       10 2023-07-12 11:59:23.000000 diz-1.0.2/diz.egg-info/top_level.txt
+-rw-r--r--   0 mj         (501) staff       (20)       38 2023-07-12 11:59:23.763528 diz-1.0.2/setup.cfg
+-rw-r--r--   0 mj         (501) staff       (20)      703 2023-07-12 11:58:23.000000 diz-1.0.2/setup.py
+drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-12 11:59:23.761932 diz-1.0.2/tests/
+-rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-10 12:23:05.000000 diz-1.0.2/tests/__init__.py
+drwxr-xr-x   0 mj         (501) staff       (20)        0 2023-07-12 11:59:23.763008 diz-1.0.2/tests/utils/
+-rw-r--r--   0 mj         (501) staff       (20)        0 2023-07-10 12:20:20.000000 diz-1.0.2/tests/utils/__init__.py
+-rw-r--r--   0 mj         (501) staff       (20)      131 2023-07-10 12:21:51.000000 diz-1.0.2/tests/utils/test_dir.py
+-rw-r--r--   0 mj         (501) staff       (20)       99 2023-07-11 02:54:04.000000 diz-1.0.2/tests/utils/test_shell.py
+-rw-r--r--   0 mj         (501) staff       (20)      124 2023-07-11 02:55:24.000000 diz-1.0.2/tests/utils/test_validators.py
+-rw-r--r--   0 mj         (501) staff       (20)      137 2023-07-11 02:51:48.000000 diz-1.0.2/tests/utils/test_venv.py
```

### Comparing `diz-1.0.0/PKG-INFO` & `diz-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diz
-Version: 1.0.0
+Version: 1.0.2
 Summary: 用来构建大模型环境的工具
 Author: mjason
 Description-Content-Type: text/markdown
 
 # diz
 
 目前开源的大模型项目普遍来说都有如下问题：
```

### Comparing `diz-1.0.0/README.md` & `diz-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `diz-1.0.0/diz/commands/setup.py` & `diz-1.0.2/diz/commands/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,59 +1,60 @@
 import os.path
 import git
 import diz.utils.dir
-from diz.utils import pip
-from diz.utils import download, yaml
+from diz.utils import download, yaml, shell, pip
 from toolz import pipe
 
 
 class SetupCommand:
     def __init__(self, pkg: str, path: str):
         self.pkg = pkg
         self.path = path
         self.config = yaml.load_yaml(self.pkg)
         self.install_path = self.path
 
-    def create_dir(self, path, print_path=True):
-        target_path = pipe(
-            path,
-            lambda p: os.path.join(self.install_path, p),
-            os.path.expanduser,
-        )
+    def find_and_create_dir(self, path):
+        target_path = self.get_dir(path)
         if not os.path.exists(target_path):
             os.makedirs(target_path)
-        if print_path:
-            print(f"创建目录：{target_path}")
+        return target_path
+
+    def create_dir(self, path):
+        target_path = self.find_and_create_dir(path)
+        print(f"创建目录：{target_path}")
         return target_path
 
     def get_dir(self, path):
         target_path = pipe(
             path,
             lambda p: os.path.join(self.install_path, p),
             os.path.expanduser,
         )
         return target_path
 
     def clone_code(self):
-        if diz.utils.dir.is_empty(self.create_dir("code", False)):
-            git.Repo.clone_from(self.config['code_repo'], self.create_dir("code", False))
+        code_path = self.find_and_create_dir("code")
+        if diz.utils.dir.is_empty(code_path):
+            git.Repo.clone_from(self.config['code_repo'], code_path)
             print("下载完成！")
         else:
             print("已经下载过了，无需下载。")
 
     def download_model_from_huggingface(self):
-        if diz.utils.dir.is_empty(self.create_dir("model", False)):
-            download.save_huggingface_model(self.config['huggingface'], self.create_dir("model", False))
+        model_path = self.find_and_create_dir("model")
+        if diz.utils.dir.is_empty(model_path):
+            download.save_huggingface_model(self.config['huggingface'], model_path)
             print("下载完成！")
         else:
             print("已经下载过了，无需下载。")
 
     def create_venv(self):
-        if diz.utils.dir.is_empty(self.create_dir("venv", False)):
-            os.system(f"cd {self.path} && python -m venv venv")
+        venv_path = self.get_dir("venv")
+        if not diz.utils.dir.is_empty(venv_path):
+            shell.run(f"cd {self.path} && python -m venv venv")
             print("创建虚拟环境完成！")
 
     def install_deps(self):
         venv_path = self.get_dir("venv")
         for dep in self.config['deps']:
             pip.install(dep, venv_path)
         pip.install("diz", venv_path)
```

### Comparing `diz-1.0.0/diz/commands/shell.py` & `diz-1.0.2/diz/commands/shell.py`

 * *Files identical despite different names*

### Comparing `diz-1.0.0/diz/main.py` & `diz-1.0.2/diz/main.py`

 * *Files identical despite different names*

### Comparing `diz-1.0.0/diz/utils/pip.py` & `diz-1.0.2/diz/utils/pip.py`

 * *Files identical despite different names*

### Comparing `diz-1.0.0/diz/utils/venv.py` & `diz-1.0.2/diz/utils/venv.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,14 @@
 import platform
-import os
-
-
-def get_current_shell():
-    shell = os.environ.get('SHELL', '')
-    if shell.endswith('bash'):
-        return 'bash'
-    elif shell.endswith('zsh'):
-        return 'zsh'
-    elif shell.endswith('fish'):
-        return 'fish'
-    elif 'csh' in shell or 'tcsh' in shell:
-        return 'csh'
-    else:
-        raise ValueError("Unsupported shell")
+from diz.utils.shell import current as get_current_shell
 
 
 def get_activate_command(venv_path):
     system = platform.system()
-    shell = get_current_shell()
+    shell, _ = get_current_shell()
 
     if system == 'Windows':
         if shell == 'cmd.exe':
             return f'call {venv_path}\\Scripts\\activate.bat'
         elif shell == 'PowerShell':
             return f'& {venv_path}\\Scripts\\Activate.ps1'
         else:
```

### Comparing `diz-1.0.0/diz.egg-info/PKG-INFO` & `diz-1.0.2/diz.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diz
-Version: 1.0.0
+Version: 1.0.2
 Summary: 用来构建大模型环境的工具
 Author: mjason
 Description-Content-Type: text/markdown
 
 # diz
 
 目前开源的大模型项目普遍来说都有如下问题：
```

### Comparing `diz-1.0.0/setup.py` & `diz-1.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='diz',
-    version='1.0.0',
+    version='1.0.2',
     author='mjason',
     description='用来构建大模型环境的工具',
     long_description=readme(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
         'GitPython>=3.1.31',
```


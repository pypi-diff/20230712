# Comparing `tmp/flytekitplugins-envd-1.7.1b1.tar.gz` & `tmp/flytekitplugins-envd-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-envd-1.7.1b1.tar", last modified: Tue Jun 27 22:00:54 2023, max compression
+gzip compressed data, was "flytekitplugins-envd-1.8.0.tar", last modified: Tue Jul 11 22:07:17 2023, max compression
```

## Comparing `flytekitplugins-envd-1.7.1b1.tar` & `flytekitplugins-envd-1.8.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:54.636640 flytekitplugins-envd-1.7.1b1/
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-27 22:00:54.636640 flytekitplugins-envd-1.7.1b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-27 22:00:35.000000 flytekitplugins-envd-1.7.1b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:54.636640 flytekitplugins-envd-1.7.1b1/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:54.636640 flytekitplugins-envd-1.7.1b1/flytekitplugins/envd/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-27 22:00:35.000000 flytekitplugins-envd-1.7.1b1/flytekitplugins/envd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-06-27 22:00:35.000000 flytekitplugins-envd-1.7.1b1/flytekitplugins/envd/image_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 22:00:54.636640 flytekitplugins-envd-1.7.1b1/flytekitplugins_envd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-27 22:00:54.000000 flytekitplugins-envd-1.7.1b1/flytekitplugins_envd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-27 22:00:54.000000 flytekitplugins-envd-1.7.1b1/flytekitplugins_envd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 22:00:54.000000 flytekitplugins-envd-1.7.1b1/flytekitplugins_envd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-27 22:00:54.000000 flytekitplugins-envd-1.7.1b1/flytekitplugins_envd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 22:00:54.000000 flytekitplugins-envd-1.7.1b1/flytekitplugins_envd.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-27 22:00:54.000000 flytekitplugins-envd-1.7.1b1/flytekitplugins_envd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-27 22:00:54.000000 flytekitplugins-envd-1.7.1b1/flytekitplugins_envd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 22:00:54.636640 flytekitplugins-envd-1.7.1b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-27 22:00:50.000000 flytekitplugins-envd-1.7.1b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:17.291687 flytekitplugins-envd-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-11 22:07:17.291687 flytekitplugins-envd-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-11 22:06:52.000000 flytekitplugins-envd-1.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:17.287687 flytekitplugins-envd-1.8.0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:17.291687 flytekitplugins-envd-1.8.0/flytekitplugins/envd/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-11 22:06:52.000000 flytekitplugins-envd-1.8.0/flytekitplugins/envd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-11 22:06:52.000000 flytekitplugins-envd-1.8.0/flytekitplugins/envd/image_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:07:17.291687 flytekitplugins-envd-1.8.0/flytekitplugins_envd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-11 22:07:17.000000 flytekitplugins-envd-1.8.0/flytekitplugins_envd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-11 22:07:17.000000 flytekitplugins-envd-1.8.0/flytekitplugins_envd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 22:07:17.000000 flytekitplugins-envd-1.8.0/flytekitplugins_envd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-11 22:07:17.000000 flytekitplugins-envd-1.8.0/flytekitplugins_envd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 22:07:17.000000 flytekitplugins-envd-1.8.0/flytekitplugins_envd.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 22:07:17.000000 flytekitplugins-envd-1.8.0/flytekitplugins_envd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 22:07:17.000000 flytekitplugins-envd-1.8.0/flytekitplugins_envd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 22:07:17.291687 flytekitplugins-envd-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-11 22:07:11.000000 flytekitplugins-envd-1.8.0/setup.py
```

### Comparing `flytekitplugins-envd-1.7.1b1/PKG-INFO` & `flytekitplugins-envd-1.8.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-envd
-Version: 1.7.1b1
+Version: 1.8.0
 Summary: This package enables users to easily build a Docker image for tasks or workflows.
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-envd-1.7.1b1/README.md` & `flytekitplugins-envd-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-envd-1.7.1b1/flytekitplugins/envd/image_builder.py` & `flytekitplugins-envd-1.8.0/flytekitplugins/envd/image_builder.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,49 @@
+import os
 import pathlib
 import shutil
 import subprocess
 
 import click
 
 from flytekit.configuration import DefaultImages
 from flytekit.core import context_manager
+from flytekit.core.constants import REQUIREMENTS_FILE_NAME
 from flytekit.image_spec.image_spec import _F_IMG_ID, ImageBuildEngine, ImageSpec, ImageSpecBuilder
 
 
 class EnvdImageSpecBuilder(ImageSpecBuilder):
     """
     This class is used to build a docker image using envd.
     """
 
-    def build_image(self, image_spec: ImageSpec):
-        cfg_path = create_envd_config(image_spec)
-        command = f"envd build --path {pathlib.Path(cfg_path).parent}  --platform {image_spec.platform}"
-        if image_spec.registry:
-            command += f" --output type=image,name={image_spec.image_name()},push=true"
+    def execute_command(self, command):
         click.secho(f"Run command: {command} ", fg="blue")
         p = subprocess.Popen(command.split(), stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         for line in iter(p.stdout.readline, ""):
             if p.poll() is not None:
                 break
             if line.decode().strip() != "":
                 click.secho(line.decode().strip(), fg="blue")
 
         if p.returncode != 0:
             _, stderr = p.communicate()
-            raise Exception(
-                f"failed to build the imageSpec at {cfg_path} with error {stderr}",
-            )
+            raise Exception(f"failed to run command {command} with error {stderr}")
+
+    def build_image(self, image_spec: ImageSpec):
+        cfg_path = create_envd_config(image_spec)
+
+        if image_spec.registry_config:
+            bootstrap_command = f"envd bootstrap --registry-config {image_spec.registry_config}"
+            self.execute_command(bootstrap_command)
+
+        build_command = f"envd build --path {pathlib.Path(cfg_path).parent}  --platform {image_spec.platform}"
+        if image_spec.registry:
+            build_command += f" --output type=image,name={image_spec.image_name()},push=true"
+        self.execute_command(build_command)
 
 
 def create_envd_config(image_spec: ImageSpec) -> str:
     base_image = DefaultImages.default_image() if image_spec.base_image is None else image_spec.base_image
     if image_spec.cuda:
         if image_spec.python_version is None:
             raise Exception("python_version is required when cuda and cudnn are specified")
@@ -48,23 +56,28 @@
         env.update(image_spec.env)
     pip_index = "https://pypi.org/simple" if image_spec.pip_index is None else image_spec.pip_index
 
     envd_config = f"""# syntax=v1
 
 def build():
     base(image="{base_image}", dev=False)
-    install.python_packages(name = [{', '.join(map(str, map(lambda x: f'"{x}"', packages)))}])
-    install.apt_packages(name = [{', '.join(map(str, map(lambda x: f'"{x}"', apt_packages)))}])
+    install.python_packages(name=[{', '.join(map(str, map(lambda x: f'"{x}"', packages)))}])
+    install.apt_packages(name=[{', '.join(map(str, map(lambda x: f'"{x}"', apt_packages)))}])
     runtime.environ(env={env})
-    config.pip_index(url = "{pip_index}")
+    config.pip_index(url="{pip_index}")
 """
     ctx = context_manager.FlyteContextManager.current_context()
     cfg_path = ctx.file_access.get_random_local_path("build.envd")
     pathlib.Path(cfg_path).parent.mkdir(parents=True, exist_ok=True)
 
+    if image_spec.requirements:
+        requirement_path = f"{pathlib.Path(cfg_path).parent}{os.sep}{REQUIREMENTS_FILE_NAME}"
+        shutil.copyfile(image_spec.requirements, requirement_path)
+        envd_config += f'    install.python_packages(requirements="{REQUIREMENTS_FILE_NAME}")\n'
+
     if image_spec.python_version:
         # Indentation is required by envd
         envd_config += f'    install.python(version="{image_spec.python_version}")\n'
 
     if image_spec.cuda:
         cudnn = image_spec.cudnn if image_spec.cudnn else ""
         envd_config += f'    install.cuda(version="{image_spec.cuda}", cudnn="{cudnn}")\n'
```

### Comparing `flytekitplugins-envd-1.7.1b1/flytekitplugins_envd.egg-info/PKG-INFO` & `flytekitplugins-envd-1.8.0/flytekitplugins_envd.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-envd
-Version: 1.7.1b1
+Version: 1.8.0
 Summary: This package enables users to easily build a Docker image for tasks or workflows.
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-envd-1.7.1b1/setup.py` & `flytekitplugins-envd-1.8.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup
 
 PLUGIN_NAME = "envd"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
-plugin_requires = ["flytekit", "envd>=0.3.22"]
+plugin_requires = ["flytekit", "envd>=0.3.33"]
 
-__version__ = "1.7.1b1"
+__version__ = "1.8.0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This package enables users to easily build a Docker image for tasks or workflows.",
```


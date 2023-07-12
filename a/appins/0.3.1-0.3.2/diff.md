# Comparing `tmp/appins-0.3.1.tar.gz` & `tmp/appins-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appins-0.3.1.tar", last modified: Wed Jul 12 08:51:55 2023, max compression
+gzip compressed data, was "appins-0.3.2.tar", last modified: Wed Jul 12 11:06:41 2023, max compression
```

## Comparing `appins-0.3.1.tar` & `appins-0.3.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1342 2023-02-18 13:26:33.609851 appins-0.3.1/.gitignore
--rw-r--r--   0        0        0     1069 2023-02-18 13:26:33.609851 appins-0.3.1/LICENSE
--rw-r--r--   0        0        0      343 2023-02-18 14:52:19.365671 appins-0.3.1/Makefile
--rw-r--r--   0        0        0      370 2023-02-18 20:34:14.382069 appins-0.3.1/README.md
--rw-r--r--   0        0        0       22 2023-07-12 08:50:21.966094 appins-0.3.1/appins/__init__.py
--rw-r--r--   0        0        0       29 2023-02-18 20:04:53.442182 appins-0.3.1/appins/__main__.py
--rw-r--r--   0        0        0     8763 2023-07-05 20:08:43.691377 appins-0.3.1/appins/main.py
--rw-r--r--   0        0        0     4759 2023-07-12 08:49:03.528997 appins-0.3.1/appins/prompt_template.txt
--rw-r--r--   0        0        0     2193 2023-07-12 08:50:05.145867 appins-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      198 2023-07-12 08:49:09.393082 appins-0.3.1/requirements.txt
--rw-r--r--   0        0        0      272 2023-02-18 14:47:26.295062 appins-0.3.1/setup.cfg
--rw-r--r--   0        0        0      106 2023-02-18 19:50:11.030745 appins-0.3.1/test_build.py
--rw-r--r--   0        0        0     1892 1970-01-01 00:00:00.000000 appins-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1342 2023-02-18 13:26:33.609851 appins-0.3.2/.gitignore
+-rw-r--r--   0        0        0     1069 2023-02-18 13:26:33.609851 appins-0.3.2/LICENSE
+-rw-r--r--   0        0        0      343 2023-02-18 14:52:19.365671 appins-0.3.2/Makefile
+-rw-r--r--   0        0        0      370 2023-02-18 20:34:14.382069 appins-0.3.2/README.md
+-rw-r--r--   0        0        0       22 2023-07-12 11:05:18.066996 appins-0.3.2/appins/__init__.py
+-rw-r--r--   0        0        0       29 2023-02-18 20:04:53.442182 appins-0.3.2/appins/__main__.py
+-rw-r--r--   0        0        0     8702 2023-07-12 11:05:18.378998 appins-0.3.2/appins/main.py
+-rw-r--r--   0        0        0     4759 2023-07-12 08:49:03.528997 appins-0.3.2/appins/prompt_template.txt
+-rw-r--r--   0        0        0     2193 2023-07-12 08:50:05.145867 appins-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      198 2023-07-12 08:49:09.393082 appins-0.3.2/requirements.txt
+-rw-r--r--   0        0        0      272 2023-02-18 14:47:26.295062 appins-0.3.2/setup.cfg
+-rw-r--r--   0        0        0      106 2023-02-18 19:50:11.030745 appins-0.3.2/test_build.py
+-rw-r--r--   0        0        0     1892 1970-01-01 00:00:00.000000 appins-0.3.2/PKG-INFO
```

### Comparing `appins-0.3.1/.gitignore` & `appins-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `appins-0.3.1/LICENSE` & `appins-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `appins-0.3.1/appins/main.py` & `appins-0.3.2/appins/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,27 +38,24 @@
         },
     )
 
     cwd = pathlib.Path.cwd()
     apps_dir = cwd / project_slug / "apps"
 
     core_app_url = "git@github.com:enabledu/enabled.git"
-    print(f"Cloning {core_app_url}...")
 
     subprocess.run(["git", "clone", core_app_url, apps_dir / "enabled"])
 
 
 @app.command(help="Clone an app repository from GitHub into apps directory.")
 def clone_app(app_url: str):
     """
     Clone an app repository from GitHub into apps directory. and install requirements.
     url: The url of the repository to clone.
     """
-    print(f"Cloning {app_url}...")
-
     apps_directory = "." if pathlib.Path.cwd().name == "apps" else "./apps"
     app_to_clone = app_url.split("/")[-1].replace(".git", "")
 
     subprocess.run(["git", "clone", app_url, apps_directory + "/" + app_to_clone])
     write_app_name(app_to_clone)
 
 
@@ -133,22 +130,22 @@
 
 @app.command()
 def install_requirements():
     """
     Install app requirements.
     app_name: The name of the app to install.
     """
-    print(f"Installing requirements")
+    print(f"Installing requirements...")
     cwd = pathlib.Path.cwd()
     is_apps_besides = True if (cwd / "apps").exists() else False
     if is_apps_besides:
         apps_dir = cwd / "apps"
         for app_dir in apps_dir.iterdir():
             if app_dir.is_dir():
-                requirements_file = app_dir / "requirements.txt"
+                requirements_file = app_dir / "backend" / "requirements.txt"
                 if requirements_file.exists():
                     subprocess.run(
                         ["python", "-m", "pip", "install", "-r", requirements_file]
                     )
     else:
         print(
             "No apps directory found. Make sure you are in the project root directory."
```

### Comparing `appins-0.3.1/appins/prompt_template.txt` & `appins-0.3.2/appins/prompt_template.txt`

 * *Files identical despite different names*

### Comparing `appins-0.3.1/pyproject.toml` & `appins-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `appins-0.3.1/PKG-INFO` & `appins-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appins
-Version: 0.3.1
+Version: 0.3.2
 Summary: appins - cli tool for enabledu ecosystem
 Author-email: 0xsirsaif <sirsaif99@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```


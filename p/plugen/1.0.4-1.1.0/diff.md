# Comparing `tmp/plugen-1.0.4.tar.gz` & `tmp/plugen-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plugen-1.0.4.tar", last modified: Mon Jul 10 05:16:47 2023, max compression
+gzip compressed data, was "plugen-1.1.0.tar", last modified: Wed Jul 12 19:02:49 2023, max compression
```

## Comparing `plugen-1.0.4.tar` & `plugen-1.1.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-10 05:16:47.279671 plugen-1.0.4/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      215 2023-07-10 05:16:47.279671 plugen-1.0.4/PKG-INFO
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     3774 2023-07-09 18:55:27.000000 plugen-1.0.4/README.md
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-10 05:16:47.279671 plugen-1.0.4/plugen/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)       19 2023-07-10 05:15:24.000000 plugen-1.0.4/plugen/__init__.py
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-10 05:16:47.279671 plugen-1.0.4/plugen/lib/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)       41 2023-07-09 05:59:38.000000 plugen-1.0.4/plugen/lib/__init__.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      942 2023-07-09 18:33:02.000000 plugen-1.0.4/plugen/lib/build.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     1968 2023-07-09 18:38:01.000000 plugen-1.0.4/plugen/lib/plugin.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     2526 2023-07-09 18:33:02.000000 plugen-1.0.4/plugen/lib/serve.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      522 2023-07-09 09:14:03.000000 plugen-1.0.4/plugen/lib/utils.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     1742 2023-07-10 05:14:56.000000 plugen-1.0.4/plugen/main.py
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-10 05:16:47.279671 plugen-1.0.4/plugen/plugins/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-1.0.4/plugen/plugins/__init__.py
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-10 05:16:47.279671 plugen-1.0.4/plugen/plugins/copydest/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-1.0.4/plugen/plugins/copydest/__init__.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      362 2023-07-09 09:15:39.000000 plugen-1.0.4/plugen/plugins/copydest/plugin.py
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-10 05:16:47.279671 plugen-1.0.4/plugen/plugins/hotreload/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-1.0.4/plugen/plugins/hotreload/__init__.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     1820 2023-07-09 09:36:13.000000 plugen-1.0.4/plugen/plugins/hotreload/plugin.py
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-10 05:16:47.279671 plugen-1.0.4/plugen/plugins/imagecompressor/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-1.0.4/plugen/plugins/imagecompressor/__init__.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      212 2023-07-09 06:47:18.000000 plugen-1.0.4/plugen/plugins/imagecompressor/plugin.py
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-10 05:16:47.279671 plugen-1.0.4/plugen/plugins/sass/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-1.0.4/plugen/plugins/sass/__init__.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      534 2023-07-09 10:19:25.000000 plugen-1.0.4/plugen/plugins/sass/plugin.py
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-10 05:16:47.279671 plugen-1.0.4/plugen/plugins/tailwind/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-1.0.4/plugen/plugins/tailwind/__init__.py
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      212 2023-07-09 06:47:22.000000 plugen-1.0.4/plugen/plugins/tailwind/plugin.py
-drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-10 05:16:47.279671 plugen-1.0.4/plugen.egg-info/
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      215 2023-07-10 05:16:47.000000 plugen-1.0.4/plugen.egg-info/PKG-INFO
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      771 2023-07-10 05:16:47.000000 plugen-1.0.4/plugen.egg-info/SOURCES.txt
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        1 2023-07-10 05:16:47.000000 plugen-1.0.4/plugen.egg-info/dependency_links.txt
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)       39 2023-07-10 05:16:47.000000 plugen-1.0.4/plugen.egg-info/entry_points.txt
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)       18 2023-07-10 05:16:47.000000 plugen-1.0.4/plugen.egg-info/requires.txt
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        7 2023-07-10 05:16:47.000000 plugen-1.0.4/plugen.egg-info/top_level.txt
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)       38 2023-07-10 05:16:47.279671 plugen-1.0.4/setup.cfg
--rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      495 2023-07-10 05:16:42.000000 plugen-1.0.4/setup.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-12 19:02:49.364956 plugen-1.1.0/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      215 2023-07-12 19:02:49.364956 plugen-1.1.0/PKG-INFO
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     3758 2023-07-12 18:56:28.000000 plugen-1.1.0/README.md
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-12 19:02:49.360957 plugen-1.1.0/plugen/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)       19 2023-07-10 05:15:24.000000 plugen-1.1.0/plugen/__init__.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-12 19:02:49.360957 plugen-1.1.0/plugen/lib/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)       41 2023-07-09 05:59:38.000000 plugen-1.1.0/plugen/lib/__init__.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      942 2023-07-09 18:33:02.000000 plugen-1.1.0/plugen/lib/build.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      256 2023-07-12 05:01:03.000000 plugen-1.1.0/plugen/lib/init.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     1968 2023-07-09 18:38:01.000000 plugen-1.1.0/plugen/lib/plugin.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     2526 2023-07-09 18:33:02.000000 plugen-1.1.0/plugen/lib/serve.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      522 2023-07-09 09:14:03.000000 plugen-1.1.0/plugen/lib/utils.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     1927 2023-07-12 05:01:40.000000 plugen-1.1.0/plugen/main.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-12 19:02:49.360957 plugen-1.1.0/plugen/plugins/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-1.1.0/plugen/plugins/__init__.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-12 19:02:49.360957 plugen-1.1.0/plugen/plugins/copydest/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-1.1.0/plugen/plugins/copydest/__init__.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      677 2023-07-12 05:19:15.000000 plugen-1.1.0/plugen/plugins/copydest/plugin.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-12 19:02:49.360957 plugen-1.1.0/plugen/plugins/hotreload/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-1.1.0/plugen/plugins/hotreload/__init__.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     1820 2023-07-09 09:36:13.000000 plugen-1.1.0/plugen/plugins/hotreload/plugin.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-12 19:02:49.360957 plugen-1.1.0/plugen/plugins/imagecompressor/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-1.1.0/plugen/plugins/imagecompressor/__init__.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      212 2023-07-09 06:47:18.000000 plugen-1.1.0/plugen/plugins/imagecompressor/plugin.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-12 19:02:49.360957 plugen-1.1.0/plugen/plugins/sass/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-1.1.0/plugen/plugins/sass/__init__.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      534 2023-07-09 10:19:25.000000 plugen-1.1.0/plugen/plugins/sass/plugin.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-12 19:02:49.364956 plugen-1.1.0/plugen/plugins/tailwind/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-09 18:33:01.000000 plugen-1.1.0/plugen/plugins/tailwind/__init__.py
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)     1356 2023-07-12 05:25:42.000000 plugen-1.1.0/plugen/plugins/tailwind/plugin.py
+drwxrwxr-x   0 aclarembeau  (1000) aclarembeau  (1000)        0 2023-07-12 19:02:49.360957 plugen-1.1.0/plugen.egg-info/
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      215 2023-07-12 19:02:49.000000 plugen-1.1.0/plugen.egg-info/PKG-INFO
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      792 2023-07-12 19:02:49.000000 plugen-1.1.0/plugen.egg-info/SOURCES.txt
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        1 2023-07-12 19:02:49.000000 plugen-1.1.0/plugen.egg-info/dependency_links.txt
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)       39 2023-07-12 19:02:49.000000 plugen-1.1.0/plugen.egg-info/entry_points.txt
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)       18 2023-07-12 19:02:49.000000 plugen-1.1.0/plugen.egg-info/requires.txt
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)        7 2023-07-12 19:02:49.000000 plugen-1.1.0/plugen.egg-info/top_level.txt
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)       38 2023-07-12 19:02:49.364956 plugen-1.1.0/setup.cfg
+-rw-rw-r--   0 aclarembeau  (1000) aclarembeau  (1000)      495 2023-07-12 19:02:46.000000 plugen-1.1.0/setup.py
```

### Comparing `plugen-1.0.4/README.md` & `plugen-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-Sure! Here's an example of a README file for Plugen, a pluggable static website generator:
-
 # Plugen
 
 Plugen is a pluggable static website generator designed to make building static websites fast, flexible, and easy. With its modular architecture, Plugen allows you to extend and customize its functionality through plugins, making it a versatile tool for creating a wide range of static websites.
 
 ## Features
 
 - **Modularity**: Plugen is built on a modular architecture that enables the use of plugins. You can easily extend its functionality by installing and configuring plugins tailored to your specific needs.
@@ -25,14 +23,20 @@
 Follow these steps to get started with Plugen:
 
 1. **Installation**: Install Plugen globally using pipx:
 
    ```shell
    $ pipx install plugen
    ```
+   
+Then, on any folder, run the following command to set up a configuration file 
+
+   ```shell 
+   $ plugen init
+   ```
 
 2. **Build your website**: Run the following command to generate your static website:
 
    ```shell
    $ plugen build
    ```
 
@@ -42,14 +46,21 @@
    $ plugen serve
    ```
 
    This will start a local development server, and you can access your website at `http://localhost:3000`.
 
 4. **Customize and extend**: Explore Plugen's plugin ecosystem and customize your website further to meet your specific requirements. Visit the Plugen documentation for more details.
 
+## Additional documentation 
+
+If you need more help, feel free to check out:
+
+ - DOCUMENTATION.md : Technical documentation, and configuration of the plugin files 
+ - CONTRIBUTING.md : A guide on how to develop your own plugins
+
 ## Contributing
 
 Contributions are welcome! If you find a bug, have a feature request, or want to contribute improvements or new plugins to Plugen, please create an issue or submit a pull request on the [GitHub repository](https://github.com/plugen/plugen).
 
 Before submitting a pull request, please make sure to review the [contribution guidelines](CONTRIBUTING.md).
 
 ## License
@@ -59,11 +70,7 @@
 ## Acknowledgments
 
 We would like to thank all the contributors who have helped make Plugen better.
 
 ## Support
 
 If you have any questions or need assistance, you can reach out to the Plugen community on our [Discord server](https://discord.com/plugen) or by opening an issue on the GitHub repository.
-
----
-
-This README file provides a brief overview of Plugen, its features, and how to get started. Feel free to update it with more specific information about your project and customize it according to your needs. Good luck with your static website development using Plugen!
```

### Comparing `plugen-1.0.4/plugen/lib/build.py` & `plugen-1.1.0/plugen/lib/build.py`

 * *Files identical despite different names*

### Comparing `plugen-1.0.4/plugen/lib/plugin.py` & `plugen-1.1.0/plugen/lib/plugin.py`

 * *Files identical despite different names*

### Comparing `plugen-1.0.4/plugen/lib/serve.py` & `plugen-1.1.0/plugen/lib/serve.py`

 * *Files identical despite different names*

### Comparing `plugen-1.0.4/plugen/lib/utils.py` & `plugen-1.1.0/plugen/lib/utils.py`

 * *Files identical despite different names*

### Comparing `plugen-1.0.4/plugen/main.py` & `plugen-1.1.0/plugen/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 import argparse
 
 from plugen.lib import build_func, serve_func
+from plugen.lib.init import init_func
 from plugen.lib.plugin import list_plugins, install_plugin, remove_plugin
 
 
 def main():
     parser = argparse.ArgumentParser(prog='plugen', description='Pluggable static website generator')
 
     # Subparsers for the different commands
     subparsers = parser.add_subparsers(title='commands', dest='command')
     subparsers.required = True
 
+    # Init command
+    init_parser = subparsers.add_parser('init', help='Initializes a config file')
+    init_parser.set_defaults(func=init_func)
+
     # Build command
     build_parser = subparsers.add_parser('build', help='Build the static website')
     build_parser.add_argument('-c', '--config', help='Specify a configuration file', default='plugen.config.yml')
     build_parser.set_defaults(func=build_func)
 
     # Serve command
     serve_parser = subparsers.add_parser('serve', help='Serve the static website locally')
```

### Comparing `plugen-1.0.4/plugen/plugins/hotreload/plugin.py` & `plugen-1.1.0/plugen/plugins/hotreload/plugin.py`

 * *Files identical despite different names*

### Comparing `plugen-1.0.4/plugen/plugins/sass/plugin.py` & `plugen-1.1.0/plugen/plugins/sass/plugin.py`

 * *Files identical despite different names*

### Comparing `plugen-1.0.4/plugen.egg-info/SOURCES.txt` & `plugen-1.1.0/plugen.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 ./plugen.egg-info/SOURCES.txt
 ./plugen.egg-info/dependency_links.txt
 ./plugen.egg-info/entry_points.txt
 ./plugen.egg-info/requires.txt
 ./plugen.egg-info/top_level.txt
 ./plugen/lib/__init__.py
 ./plugen/lib/build.py
+./plugen/lib/init.py
 ./plugen/lib/plugin.py
 ./plugen/lib/serve.py
 ./plugen/lib/utils.py
 ./plugen/plugins/__init__.py
 ./plugen/plugins/copydest/__init__.py
 ./plugen/plugins/copydest/plugin.py
 ./plugen/plugins/hotreload/__init__.py
```


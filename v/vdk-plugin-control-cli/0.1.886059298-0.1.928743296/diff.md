# Comparing `tmp/vdk-plugin-control-cli-0.1.886059298.tar.gz` & `tmp/vdk-plugin-control-cli-0.1.928743296.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-plugin-control-cli-0.1.886059298.tar", last modified: Thu Jun  1 13:09:50 2023, max compression
+gzip compressed data, was "vdk-plugin-control-cli-0.1.928743296.tar", last modified: Wed Jul 12 10:56:28 2023, max compression
```

## Comparing `vdk-plugin-control-cli-0.1.886059298.tar` & `vdk-plugin-control-cli-0.1.928743296.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:09:50.984327 vdk-plugin-control-cli-0.1.886059298/
--rw-r--r--   0 root         (0) root         (0)     2168 2023-06-01 13:09:50.984327 vdk-plugin-control-cli-0.1.886059298/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1535 2023-06-01 13:09:37.000000 vdk-plugin-control-cli-0.1.886059298/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 13:09:50.984327 vdk-plugin-control-cli-0.1.886059298/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1480 2023-06-01 13:09:41.000000 vdk-plugin-control-cli-0.1.886059298/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:09:50.984327 vdk-plugin-control-cli-0.1.886059298/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:09:50.984327 vdk-plugin-control-cli-0.1.886059298/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:09:50.984327 vdk-plugin-control-cli-0.1.886059298/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:09:50.984327 vdk-plugin-control-cli-0.1.886059298/src/vdk/plugin/control_cli_plugin/
--rw-rw-rw-   0 root         (0) root         (0)     4665 2023-06-01 13:09:37.000000 vdk-plugin-control-cli-0.1.886059298/src/vdk/plugin/control_cli_plugin/control_service_api_error_decorator.py
--rw-rw-rw-   0 root         (0) root         (0)     4460 2023-06-01 13:09:37.000000 vdk-plugin-control-cli-0.1.886059298/src/vdk/plugin/control_cli_plugin/control_service_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     1493 2023-06-01 13:09:37.000000 vdk-plugin-control-cli-0.1.886059298/src/vdk/plugin/control_cli_plugin/control_service_properties_client.py
--rw-rw-rw-   0 root         (0) root         (0)     7435 2023-06-01 13:09:37.000000 vdk-plugin-control-cli-0.1.886059298/src/vdk/plugin/control_cli_plugin/execution_skip.py
--rw-rw-rw-   0 root         (0) root         (0)     1237 2023-06-01 13:09:37.000000 vdk-plugin-control-cli-0.1.886059298/src/vdk/plugin/control_cli_plugin/properties_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     3854 2023-06-01 13:09:37.000000 vdk-plugin-control-cli-0.1.886059298/src/vdk/plugin/control_cli_plugin/vdk_plugin_control_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:09:50.984327 vdk-plugin-control-cli-0.1.886059298/src/vdk_plugin_control_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2168 2023-06-01 13:09:50.000000 vdk-plugin-control-cli-0.1.886059298/src/vdk_plugin_control_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      837 2023-06-01 13:09:50.000000 vdk-plugin-control-cli-0.1.886059298/src/vdk_plugin_control_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 13:09:50.000000 vdk-plugin-control-cli-0.1.886059298/src/vdk_plugin_control_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      242 2023-06-01 13:09:50.000000 vdk-plugin-control-cli-0.1.886059298/src/vdk_plugin_control_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       34 2023-06-01 13:09:50.000000 vdk-plugin-control-cli-0.1.886059298/src/vdk_plugin_control_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-06-01 13:09:50.000000 vdk-plugin-control-cli-0.1.886059298/src/vdk_plugin_control_cli.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 13:09:50.984327 vdk-plugin-control-cli-0.1.886059298/tests/
--rw-rw-rw-   0 root         (0) root         (0)     3283 2023-06-01 13:09:37.000000 vdk-plugin-control-cli-0.1.886059298/tests/test_control_service_properties.py
--rw-rw-rw-   0 root         (0) root         (0)     7812 2023-06-01 13:09:37.000000 vdk-plugin-control-cli-0.1.886059298/tests/test_execution_skip.py
--rw-rw-rw-   0 root         (0) root         (0)     2562 2023-06-01 13:09:37.000000 vdk-plugin-control-cli-0.1.886059298/tests/test_properties_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     2669 2023-06-01 13:09:37.000000 vdk-plugin-control-cli-0.1.886059298/tests/test_vdk_plugin_control_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:56:28.531543 vdk-plugin-control-cli-0.1.928743296/
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-07-12 10:56:28.531543 vdk-plugin-control-cli-0.1.928743296/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1535 2023-07-12 10:56:14.000000 vdk-plugin-control-cli-0.1.928743296/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 10:56:28.531543 vdk-plugin-control-cli-0.1.928743296/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1480 2023-07-12 10:56:17.000000 vdk-plugin-control-cli-0.1.928743296/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:56:28.527543 vdk-plugin-control-cli-0.1.928743296/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:56:28.527543 vdk-plugin-control-cli-0.1.928743296/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:56:28.527543 vdk-plugin-control-cli-0.1.928743296/src/vdk/plugin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:56:28.531543 vdk-plugin-control-cli-0.1.928743296/src/vdk/plugin/control_cli_plugin/
+-rw-rw-rw-   0 root         (0) root         (0)     4665 2023-07-12 10:56:14.000000 vdk-plugin-control-cli-0.1.928743296/src/vdk/plugin/control_cli_plugin/control_service_api_error_decorator.py
+-rw-rw-rw-   0 root         (0) root         (0)     4460 2023-07-12 10:56:14.000000 vdk-plugin-control-cli-0.1.928743296/src/vdk/plugin/control_cli_plugin/control_service_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     1493 2023-07-12 10:56:14.000000 vdk-plugin-control-cli-0.1.928743296/src/vdk/plugin/control_cli_plugin/control_service_properties_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1357 2023-07-12 10:56:14.000000 vdk-plugin-control-cli-0.1.928743296/src/vdk/plugin/control_cli_plugin/control_service_secrets_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     7435 2023-07-12 10:56:14.000000 vdk-plugin-control-cli-0.1.928743296/src/vdk/plugin/control_cli_plugin/execution_skip.py
+-rw-rw-rw-   0 root         (0) root         (0)     1237 2023-07-12 10:56:14.000000 vdk-plugin-control-cli-0.1.928743296/src/vdk/plugin/control_cli_plugin/properties_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1207 2023-07-12 10:56:14.000000 vdk-plugin-control-cli-0.1.928743296/src/vdk/plugin/control_cli_plugin/secrets_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     3976 2023-07-12 10:56:14.000000 vdk-plugin-control-cli-0.1.928743296/src/vdk/plugin/control_cli_plugin/vdk_plugin_control_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:56:28.531543 vdk-plugin-control-cli-0.1.928743296/src/vdk_plugin_control_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-07-12 10:56:28.000000 vdk-plugin-control-cli-0.1.928743296/src/vdk_plugin_control_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      986 2023-07-12 10:56:28.000000 vdk-plugin-control-cli-0.1.928743296/src/vdk_plugin_control_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 10:56:28.000000 vdk-plugin-control-cli-0.1.928743296/src/vdk_plugin_control_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      242 2023-07-12 10:56:28.000000 vdk-plugin-control-cli-0.1.928743296/src/vdk_plugin_control_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2023-07-12 10:56:28.000000 vdk-plugin-control-cli-0.1.928743296/src/vdk_plugin_control_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-12 10:56:28.000000 vdk-plugin-control-cli-0.1.928743296/src/vdk_plugin_control_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 10:56:28.531543 vdk-plugin-control-cli-0.1.928743296/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3283 2023-07-12 10:56:14.000000 vdk-plugin-control-cli-0.1.928743296/tests/test_control_service_properties.py
+-rw-rw-rw-   0 root         (0) root         (0)     7812 2023-07-12 10:56:14.000000 vdk-plugin-control-cli-0.1.928743296/tests/test_execution_skip.py
+-rw-rw-rw-   0 root         (0) root         (0)     2562 2023-07-12 10:56:14.000000 vdk-plugin-control-cli-0.1.928743296/tests/test_properties_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2496 2023-07-12 10:56:14.000000 vdk-plugin-control-cli-0.1.928743296/tests/test_secrets_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2669 2023-07-12 10:56:14.000000 vdk-plugin-control-cli-0.1.928743296/tests/test_vdk_plugin_control_cli.py
```

### Comparing `vdk-plugin-control-cli-0.1.886059298/PKG-INFO` & `vdk-plugin-control-cli-0.1.928743296/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-plugin-control-cli
-Version: 0.1.886059298
+Version: 0.1.928743296
 Summary: Versatile Data Kit SDK plugin exposing CLI commands for managing the lifecycle of a Data Jobs.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-plugin-control-cli-0.1.886059298/README.md` & `vdk-plugin-control-cli-0.1.928743296/README.md`

 * *Files identical despite different names*

### Comparing `vdk-plugin-control-cli-0.1.886059298/setup.py` & `vdk-plugin-control-cli-0.1.928743296/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import setuptools
 
 """
 Builds a package with the help of setuptools in order for this package to be imported in other projects
 """
 
-__version__ = "0.1.886059298"
+__version__ = "0.1.928743296"
 
 setuptools.setup(
     name="vdk-plugin-control-cli",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK plugin exposing CLI commands for managing the lifecycle of a Data Jobs.",
     long_description=pathlib.Path("README.md").read_text(),
```

### Comparing `vdk-plugin-control-cli-0.1.886059298/src/vdk/plugin/control_cli_plugin/control_service_api_error_decorator.py` & `vdk-plugin-control-cli-0.1.928743296/src/vdk/plugin/control_cli_plugin/control_service_api_error_decorator.py`

 * *Files identical despite different names*

### Comparing `vdk-plugin-control-cli-0.1.886059298/src/vdk/plugin/control_cli_plugin/control_service_configuration.py` & `vdk-plugin-control-cli-0.1.928743296/src/vdk/plugin/control_cli_plugin/control_service_configuration.py`

 * *Files identical despite different names*

### Comparing `vdk-plugin-control-cli-0.1.886059298/src/vdk/plugin/control_cli_plugin/control_service_properties_client.py` & `vdk-plugin-control-cli-0.1.928743296/src/vdk/plugin/control_cli_plugin/control_service_properties_client.py`

 * *Files identical despite different names*

### Comparing `vdk-plugin-control-cli-0.1.886059298/src/vdk/plugin/control_cli_plugin/execution_skip.py` & `vdk-plugin-control-cli-0.1.928743296/src/vdk/plugin/control_cli_plugin/execution_skip.py`

 * *Files identical despite different names*

### Comparing `vdk-plugin-control-cli-0.1.886059298/src/vdk/plugin/control_cli_plugin/properties_plugin.py` & `vdk-plugin-control-cli-0.1.928743296/src/vdk/plugin/control_cli_plugin/properties_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-plugin-control-cli-0.1.886059298/src/vdk/plugin/control_cli_plugin/vdk_plugin_control_cli.py` & `vdk-plugin-control-cli-0.1.928743296/src/vdk/plugin/control_cli_plugin/vdk_plugin_control_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from vdk.internal.control.command_groups.job.delete import delete
 from vdk.internal.control.command_groups.job.deploy_cli import deploy
 from vdk.internal.control.command_groups.job.download_job import download_job
 from vdk.internal.control.command_groups.job.download_key import download_key
 from vdk.internal.control.command_groups.job.execute import execute
 from vdk.internal.control.command_groups.job.list import list_command
 from vdk.internal.control.command_groups.job.properties import properties_command
+from vdk.internal.control.command_groups.job.secrets import secrets_command
 from vdk.internal.control.command_groups.job.show import show_command
 from vdk.internal.control.command_groups.login_group.login import login
 from vdk.internal.control.command_groups.logout_group.logout import logout
 from vdk.internal.control.configuration.default_options import DefaultOptions
 from vdk.internal.control.plugin import control_plugin_manager
 from vdk.internal.core.config import ConfigurationBuilder
 from vdk.internal.core.context import CoreContext
@@ -41,14 +42,15 @@
     root_command.add_command(execute)
     root_command.add_command(download_job)
     root_command.add_command(set_default_command)
     root_command.add_command(reset_default_command)
     root_command.add_command(show_command)
     root_command.add_command(properties_command)
     root_command.add_command(info)
+    root_command.add_command(secrets_command)
 
     plugins = control_plugin_manager.Plugins()
     default_options = DefaultOptions(plugins)
     if default_options.get_default_map():
         root_command.context_settings["default_map"] = default_options.get_default_map()
```

### Comparing `vdk-plugin-control-cli-0.1.886059298/src/vdk_plugin_control_cli.egg-info/PKG-INFO` & `vdk-plugin-control-cli-0.1.928743296/src/vdk_plugin_control_cli.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-plugin-control-cli
-Version: 0.1.886059298
+Version: 0.1.928743296
 Summary: Versatile Data Kit SDK plugin exposing CLI commands for managing the lifecycle of a Data Jobs.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-plugin-control-cli-0.1.886059298/src/vdk_plugin_control_cli.egg-info/SOURCES.txt` & `vdk-plugin-control-cli-0.1.928743296/src/vdk_plugin_control_cli.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 README.md
 setup.py
 src/vdk/plugin/control_cli_plugin/control_service_api_error_decorator.py
 src/vdk/plugin/control_cli_plugin/control_service_configuration.py
 src/vdk/plugin/control_cli_plugin/control_service_properties_client.py
+src/vdk/plugin/control_cli_plugin/control_service_secrets_client.py
 src/vdk/plugin/control_cli_plugin/execution_skip.py
 src/vdk/plugin/control_cli_plugin/properties_plugin.py
+src/vdk/plugin/control_cli_plugin/secrets_plugin.py
 src/vdk/plugin/control_cli_plugin/vdk_plugin_control_cli.py
 src/vdk_plugin_control_cli.egg-info/PKG-INFO
 src/vdk_plugin_control_cli.egg-info/SOURCES.txt
 src/vdk_plugin_control_cli.egg-info/dependency_links.txt
 src/vdk_plugin_control_cli.egg-info/entry_points.txt
 src/vdk_plugin_control_cli.egg-info/requires.txt
 src/vdk_plugin_control_cli.egg-info/top_level.txt
 tests/test_control_service_properties.py
 tests/test_execution_skip.py
 tests/test_properties_plugin.py
+tests/test_secrets_plugin.py
 tests/test_vdk_plugin_control_cli.py
```

### Comparing `vdk-plugin-control-cli-0.1.886059298/tests/test_control_service_properties.py` & `vdk-plugin-control-cli-0.1.928743296/tests/test_control_service_properties.py`

 * *Files identical despite different names*

### Comparing `vdk-plugin-control-cli-0.1.886059298/tests/test_execution_skip.py` & `vdk-plugin-control-cli-0.1.928743296/tests/test_execution_skip.py`

 * *Files identical despite different names*

### Comparing `vdk-plugin-control-cli-0.1.886059298/tests/test_properties_plugin.py` & `vdk-plugin-control-cli-0.1.928743296/tests/test_properties_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-plugin-control-cli-0.1.886059298/tests/test_vdk_plugin_control_cli.py` & `vdk-plugin-control-cli-0.1.928743296/tests/test_vdk_plugin_control_cli.py`

 * *Files identical despite different names*


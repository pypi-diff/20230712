# Comparing `tmp/openplugin-py-0.0.3.tar.gz` & `tmp/openplugin-py-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openplugin-py-0.0.3.tar", last modified: Thu Jul  6 10:01:27 2023, max compression
+gzip compressed data, was "openplugin-py-0.0.4.tar", last modified: Wed Jul 12 05:07:36 2023, max compression
```

## Comparing `openplugin-py-0.0.3.tar` & `openplugin-py-0.0.4.tar`

### file list

```diff
@@ -1,33 +1,41 @@
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-06 10:01:27.218741 openplugin-py-0.0.3/
--rw-r--r--   0 4paradigm   (501) staff       (20)    11357 2023-06-28 13:02:04.000000 openplugin-py-0.0.3/LICENSE
--rw-r--r--   0 4paradigm   (501) staff       (20)     3621 2023-07-06 10:01:27.218600 openplugin-py-0.0.3/PKG-INFO
--rw-r--r--   0 4paradigm   (501) staff       (20)     2540 2023-07-06 09:48:54.000000 openplugin-py-0.0.3/README.md
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-06 10:01:27.213482 openplugin-py-0.0.3/openplugin/
--rw-r--r--   0 4paradigm   (501) staff       (20)     1114 2023-07-06 06:46:44.000000 openplugin-py-0.0.3/openplugin/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-06 10:01:27.213860 openplugin-py-0.0.3/openplugin/cli/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-06-26 08:37:33.000000 openplugin-py-0.0.3/openplugin/cli/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     3080 2023-07-02 15:52:03.000000 openplugin-py-0.0.3/openplugin/cli/cli.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-06 10:01:27.214234 openplugin-py-0.0.3/openplugin/install/
--rw-r--r--   0 4paradigm   (501) staff       (20)     3559 2023-07-06 09:33:01.000000 openplugin-py-0.0.3/openplugin/install/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-06 10:01:27.214622 openplugin-py-0.0.3/openplugin/run/
--rw-r--r--   0 4paradigm   (501) staff       (20)     3342 2023-07-02 14:58:56.000000 openplugin-py-0.0.3/openplugin/run/__init__.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-06 10:01:27.216258 openplugin-py-0.0.3/openplugin/template/
--rw-r--r--   0 4paradigm   (501) staff       (20)      876 2023-07-02 15:52:03.000000 openplugin-py-0.0.3/openplugin/template/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     1192 2023-07-02 15:52:03.000000 openplugin-py-0.0.3/openplugin/template/base_template.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      901 2023-07-02 15:52:03.000000 openplugin-py-0.0.3/openplugin/template/json_template.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      901 2023-07-02 15:52:03.000000 openplugin-py-0.0.3/openplugin/template/utils.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      902 2023-07-02 15:52:03.000000 openplugin-py-0.0.3/openplugin/template/yaml_template.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-06 10:01:27.217484 openplugin-py-0.0.3/openplugin/utils/
--rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-06-26 08:58:04.000000 openplugin-py-0.0.3/openplugin/utils/__init__.py
--rw-r--r--   0 4paradigm   (501) staff       (20)    17531 2023-06-30 09:22:51.000000 openplugin-py-0.0.3/openplugin/utils/app_util.py
--rw-r--r--   0 4paradigm   (501) staff       (20)      915 2023-06-30 09:22:51.000000 openplugin-py-0.0.3/openplugin/utils/errors.py
--rw-r--r--   0 4paradigm   (501) staff       (20)     2314 2023-07-06 09:30:48.000000 openplugin-py-0.0.3/openplugin/utils/util.py
-drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-06 10:01:27.218408 openplugin-py-0.0.3/openplugin_py.egg-info/
--rw-r--r--   0 4paradigm   (501) staff       (20)     3621 2023-07-06 10:01:27.000000 openplugin-py-0.0.3/openplugin_py.egg-info/PKG-INFO
--rw-r--r--   0 4paradigm   (501) staff       (20)      662 2023-07-06 10:01:27.000000 openplugin-py-0.0.3/openplugin_py.egg-info/SOURCES.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)        1 2023-07-06 10:01:27.000000 openplugin-py-0.0.3/openplugin_py.egg-info/dependency_links.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       46 2023-07-06 10:01:27.000000 openplugin-py-0.0.3/openplugin_py.egg-info/entry_points.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)      167 2023-07-06 10:01:27.000000 openplugin-py-0.0.3/openplugin_py.egg-info/requires.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       11 2023-07-06 10:01:27.000000 openplugin-py-0.0.3/openplugin_py.egg-info/top_level.txt
--rw-r--r--   0 4paradigm   (501) staff       (20)       38 2023-07-06 10:01:27.218786 openplugin-py-0.0.3/setup.cfg
--rw-r--r--   0 4paradigm   (501) staff       (20)     2869 2023-06-30 09:40:35.000000 openplugin-py-0.0.3/setup.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-12 05:07:36.323142 openplugin-py-0.0.4/
+-rw-r--r--   0 4paradigm   (501) staff       (20)    11357 2023-06-28 13:02:04.000000 openplugin-py-0.0.4/LICENSE
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3838 2023-07-12 05:07:36.322995 openplugin-py-0.0.4/PKG-INFO
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2757 2023-07-12 03:42:45.000000 openplugin-py-0.0.4/README.md
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-12 05:07:36.315893 openplugin-py-0.0.4/openplugin/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1114 2023-07-06 10:55:36.000000 openplugin-py-0.0.4/openplugin/__init__.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-12 05:07:36.316258 openplugin-py-0.0.4/openplugin/cli/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-06-26 08:37:33.000000 openplugin-py-0.0.4/openplugin/cli/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3080 2023-07-02 15:52:03.000000 openplugin-py-0.0.4/openplugin/cli/cli.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-12 05:07:36.317027 openplugin-py-0.0.4/openplugin/install/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2656 2023-07-12 02:25:08.000000 openplugin-py-0.0.4/openplugin/install/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1528 2023-07-12 02:25:06.000000 openplugin-py-0.0.4/openplugin/install/local_install.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-12 05:07:36.317903 openplugin-py-0.0.4/openplugin/plugin/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-07-12 02:12:45.000000 openplugin-py-0.0.4/openplugin/plugin/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      928 2023-07-12 02:20:17.000000 openplugin-py-0.0.4/openplugin/plugin/base_plugin.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2194 2023-07-12 02:25:08.000000 openplugin-py-0.0.4/openplugin/plugin/webapp_plugin.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-12 05:07:36.318530 openplugin-py-0.0.4/openplugin/run/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1259 2023-07-12 02:25:06.000000 openplugin-py-0.0.4/openplugin/run/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1014 2023-07-12 02:25:06.000000 openplugin-py-0.0.4/openplugin/run/local_run.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-12 05:07:36.320116 openplugin-py-0.0.4/openplugin/template/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      876 2023-07-02 15:52:03.000000 openplugin-py-0.0.4/openplugin/template/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1192 2023-07-02 15:52:03.000000 openplugin-py-0.0.4/openplugin/template/base_template.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      901 2023-07-02 15:52:03.000000 openplugin-py-0.0.4/openplugin/template/json_template.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      901 2023-07-02 15:52:03.000000 openplugin-py-0.0.4/openplugin/template/utils.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      902 2023-07-02 15:52:03.000000 openplugin-py-0.0.4/openplugin/template/yaml_template.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-12 05:07:36.321740 openplugin-py-0.0.4/openplugin/utils/
+-rw-r--r--   0 4paradigm   (501) staff       (20)      638 2023-06-26 08:58:04.000000 openplugin-py-0.0.4/openplugin/utils/__init__.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)    17531 2023-06-30 09:22:51.000000 openplugin-py-0.0.4/openplugin/utils/app_util.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      915 2023-06-30 09:22:51.000000 openplugin-py-0.0.4/openplugin/utils/errors.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)      989 2023-07-12 02:25:06.000000 openplugin-py-0.0.4/openplugin/utils/local_plugin_utils.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     1798 2023-07-12 02:25:06.000000 openplugin-py-0.0.4/openplugin/utils/network_utils.py
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2321 2023-07-12 02:25:06.000000 openplugin-py-0.0.4/openplugin/utils/util.py
+drwxr-xr-x   0 4paradigm   (501) staff       (20)        0 2023-07-12 05:07:36.322786 openplugin-py-0.0.4/openplugin_py.egg-info/
+-rw-r--r--   0 4paradigm   (501) staff       (20)     3838 2023-07-12 05:07:36.000000 openplugin-py-0.0.4/openplugin_py.egg-info/PKG-INFO
+-rw-r--r--   0 4paradigm   (501) staff       (20)      897 2023-07-12 05:07:36.000000 openplugin-py-0.0.4/openplugin_py.egg-info/SOURCES.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)        1 2023-07-12 05:07:36.000000 openplugin-py-0.0.4/openplugin_py.egg-info/dependency_links.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       46 2023-07-12 05:07:36.000000 openplugin-py-0.0.4/openplugin_py.egg-info/entry_points.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)      167 2023-07-12 05:07:36.000000 openplugin-py-0.0.4/openplugin_py.egg-info/requires.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       11 2023-07-12 05:07:36.000000 openplugin-py-0.0.4/openplugin_py.egg-info/top_level.txt
+-rw-r--r--   0 4paradigm   (501) staff       (20)       38 2023-07-12 05:07:36.323193 openplugin-py-0.0.4/setup.cfg
+-rw-r--r--   0 4paradigm   (501) staff       (20)     2869 2023-06-30 09:40:35.000000 openplugin-py-0.0.4/setup.py
```

### Comparing `openplugin-py-0.0.3/LICENSE` & `openplugin-py-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.3/PKG-INFO` & `openplugin-py-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openplugin-py
-Version: 0.0.3
+Version: 0.0.4
 Summary: Toolkit and Collection for Plugins of Large Language Models
 Home-page: https://github.com/OpenRL-Lab/openplugin
 Author: openrl contributors
 Author-email: huangsy1314@163.com
 Project-URL: Code, https://github.com/OpenRL-Lab/openplugin
 Project-URL: Documentation, https://openplugin.readthedocs.io/
 Keywords: LLM plugin toolkit
@@ -46,25 +46,28 @@
 
 ## Usage
 
 - Check OpenPlugin's version with: `op --version`
 - Check system information: `op --system_info`
 - Install a plugin: `op install <plugin_name>`. You can also install local plugins with `op install ./`.
 - Uninstall a plugin: `op uninstall <plugin_name>`
-- Start a plugin: `op run <plugin_name>`. You can use `-p` to specify the port of the plugin. By default, the port is 5003.
+- Start a plugin: `op run <plugin_name>`. You can use `-p` to specify the port of the plugin. By default, the port is 5003.  You can also run a local plugin with `op run ./`.
 - List installed plugins: `op list`
 - Reinstall plugin: `op reinstall <plugin_name>`
 
 ## An example for using QRcode_plugin
 
 - Install QRcode_plugin: `op install QRcode_plugin`
 - Or You can install QRcode_plugin from local:
   - Go to the directory of QRcode_plugin: `cd plugins/QRcode_plugin`
   - Install QRcode_plugin: `op install ./`
 - Start QRcode_plugin: `op run QRcode_plugin -p server_port`
+- Or you can start QRcode_plugin from local:
+  - Go to the directory of QRcode_plugin: `cd plugins/QRcode_plugin`
+  - Start QRcode_plugin: `op run ./ -p server_port`
 - Then you can get the `ai-plugin.json` file via visiting `http://<server_ip>:server_port/ai-plugin.json`
 - You can get the `openaip.yaml` file via visiting `http://<server_ip>:server_port/openaip.yaml`
 
 ## Plugins
 
 We provide some source codes of plugins. You can find them in [plugins](./plugins). 
 We call for contributions of plugins.
```

### Comparing `openplugin-py-0.0.3/README.md` & `openplugin-py-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -20,25 +20,28 @@
 
 ## Usage
 
 - Check OpenPlugin's version with: `op --version`
 - Check system information: `op --system_info`
 - Install a plugin: `op install <plugin_name>`. You can also install local plugins with `op install ./`.
 - Uninstall a plugin: `op uninstall <plugin_name>`
-- Start a plugin: `op run <plugin_name>`. You can use `-p` to specify the port of the plugin. By default, the port is 5003.
+- Start a plugin: `op run <plugin_name>`. You can use `-p` to specify the port of the plugin. By default, the port is 5003.  You can also run a local plugin with `op run ./`.
 - List installed plugins: `op list`
 - Reinstall plugin: `op reinstall <plugin_name>`
 
 ## An example for using QRcode_plugin
 
 - Install QRcode_plugin: `op install QRcode_plugin`
 - Or You can install QRcode_plugin from local:
   - Go to the directory of QRcode_plugin: `cd plugins/QRcode_plugin`
   - Install QRcode_plugin: `op install ./`
 - Start QRcode_plugin: `op run QRcode_plugin -p server_port`
+- Or you can start QRcode_plugin from local:
+  - Go to the directory of QRcode_plugin: `cd plugins/QRcode_plugin`
+  - Start QRcode_plugin: `op run ./ -p server_port`
 - Then you can get the `ai-plugin.json` file via visiting `http://<server_ip>:server_port/ai-plugin.json`
 - You can get the `openaip.yaml` file via visiting `http://<server_ip>:server_port/openaip.yaml`
 
 ## Plugins
 
 We provide some source codes of plugins. You can find them in [plugins](./plugins). 
 We call for contributions of plugins.
```

### Comparing `openplugin-py-0.0.3/openplugin/__init__.py` & `openplugin-py-0.0.4/openplugin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 
 
 __TITLE__ = "openplugin"
-__VERSION__ = "v0.0.3"
+__VERSION__ = "v0.0.4"
 __DESCRIPTION__ = "Toolkit and Collection for Plugins of Large Language Models"
 __AUTHOR__ = "OpenRL Contributors"
 __EMAIL__ = "huangshiyu@4paradigm.com"
 __version__ = __VERSION__
 
 import platform
```

### Comparing `openplugin-py-0.0.3/openplugin/cli/__init__.py` & `openplugin-py-0.0.4/openplugin/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.3/openplugin/cli/cli.py` & `openplugin-py-0.0.4/openplugin/cli/cli.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.3/openplugin/install/__init__.py` & `openplugin-py-0.0.4/openplugin/install/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,29 +12,27 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 import io
-import os
 import shutil
 import zipfile
-import tempfile
 
-from pathlib import Path
 import requests
-import json
 
+from openplugin.install.local_install import install_local_plugin
 from openplugin.utils.util import (
     get_plugin_directory,
     get_plugin_list,
     get_zip_file_url,
-    make_zip_file,
 )
+
+
 # import urllib
 def install_plugin(plugin_name: str) -> bool:
     if plugin_name == "./":
         print("Installing current directory as plugin...")
         return install_local_plugin()
 
     plugin_list = get_plugin_list()
@@ -55,34 +53,15 @@
         z.extractall(get_plugin_directory())
     except:
         raise ValueError("plugin {} not found".format(plugin_name))
     print("Installed plugin: {}!".format(plugin_name))
     return True
     # urllib.request.urlretrieve(zip_file_url, f'{plugin_name}.zip')
 
-def install_local_plugin() -> bool:
-    info_file = Path("info.json")
-    assert info_file.exists(), "info.json not found"
-    info_dict = json.load(open("info.json", "r"))
-    assert "plugin_name" in info_dict, "plugin_name not found in info.json"
-    plugin_name = info_dict["plugin_name"]
-    print("Installing plugin: {}...".format(plugin_name))
 
-    tempdir = tempfile.mkdtemp()
-    filepath = make_zip_file(dir_to_put_file_in=tempdir,
-                             plugin_directory="./", plugin_name = plugin_name)
-
-    z = zipfile.ZipFile(filepath)
-    plugin_directory = get_plugin_directory()
-    if not plugin_directory.exists():
-        plugin_directory.mkdir(parents=True)
-    print("Extracting plugin to {}".format(plugin_directory / plugin_name))
-    z.extractall(os.path.join(get_plugin_directory(),plugin_name))
-    shutil.rmtree(tempdir, ignore_errors=True)
-    return True
 def uninstall_plugin(plugin_name: str) -> bool:
     plugin_list = get_plugin_list()
     if plugin_name not in plugin_list:
         print("Plugin {} not installed!".format(plugin_name))
         return True
 
     plugin_path = get_plugin_directory() / plugin_name
```

### Comparing `openplugin-py-0.0.3/openplugin/run/__init__.py` & `openplugin-py-0.0.4/openplugin/plugin/webapp_plugin.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,100 +13,53 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 import os
 import sys
-import urllib.request
-from pathlib import Path
 
 import ifaddr
 
+from openplugin.plugin.base_plugin import BasePlugin
 from openplugin.utils.app_util import import_app
-from openplugin.utils.util import get_plugin_list
+from openplugin.utils.network_utils import display_host_info, getIp, local_addresses
 
-IP_WEBSITES = (
-    "https://ipinfo.io/ip",
-    "https://ipecho.net/plain",
-    "https://api.ipify.org",
-    "https://ipaddr.site",
-    "https://icanhazip.com",
-    "https://ident.me",
-    "https://curlmyip.net",
-)
 
-
-def getIp():
-    for ipWebsite in IP_WEBSITES:
+class WebAppPlugin(BasePlugin):
+    def run(self, host: str, port: int):
+        os.chdir(self.plugin_path)
+        sys.path.append("./")
         try:
-            response = urllib.request.urlopen(ipWebsite)
-
-            charsets = response.info().get_charsets()
-            if len(charsets) == 0 or charsets[0] is None:
-                charset = "utf-8"  # Use utf-8 by default
-            else:
-                charset = charsets[0]
-
-            userIp = response.read().decode(charset).strip()
-
-            return userIp
+            print("Loading plugin from {}".format(self.plugin_path))
+            app = import_app("main:app")
         except:
-            pass  # Network error, just continue on to next website.
+            raise ValueError("plugin {} not found".format(self.plugin_name))
+
+        print("Running plugin: {} on {}:{}".format(self.plugin_name, host, port))
 
-    # Either all of the websites are down or returned invalid response
-    # (unlikely) or you are disconnected from the internet.
-    return None
-
-
-local_addresses = ["0.0.0.0", "127.0.0.1"]
-
-
-def display_host_info(ip, host):
-    print(f"Launched at {ip}:{host}")
-    print(f"\tYou can get json file at {ip}:{host}/ai-plugin.json")
-    print(f"\tYou can get YAML file at {ip}:{host}/openapi.yaml")
-
-
-def run_plugin(plugin_name, host: str, port: int):
-    plugin_list = get_plugin_list()
-    if plugin_name not in plugin_list:
-        print(f"Plugin {plugin_name} not installed!")
-        return
-
-    plugin_path = f"{str(Path.home())}/.openplugin/plugins/{plugin_name}"
-    os.chdir(plugin_path)
-    sys.path.append("./")
-    try:
-        print("Loading plugin from {}".format(plugin_path))
-        app = import_app("main:app")
-    except:
-        raise ValueError("plugin {} not found".format(plugin_name))
-
-    print("Running plugin: {} on {}:{}".format(plugin_name, host, port))
-
-    ips = set()
-    outip = getIp()
-    if outip is not None:
-        ips.add(outip)
-    ips.add("0.0.0.0")
-    adapters = ifaddr.get_adapters()
-
-    for adapter in adapters:
-        # print("IPs of network adapter " + adapter.nice_name)
-        for ip in adapter.ips:
-            # print("   %s/%s" % (ip.ip, ip.network_prefix))
-            ip_address = ip.ip
-            if (
-                isinstance(ip_address, str)
-                and "(" not in ip_address
-                and ":" not in ip_address
-                and ip_address not in local_addresses
-                and not ip_address.startswith("192.168")
-            ):
-                ips.add(ip_address)
-
-    if len(ips) > 0:
-        for ip in ips:
-            display_host_info(ip, port)
+        ips = set()
+        outip = getIp()
+        if outip is not None:
+            ips.add(outip)
+        ips.add("0.0.0.0")
+        adapters = ifaddr.get_adapters()
+
+        for adapter in adapters:
+            # print("IPs of network adapter " + adapter.nice_name)
+            for ip in adapter.ips:
+                # print("   %s/%s" % (ip.ip, ip.network_prefix))
+                ip_address = ip.ip
+                if (
+                    isinstance(ip_address, str)
+                    and "(" not in ip_address
+                    and ":" not in ip_address
+                    and ip_address not in local_addresses
+                    and not ip_address.startswith("192.168")
+                ):
+                    ips.add(ip_address)
+
+        if len(ips) > 0:
+            for ip in ips:
+                display_host_info(ip, port)
 
-    app.run(debug=True, host=host, port=port)
+        app.run(debug=True, host=host, port=port)
```

### Comparing `openplugin-py-0.0.3/openplugin/template/__init__.py` & `openplugin-py-0.0.4/openplugin/template/__init__.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.3/openplugin/template/base_template.py` & `openplugin-py-0.0.4/openplugin/template/base_template.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.3/openplugin/template/json_template.py` & `openplugin-py-0.0.4/openplugin/template/json_template.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.3/openplugin/template/utils.py` & `openplugin-py-0.0.4/openplugin/template/utils.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.3/openplugin/template/yaml_template.py` & `openplugin-py-0.0.4/openplugin/template/yaml_template.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.3/openplugin/utils/__init__.py` & `openplugin-py-0.0.4/openplugin/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.3/openplugin/utils/app_util.py` & `openplugin-py-0.0.4/openplugin/utils/app_util.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.3/openplugin/utils/errors.py` & `openplugin-py-0.0.4/openplugin/utils/errors.py`

 * *Files identical despite different names*

### Comparing `openplugin-py-0.0.3/openplugin/utils/util.py` & `openplugin-py-0.0.4/openplugin/utils/util.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,25 +12,27 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """"""
 import os
-import shutil
 import platform
 import re
+import shutil
 from pathlib import Path
 from typing import Dict
 
 import numpy as np
 
 import openplugin
 
 REMOTE_URL = "https://openrl.net/plugin-store/download"
+
+
 def get_zip_file_url(plugin_name: str) -> str:
     return "{}/{}".format(REMOTE_URL, plugin_name)
 
 
 def get_plugin_directory() -> Path:
     return Path.home() / ".openplugin" / "plugins"
 
@@ -40,21 +42,23 @@
     plugin_directory = get_plugin_directory()
     if plugin_directory.is_dir():
         for plugin in plugin_directory.iterdir():
             if plugin.is_dir():
                 plugin_list.append(plugin.name)
     return plugin_list
 
-def make_zip_file(dir_to_put_file_in,plugin_directory,plugin_name):
+
+def make_zip_file(dir_to_put_file_in, plugin_directory, plugin_name):
     # create a zip file
     zip_file_name = plugin_name
     zip_file_parent = Path(plugin_directory).parent
     zip_file_path = os.path.join(dir_to_put_file_in, zip_file_name)
-    shutil.make_archive(zip_file_path, 'zip', zip_file_parent,plugin_directory)
-    return os.path.join(dir_to_put_file_in, zip_file_name + '.zip')
+    shutil.make_archive(zip_file_path, "zip", zip_file_parent, plugin_directory)
+    return os.path.join(dir_to_put_file_in, zip_file_name + ".zip")
+
 
 def get_system_info() -> Dict[str, str]:
     """
     Retrieve system and python env info for the current system.
 
     :return: Dictionary summing up the version for each relevant package
         and a formatted string.
```

### Comparing `openplugin-py-0.0.3/openplugin_py.egg-info/PKG-INFO` & `openplugin-py-0.0.4/openplugin_py.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openplugin-py
-Version: 0.0.3
+Version: 0.0.4
 Summary: Toolkit and Collection for Plugins of Large Language Models
 Home-page: https://github.com/OpenRL-Lab/openplugin
 Author: openrl contributors
 Author-email: huangsy1314@163.com
 Project-URL: Code, https://github.com/OpenRL-Lab/openplugin
 Project-URL: Documentation, https://openplugin.readthedocs.io/
 Keywords: LLM plugin toolkit
@@ -46,25 +46,28 @@
 
 ## Usage
 
 - Check OpenPlugin's version with: `op --version`
 - Check system information: `op --system_info`
 - Install a plugin: `op install <plugin_name>`. You can also install local plugins with `op install ./`.
 - Uninstall a plugin: `op uninstall <plugin_name>`
-- Start a plugin: `op run <plugin_name>`. You can use `-p` to specify the port of the plugin. By default, the port is 5003.
+- Start a plugin: `op run <plugin_name>`. You can use `-p` to specify the port of the plugin. By default, the port is 5003.  You can also run a local plugin with `op run ./`.
 - List installed plugins: `op list`
 - Reinstall plugin: `op reinstall <plugin_name>`
 
 ## An example for using QRcode_plugin
 
 - Install QRcode_plugin: `op install QRcode_plugin`
 - Or You can install QRcode_plugin from local:
   - Go to the directory of QRcode_plugin: `cd plugins/QRcode_plugin`
   - Install QRcode_plugin: `op install ./`
 - Start QRcode_plugin: `op run QRcode_plugin -p server_port`
+- Or you can start QRcode_plugin from local:
+  - Go to the directory of QRcode_plugin: `cd plugins/QRcode_plugin`
+  - Start QRcode_plugin: `op run ./ -p server_port`
 - Then you can get the `ai-plugin.json` file via visiting `http://<server_ip>:server_port/ai-plugin.json`
 - You can get the `openaip.yaml` file via visiting `http://<server_ip>:server_port/openaip.yaml`
 
 ## Plugins
 
 We provide some source codes of plugins. You can find them in [plugins](./plugins). 
 We call for contributions of plugins.
```

### Comparing `openplugin-py-0.0.3/openplugin_py.egg-info/SOURCES.txt` & `openplugin-py-0.0.4/openplugin_py.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 LICENSE
 README.md
 setup.py
 openplugin/__init__.py
 openplugin/cli/__init__.py
 openplugin/cli/cli.py
 openplugin/install/__init__.py
+openplugin/install/local_install.py
+openplugin/plugin/__init__.py
+openplugin/plugin/base_plugin.py
+openplugin/plugin/webapp_plugin.py
 openplugin/run/__init__.py
+openplugin/run/local_run.py
 openplugin/template/__init__.py
 openplugin/template/base_template.py
 openplugin/template/json_template.py
 openplugin/template/utils.py
 openplugin/template/yaml_template.py
 openplugin/utils/__init__.py
 openplugin/utils/app_util.py
 openplugin/utils/errors.py
+openplugin/utils/local_plugin_utils.py
+openplugin/utils/network_utils.py
 openplugin/utils/util.py
 openplugin_py.egg-info/PKG-INFO
 openplugin_py.egg-info/SOURCES.txt
 openplugin_py.egg-info/dependency_links.txt
 openplugin_py.egg-info/entry_points.txt
 openplugin_py.egg-info/requires.txt
 openplugin_py.egg-info/top_level.txt
```

### Comparing `openplugin-py-0.0.3/setup.py` & `openplugin-py-0.0.4/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/fichub-cli-0.9.2.tar.gz` & `tmp/fichub-cli-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Projects\Personal\Projects\Langs\Python\Others\fichub\fichub-cli\fichub-cli\dist\.tmp-2wum0ush\fichub-cli-0.9.2.tar", last modified: Sun Jun 18 20:25:30 2023, max compression
+gzip compressed data, was "D:\Projects\Personal\Projects\Langs\Python\Others\fichub\fichub-cli\fichub-cli\dist\.tmp-0flk41iy\fichub-cli-0.9.3.tar", last modified: Wed Jul 12 18:07:14 2023, max compression
```

## Comparing `fichub-cli-0.9.2.tar` & `fichub-cli-0.9.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 20:25:30.635617 fichub-cli-0.9.2/
--rw-rw-rw-   0        0        0    11558 2023-06-04 18:06:14.000000 fichub-cli-0.9.2/LICENSE.txt
--rw-rw-rw-   0        0        0     5262 2023-06-18 20:25:30.635617 fichub-cli-0.9.2/PKG-INFO
--rw-rw-rw-   0        0        0     4802 2023-06-04 18:06:14.000000 fichub-cli-0.9.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-18 20:25:30.613620 fichub-cli-0.9.2/fichub_cli/
--rw-rw-rw-   0        0        0       23 2023-06-18 20:19:24.000000 fichub-cli-0.9.2/fichub_cli/__init__.py
--rw-rw-rw-   0        0        0     7791 2023-06-04 18:06:14.000000 fichub-cli-0.9.2/fichub_cli/cli.py
-drwxrwxrwx   0        0        0        0 2023-06-18 20:25:30.633616 fichub-cli-0.9.2/fichub_cli/utils/
--rw-rw-rw-   0        0        0        0 2023-06-04 18:06:14.000000 fichub-cli-0.9.2/fichub_cli/utils/__init__.py
--rw-rw-rw-   0        0        0    11811 2023-06-04 18:06:14.000000 fichub-cli-0.9.2/fichub_cli/utils/fetch_data.py
--rw-rw-rw-   0        0        0     6194 2023-06-18 20:24:03.000000 fichub-cli-0.9.2/fichub_cli/utils/fichub.py
--rw-rw-rw-   0        0        0     2384 2023-06-04 18:06:14.000000 fichub-cli-0.9.2/fichub_cli/utils/logging.py
--rw-rw-rw-   0        0        0    14639 2023-06-04 18:06:14.000000 fichub-cli-0.9.2/fichub_cli/utils/processing.py
-drwxrwxrwx   0        0        0        0 2023-06-18 20:25:30.629616 fichub-cli-0.9.2/fichub_cli.egg-info/
--rw-rw-rw-   0        0        0     5262 2023-06-18 20:25:30.000000 fichub-cli-0.9.2/fichub_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      466 2023-06-18 20:25:30.000000 fichub-cli-0.9.2/fichub_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 20:25:30.000000 fichub-cli-0.9.2/fichub_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-06-18 20:25:30.000000 fichub-cli-0.9.2/fichub_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      115 2023-06-18 20:25:30.000000 fichub-cli-0.9.2/fichub_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-18 20:25:30.000000 fichub-cli-0.9.2/fichub_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      233 2023-06-04 18:06:14.000000 fichub-cli-0.9.2/pyproject.toml
--rw-rw-rw-   0        0        0      114 2023-06-18 20:25:30.640616 fichub-cli-0.9.2/setup.cfg
--rw-rw-rw-   0        0        0     1101 2023-06-18 20:19:24.000000 fichub-cli-0.9.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-18 20:25:30.634618 fichub-cli-0.9.2/tests/
--rw-rw-rw-   0        0        0     2227 2023-06-18 20:19:24.000000 fichub-cli-0.9.2/tests/test_cli.py
+drwxrwxrwx   0        0        0        0 2023-07-12 18:07:14.579791 fichub-cli-0.9.3/
+-rw-rw-rw-   0        0        0    11558 2023-06-04 18:06:14.000000 fichub-cli-0.9.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     5262 2023-07-12 18:07:14.579791 fichub-cli-0.9.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4802 2023-07-05 18:10:23.000000 fichub-cli-0.9.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 18:07:14.547791 fichub-cli-0.9.3/fichub_cli/
+-rw-rw-rw-   0        0        0       23 2023-07-12 17:47:08.000000 fichub-cli-0.9.3/fichub_cli/__init__.py
+-rw-rw-rw-   0        0        0     7209 2023-07-12 17:56:27.000000 fichub-cli-0.9.3/fichub_cli/cli.py
+drwxrwxrwx   0        0        0        0 2023-07-12 18:07:14.577791 fichub-cli-0.9.3/fichub_cli/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-04 18:06:14.000000 fichub-cli-0.9.3/fichub_cli/utils/__init__.py
+-rw-rw-rw-   0        0        0    11837 2023-07-12 17:57:22.000000 fichub-cli-0.9.3/fichub_cli/utils/fetch_data.py
+-rw-rw-rw-   0        0        0     6263 2023-07-05 18:30:04.000000 fichub-cli-0.9.3/fichub_cli/utils/fichub.py
+-rw-rw-rw-   0        0        0     2384 2023-06-04 18:06:14.000000 fichub-cli-0.9.3/fichub_cli/utils/logging.py
+-rw-rw-rw-   0        0        0    15260 2023-07-12 17:44:39.000000 fichub-cli-0.9.3/fichub_cli/utils/processing.py
+drwxrwxrwx   0        0        0        0 2023-07-12 18:07:14.572794 fichub-cli-0.9.3/fichub_cli.egg-info/
+-rw-rw-rw-   0        0        0     5262 2023-07-12 18:07:14.000000 fichub-cli-0.9.3/fichub_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      466 2023-07-12 18:07:14.000000 fichub-cli-0.9.3/fichub_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 18:07:14.000000 fichub-cli-0.9.3/fichub_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-07-12 18:07:14.000000 fichub-cli-0.9.3/fichub_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      115 2023-07-12 18:07:14.000000 fichub-cli-0.9.3/fichub_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-12 18:07:14.000000 fichub-cli-0.9.3/fichub_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      233 2023-06-04 18:06:14.000000 fichub-cli-0.9.3/pyproject.toml
+-rw-rw-rw-   0        0        0      114 2023-07-12 18:07:14.585793 fichub-cli-0.9.3/setup.cfg
+-rw-rw-rw-   0        0        0     1101 2023-07-12 17:47:08.000000 fichub-cli-0.9.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 18:07:14.578793 fichub-cli-0.9.3/tests/
+-rw-rw-rw-   0        0        0     2227 2023-07-12 17:47:08.000000 fichub-cli-0.9.3/tests/test_cli.py
```

### Comparing `fichub-cli-0.9.2/LICENSE.txt` & `fichub-cli-0.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fichub-cli-0.9.2/PKG-INFO` & `fichub-cli-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fichub-cli
-Version: 0.9.2
+Version: 0.9.3
 Summary: A CLI for the fichub.net API
 Home-page: https://github.com/FicHub/fichub-cli
 Author: Arbaaz Laskar
 Author-email: arzkar.dev@gmail.com
 License: Apache License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `fichub-cli-0.9.2/README.md` & `fichub-cli-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `fichub-cli-0.9.2/fichub_cli/cli.py` & `fichub-cli-0.9.3/fichub_cli/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from colorama import init, Fore, Style
 
 import importlib
 import pkgutil
 
 from .utils.fetch_data import FetchData
 from .utils.processing import get_format_type, out_dir_exists_check, \
-     appdir_builder, appdir_config_info, check_cli_outdated
+     appdir_builder, appdir_config_info, check_cli_outdated, output_log_cleanup
 from fichub_cli import __version__
 
 init(autoreset=True)  # colorama init
 timestamp = datetime.now().strftime("%Y-%m-%d T%H%M%S")
 
 app = typer.Typer(add_completion=False)
 app_dirs = PlatformDirs("fichub_cli", "fichub")
@@ -188,28 +188,14 @@
 
     try:
         if fic.exit_status == 1:
             typer.echo(
                 Fore.RED +
                 "\nThe CLI ran into some errors! Check the console for the log messages!" + Style.RESET_ALL)
 
-        if os.path.exists("output.log"):
-            with open(os.path.join(app_dirs.user_data_dir, "config.json"), 'r') as f:
-                config = json.load(f)
-            
-            if config["delete_output_log"] == "":
-                rm_output_log = typer.confirm(
-                    Fore.BLUE+"Delete the output.log?", abort=False, show_default=True)
-                if rm_output_log is True:
-                    os.remove("output.log")
-            elif config["delete_output_log"] == "true":
-                os.remove("output.log")
-            elif config["delete_output_log"] == "false":
-                pass
-
-
+        output_log_cleanup(app_dirs)
         sys.exit(fic.exit_status)
 
     # FileNotFoundError: output.log doesnt exist, when run 1st time
     # UnboundLocalError: 'fic' is not assigned value for --version flag
     except (FileNotFoundError, UnboundLocalError):
         sys.exit(0)
```

### Comparing `fichub-cli-0.9.2/fichub_cli/utils/fetch_data.py` & `fichub-cli-0.9.3/fichub_cli/utils/fetch_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import typer
+import sys
 from tqdm import tqdm
 from colorama import Fore
 from loguru import logger
 import traceback
 
 from .fichub import FicHub
 from .logging import init_log, download_processing_log, \
@@ -124,15 +125,15 @@
                             continue
 
             else:
                 typer.echo(Fore.RED +
                            "No new urls found! If output.log exists, please clear it.")
 
         except KeyboardInterrupt:
-            pass
+            sys.exit(2)
 
         finally:
             if self.changelog:
                 build_changelog(urls_input, urls_input_dedup, urls,
                                 downloaded_urls, err_urls, no_updates_urls, self.out_dir)
 
     def get_fic_with_list(self, list_url: str):
@@ -206,15 +207,15 @@
                             pbar.update(1)
                             continue
             else:
                 typer.echo(Fore.RED +
                            "No new urls found! If output.log exists, please clear it.")
 
         except KeyboardInterrupt:
-            pass
+            sys.exit(2)
 
         finally:
             if self.changelog:
                 build_changelog(urls_input, urls_input_dedup, urls,
                                 downloaded_urls, err_urls, no_updates_urls, self.out_dir)
 
     def get_fic_with_url(self, url_input: str):
```

### Comparing `fichub-cli-0.9.2/fichub_cli/utils/fichub.py` & `fichub-cli-0.9.3/fichub_cli/utils/fichub.py`

 * *Files 4% similar despite different names*

```diff
@@ -112,14 +112,15 @@
                     "download_url": "https://fichub.net" + cache_urls[file_format.replace(".", "")]
                 }
         # Error: 'epub_url'
         # Reason: Unsupported URL
         except (KeyError, UnboundLocalError) as e:
             if self.debug:
                 logger.error(f"Error: {str(e)} not found!")
+                logger.error(f"GET:Response: {str(self.response)}")
                 logger.error(
                     f"Skipping unsupported URL: {url}")
 
             self.exit_status = 1
             tqdm.write(
                 Fore.RED + f"\nSkipping unsupported URL: {url}" +
                 Style.RESET_ALL + Fore.CYAN +
```

### Comparing `fichub-cli-0.9.2/fichub_cli/utils/logging.py` & `fichub-cli-0.9.3/fichub_cli/utils/logging.py`

 * *Files identical despite different names*

### Comparing `fichub-cli-0.9.2/fichub_cli/utils/processing.py` & `fichub-cli-0.9.3/fichub_cli/utils/processing.py`

 * *Files 4% similar despite different names*

```diff
@@ -412,8 +412,23 @@
     for x in extraMeta:
         if re.match(prop, x.strip(), re.IGNORECASE):
             found =  (re.sub(prop+":","",x.strip(),0, re.MULTILINE | re.IGNORECASE)).strip()
             break
         else:
             found = None
 
-    return found
+    return found
+
+def output_log_cleanup(app_dirs):
+    if os.path.exists("output.log"):
+        with open(os.path.join(app_dirs.user_data_dir, "config.json"), 'r') as f:
+            config = json.load(f)
+        
+        if config["delete_output_log"] == "":
+            rm_output_log = typer.confirm(
+                Fore.BLUE+"Delete the output.log?", abort=False, show_default=True)
+            if rm_output_log is True:
+                os.remove("output.log")
+        elif config["delete_output_log"] == "true":
+            os.remove("output.log")
+        elif config["delete_output_log"] == "false":
+            pass
```

### Comparing `fichub-cli-0.9.2/fichub_cli.egg-info/PKG-INFO` & `fichub-cli-0.9.3/fichub_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fichub-cli
-Version: 0.9.2
+Version: 0.9.3
 Summary: A CLI for the fichub.net API
 Home-page: https://github.com/FicHub/fichub-cli
 Author: Arbaaz Laskar
 Author-email: arzkar.dev@gmail.com
 License: Apache License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `fichub-cli-0.9.2/setup.py` & `fichub-cli-0.9.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 setup(
     name='fichub-cli',
     author='Arbaaz Laskar',
     author_email="arzkar.dev@gmail.com",
     description="A CLI for the fichub.net API",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="0.9.2",
+    version="0.9.3",
     license='Apache License',
     url="https://github.com/FicHub/fichub-cli",
     packages=find_packages(include=['fichub_cli', 'fichub_cli.*']),
     include_package_data=True,
     install_requires=[
         'typer>=0.4.0',
         'requests>=2.31.0',
```

### Comparing `fichub-cli-0.9.2/tests/test_cli.py` & `fichub-cli-0.9.3/tests/test_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,8 +57,8 @@
 def test_cli_version():
     print("----------------------------------------")
     runner = CliRunner()
     result = runner.invoke(app, ['--version'])
 
     assert not result.exception
     assert result.exit_code == 0
-    assert result.output.strip() == 'fichub-cli: v0.9.2'
+    assert result.output.strip() == 'fichub-cli: v0.9.3'
```


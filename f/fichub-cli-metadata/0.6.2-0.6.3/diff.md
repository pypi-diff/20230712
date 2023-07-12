# Comparing `tmp/fichub-cli-metadata-0.6.2.tar.gz` & `tmp/fichub-cli-metadata-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Projects\Personal\Projects\Langs\Python\Others\fichub\fichub-cli\fichub-cli-contrib\fichub-cli-metadata\dist\.tmp-ydaiioi8\f", last modified: Wed Jul  5 18:36:03 2023, max compression
+gzip compressed data, was "D:\Projects\Personal\Projects\Langs\Python\Others\fichub\fichub-cli\fichub-cli-contrib\fichub-cli-metadata\dist\.tmp-2zg_jvqf\f", last modified: Wed Jul 12 18:14:53 2023, max compression
```

## Comparing `fichub-cli-metadata-0.6.2.tar` & `fichub-cli-metadata-0.6.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 18:36:03.574312 fichub-cli-metadata-0.6.2/
--rw-rw-rw-   0        0        0    11357 2022-02-09 16:27:55.000000 fichub-cli-metadata-0.6.2/LICENSE.txt
--rw-rw-rw-   0        0        0     5196 2023-07-05 18:36:03.574312 fichub-cli-metadata-0.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     4656 2023-01-28 09:21:55.000000 fichub-cli-metadata-0.6.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-05 18:36:03.534311 fichub-cli-metadata-0.6.2/fichub_cli_metadata/
--rw-rw-rw-   0        0        0      736 2023-07-05 18:32:56.000000 fichub-cli-metadata-0.6.2/fichub_cli_metadata/__init__.py
--rw-rw-rw-   0        0        0     6493 2023-07-05 18:32:56.000000 fichub-cli-metadata-0.6.2/fichub_cli_metadata/cli.py
-drwxrwxrwx   0        0        0        0 2023-07-05 18:36:03.572312 fichub-cli-metadata-0.6.2/fichub_cli_metadata/utils/
--rw-rw-rw-   0        0        0        0 2022-05-02 16:36:05.000000 fichub-cli-metadata-0.6.2/fichub_cli_metadata/utils/__init__.py
--rw-rw-rw-   0        0        0    11124 2023-07-05 18:32:56.000000 fichub-cli-metadata-0.6.2/fichub_cli_metadata/utils/crud.py
--rw-rw-rw-   0        0        0    20582 2023-07-05 17:06:07.000000 fichub-cli-metadata-0.6.2/fichub_cli_metadata/utils/fetch_data.py
--rw-rw-rw-   0        0        0     1138 2023-07-05 17:06:07.000000 fichub-cli-metadata-0.6.2/fichub_cli_metadata/utils/logging.py
--rw-rw-rw-   0        0        0     1522 2023-06-19 06:33:58.000000 fichub-cli-metadata-0.6.2/fichub_cli_metadata/utils/models.py
--rw-rw-rw-   0        0        0     4264 2023-01-28 09:21:55.000000 fichub-cli-metadata-0.6.2/fichub_cli_metadata/utils/processing.py
-drwxrwxrwx   0        0        0        0 2023-07-05 18:36:03.564312 fichub-cli-metadata-0.6.2/fichub_cli_metadata.egg-info/
--rw-rw-rw-   0        0        0     5196 2023-07-05 18:36:03.000000 fichub-cli-metadata-0.6.2/fichub_cli_metadata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      617 2023-07-05 18:36:03.000000 fichub-cli-metadata-0.6.2/fichub_cli_metadata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 18:36:03.000000 fichub-cli-metadata-0.6.2/fichub_cli_metadata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2023-07-05 18:36:03.000000 fichub-cli-metadata-0.6.2/fichub_cli_metadata.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       50 2023-07-05 18:36:03.000000 fichub-cli-metadata-0.6.2/fichub_cli_metadata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-05 18:36:03.000000 fichub-cli-metadata-0.6.2/fichub_cli_metadata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      229 2022-02-09 16:18:06.000000 fichub-cli-metadata-0.6.2/pyproject.toml
--rw-rw-rw-   0        0        0      114 2023-07-05 18:36:03.581311 fichub-cli-metadata-0.6.2/setup.cfg
--rw-rw-rw-   0        0        0     1114 2023-07-05 18:32:56.000000 fichub-cli-metadata-0.6.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-05 18:36:03.573312 fichub-cli-metadata-0.6.2/tests/
--rw-rw-rw-   0        0        0     1360 2023-07-05 18:32:56.000000 fichub-cli-metadata-0.6.2/tests/test_cli.py
+drwxrwxrwx   0        0        0        0 2023-07-12 18:14:53.542312 fichub-cli-metadata-0.6.3/
+-rw-rw-rw-   0        0        0    11357 2022-02-09 16:27:55.000000 fichub-cli-metadata-0.6.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     5196 2023-07-12 18:14:53.542312 fichub-cli-metadata-0.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4656 2023-01-28 09:21:55.000000 fichub-cli-metadata-0.6.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 18:14:53.506311 fichub-cli-metadata-0.6.3/fichub_cli_metadata/
+-rw-rw-rw-   0        0        0      736 2023-07-12 18:10:38.000000 fichub-cli-metadata-0.6.3/fichub_cli_metadata/__init__.py
+-rw-rw-rw-   0        0        0     6569 2023-07-12 18:08:59.000000 fichub-cli-metadata-0.6.3/fichub_cli_metadata/cli.py
+drwxrwxrwx   0        0        0        0 2023-07-12 18:14:53.541311 fichub-cli-metadata-0.6.3/fichub_cli_metadata/utils/
+-rw-rw-rw-   0        0        0        0 2022-05-02 16:36:05.000000 fichub-cli-metadata-0.6.3/fichub_cli_metadata/utils/__init__.py
+-rw-rw-rw-   0        0        0    11124 2023-07-05 18:32:56.000000 fichub-cli-metadata-0.6.3/fichub_cli_metadata/utils/crud.py
+-rw-rw-rw-   0        0        0    20596 2023-07-12 18:07:36.000000 fichub-cli-metadata-0.6.3/fichub_cli_metadata/utils/fetch_data.py
+-rw-rw-rw-   0        0        0     1138 2023-07-05 17:06:07.000000 fichub-cli-metadata-0.6.3/fichub_cli_metadata/utils/logging.py
+-rw-rw-rw-   0        0        0     1522 2023-06-19 06:33:58.000000 fichub-cli-metadata-0.6.3/fichub_cli_metadata/utils/models.py
+-rw-rw-rw-   0        0        0     4264 2023-01-28 09:21:55.000000 fichub-cli-metadata-0.6.3/fichub_cli_metadata/utils/processing.py
+drwxrwxrwx   0        0        0        0 2023-07-12 18:14:53.534313 fichub-cli-metadata-0.6.3/fichub_cli_metadata.egg-info/
+-rw-rw-rw-   0        0        0     5196 2023-07-12 18:14:53.000000 fichub-cli-metadata-0.6.3/fichub_cli_metadata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      617 2023-07-12 18:14:53.000000 fichub-cli-metadata-0.6.3/fichub_cli_metadata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 18:14:53.000000 fichub-cli-metadata-0.6.3/fichub_cli_metadata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-07-12 18:14:53.000000 fichub-cli-metadata-0.6.3/fichub_cli_metadata.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       50 2023-07-12 18:14:53.000000 fichub-cli-metadata-0.6.3/fichub_cli_metadata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-12 18:14:53.000000 fichub-cli-metadata-0.6.3/fichub_cli_metadata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      229 2022-02-09 16:18:06.000000 fichub-cli-metadata-0.6.3/pyproject.toml
+-rw-rw-rw-   0        0        0      114 2023-07-12 18:14:53.547310 fichub-cli-metadata-0.6.3/setup.cfg
+-rw-rw-rw-   0        0        0     1114 2023-07-12 18:10:38.000000 fichub-cli-metadata-0.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 18:14:53.541311 fichub-cli-metadata-0.6.3/tests/
+-rw-rw-rw-   0        0        0     1360 2023-07-12 18:10:38.000000 fichub-cli-metadata-0.6.3/tests/test_cli.py
```

### Comparing `fichub-cli-metadata-0.6.2/LICENSE.txt` & `fichub-cli-metadata-0.6.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fichub-cli-metadata-0.6.2/PKG-INFO` & `fichub-cli-metadata-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fichub-cli-metadata
-Version: 0.6.2
+Version: 0.6.3
 Summary: A metadata plugin for fetching Metadata from the Fichub API for the fichub-cli
 Home-page: https://github.com/fichub-cli-contrib/fichub-cli-metadata
 Author: Arbaaz Laskar
 Author-email: arzkar.dev@gmail.com
 License: Apache License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `fichub-cli-metadata-0.6.2/README.md` & `fichub-cli-metadata-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `fichub-cli-metadata-0.6.2/fichub_cli_metadata/__init__.py` & `fichub-cli-metadata-0.6.3/fichub_cli_metadata/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,10 +9,10 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # __version__ at the top to prevent ImportError: ... partially initialized module ...
-__version__ = "0.6.2"
+__version__ = "0.6.3"
 
 from .cli import app  # entry_point
```

### Comparing `fichub-cli-metadata-0.6.2/fichub_cli_metadata/cli.py` & `fichub-cli-metadata-0.6.3/fichub_cli_metadata/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from platformdirs import PlatformDirs
 from loguru import logger
 from datetime import datetime
 from colorama import init, Fore, Style
 
 from .utils.fetch_data import FetchData
 from fichub_cli.utils.processing import get_format_type, check_cli_outdated,\
-    appdir_exists_check, appdir_builder, appdir_config_info
+    appdir_exists_check, appdir_builder, appdir_config_info, output_log_cleanup
 from fichub_cli_metadata import __version__
 
 
 init(autoreset=True)  # colorama init
 app = typer.Typer(add_completion=False)
 app_dirs = PlatformDirs("fichub_cli", "fichub")
 
@@ -110,19 +110,19 @@
     if config_info:
         # overwrite the config files
         appdir_config_info(app_dirs)
 
     if debug_log:
         timestamp = datetime.now().strftime("%Y-%m-%d T%H%M%S")
         logger.remove()  # remove all existing handlers
-        logger.add(f"fichub_cli - {timestamp}.log")
+        logger.add(f"fichub_cli_metadata - {timestamp}.log")
         debug = True
         typer.echo(
             Fore.GREEN + "Creating " + Style.RESET_ALL + Fore.YELLOW +
-            f"fichub_cli - {timestamp}.log" + Style.RESET_ALL +
+            f"fichub_cli_metadata - {timestamp}.log" + Style.RESET_ALL +
             Fore.GREEN + " in the current directory!" + Style.RESET_ALL)
 
     if not download_ebook == "":
         format_type = get_format_type(download_ebook)
     else:
         format_type = []
 
@@ -157,13 +157,14 @@
 
     try:
         if fic.exit_status == 1:
             typer.echo(
                 Fore.RED +
                 "\nThe CLI ran into some errors! Check the console for the log messages!" + Style.RESET_ALL)
 
+        output_log_cleanup(app_dirs)
         sys.exit(fic.exit_status)
 
     # FileNotFoundError: output.log doesnt exist, when run 1st time
     # UnboundLocalError: 'fic' is not assigned value for --version flag
     except (FileNotFoundError, UnboundLocalError):
         sys.exit(0)
```

### Comparing `fichub-cli-metadata-0.6.2/fichub_cli_metadata/utils/crud.py` & `fichub-cli-metadata-0.6.3/fichub_cli_metadata/utils/crud.py`

 * *Files identical despite different names*

### Comparing `fichub-cli-metadata-0.6.2/fichub_cli_metadata/utils/fetch_data.py` & `fichub-cli-metadata-0.6.3/fichub_cli_metadata/utils/fetch_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,15 +192,15 @@
                                    "\nMetadata saved as " + Fore.BLUE +
                                    f"{os.path.abspath(self.db_file)}"+Style.RESET_ALL +
                                    Style.RESET_ALL)
             else:
                 typer.echo(Fore.RED +
                            "No new urls found! If output.log exists, please clear it.")
         except KeyboardInterrupt:
-            pass
+            sys.exit(2)
 
         finally:
             if self.changelog:
                 build_changelog(urls_input, urls_input_dedup, urls, downloaded_urls,
                                 err_urls, no_updates_urls, self.out_dir)
 
     def save_to_db(self, item):
@@ -321,15 +321,15 @@
                             file.write(url+"\n")
                         err_urls.append(url)
                         self.exit_status = 1
                         pbar.update(1)
                         continue  # skip the unsupported url
 
         except KeyboardInterrupt:
-            pass
+            sys.exit(2)
 
         finally:
             if self.changelog:
                 build_changelog(urls_input, urls, urls, downloaded_urls,
                                 err_urls, no_updates_urls, self.out_dir)
 
     def export_db_as_json(self):
```

### Comparing `fichub-cli-metadata-0.6.2/fichub_cli_metadata/utils/logging.py` & `fichub-cli-metadata-0.6.3/fichub_cli_metadata/utils/logging.py`

 * *Files identical despite different names*

### Comparing `fichub-cli-metadata-0.6.2/fichub_cli_metadata/utils/models.py` & `fichub-cli-metadata-0.6.3/fichub_cli_metadata/utils/models.py`

 * *Files identical despite different names*

### Comparing `fichub-cli-metadata-0.6.2/fichub_cli_metadata/utils/processing.py` & `fichub-cli-metadata-0.6.3/fichub_cli_metadata/utils/processing.py`

 * *Files identical despite different names*

### Comparing `fichub-cli-metadata-0.6.2/fichub_cli_metadata.egg-info/PKG-INFO` & `fichub-cli-metadata-0.6.3/fichub_cli_metadata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fichub-cli-metadata
-Version: 0.6.2
+Version: 0.6.3
 Summary: A metadata plugin for fetching Metadata from the Fichub API for the fichub-cli
 Home-page: https://github.com/fichub-cli-contrib/fichub-cli-metadata
 Author: Arbaaz Laskar
 Author-email: arzkar.dev@gmail.com
 License: Apache License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `fichub-cli-metadata-0.6.2/fichub_cli_metadata.egg-info/SOURCES.txt` & `fichub-cli-metadata-0.6.3/fichub_cli_metadata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fichub-cli-metadata-0.6.2/setup.py` & `fichub-cli-metadata-0.6.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 setup(
     name='fichub-cli-metadata',
     author='Arbaaz Laskar',
     author_email="arzkar.dev@gmail.com",
     description="A metadata plugin for fetching Metadata from the Fichub API for the fichub-cli",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version='0.6.2',
+    version='0.6.3',
     license='Apache License',
     url="https://github.com/fichub-cli-contrib/fichub-cli-metadata",
     packages=find_packages(
         include=['fichub_cli_metadata', 'fichub_cli_metadata.*']),
     include_package_data=True,
     install_requires=[
-        'fichub-cli>=0.8.2',
+        'fichub-cli>=0.9.3',
         'rich>=10.4.0',
         'sqlalchemy>=1.4.31'
     ],
     entry_points= {
         'console_scripts': [
             'fichub_cli_metadata=fichub_cli_metadata.cli:app'
         ]
```

### Comparing `fichub-cli-metadata-0.6.2/tests/test_cli.py` & `fichub-cli-metadata-0.6.3/tests/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,8 +31,8 @@
 def test_cli_version():
     print("----------------------------------------")
     runner = CliRunner()
     result = runner.invoke(app, ['--version'])
     
     assert not result.exception
     assert result.exit_code == 0
-    assert result.output.strip() == 'fichub-cli-metadata: v0.6.2'
+    assert result.output.strip() == 'fichub-cli-metadata: v0.6.3'
```


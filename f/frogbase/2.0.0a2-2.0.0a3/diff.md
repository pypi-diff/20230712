# Comparing `tmp/frogbase-2.0.0a2.tar.gz` & `tmp/frogbase-2.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frogbase-2.0.0a2.tar", max compression
+gzip compressed data, was "frogbase-2.0.0a3.tar", max compression
```

## Comparing `frogbase-2.0.0a2.tar` & `frogbase-2.0.0a3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1070 2023-06-17 23:46:09.847926 frogbase-2.0.0a2/LICENSE
--rw-r--r--   0        0        0     4016 2023-07-06 21:02:27.903992 frogbase-2.0.0a2/README.md
--rw-r--r--   0        0        0       27 2023-07-05 10:01:59.615234 frogbase-2.0.0a2/frogbase/__init__.py
--rw-r--r--   0        0        0      984 2023-07-05 10:01:59.615234 frogbase-2.0.0a2/frogbase/__main__.py
--rw-r--r--   0        0        0     8263 2023-07-06 22:12:19.492087 frogbase-2.0.0a2/frogbase/captions.py
--rw-r--r--   0        0        0      946 2023-07-05 10:01:59.615234 frogbase-2.0.0a2/frogbase/config.py
--rw-r--r--   0        0        0    16491 2023-07-06 23:28:55.421394 frogbase-2.0.0a2/frogbase/core.py
--rw-r--r--   0        0        0    29577 2023-07-06 21:59:29.299325 frogbase-2.0.0a2/frogbase/media.py
--rw-r--r--   0        0        0    25161 2023-07-06 22:11:30.461311 frogbase-2.0.0a2/frogbase/models.py
--rw-r--r--   0        0        0     2975 2023-07-06 23:33:01.546938 frogbase-2.0.0a2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-05 10:01:59.619233 frogbase-2.0.0a2/tests/__init__.py
--rw-r--r--   0        0        0      242 2023-07-05 10:01:59.619233 frogbase-2.0.0a2/tests/conftest.py
--rw-r--r--   0        0        0     1160 2023-07-05 10:01:59.619233 frogbase-2.0.0a2/tests/test_config.py
--rw-r--r--   0        0        0     6031 2023-07-05 10:01:59.619233 frogbase-2.0.0a2/tests/test_core.py
--rw-r--r--   0        0        0     3289 2023-07-05 10:01:59.619233 frogbase-2.0.0a2/tests/test_media.py
--rw-r--r--   0        0        0     5541 1970-01-01 00:00:00.000000 frogbase-2.0.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-12 17:23:12.593038 frogbase-2.0.0a3/LICENSE
+-rw-r--r--   0        0        0     4047 2023-07-12 17:23:12.593038 frogbase-2.0.0a3/README.md
+-rw-r--r--   0        0        0       27 2023-07-12 17:23:12.593038 frogbase-2.0.0a3/frogbase/__init__.py
+-rw-r--r--   0        0        0      984 2023-07-12 17:23:12.593038 frogbase-2.0.0a3/frogbase/__main__.py
+-rw-r--r--   0        0        0     8263 2023-07-12 17:23:12.593038 frogbase-2.0.0a3/frogbase/captions.py
+-rw-r--r--   0        0        0      946 2023-07-12 17:23:12.593038 frogbase-2.0.0a3/frogbase/config.py
+-rw-r--r--   0        0        0    16479 2023-07-12 17:27:02.207196 frogbase-2.0.0a3/frogbase/core.py
+-rw-r--r--   0        0        0    29577 2023-07-12 17:23:12.593038 frogbase-2.0.0a3/frogbase/media.py
+-rw-r--r--   0        0        0    25161 2023-07-12 17:23:12.597038 frogbase-2.0.0a3/frogbase/models.py
+-rw-r--r--   0        0        0     2990 2023-07-12 17:26:48.211552 frogbase-2.0.0a3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-12 17:23:12.597038 frogbase-2.0.0a3/tests/__init__.py
+-rw-r--r--   0        0        0      242 2023-07-12 17:23:12.597038 frogbase-2.0.0a3/tests/conftest.py
+-rw-r--r--   0        0        0     1160 2023-07-12 17:23:12.597038 frogbase-2.0.0a3/tests/test_config.py
+-rw-r--r--   0        0        0     6031 2023-07-12 17:23:12.597038 frogbase-2.0.0a3/tests/test_core.py
+-rw-r--r--   0        0        0     3289 2023-07-12 17:23:12.597038 frogbase-2.0.0a3/tests/test_media.py
+-rw-r--r--   0        0        0     5669 1970-01-01 00:00:00.000000 frogbase-2.0.0a3/PKG-INFO
```

### Comparing `frogbase-2.0.0a2/LICENSE` & `frogbase-2.0.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `frogbase-2.0.0a2/README.md` & `frogbase-2.0.0a3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 **FrogBase** (previously whisper-ui) simplifies the `download-transcribe-embed-index` workflow for multi-media content.
 It does so by linking content from various platforms
 ([yt_dlp](https://github.com/yt-dlp/yt-dlp))
 with speech-to-text models ([OpenAI's Whisper](https://github.com/openai/whisper)),
 image & text encoders ([SentenceTransformers](https://github.com/UKPLab/sentence-transformers)),
 and embedding stores ([hnswlib](https://github.com/nmslib/hnswlib)).
 
+> ⚠️ Warning: This is currently a pre-release version and is known to be very unstable. For stable releases, please use any 1.x versions.
+
 ```python
 from frogbase import FrogBase
 fb = FrogBase()
 fb.demo()
 fb.search("What is the name of the squeaky frog?")
 ```
 
@@ -22,20 +24,18 @@
 
 https://user-images.githubusercontent.com/6735526/216852681-53b6c3db-3e74-4c86-806f-6f6774a9003a.mp4
 
 [![PyPI](https://img.shields.io/pypi/v/frogbase.svg)][pypi_]
 [![Status](https://img.shields.io/pypi/status/frogbase.svg)][status]
 [![Python Version](https://img.shields.io/pypi/pyversions/frogbase)][python version]
 [![License](https://img.shields.io/pypi/l/frogbase)][license]
-[![Discord](https://img.shields.io/discord/1120743576435949689)][discord]
 
 [pypi_]: https://pypi.org/project/frogbase/
 [status]: https://pypi.org/project/frogbase/
 [python version]: https://pypi.org/project/frogbase
-[discord]: https://discord.gg/e23YJWqu
 [license]: https://github.com/hayabhay/frogbase/blob/main/LICENSE
 
 ## Features
 
 FrogBase currently provides functionality to:
 
 - Download media files from a wide range of platforms (YouTube, TikTok, Vimeo, etc.) using [yt_dlp](https://github.com/yt-dlp/yt-dlp)
@@ -104,12 +104,12 @@
 
 > [Coming soon] Instructions, environment for installation using Docker & Anaconda
 
 ## Links
 
 - [Documentation](https://hayabhay.github.io/frogbase/)
 - [Issues](https://github.com/hayabhay/frogbase/issues) & [Discussions](https://github.com/hayabhay/frogbase/discussions)
-- [Discord](https://discord.gg/e23YJWqu)
+- [Discord](https://discord.gg/HKkpnx8pU)
 - [History](docs/history.md)
 - [Roadmap](docs/roadmap.md)
 - [Contributing Guide](docs/contributing.md)
 - [License](LICENSE) (MIT)
```

### Comparing `frogbase-2.0.0a2/frogbase/__main__.py` & `frogbase-2.0.0a3/frogbase/__main__.py`

 * *Files identical despite different names*

### Comparing `frogbase-2.0.0a2/frogbase/captions.py` & `frogbase-2.0.0a3/frogbase/captions.py`

 * *Files identical despite different names*

### Comparing `frogbase-2.0.0a2/frogbase/config.py` & `frogbase-2.0.0a3/frogbase/config.py`

 * *Files identical despite different names*

### Comparing `frogbase-2.0.0a2/frogbase/core.py` & `frogbase-2.0.0a3/frogbase/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,15 @@
         try:
             db_meta = self._db.get(Query().type == "meta") if self._db else None
         except Exception as e:
             self._logger.error(f"Failed to load tinydb instance. Error: {e}")
             self._db.close()
             self._dbpath.unlink()
             self._db = None
-            
+
         if db_meta and db_meta["__version__"] < self._version:
             self._logger.info(f"Existing tinydb version: {db_meta['__version__']} is stale. Removing.")
             self._db.close()
             self._dbpath.unlink()
             self._db = None
 
         # Next, if the tinydb instance never existed or was deleted from being stale, create a new one.
```

### Comparing `frogbase-2.0.0a2/frogbase/media.py` & `frogbase-2.0.0a3/frogbase/media.py`

 * *Files identical despite different names*

### Comparing `frogbase-2.0.0a2/frogbase/models.py` & `frogbase-2.0.0a3/frogbase/models.py`

 * *Files identical despite different names*

### Comparing `frogbase-2.0.0a2/pyproject.toml` & `frogbase-2.0.0a3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool]
 
 # ==== Poetry ====
 [tool.poetry]
 name = "frogbase"
-version = "2.0.0a2"
+version = "2.0.0a3"
 description = "FrogBase simplifies the download-transcribe-embed-index workflow for multi-media content. It does so by linking content from various platforms with speech-to-text models, image & text encoders and embedding stores."
 homepage = "https://hayabhay.github.io/frogbase"
 repository = "https://github.com/hayabhay/frogbase"
 documentation = "https://hayabhay.github.io/frogbase"
 authors = ["Abhay Kashyap"]
 readme = "README.md"
 license =  "MIT"
@@ -37,14 +37,16 @@
 tinydb = "^4.8.0"
 humanize = "^4.6.0"
 webvtt-py = "^0.4.6"
 pydantic = "^2.0"
 openai-whisper = "^20230314"
 sentence-transformers = "^2.2.2"
 hnswlib = "^0.7.0"
+streamlit = {version = "^1.24.1", optional = true, extras = ["ui"]}
+python-dotenv = {version = "^1.0.0", optional = true, extras = ["ui"]}
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 tox = "^4.6.2"
 pre-commit = "^3.3.3"
@@ -74,21 +76,14 @@
 mkdocs-material = "^9.1.16"
 mkdocs-video = "^1.5.0"
 mkdocstrings = "^0.22.0"
 mkdocs-autorefs = "^0.4.1"
 mike = "^1.1.2"
 
 
-[tool.poetry.group.ui]
-optional = true
-
-[tool.poetry.group.ui.dependencies]
-streamlit = "^1.23.1"
-python-dotenv = "^1.0.0"
-
 [tool.poetry.scripts]
 frogbase = "frogbase.__main__:ui"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `frogbase-2.0.0a2/tests/test_config.py` & `frogbase-2.0.0a3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `frogbase-2.0.0a2/tests/test_core.py` & `frogbase-2.0.0a3/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `frogbase-2.0.0a2/tests/test_media.py` & `frogbase-2.0.0a3/tests/test_media.py`

 * *Files identical despite different names*

### Comparing `frogbase-2.0.0a2/PKG-INFO` & `frogbase-2.0.0a3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frogbase
-Version: 2.0.0a2
+Version: 2.0.0a3
 Summary: FrogBase simplifies the download-transcribe-embed-index workflow for multi-media content. It does so by linking content from various platforms with speech-to-text models, image & text encoders and embedding stores.
 Home-page: https://hayabhay.github.io/frogbase
 License: MIT
 Author: Abhay Kashyap
 Requires-Python: >=3.8, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -16,15 +16,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: hnswlib (>=0.7.0,<0.8.0)
 Requires-Dist: humanize (>=4.6.0,<5.0.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: openai-whisper (>=20230314,<20230315)
 Requires-Dist: pydantic (>=2.0,<3.0)
+Requires-Dist: python-dotenv[ui] (>=1.0.0,<2.0.0)
 Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0)
+Requires-Dist: streamlit[ui] (>=1.24.1,<2.0.0)
 Requires-Dist: tinydb (>=4.8.0,<5.0.0)
 Requires-Dist: webvtt-py (>=0.4.6,<0.5.0)
 Requires-Dist: yt-dlp (>=2023.3.4,<2024.0.0)
 Project-URL: Changelog, https://github.com/hayabhay/frogbase/releases
 Project-URL: Documentation, https://hayabhay.github.io/frogbase
 Project-URL: Repository, https://github.com/hayabhay/frogbase
 Description-Content-Type: text/markdown
@@ -36,14 +38,16 @@
 **FrogBase** (previously whisper-ui) simplifies the `download-transcribe-embed-index` workflow for multi-media content.
 It does so by linking content from various platforms
 ([yt_dlp](https://github.com/yt-dlp/yt-dlp))
 with speech-to-text models ([OpenAI's Whisper](https://github.com/openai/whisper)),
 image & text encoders ([SentenceTransformers](https://github.com/UKPLab/sentence-transformers)),
 and embedding stores ([hnswlib](https://github.com/nmslib/hnswlib)).
 
+> ⚠️ Warning: This is currently a pre-release version and is known to be very unstable. For stable releases, please use any 1.x versions.
+
 ```python
 from frogbase import FrogBase
 fb = FrogBase()
 fb.demo()
 fb.search("What is the name of the squeaky frog?")
 ```
 
@@ -53,20 +57,18 @@
 
 https://user-images.githubusercontent.com/6735526/216852681-53b6c3db-3e74-4c86-806f-6f6774a9003a.mp4
 
 [![PyPI](https://img.shields.io/pypi/v/frogbase.svg)][pypi_]
 [![Status](https://img.shields.io/pypi/status/frogbase.svg)][status]
 [![Python Version](https://img.shields.io/pypi/pyversions/frogbase)][python version]
 [![License](https://img.shields.io/pypi/l/frogbase)][license]
-[![Discord](https://img.shields.io/discord/1120743576435949689)][discord]
 
 [pypi_]: https://pypi.org/project/frogbase/
 [status]: https://pypi.org/project/frogbase/
 [python version]: https://pypi.org/project/frogbase
-[discord]: https://discord.gg/e23YJWqu
 [license]: https://github.com/hayabhay/frogbase/blob/main/LICENSE
 
 ## Features
 
 FrogBase currently provides functionality to:
 
 - Download media files from a wide range of platforms (YouTube, TikTok, Vimeo, etc.) using [yt_dlp](https://github.com/yt-dlp/yt-dlp)
@@ -135,13 +137,13 @@
 
 > [Coming soon] Instructions, environment for installation using Docker & Anaconda
 
 ## Links
 
 - [Documentation](https://hayabhay.github.io/frogbase/)
 - [Issues](https://github.com/hayabhay/frogbase/issues) & [Discussions](https://github.com/hayabhay/frogbase/discussions)
-- [Discord](https://discord.gg/e23YJWqu)
+- [Discord](https://discord.gg/HKkpnx8pU)
 - [History](docs/history.md)
 - [Roadmap](docs/roadmap.md)
 - [Contributing Guide](docs/contributing.md)
 - [License](LICENSE) (MIT)
```


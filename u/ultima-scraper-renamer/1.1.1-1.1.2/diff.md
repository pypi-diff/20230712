# Comparing `tmp/ultima_scraper_renamer-1.1.1.tar.gz` & `tmp/ultima_scraper_renamer-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultima_scraper_renamer-1.1.1.tar", max compression
+gzip compressed data, was "ultima_scraper_renamer-1.1.2.tar", max compression
```

## Comparing `ultima_scraper_renamer-1.1.1.tar` & `ultima_scraper_renamer-1.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2022-12-05 14:42:02.218210 ultima_scraper_renamer-1.1.1/README.md
--rw-r--r--   0        0        0      681 2023-06-15 09:18:21.582794 ultima_scraper_renamer-1.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2022-12-05 14:42:02.218210 ultima_scraper_renamer-1.1.1/ultima_scraper_renamer/__init__.py
--rw-r--r--   0        0        0        0 2022-12-06 16:13:32.768074 ultima_scraper_renamer-1.1.1/ultima_scraper_renamer/py.typed
--rw-r--r--   0        0        0    17639 2023-06-15 07:54:48.280407 ultima_scraper_renamer-1.1.1/ultima_scraper_renamer/reformat.py
--rw-r--r--   0        0        0     7872 2023-05-14 17:44:23.086692 ultima_scraper_renamer-1.1.1/ultima_scraper_renamer/renamer.py
--rw-r--r--   0        0        0      574 1970-01-01 00:00:00.000000 ultima_scraper_renamer-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-12-05 14:42:02.218210 ultima_scraper_renamer-1.1.2/README.md
+-rw-r--r--   0        0        0      681 2023-07-12 03:43:02.459046 ultima_scraper_renamer-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-12-05 14:42:02.218210 ultima_scraper_renamer-1.1.2/ultima_scraper_renamer/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-06 16:13:32.768074 ultima_scraper_renamer-1.1.2/ultima_scraper_renamer/py.typed
+-rw-r--r--   0        0        0    17669 2023-07-11 07:23:24.246442 ultima_scraper_renamer-1.1.2/ultima_scraper_renamer/reformat.py
+-rw-r--r--   0        0        0     7872 2023-05-14 17:44:23.086692 ultima_scraper_renamer-1.1.2/ultima_scraper_renamer/renamer.py
+-rw-r--r--   0        0        0      574 1970-01-01 00:00:00.000000 ultima_scraper_renamer-1.1.2/PKG-INFO
```

### Comparing `ultima_scraper_renamer-1.1.1/pyproject.toml` & `ultima_scraper_renamer-1.1.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "ultima-scraper-renamer"
-version = "1.1.1"
+version = "1.1.2"
 description = ""
 authors = [
     "DIGITALCRIMINALS <89371864+digitalcriminals@users.noreply.github.com>",
 ]
 readme = "README.md"
 packages = [{include = "ultima_scraper_renamer"}]
 include = ["ultima_scraper_renamer/py.typed"]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 tqdm = "^4.64.1"
 orjson = "^3.8.3"
-ultima-scraper-api = "^1.1.0"
-ultima-scraper-collection = "^1.1.0"
+ultima-scraper-api = "^2.0.0"
+ultima-scraper-collection = "^2.0.0"
 
 
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.2"
 
 [tool.semantic_release]
```

### Comparing `ultima_scraper_renamer-1.1.1/ultima_scraper_renamer/reformat.py` & `ultima_scraper_renamer-1.1.2/ultima_scraper_renamer/reformat.py`

 * *Files 0% similar despite different names*

```diff
@@ -380,17 +380,17 @@
         option["filename"] = name
         option["ext"] = ext
         option["api_type"] = final_api_type
         option["media_type"] = media_item.media_type
         option["text"] = content_metadata.text
         option["profile_username"] = self.authed.username
         option["model_username"] = content_metadata.__soft__.author.username
-        option["date_format"] = site_settings.date_format
+        option["date_format"] = site_settings.download_setup.date_format
         option["postedAt"] = media_item.created_at
-        option["text_length"] = site_settings.text_length
+        option["text_length"] = site_settings.download_setup.text_length
         option["directory"] = download_path
         option["price"] = content_metadata.price
         option["preview"] = media_item.preview
         option["archived"] = content_metadata.archived
         return ReformatItem(option)
 
     def drm_format(self, media_url: str, media_item: MediaMetadata):
```

### Comparing `ultima_scraper_renamer-1.1.1/ultima_scraper_renamer/renamer.py` & `ultima_scraper_renamer-1.1.2/ultima_scraper_renamer/renamer.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_renamer-1.1.1/PKG-INFO` & `ultima_scraper_renamer-1.1.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: ultima-scraper-renamer
-Version: 1.1.1
+Version: 1.1.2
 Summary: 
 Author: DIGITALCRIMINALS
 Author-email: 89371864+digitalcriminals@users.noreply.github.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: orjson (>=3.8.3,<4.0.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
-Requires-Dist: ultima-scraper-api (>=1.1.0,<2.0.0)
-Requires-Dist: ultima-scraper-collection (>=1.1.0,<2.0.0)
+Requires-Dist: ultima-scraper-api (>=2.0.0,<3.0.0)
+Requires-Dist: ultima-scraper-collection (>=2.0.0,<3.0.0)
 Description-Content-Type: text/markdown
```


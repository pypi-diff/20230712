# Comparing `tmp/hoyolab-rss-feeds-2.1.1.tar.gz` & `tmp/hoyolab-rss-feeds-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoyolab-rss-feeds-2.1.1.tar", last modified: Tue Jan 24 00:00:56 2023, max compression
+gzip compressed data, was "hoyolab-rss-feeds-2.2.0.tar", last modified: Tue Jul 11 22:09:06 2023, max compression
```

## Comparing `hoyolab-rss-feeds-2.1.1.tar` & `hoyolab-rss-feeds-2.2.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 00:00:56.130324 hoyolab-rss-feeds-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-24 00:00:40.000000 hoyolab-rss-feeds-2.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-01-24 00:00:40.000000 hoyolab-rss-feeds-2.1.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-01-24 00:00:40.000000 hoyolab-rss-feeds-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-24 00:00:40.000000 hoyolab-rss-feeds-2.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6097 2023-01-24 00:00:56.130324 hoyolab-rss-feeds-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-01-24 00:00:40.000000 hoyolab-rss-feeds-2.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-01-24 00:00:40.000000 hoyolab-rss-feeds-2.1.1/RELEASENOTES.md
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-01-24 00:00:40.000000 hoyolab-rss-feeds-2.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-24 00:00:56.130324 hoyolab-rss-feeds-2.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 00:00:56.126324 hoyolab-rss-feeds-2.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 00:00:56.130324 hoyolab-rss-feeds-2.1.1/src/hoyolab_rss_feeds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6097 2023-01-24 00:00:56.000000 hoyolab-rss-feeds-2.1.1/src/hoyolab_rss_feeds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-01-24 00:00:56.000000 hoyolab-rss-feeds-2.1.1/src/hoyolab_rss_feeds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 00:00:56.000000 hoyolab-rss-feeds-2.1.1/src/hoyolab_rss_feeds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-24 00:00:56.000000 hoyolab-rss-feeds-2.1.1/src/hoyolab_rss_feeds.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-01-24 00:00:56.000000 hoyolab-rss-feeds-2.1.1/src/hoyolab_rss_feeds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-24 00:00:56.000000 hoyolab-rss-feeds-2.1.1/src/hoyolab_rss_feeds.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 00:00:56.130324 hoyolab-rss-feeds-2.1.1/src/hoyolabrssfeeds/
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-01-24 00:00:40.000000 hoyolab-rss-feeds-2.1.1/src/hoyolabrssfeeds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-01-24 00:00:40.000000 hoyolab-rss-feeds-2.1.1/src/hoyolabrssfeeds/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-01-24 00:00:40.000000 hoyolab-rss-feeds-2.1.1/src/hoyolabrssfeeds/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-01-24 00:00:40.000000 hoyolab-rss-feeds-2.1.1/src/hoyolabrssfeeds/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7194 2023-01-24 00:00:40.000000 hoyolab-rss-feeds-2.1.1/src/hoyolabrssfeeds/feeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-01-24 00:00:40.000000 hoyolab-rss-feeds-2.1.1/src/hoyolabrssfeeds/hoyolab.py
--rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-01-24 00:00:40.000000 hoyolab-rss-feeds-2.1.1/src/hoyolabrssfeeds/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-01-24 00:00:40.000000 hoyolab-rss-feeds-2.1.1/src/hoyolabrssfeeds/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 00:00:40.000000 hoyolab-rss-feeds-2.1.1/src/hoyolabrssfeeds/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-01-24 00:00:40.000000 hoyolab-rss-feeds-2.1.1/src/hoyolabrssfeeds/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 00:00:56.130324 hoyolab-rss-feeds-2.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 00:00:40.000000 hoyolab-rss-feeds-2.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-01-24 00:00:40.000000 hoyolab-rss-feeds-2.1.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-01-24 00:00:40.000000 hoyolab-rss-feeds-2.1.1/tests/test_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9514 2023-01-24 00:00:40.000000 hoyolab-rss-feeds-2.1.1/tests/test_feeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-01-24 00:00:40.000000 hoyolab-rss-feeds-2.1.1/tests/test_hoyolab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-01-24 00:00:40.000000 hoyolab-rss-feeds-2.1.1/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-01-24 00:00:40.000000 hoyolab-rss-feeds-2.1.1/tests/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-01-24 00:00:40.000000 hoyolab-rss-feeds-2.1.1/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-01-24 00:00:40.000000 hoyolab-rss-feeds-2.1.1/tests/test_writers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-01-24 00:00:40.000000 hoyolab-rss-feeds-2.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:09:06.855263 hoyolab-rss-feeds-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-11 22:08:50.000000 hoyolab-rss-feeds-2.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-11 22:08:50.000000 hoyolab-rss-feeds-2.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-11 22:08:50.000000 hoyolab-rss-feeds-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-11 22:08:50.000000 hoyolab-rss-feeds-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-07-11 22:09:06.855263 hoyolab-rss-feeds-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-07-11 22:08:50.000000 hoyolab-rss-feeds-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-11 22:08:50.000000 hoyolab-rss-feeds-2.2.0/RELEASENOTES.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-07-11 22:08:50.000000 hoyolab-rss-feeds-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 22:09:06.855263 hoyolab-rss-feeds-2.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:09:06.843262 hoyolab-rss-feeds-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:09:06.847262 hoyolab-rss-feeds-2.2.0/src/hoyolab_rss_feeds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-07-11 22:09:06.000000 hoyolab-rss-feeds-2.2.0/src/hoyolab_rss_feeds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-11 22:09:06.000000 hoyolab-rss-feeds-2.2.0/src/hoyolab_rss_feeds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 22:09:06.000000 hoyolab-rss-feeds-2.2.0/src/hoyolab_rss_feeds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-11 22:09:06.000000 hoyolab-rss-feeds-2.2.0/src/hoyolab_rss_feeds.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-11 22:09:06.000000 hoyolab-rss-feeds-2.2.0/src/hoyolab_rss_feeds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 22:09:06.000000 hoyolab-rss-feeds-2.2.0/src/hoyolab_rss_feeds.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:09:06.851263 hoyolab-rss-feeds-2.2.0/src/hoyolabrssfeeds/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-11 22:08:50.000000 hoyolab-rss-feeds-2.2.0/src/hoyolabrssfeeds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-11 22:08:50.000000 hoyolab-rss-feeds-2.2.0/src/hoyolabrssfeeds/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-07-11 22:08:50.000000 hoyolab-rss-feeds-2.2.0/src/hoyolabrssfeeds/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-11 22:08:50.000000 hoyolab-rss-feeds-2.2.0/src/hoyolabrssfeeds/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-07-11 22:08:50.000000 hoyolab-rss-feeds-2.2.0/src/hoyolabrssfeeds/feeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-07-11 22:08:50.000000 hoyolab-rss-feeds-2.2.0/src/hoyolabrssfeeds/hoyolab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-07-11 22:08:50.000000 hoyolab-rss-feeds-2.2.0/src/hoyolabrssfeeds/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-11 22:08:50.000000 hoyolab-rss-feeds-2.2.0/src/hoyolabrssfeeds/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:08:50.000000 hoyolab-rss-feeds-2.2.0/src/hoyolabrssfeeds/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-07-11 22:08:50.000000 hoyolab-rss-feeds-2.2.0/src/hoyolabrssfeeds/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:09:06.855263 hoyolab-rss-feeds-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 22:08:50.000000 hoyolab-rss-feeds-2.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-07-11 22:08:50.000000 hoyolab-rss-feeds-2.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-07-11 22:08:50.000000 hoyolab-rss-feeds-2.2.0/tests/test_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10796 2023-07-11 22:08:50.000000 hoyolab-rss-feeds-2.2.0/tests/test_feeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-07-11 22:08:50.000000 hoyolab-rss-feeds-2.2.0/tests/test_hoyolab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-11 22:08:50.000000 hoyolab-rss-feeds-2.2.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-07-11 22:08:50.000000 hoyolab-rss-feeds-2.2.0/tests/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-11 22:08:50.000000 hoyolab-rss-feeds-2.2.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-11 22:08:50.000000 hoyolab-rss-feeds-2.2.0/tests/test_writers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-11 22:08:50.000000 hoyolab-rss-feeds-2.2.0/tox.ini
```

### Comparing `hoyolab-rss-feeds-2.1.1/CONTRIBUTING.md` & `hoyolab-rss-feeds-2.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hoyolab-rss-feeds-2.1.1/LICENSE` & `hoyolab-rss-feeds-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hoyolab-rss-feeds-2.1.1/PKG-INFO` & `hoyolab-rss-feeds-2.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: hoyolab-rss-feeds
-Version: 2.1.1
+Version: 2.2.0
 Summary: RSS feed generator for official game news from Hoyolab.
 Author: c3kay
 License: MIT License
 Project-URL: Homepage, https://github.com/c3kay/hoyolab-rss-feeds
 Project-URL: Tracker, https://github.com/c3kay/hoyolab-rss-feeds/issues
 Keywords: hoyolab,rss,feed,rss-generator,jsonfeed,atom,genshin-impact,honkai-impact,zenless-zone-zero
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: News/Diary
 Requires-Python: >=3.8
@@ -27,70 +28,58 @@
 [![PyPI](https://img.shields.io/pypi/v/hoyolab-rss-feeds)](https://pypi.org/project/hoyolab-rss-feeds/)
 [![Python Version](https://img.shields.io/pypi/pyversions/hoyolab-rss-feeds)](https://pypi.org/project/hoyolab-rss-feeds/)
 [![Tests Status](https://img.shields.io/github/actions/workflow/status/c3kay/hoyolab-rss-feeds/test.yaml?branch=master)](https://github.com/c3kay/hoyolab-rss-feeds/actions/workflows/test.yaml)
 [![Codecov](https://img.shields.io/codecov/c/gh/c3kay/hoyolab-rss-feeds/master)](https://app.codecov.io/gh/c3kay/hoyolab-rss-feeds)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 
-Generate RSS news feeds for games like *Genshin Impact* or *Honkai Impact 3rd* based 
-on the official [Hoyolab](https://www.hoyolab.com) forum posts. The current available 
-feed formats are [Atom](https://datatracker.ietf.org/doc/html/rfc4287) and 
-[JSON Feed](https://jsonfeed.org). This feed generator is supposed to be run
-periodically by e.g. a cronjob.
+Generate RSS news feeds for Hoyoverse games like Genshin Impact or Honkai Starrail based
+on the official [Hoyolab](https://www.hoyolab.com) forum posts. Available feed formats
+are [Atom](https://datatracker.ietf.org/doc/html/rfc4287) and [JSON Feed](https://jsonfeed.org).
+This application is supposed to run periodically by a cronjob for example.
 
-There are [some feeds](https://c3kay.de/hoyolab-rss-feeds) already hosted by myself!
+There are some [feeds](https://c3kay.de/hoyolab-rss-feeds) already hosted by myself!
 
 ## Installation
 
-You need at least Python 3.8 and the package manager Pip installed. You can then 
+You need at least Python 3.8 and the package manager Pip installed. You can then
 install this package from PyPI with:
 
 ```shell
 pip install hoyolab-rss-feeds
 ```
 
-To get the latest development version, you can also install it directly from GitHub:
-
-```shell
-pip install git+https://github.com/c3kay/hoyolab-rss-feeds.git@master
-```
-
 ## Usage
 
 ### CLI
 
-You can run the application with:
+You can run the application like this:
 
 ```shell
 hoyolab-rss-feeds
 ```
 
-or via Python with:
+or as module:
 
 ```shell
 python -m hoyolabrssfeeds
 ```
 
-The first time, when the application is started, it will create a default TOML config
-file in your current working directory (`./hoyolab-rss-feeds.toml`) and will exit 
-afterwards. You can specify a custom path for the config file via a parameter:
-
-```shell
-hoyolab-rss-feeds -c path/to/config.toml
-```
+If no configuration can be found, the application will create a default config
+in your current directory (`./hoyolab-rss-feeds.toml`) and will exit afterwards.
 
-or equivalent:
+You can specify a path for the config file with a parameter:
 
 ```shell
-python -m hoyolabrssfeeds -c path/to/config.toml
+hoyolab-rss-feeds -c path/to/config.toml
 ```
 
-### Library
+### Module
 
-It is also possible to generate the feeds directly from your Python application:
+It is also possible to generate the feeds via code:
 
 ```python
 from hoyolabrssfeeds import FeedConfigLoader, GameFeed, GameFeedCollection, Game
 
 async def generate_feeds():
     loader = FeedConfigLoader("path/to/config.toml")
     
@@ -101,53 +90,57 @@
     
     # only a single game
     genshin_config = await loader.get_feed_config(Game.GENSHIN)
     genshin_feed = GameFeed.from_config(genshin_config)
     await genshin_feed.create_feed()
 ```
 
+[Here](https://gist.github.com/c3kay/2cd9833ef1c527e210aebf7a866336ed)
+you can find an example on how to create a feed without using the TOML config file.
+
 ## Configuration
 
 In the TOML config file you can define for which games you want to create a feed
-and in which format they should be. A config file might look like this:
+and in which format the feeds should be. Here is an example config:
 
 ```toml
 language = "de-de"
 category_size = 15
 
 [genshin]
 feed.json.path = "path/to/genshin.json"
 feed.json.url = "https://example.org/genshin.json"
+category_size = 5
+categories = ["Info", "Notices"]
 title = "Genshin Impact News"
 icon = "https://example.org/icon.png"
 
-[honkai]
-feed.json.path = "path/to/honkai.json"
-feed.json.url = "https://example.org/honkai.json"
-feed.atom.path = "path/to/honkai.xml"
-feed.atom.url = "https://example.org/honkai.xml"
-category_size = 5
-```
-
-A minimal configuration requires at least one game section with a `feed.<format>.path` 
-entry. Available feed formats are currently `json` and `atom`. You can either use 
-only one format or both.
-
-Entries defined at root level are considered default values and will apply to every 
-game section. The `feed` key can only be used in a game section. All other keys 
-can be defined at root level and can be overwritten by a game section.
-
-The `category_size` entry defines the amount of feed items (default: 5) of a Hoyolab news 
-category (Info, Event and Notices) for each feed. Therefore, the maximum size of a 
-feed will be `3 * category_size`.
-
-**Note:** When using Windows file paths (like `C:\\path\to\config.toml`), you should
-use single quotes (`'`) to avoid a misinterpretation of the backslashes by the TOML 
-parser. More info about the TOML format can be found in the 
-[official documentation](https://toml.io/en/).
+[starrail]
+feed.json.path = "path/to/starrail.json"
+feed.json.url = "https://example.org/starrail.json"
+feed.atom.path = "path/to/starrail.xml"
+feed.atom.url = "https://example.org/starrail.xml"
+```
+
+A minimal configuration requires at least one game section with a `feed.<format>.path`
+entry. Available feed formats are currently `json` and `atom`. You can either use
+one format or both.
+
+Entries defined at root level are considered default values and will apply to every
+game section. The `feed` key can only be used in a game section. All other keys
+can be defined at root level and they can be overwritten by a game section.
+
+The `category_size` entry defines the amount of feed items (default: 5) of a Hoyolab
+category (*Info*, *Event* and *Notices*) for each feed. The `category` list entry 
+defines the categories selected for this feed. If this entry is omitted, all 
+categories are selected.
+
+**Note:** When using Windows file paths (like `C:\\path\to\config.toml`), single quotes
+should be used to avoid wrong auto-escaping of backslashes. More info about the TOML 
+format can be found in the [official documentation](https://toml.io/en/).
 
 ### Options
 
 #### Games
 
 | Game              | Section    |
 |-------------------|------------|
```

### Comparing `hoyolab-rss-feeds-2.1.1/README.md` & `hoyolab-rss-feeds-2.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -3,70 +3,58 @@
 [![PyPI](https://img.shields.io/pypi/v/hoyolab-rss-feeds)](https://pypi.org/project/hoyolab-rss-feeds/)
 [![Python Version](https://img.shields.io/pypi/pyversions/hoyolab-rss-feeds)](https://pypi.org/project/hoyolab-rss-feeds/)
 [![Tests Status](https://img.shields.io/github/actions/workflow/status/c3kay/hoyolab-rss-feeds/test.yaml?branch=master)](https://github.com/c3kay/hoyolab-rss-feeds/actions/workflows/test.yaml)
 [![Codecov](https://img.shields.io/codecov/c/gh/c3kay/hoyolab-rss-feeds/master)](https://app.codecov.io/gh/c3kay/hoyolab-rss-feeds)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 
-Generate RSS news feeds for games like *Genshin Impact* or *Honkai Impact 3rd* based 
-on the official [Hoyolab](https://www.hoyolab.com) forum posts. The current available 
-feed formats are [Atom](https://datatracker.ietf.org/doc/html/rfc4287) and 
-[JSON Feed](https://jsonfeed.org). This feed generator is supposed to be run
-periodically by e.g. a cronjob.
+Generate RSS news feeds for Hoyoverse games like Genshin Impact or Honkai Starrail based
+on the official [Hoyolab](https://www.hoyolab.com) forum posts. Available feed formats
+are [Atom](https://datatracker.ietf.org/doc/html/rfc4287) and [JSON Feed](https://jsonfeed.org).
+This application is supposed to run periodically by a cronjob for example.
 
-There are [some feeds](https://c3kay.de/hoyolab-rss-feeds) already hosted by myself!
+There are some [feeds](https://c3kay.de/hoyolab-rss-feeds) already hosted by myself!
 
 ## Installation
 
-You need at least Python 3.8 and the package manager Pip installed. You can then 
+You need at least Python 3.8 and the package manager Pip installed. You can then
 install this package from PyPI with:
 
 ```shell
 pip install hoyolab-rss-feeds
 ```
 
-To get the latest development version, you can also install it directly from GitHub:
-
-```shell
-pip install git+https://github.com/c3kay/hoyolab-rss-feeds.git@master
-```
-
 ## Usage
 
 ### CLI
 
-You can run the application with:
+You can run the application like this:
 
 ```shell
 hoyolab-rss-feeds
 ```
 
-or via Python with:
+or as module:
 
 ```shell
 python -m hoyolabrssfeeds
 ```
 
-The first time, when the application is started, it will create a default TOML config
-file in your current working directory (`./hoyolab-rss-feeds.toml`) and will exit 
-afterwards. You can specify a custom path for the config file via a parameter:
-
-```shell
-hoyolab-rss-feeds -c path/to/config.toml
-```
+If no configuration can be found, the application will create a default config
+in your current directory (`./hoyolab-rss-feeds.toml`) and will exit afterwards.
 
-or equivalent:
+You can specify a path for the config file with a parameter:
 
 ```shell
-python -m hoyolabrssfeeds -c path/to/config.toml
+hoyolab-rss-feeds -c path/to/config.toml
 ```
 
-### Library
+### Module
 
-It is also possible to generate the feeds directly from your Python application:
+It is also possible to generate the feeds via code:
 
 ```python
 from hoyolabrssfeeds import FeedConfigLoader, GameFeed, GameFeedCollection, Game
 
 async def generate_feeds():
     loader = FeedConfigLoader("path/to/config.toml")
     
@@ -77,53 +65,57 @@
     
     # only a single game
     genshin_config = await loader.get_feed_config(Game.GENSHIN)
     genshin_feed = GameFeed.from_config(genshin_config)
     await genshin_feed.create_feed()
 ```
 
+[Here](https://gist.github.com/c3kay/2cd9833ef1c527e210aebf7a866336ed)
+you can find an example on how to create a feed without using the TOML config file.
+
 ## Configuration
 
 In the TOML config file you can define for which games you want to create a feed
-and in which format they should be. A config file might look like this:
+and in which format the feeds should be. Here is an example config:
 
 ```toml
 language = "de-de"
 category_size = 15
 
 [genshin]
 feed.json.path = "path/to/genshin.json"
 feed.json.url = "https://example.org/genshin.json"
+category_size = 5
+categories = ["Info", "Notices"]
 title = "Genshin Impact News"
 icon = "https://example.org/icon.png"
 
-[honkai]
-feed.json.path = "path/to/honkai.json"
-feed.json.url = "https://example.org/honkai.json"
-feed.atom.path = "path/to/honkai.xml"
-feed.atom.url = "https://example.org/honkai.xml"
-category_size = 5
-```
-
-A minimal configuration requires at least one game section with a `feed.<format>.path` 
-entry. Available feed formats are currently `json` and `atom`. You can either use 
-only one format or both.
-
-Entries defined at root level are considered default values and will apply to every 
-game section. The `feed` key can only be used in a game section. All other keys 
-can be defined at root level and can be overwritten by a game section.
-
-The `category_size` entry defines the amount of feed items (default: 5) of a Hoyolab news 
-category (Info, Event and Notices) for each feed. Therefore, the maximum size of a 
-feed will be `3 * category_size`.
-
-**Note:** When using Windows file paths (like `C:\\path\to\config.toml`), you should
-use single quotes (`'`) to avoid a misinterpretation of the backslashes by the TOML 
-parser. More info about the TOML format can be found in the 
-[official documentation](https://toml.io/en/).
+[starrail]
+feed.json.path = "path/to/starrail.json"
+feed.json.url = "https://example.org/starrail.json"
+feed.atom.path = "path/to/starrail.xml"
+feed.atom.url = "https://example.org/starrail.xml"
+```
+
+A minimal configuration requires at least one game section with a `feed.<format>.path`
+entry. Available feed formats are currently `json` and `atom`. You can either use
+one format or both.
+
+Entries defined at root level are considered default values and will apply to every
+game section. The `feed` key can only be used in a game section. All other keys
+can be defined at root level and they can be overwritten by a game section.
+
+The `category_size` entry defines the amount of feed items (default: 5) of a Hoyolab
+category (*Info*, *Event* and *Notices*) for each feed. The `category` list entry 
+defines the categories selected for this feed. If this entry is omitted, all 
+categories are selected.
+
+**Note:** When using Windows file paths (like `C:\\path\to\config.toml`), single quotes
+should be used to avoid wrong auto-escaping of backslashes. More info about the TOML 
+format can be found in the [official documentation](https://toml.io/en/).
 
 ### Options
 
 #### Games
 
 | Game              | Section    |
 |-------------------|------------|
```

### Comparing `hoyolab-rss-feeds-2.1.1/pyproject.toml` & `hoyolab-rss-feeds-2.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -21,50 +21,52 @@
     "zenless-zone-zero"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Intended Audience :: System Administrators",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content :: News/Diary"
 ]
 dependencies = [
-    "aiohttp >= 3.8.3",
-    "aiofiles >= 22.1.0",
-    "pydantic >= 1.10.2",
-    "tomli >= 2.0.1"
+    "aiohttp >= 3.8.4",
+    "aiofiles >= 23.1.0",
+    "pydantic >= 1.10.11, < 2",
+    'tomli >= 2.0.1 ; python_version < "3.11"'
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
-    "tox >= 3.26.0",
-    "pytest >= 7.1.3",
-    "pytest-asyncio >= 0.20.1",
-    "pytest-cov >= 4.0.0",
-    "pytest-mock >= 3.10.0",
+    "tox >= 4.6.4",
+    "pytest >= 7.4.0",
+    "pytest-asyncio >= 0.21.0",
+    "pytest-cov >= 4.1.0",
+    "pytest-mock >= 3.11.1",
     "atoma >= 0.0.17",
     "langdetect >= 1.0.9"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/c3kay/hoyolab-rss-feeds"
 "Tracker" = "https://github.com/c3kay/hoyolab-rss-feeds/issues"
 
 [project.scripts]
 hoyolab-rss-feeds = "hoyolabrssfeeds.__main__:cli"
 
 # infer version from git
 [tool.setuptools_scm]
 local_scheme = "no-local-version"
+version_scheme = "python-simplified-semver"
 
 [tool.pytest.ini_options]
 addopts = "-vv --cov --cov-append --cov-report=xml --cov-report=term-missing"
 asyncio_mode = "auto"
 testpaths = ["tests"]
 markers = ["hoyolabapi: marker for hoyolab api tests"]
```

### Comparing `hoyolab-rss-feeds-2.1.1/src/hoyolab_rss_feeds.egg-info/PKG-INFO` & `hoyolab-rss-feeds-2.2.0/src/hoyolab_rss_feeds.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: hoyolab-rss-feeds
-Version: 2.1.1
+Version: 2.2.0
 Summary: RSS feed generator for official game news from Hoyolab.
 Author: c3kay
 License: MIT License
 Project-URL: Homepage, https://github.com/c3kay/hoyolab-rss-feeds
 Project-URL: Tracker, https://github.com/c3kay/hoyolab-rss-feeds/issues
 Keywords: hoyolab,rss,feed,rss-generator,jsonfeed,atom,genshin-impact,honkai-impact,zenless-zone-zero
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: News/Diary
 Requires-Python: >=3.8
@@ -27,70 +28,58 @@
 [![PyPI](https://img.shields.io/pypi/v/hoyolab-rss-feeds)](https://pypi.org/project/hoyolab-rss-feeds/)
 [![Python Version](https://img.shields.io/pypi/pyversions/hoyolab-rss-feeds)](https://pypi.org/project/hoyolab-rss-feeds/)
 [![Tests Status](https://img.shields.io/github/actions/workflow/status/c3kay/hoyolab-rss-feeds/test.yaml?branch=master)](https://github.com/c3kay/hoyolab-rss-feeds/actions/workflows/test.yaml)
 [![Codecov](https://img.shields.io/codecov/c/gh/c3kay/hoyolab-rss-feeds/master)](https://app.codecov.io/gh/c3kay/hoyolab-rss-feeds)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 
-Generate RSS news feeds for games like *Genshin Impact* or *Honkai Impact 3rd* based 
-on the official [Hoyolab](https://www.hoyolab.com) forum posts. The current available 
-feed formats are [Atom](https://datatracker.ietf.org/doc/html/rfc4287) and 
-[JSON Feed](https://jsonfeed.org). This feed generator is supposed to be run
-periodically by e.g. a cronjob.
+Generate RSS news feeds for Hoyoverse games like Genshin Impact or Honkai Starrail based
+on the official [Hoyolab](https://www.hoyolab.com) forum posts. Available feed formats
+are [Atom](https://datatracker.ietf.org/doc/html/rfc4287) and [JSON Feed](https://jsonfeed.org).
+This application is supposed to run periodically by a cronjob for example.
 
-There are [some feeds](https://c3kay.de/hoyolab-rss-feeds) already hosted by myself!
+There are some [feeds](https://c3kay.de/hoyolab-rss-feeds) already hosted by myself!
 
 ## Installation
 
-You need at least Python 3.8 and the package manager Pip installed. You can then 
+You need at least Python 3.8 and the package manager Pip installed. You can then
 install this package from PyPI with:
 
 ```shell
 pip install hoyolab-rss-feeds
 ```
 
-To get the latest development version, you can also install it directly from GitHub:
-
-```shell
-pip install git+https://github.com/c3kay/hoyolab-rss-feeds.git@master
-```
-
 ## Usage
 
 ### CLI
 
-You can run the application with:
+You can run the application like this:
 
 ```shell
 hoyolab-rss-feeds
 ```
 
-or via Python with:
+or as module:
 
 ```shell
 python -m hoyolabrssfeeds
 ```
 
-The first time, when the application is started, it will create a default TOML config
-file in your current working directory (`./hoyolab-rss-feeds.toml`) and will exit 
-afterwards. You can specify a custom path for the config file via a parameter:
-
-```shell
-hoyolab-rss-feeds -c path/to/config.toml
-```
+If no configuration can be found, the application will create a default config
+in your current directory (`./hoyolab-rss-feeds.toml`) and will exit afterwards.
 
-or equivalent:
+You can specify a path for the config file with a parameter:
 
 ```shell
-python -m hoyolabrssfeeds -c path/to/config.toml
+hoyolab-rss-feeds -c path/to/config.toml
 ```
 
-### Library
+### Module
 
-It is also possible to generate the feeds directly from your Python application:
+It is also possible to generate the feeds via code:
 
 ```python
 from hoyolabrssfeeds import FeedConfigLoader, GameFeed, GameFeedCollection, Game
 
 async def generate_feeds():
     loader = FeedConfigLoader("path/to/config.toml")
     
@@ -101,53 +90,57 @@
     
     # only a single game
     genshin_config = await loader.get_feed_config(Game.GENSHIN)
     genshin_feed = GameFeed.from_config(genshin_config)
     await genshin_feed.create_feed()
 ```
 
+[Here](https://gist.github.com/c3kay/2cd9833ef1c527e210aebf7a866336ed)
+you can find an example on how to create a feed without using the TOML config file.
+
 ## Configuration
 
 In the TOML config file you can define for which games you want to create a feed
-and in which format they should be. A config file might look like this:
+and in which format the feeds should be. Here is an example config:
 
 ```toml
 language = "de-de"
 category_size = 15
 
 [genshin]
 feed.json.path = "path/to/genshin.json"
 feed.json.url = "https://example.org/genshin.json"
+category_size = 5
+categories = ["Info", "Notices"]
 title = "Genshin Impact News"
 icon = "https://example.org/icon.png"
 
-[honkai]
-feed.json.path = "path/to/honkai.json"
-feed.json.url = "https://example.org/honkai.json"
-feed.atom.path = "path/to/honkai.xml"
-feed.atom.url = "https://example.org/honkai.xml"
-category_size = 5
-```
-
-A minimal configuration requires at least one game section with a `feed.<format>.path` 
-entry. Available feed formats are currently `json` and `atom`. You can either use 
-only one format or both.
-
-Entries defined at root level are considered default values and will apply to every 
-game section. The `feed` key can only be used in a game section. All other keys 
-can be defined at root level and can be overwritten by a game section.
-
-The `category_size` entry defines the amount of feed items (default: 5) of a Hoyolab news 
-category (Info, Event and Notices) for each feed. Therefore, the maximum size of a 
-feed will be `3 * category_size`.
-
-**Note:** When using Windows file paths (like `C:\\path\to\config.toml`), you should
-use single quotes (`'`) to avoid a misinterpretation of the backslashes by the TOML 
-parser. More info about the TOML format can be found in the 
-[official documentation](https://toml.io/en/).
+[starrail]
+feed.json.path = "path/to/starrail.json"
+feed.json.url = "https://example.org/starrail.json"
+feed.atom.path = "path/to/starrail.xml"
+feed.atom.url = "https://example.org/starrail.xml"
+```
+
+A minimal configuration requires at least one game section with a `feed.<format>.path`
+entry. Available feed formats are currently `json` and `atom`. You can either use
+one format or both.
+
+Entries defined at root level are considered default values and will apply to every
+game section. The `feed` key can only be used in a game section. All other keys
+can be defined at root level and they can be overwritten by a game section.
+
+The `category_size` entry defines the amount of feed items (default: 5) of a Hoyolab
+category (*Info*, *Event* and *Notices*) for each feed. The `category` list entry 
+defines the categories selected for this feed. If this entry is omitted, all 
+categories are selected.
+
+**Note:** When using Windows file paths (like `C:\\path\to\config.toml`), single quotes
+should be used to avoid wrong auto-escaping of backslashes. More info about the TOML 
+format can be found in the [official documentation](https://toml.io/en/).
 
 ### Options
 
 #### Games
 
 | Game              | Section    |
 |-------------------|------------|
```

### Comparing `hoyolab-rss-feeds-2.1.1/src/hoyolab_rss_feeds.egg-info/SOURCES.txt` & `hoyolab-rss-feeds-2.2.0/src/hoyolab_rss_feeds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hoyolab-rss-feeds-2.1.1/src/hoyolabrssfeeds/__init__.py` & `hoyolab-rss-feeds-2.2.0/src/hoyolabrssfeeds/__init__.py`

 * *Files identical despite different names*

### Comparing `hoyolab-rss-feeds-2.1.1/src/hoyolabrssfeeds/__main__.py` & `hoyolab-rss-feeds-2.2.0/src/hoyolabrssfeeds/__main__.py`

 * *Files identical despite different names*

### Comparing `hoyolab-rss-feeds-2.1.1/src/hoyolabrssfeeds/configs.py` & `hoyolab-rss-feeds-2.2.0/src/hoyolabrssfeeds/configs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 from pathlib import Path
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 
 import aiofiles
-import tomli
 import pydantic
 
+try:
+    import tomllib as toml
+except ImportError:
+    import tomli as toml  # type: ignore
+
 from .errors import ConfigIOError
 from .errors import ConfigFormatError
 from .models import FeedConfig
 from .models import FeedFileWriterConfig
+from .models import FeedItemCategory
 from .models import FeedMeta
 from .models import Game
 
 
 class FeedConfigLoader:
     """TOML config file loader."""
 
@@ -30,20 +35,20 @@
     async def _load_from_file(self) -> Dict[str, Any]:
         """Load and parse config from TOML file."""
 
         try:
             async with aiofiles.open(self._path, "r") as fd:
                 conf_str = await fd.read()
 
-            config: Dict[str, Any] = tomli.loads(conf_str)
+            config: Dict[str, Any] = toml.loads(conf_str)
         except IOError as err:
             raise ConfigIOError(
                 'Could not open config file at "{}"!'.format(self._path)
             ) from err
-        except tomli.TOMLDecodeError as err:
+        except toml.TOMLDecodeError as err:
             raise ConfigFormatError("Could not parse TOML config file!") from err
 
         if not any([game.name.lower() in config for game in Game]):
             raise ConfigFormatError("Could not find any game configs!")
 
         return config
 
@@ -65,19 +70,27 @@
             feed_config_dict = game_config_dict.pop("feed")
 
             writer_configs = [
                 FeedFileWriterConfig(feed_type=feed_type, **feed_config)
                 for feed_type, feed_config in feed_config_dict.items()
             ]
 
+            if "categories" in game_config_dict:
+                game_config_dict["categories"] = list(
+                    map(
+                        lambda cat: FeedItemCategory.from_str(cat),
+                        game_config_dict["categories"],
+                    )
+                )
+
             feed_meta = FeedMeta(game=game, **game_config_dict)
             feed_config = FeedConfig(feed_meta=feed_meta, writer_configs=writer_configs)
         except KeyError as err:
             raise ConfigFormatError("Could not find required key in config!") from err
-        except pydantic.ValidationError as err:
+        except (pydantic.ValidationError, ValueError) as err:
             raise ConfigFormatError("Invalid config value!") from err
 
         return feed_config
 
     async def get_feed_config(self, game: Game) -> FeedConfig:
         """Load and create a feed config for a given game."""
```

### Comparing `hoyolab-rss-feeds-2.1.1/src/hoyolabrssfeeds/errors.py` & `hoyolab-rss-feeds-2.2.0/src/hoyolabrssfeeds/errors.py`

 * *Files identical despite different names*

### Comparing `hoyolab-rss-feeds-2.1.1/src/hoyolabrssfeeds/feeds.py` & `hoyolab-rss-feeds-2.2.0/src/hoyolabrssfeeds/feeds.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,25 +25,29 @@
 class GameFeed:
     """Feed generator for a single game."""
 
     def __init__(
         self,
         feed_meta: FeedMeta,
         feed_writers: List[AbstractFeedFileWriter],
-        feed_loader: AbstractFeedFileLoader,
+        feed_loader: Optional[AbstractFeedFileLoader] = None,
     ) -> None:
         # warn if identical paths for writers are found
         writer_paths = [str(writer.config.path) for writer in feed_writers]
         if len(writer_paths) != len(set(writer_paths)):
             warnings.warn(
                 "Writers for {} game feed contain identical paths".format(
                     feed_meta.game.name.title()
                 )
             )
 
+        if feed_loader is None:
+            loader_factory = FeedFileLoaderFactory()
+            feed_loader = loader_factory.create_any_loader(feed_writers)
+
         self._feed_meta = feed_meta
         self._feed_writers = feed_writers
         self._feed_loader = feed_loader
         self._hoyolab = HoyolabNews(feed_meta.game, feed_meta.language)
         self._was_updated = False
 
     @property
@@ -72,27 +76,28 @@
 
     async def create_feed(
         self, session: Optional[aiohttp.ClientSession] = None
     ) -> None:
         """Create or update a feed and write it to files."""
 
         local_session = session or aiohttp.ClientSession()
+        feed_categories = self._feed_meta.categories or [c for c in FeedItemCategory]
         self._was_updated = False
 
         feed_items = await self._feed_loader.get_feed_items()
 
         try:
             category_feeds = await asyncio.gather(
                 *[
                     self._update_category_feed(
                         local_session,
                         category,
                         [item for item in feed_items if item.category == category],
                     )
-                    for category in FeedItemCategory
+                    for category in feed_categories
                 ]
             )
         finally:
             if session is None:
                 await local_session.close()
 
         if self._was_updated:
@@ -164,47 +169,49 @@
 class GameFeedCollection:
     """Collection of feed generators for multiple games."""
 
     def __init__(
         self,
         feed_metas: List[FeedMeta],
         feed_writers: List[List[AbstractFeedFileWriter]],
-        feed_loaders: List[AbstractFeedFileLoader],
+        feed_loaders: List[Optional[AbstractFeedFileLoader]],
     ) -> None:
         if not (len(feed_metas) == len(feed_writers) == len(feed_loaders)):
             raise ValueError("Parameter lists do not have the same length!")
 
         self._game_feeds = [
             GameFeed(meta, writer, loader)
             for meta, writer, loader in zip(feed_metas, feed_writers, feed_loaders)
         ]
 
     @classmethod
     def from_configs(cls: Type[_GFC], feed_configs: List[FeedConfig]) -> _GFC:
         """Create an instance via feed configs."""
 
-        metas = []
-        writers = []
-        loaders = []
+        metas: List[FeedMeta] = []
+        writers: List[List[AbstractFeedFileWriter]] = []
+        loaders: List[Optional[AbstractFeedFileLoader]] = []
 
         for feed_config in feed_configs:
             metas.append(feed_config.feed_meta)
 
             writer_factory = FeedFileWriterFactory()
             writers_configs = [
                 writer_factory.create_writer(conf)
                 for conf in feed_config.writer_configs
             ]
             writers.append(writers_configs)
 
             loader_factory = FeedFileLoaderFactory()
-            if feed_config.loader_config:
-                loaders.append(loader_factory.create_loader(feed_config.loader_config))
-            else:
-                loaders.append(loader_factory.create_any_loader(writers_configs))
+            loader = (
+                loader_factory.create_loader(feed_config.loader_config)
+                if feed_config.loader_config
+                else None
+            )
+            loaders.append(loader)
 
         return cls(metas, writers, loaders)
 
     async def create_feeds(
         self, session: Optional[aiohttp.ClientSession] = None
     ) -> None:
         """Create or update a feed and write it to files."""
```

### Comparing `hoyolab-rss-feeds-2.1.1/src/hoyolabrssfeeds/hoyolab.py` & `hoyolab-rss-feeds-2.2.0/src/hoyolabrssfeeds/hoyolab.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,17 @@
         url: pydantic.HttpUrl,
     ) -> Dict[str, Any]:
         """Send a GET request to the Hoyolab API endpoint."""
 
         headers = {"Origin": "https://www.hoyolab.com", "X-Rpc-Language": self._lang}
 
         try:
-            async with session.get(url, headers=headers, params=params) as response:
+            async with session.get(
+                str(url), headers=headers, params=params
+            ) as response:
                 response.raise_for_status()
                 response_json: Dict[str, Any] = await response.json()
 
             if response_json["retcode"] != 0:
                 # the message might be in chinese
                 raise HoyolabApiError(response_json["message"])
         except aiohttp.ContentTypeError as err:
```

### Comparing `hoyolab-rss-feeds-2.1.1/src/hoyolabrssfeeds/loaders.py` & `hoyolab-rss-feeds-2.2.0/src/hoyolabrssfeeds/loaders.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,22 +101,22 @@
                     if "date_modified" in item:
                         item_dict["updated"] = item["date_modified"]
 
                     if "image" in item:
                         item_dict["image"] = item["image"]
 
                     feed_items.append(item_dict)
-
-                return pydantic.parse_obj_as(List[FeedItem], feed_items)
             except KeyError as err:
                 raise FeedFormatError(
                     "Could not find required key in JSON feed!"
                 ) from err
             except ValueError as err:
                 raise FeedFormatError("Could not load JSON feed items!") from err
+
+            return pydantic.parse_obj_as(List[FeedItem], feed_items)
         else:
             return []
 
     async def _load_from_file(self) -> Dict[str, Any]:
         """Load JSON-Feed from file."""
 
         try:
```

### Comparing `hoyolab-rss-feeds-2.1.1/src/hoyolabrssfeeds/models.py` & `hoyolab-rss-feeds-2.2.0/src/hoyolabrssfeeds/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     JSON = "json"
     ATOM = "atom"
 
     def __str__(self) -> str:  # pragma: no cover
         return self.value
 
 
+@unique
 class Language(str, Enum):
     GERMAN = "de-de"
     ENGLISH = "en-us"
     SPANISH = "es-es"
     FRENCH = "fr-fr"
     INDONESIAN = "id-id"
     ITALIAN = "it-it"
@@ -88,14 +89,15 @@
         anystr_strip_whitespace = True
         min_anystr_length = 1
 
 
 class FeedMeta(MyBaseModel):
     game: Game
     category_size: int = 5
+    categories: List[FeedItemCategory] = [c for c in FeedItemCategory]
     language: Language = Language.ENGLISH
     title: Optional[str] = None
     icon: Optional[HttpUrl] = None
 
 
 class FeedItem(MyBaseModel):
     id: int
```

### Comparing `hoyolab-rss-feeds-2.1.1/src/hoyolabrssfeeds/writers.py` & `hoyolab-rss-feeds-2.2.0/src/hoyolabrssfeeds/writers.py`

 * *Files identical despite different names*

### Comparing `hoyolab-rss-feeds-2.1.1/tests/conftest.py` & `hoyolab-rss-feeds-2.2.0/tests/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,25 @@
 
 @pytest.fixture(scope="session")
 def event_loop():
     if system() == "Windows":
         # default policy not working on windows
         asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
 
-    return asyncio.get_event_loop()
+    loop = asyncio.get_event_loop()
+
+    yield loop
+
+    pending = asyncio.tasks.all_tasks(loop)
+    loop.run_until_complete(asyncio.gather(*pending))
+    loop.run_until_complete(asyncio.sleep(1))
+
+    loop.close()
+
+    # https://stackoverflow.com/questions/65740542/exception-ignored-runtimeerror-event-loop-is-closed-when-using-pytest-asynci
 
 
 @pytest.fixture(scope="session")
 async def client_session(event_loop):
     async with aiohttp.ClientSession(loop=event_loop, raise_for_status=True) as cs:
         yield cs
 
@@ -147,15 +157,16 @@
             "icon": str(feed_meta.icon),
         },
         models.Game.ZENLESS.name.lower(): {
             "feed": {
                 str(models.FeedType.ATOM): {
                     "path": str(atom_feed_file_writer_config.path)
                 }
-            }
+            },
+            "categories": [models.FeedItemCategory.EVENTS.name.lower()],
         },
     }
 
 
 # ---- FEED FIXTURES ----
 
 
@@ -231,14 +242,15 @@
 
 
 @pytest.fixture
 def feed_meta() -> models.FeedMeta:
     return models.FeedMeta(
         game=models.Game.GENSHIN,
         category_size=1,
+        categories=[c for c in models.FeedItemCategory],
         language=models.Language.GERMAN,
         title="Example Feed",
         icon=pydantic.parse_obj_as(pydantic.HttpUrl, "https://example.org/"),
     )
 
 
 @pytest.fixture
```

### Comparing `hoyolab-rss-feeds-2.1.1/tests/test_configs.py` & `hoyolab-rss-feeds-2.2.0/tests/test_configs.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 from stat import S_IWRITE
 from stat import S_IREAD
 from typing import Dict
 
 import aiofiles
 import pytest
 import pytest_mock
-import tomli
+
+try:
+    import tomllib as toml
+except ImportError:
+    import tomli as toml  # type: ignore
 
 from hoyolabrssfeeds import configs
 from hoyolabrssfeeds import errors
 from hoyolabrssfeeds import models
 
 
 def test_config_paths(config_path: Path):
@@ -64,15 +68,15 @@
     await loader.create_default_config_file()
 
     assert config_path.exists()
 
     async with aiofiles.open(config_path, "r") as fd:
         toml_str = await fd.read()
 
-    default_config = tomli.loads(toml_str)
+    default_config = toml.loads(toml_str)
 
     expected = {
         "genshin": {"feed": {"json": {"path": "genshin.json"}}},
     }
 
     assert default_config == expected
```

### Comparing `hoyolab-rss-feeds-2.1.1/tests/test_feeds.py` & `hoyolab-rss-feeds-2.2.0/tests/test_feeds.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,36 +31,46 @@
     writer = JSONFeedFileWriter(json_feed_file_writer_config)
     duplicate_writers = [writer, writer]
 
     with pytest.warns(UserWarning, match="identical paths"):
         feeds.GameFeed(feed_meta, duplicate_writers, mocked_loader)
 
 
-def test_create_from_config(feed_config: models.FeedConfig):
+def test_from_config(feed_config: models.FeedConfig):
     game_feed = feeds.GameFeed.from_config(feed_config)
 
     assert game_feed._feed_meta == feed_config.feed_meta
 
     for writer in game_feed._feed_writers:
         assert issubclass(type(writer), AbstractFeedFileWriter)
 
     writer_configs = [writer.config for writer in game_feed._feed_writers]
     assert writer_configs == feed_config.writer_configs
 
     assert issubclass(type(game_feed._feed_loader), AbstractFeedFileLoader)
     assert game_feed._feed_loader.config == feed_config.loader_config
 
 
-def test_create_from_config_no_loader(feed_config_no_loader: models.FeedConfig):
+def test_from_config_no_loader(feed_config_no_loader: models.FeedConfig):
     game_feed = feeds.GameFeed.from_config(feed_config_no_loader)
 
     assert game_feed._feed_loader is not None
     assert issubclass(type(game_feed._feed_loader), AbstractFeedFileLoader)
 
 
+def test_init_no_loader(
+    feed_meta: models.FeedMeta,
+    json_feed_file_writer_config: models.FeedFileWriterConfig,
+):
+    writers = [JSONFeedFileWriter(json_feed_file_writer_config)]
+    game_feed = feeds.GameFeed(feed_meta, writers)
+
+    assert game_feed._feed_loader.config.feed_type == models.FeedType.JSON
+
+
 async def test_category_feed_new_item(
     mocker: pytest_mock.MockFixture,
     client_session: aiohttp.ClientSession,
     feed_meta: models.FeedMeta,
     mocked_writers: List[MagicMock],
     mocked_loader: MagicMock,
     feed_item: models.FeedItem,
@@ -256,15 +266,50 @@
     mocked_update_feed.assert_awaited()
     mocked_update_feed.assert_called()
 
     for writer in mocked_writers:
         writer.write_feed.assert_not_called()
 
 
-def test_create_collection_from_config(
+async def test_create_feed_one_category(
+    mocker: pytest_mock.MockFixture,
+    client_session: aiohttp.ClientSession,
+    feed_meta: models.FeedMeta,
+    feed_item: models.FeedItem,
+    mocked_writers: List[MagicMock],
+    mocked_loader: MagicMock,
+):
+    feed_meta.categories = [feed_item.category]
+
+    mocked_update_feed = mocker.patch(
+        "hoyolabrssfeeds.feeds.GameFeed._update_category_feed",
+        spec=True,
+        return_value=[feed_item],
+    )
+
+    # needed for writers to trigger
+    mocker.patch(
+        "hoyolabrssfeeds.feeds.GameFeed._was_updated",
+        new_callable=mocker.PropertyMock,
+        create=True,
+        return_value=True,
+    )
+
+    game_feed = feeds.GameFeed(feed_meta, mocked_writers, mocked_loader)
+
+    await game_feed.create_feed(client_session)
+
+    mocked_update_feed.assert_awaited()
+    mocked_update_feed.assert_called_once()
+
+    for writer in mocked_writers:
+        writer.write_feed.assert_called_with(feed_meta, [feed_item])
+
+
+def test_collection_from_config(
     feed_config: models.FeedConfig, feed_config_no_loader: models.FeedConfig
 ):
     # NOTE: there is currently no check for identical paths of multiple game feeds
     configs = [feed_config, feed_config_no_loader]
 
     collection = feeds.GameFeedCollection.from_configs(configs)
```

### Comparing `hoyolab-rss-feeds-2.1.1/tests/test_hoyolab.py` & `hoyolab-rss-feeds-2.2.0/tests/test_hoyolab.py`

 * *Files identical despite different names*

### Comparing `hoyolab-rss-feeds-2.1.1/tests/test_integration.py` & `hoyolab-rss-feeds-2.2.0/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `hoyolab-rss-feeds-2.1.1/tests/test_loaders.py` & `hoyolab-rss-feeds-2.2.0/tests/test_loaders.py`

 * *Files identical despite different names*

### Comparing `hoyolab-rss-feeds-2.1.1/tests/test_models.py` & `hoyolab-rss-feeds-2.2.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `hoyolab-rss-feeds-2.1.1/tests/test_writers.py` & `hoyolab-rss-feeds-2.2.0/tests/test_writers.py`

 * *Files identical despite different names*

### Comparing `hoyolab-rss-feeds-2.1.1/tox.ini` & `hoyolab-rss-feeds-2.2.0/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [tox]
 isolated_build = True
 skip_missing_interpreters = True
-envlist = clean, black, flake, type, py38, py39, py310
+envlist = clean, black, flake, type, py38, py39, py310, py311
 
 [gh-actions]
 python =
     3.8: py38
     3.9: py39
     3.10: py310
+    3.11: py311
 
 [testenv]
 deps =
     pytest >= 7.1.3
     pytest-asyncio >= 0.20.1
     pytest-cov >= 4.0.0
     pytest-mock >= 3.10.0
```


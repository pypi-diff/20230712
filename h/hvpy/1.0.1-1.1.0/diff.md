# Comparing `tmp/hvpy-1.0.1.tar.gz` & `tmp/hvpy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hvpy-1.0.1.tar", last modified: Wed Oct 19 16:42:10 2022, max compression
+gzip compressed data, was "hvpy-1.1.0.tar", last modified: Wed Jul 12 13:12:43 2023, max compression
```

## Comparing `hvpy-1.0.1.tar` & `hvpy-1.1.0.tar`

### file list

```diff
@@ -1,108 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 16:42:10.123768 hvpy-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 16:42:10.115768 hvpy-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 16:42:10.119768 hvpy-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1655 2022-10-19 16:41:47.000000 hvpy-1.0.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1924 2022-10-19 16:41:47.000000 hvpy-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1291 2022-10-19 16:41:47.000000 hvpy-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      309 2022-10-19 16:41:47.000000 hvpy-1.0.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1329 2022-10-19 16:41:47.000000 hvpy-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1713 2022-10-19 16:42:10.123768 hvpy-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      781 2022-10-19 16:41:47.000000 hvpy-1.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 16:42:10.119768 hvpy-1.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-10-19 16:41:47.000000 hvpy-1.0.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      413 2022-10-19 16:41:47.000000 hvpy-1.0.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2175 2022-10-19 16:41:47.000000 hvpy-1.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     3885 2022-10-19 16:41:47.000000 hvpy-1.0.1/docs/dev_guide.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3296 2022-10-19 16:41:47.000000 hvpy-1.0.1/docs/guide.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1245 2022-10-19 16:41:47.000000 hvpy-1.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1502 2022-10-19 16:41:47.000000 hvpy-1.0.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)      760 2022-10-19 16:41:47.000000 hvpy-1.0.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-10-19 16:41:47.000000 hvpy-1.0.1/docs/nitpick-exceptions
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 16:42:10.119768 hvpy-1.0.1/hvpy/
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 16:42:10.119768 hvpy-1.0.1/hvpy/api_groups/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/api_groups/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 16:42:10.119768 hvpy-1.0.1/hvpy/api_groups/communications/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/api_groups/communications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      711 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/api_groups/communications/get_news_feed.py
--rw-r--r--   0 runner    (1001) docker     (121)      852 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/api_groups/communications/shorten_url.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 16:42:10.119768 hvpy-1.0.1/hvpy/api_groups/communications/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/api_groups/communications/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      476 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/api_groups/communications/tests/test_get_news_feed.py
--rw-r--r--   0 runner    (1001) docker     (121)      791 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/api_groups/communications/tests/test_shorten_url.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 16:42:10.119768 hvpy-1.0.1/hvpy/api_groups/jpeg2000/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/api_groups/jpeg2000/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      770 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/api_groups/jpeg2000/get_jp2_header.py
--rw-r--r--   0 runner    (1001) docker     (121)     1507 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/api_groups/jpeg2000/get_jp2_image.py
--rw-r--r--   0 runner    (1001) docker     (121)     2245 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/api_groups/jpeg2000/get_jpx.py
--rw-r--r--   0 runner    (1001) docker     (121)     2114 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/api_groups/jpeg2000/get_jpx_closest_to_mid_point.py
--rw-r--r--   0 runner    (1001) docker     (121)      473 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/api_groups/jpeg2000/get_status.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 16:42:10.123768 hvpy-1.0.1/hvpy/api_groups/jpeg2000/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/api_groups/jpeg2000/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      793 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/api_groups/jpeg2000/tests/test_get_jp2_header.py
--rw-r--r--   0 runner    (1001) docker     (121)     1442 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/api_groups/jpeg2000/tests/test_get_jp2_image.py
--rw-r--r--   0 runner    (1001) docker     (121)     2095 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/api_groups/jpeg2000/tests/test_get_jpx.py
--rw-r--r--   0 runner    (1001) docker     (121)     2232 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/api_groups/jpeg2000/tests/test_get_jpx_closest_to_mid_point.py
--rw-r--r--   0 runner    (1001) docker     (121)      345 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/api_groups/jpeg2000/tests/test_get_status.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 16:42:10.123768 hvpy-1.0.1/hvpy/api_groups/movies/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/api_groups/movies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      856 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/api_groups/movies/download_movie.py
--rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/api_groups/movies/get_movie_status.py
--rw-r--r--   0 runner    (1001) docker     (121)     5406 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/api_groups/movies/queue_movie.py
--rw-r--r--   0 runner    (1001) docker     (121)      746 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/api_groups/movies/re_queue_movie.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 16:42:10.123768 hvpy-1.0.1/hvpy/api_groups/movies/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/api_groups/movies/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      793 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/api_groups/movies/tests/test_download_movie.py
--rw-r--r--   0 runner    (1001) docker     (121)     1184 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/api_groups/movies/tests/test_get_movie_status.py
--rw-r--r--   0 runner    (1001) docker     (121)     1283 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/api_groups/movies/tests/test_queue_movie.py
--rw-r--r--   0 runner    (1001) docker     (121)     1061 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/api_groups/movies/tests/test_re_queue_movie.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 16:42:10.123768 hvpy-1.0.1/hvpy/api_groups/official_clients/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/api_groups/official_clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1304 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/api_groups/official_clients/get_closest_image.py
--rw-r--r--   0 runner    (1001) docker     (121)     1184 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/api_groups/official_clients/get_data_sources.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 16:42:10.123768 hvpy-1.0.1/hvpy/api_groups/official_clients/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/api_groups/official_clients/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      969 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/api_groups/official_clients/tests/test_get_closest_image.py
--rw-r--r--   0 runner    (1001) docker     (121)      440 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/api_groups/official_clients/tests/test_get_data_sources.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 16:42:10.123768 hvpy-1.0.1/hvpy/api_groups/screenshots/
--rw-r--r--   0 runner    (1001) docker     (121)      650 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/api_groups/screenshots/download_screenshot.py
--rw-r--r--   0 runner    (1001) docker     (121)     1858 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/api_groups/screenshots/get_tile.py
--rw-r--r--   0 runner    (1001) docker     (121)     4496 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/api_groups/screenshots/take_screenshot.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 16:42:10.123768 hvpy-1.0.1/hvpy/api_groups/screenshots/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      573 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/api_groups/screenshots/tests/test_download_screenshot.py
--rw-r--r--   0 runner    (1001) docker     (121)     1247 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/api_groups/screenshots/tests/test_get_tile.py
--rw-r--r--   0 runner    (1001) docker     (121)     1553 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/api_groups/screenshots/tests/test_take_screenshot.py
--rw-r--r--   0 runner    (1001) docker     (121)      604 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      977 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1409 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     8991 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/datasource.py
--rw-r--r--   0 runner    (1001) docker     (121)      608 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/event.py
--rw-r--r--   0 runner    (1001) docker     (121)    15843 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/facade.py
--rw-r--r--   0 runner    (1001) docker     (121)     6614 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/io.py
--rw-r--r--   0 runner    (1001) docker     (121)     1900 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 16:42:10.123768 hvpy-1.0.1/hvpy/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      185 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (121)      855 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/tests/test_datasources.py
--rw-r--r--   0 runner    (1001) docker     (121)      670 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/tests/test_event.py
--rw-r--r--   0 runner    (1001) docker     (121)     3534 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     1502 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (121)     4533 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5422 2022-10-19 16:41:47.000000 hvpy-1.0.1/hvpy/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      345 2022-10-19 16:42:10.000000 hvpy-1.0.1/hvpy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 16:42:10.119768 hvpy-1.0.1/hvpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1713 2022-10-19 16:42:10.000000 hvpy-1.0.1/hvpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2868 2022-10-19 16:42:10.000000 hvpy-1.0.1/hvpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-19 16:42:10.000000 hvpy-1.0.1/hvpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-10-19 16:42:10.000000 hvpy-1.0.1/hvpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-10-19 16:42:10.000000 hvpy-1.0.1/hvpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-19 16:42:10.000000 hvpy-1.0.1/hvpy.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-19 16:42:10.123768 hvpy-1.0.1/licenses/
--rw-r--r--   0 runner    (1001) docker     (121)     1272 2022-10-19 16:41:47.000000 hvpy-1.0.1/licenses/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (121)      372 2022-10-19 16:41:47.000000 hvpy-1.0.1/licenses/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1659 2022-10-19 16:41:47.000000 hvpy-1.0.1/licenses/TEMPLATE_LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (121)      507 2022-10-19 16:41:47.000000 hvpy-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2482 2022-10-19 16:42:10.127768 hvpy-1.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)      567 2022-10-19 16:41:47.000000 hvpy-1.0.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     1412 2022-10-19 16:41:47.000000 hvpy-1.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:12:43.471241 hvpy-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:12:43.463241 hvpy-1.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-12 13:12:27.000000 hvpy-1.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:12:43.463241 hvpy-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-12 13:12:27.000000 hvpy-1.1.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-12 13:12:27.000000 hvpy-1.1.0/.github/workflows/cron.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-07-12 13:12:27.000000 hvpy-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-12 13:12:27.000000 hvpy-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-12 13:12:27.000000 hvpy-1.1.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-12 13:12:27.000000 hvpy-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-12 13:12:43.471241 hvpy-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-12 13:12:27.000000 hvpy-1.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:12:43.463241 hvpy-1.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-12 13:12:27.000000 hvpy-1.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-12 13:12:27.000000 hvpy-1.1.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-12 13:12:27.000000 hvpy-1.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-07-12 13:12:27.000000 hvpy-1.1.0/docs/dev_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-07-12 13:12:27.000000 hvpy-1.1.0/docs/guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-12 13:12:27.000000 hvpy-1.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-12 13:12:27.000000 hvpy-1.1.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-12 13:12:27.000000 hvpy-1.1.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-12 13:12:27.000000 hvpy-1.1.0/docs/nitpick-exceptions
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:12:43.467241 hvpy-1.1.0/hvpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:12:43.467241 hvpy-1.1.0/hvpy/api_groups/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/api_groups/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:12:43.467241 hvpy-1.1.0/hvpy/api_groups/communications/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/api_groups/communications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/api_groups/communications/get_news_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/api_groups/communications/shorten_url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:12:43.467241 hvpy-1.1.0/hvpy/api_groups/communications/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/api_groups/communications/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/api_groups/communications/tests/test_get_news_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/api_groups/communications/tests/test_shorten_url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:12:43.467241 hvpy-1.1.0/hvpy/api_groups/jpeg2000/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/api_groups/jpeg2000/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/api_groups/jpeg2000/get_jp2_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/api_groups/jpeg2000/get_jp2_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/api_groups/jpeg2000/get_jpx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/api_groups/jpeg2000/get_jpx_closest_to_mid_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/api_groups/jpeg2000/get_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:12:43.467241 hvpy-1.1.0/hvpy/api_groups/jpeg2000/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/api_groups/jpeg2000/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/api_groups/jpeg2000/tests/test_get_jp2_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/api_groups/jpeg2000/tests/test_get_jp2_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/api_groups/jpeg2000/tests/test_get_jpx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/api_groups/jpeg2000/tests/test_get_jpx_closest_to_mid_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/api_groups/jpeg2000/tests/test_get_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:12:43.467241 hvpy-1.1.0/hvpy/api_groups/movies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/api_groups/movies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/api_groups/movies/download_movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/api_groups/movies/get_movie_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/api_groups/movies/queue_movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/api_groups/movies/re_queue_movie.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:12:43.471241 hvpy-1.1.0/hvpy/api_groups/movies/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/api_groups/movies/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/api_groups/movies/tests/test_download_movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/api_groups/movies/tests/test_get_movie_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/api_groups/movies/tests/test_queue_movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/api_groups/movies/tests/test_re_queue_movie.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:12:43.471241 hvpy-1.1.0/hvpy/api_groups/official_clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/api_groups/official_clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/api_groups/official_clients/get_closest_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/api_groups/official_clients/get_data_sources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:12:43.471241 hvpy-1.1.0/hvpy/api_groups/official_clients/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/api_groups/official_clients/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/api_groups/official_clients/tests/test_get_closest_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/api_groups/official_clients/tests/test_get_data_sources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:12:43.471241 hvpy-1.1.0/hvpy/api_groups/screenshots/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/api_groups/screenshots/download_screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/api_groups/screenshots/get_tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/api_groups/screenshots/take_screenshot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:12:43.471241 hvpy-1.1.0/hvpy/api_groups/screenshots/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/api_groups/screenshots/tests/test_download_screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/api_groups/screenshots/tests/test_get_tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/api_groups/screenshots/tests/test_take_screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9531 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15790 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/facade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:12:43.471241 hvpy-1.1.0/hvpy/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/tests/test_datasources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/tests/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-07-12 13:12:27.000000 hvpy-1.1.0/hvpy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-12 13:12:43.000000 hvpy-1.1.0/hvpy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:12:43.467241 hvpy-1.1.0/hvpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-12 13:12:43.000000 hvpy-1.1.0/hvpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-07-12 13:12:43.000000 hvpy-1.1.0/hvpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 13:12:43.000000 hvpy-1.1.0/hvpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-12 13:12:43.000000 hvpy-1.1.0/hvpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-12 13:12:43.000000 hvpy-1.1.0/hvpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 13:12:43.000000 hvpy-1.1.0/hvpy.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:12:43.471241 hvpy-1.1.0/licenses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-12 13:12:27.000000 hvpy-1.1.0/licenses/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-12 13:12:27.000000 hvpy-1.1.0/licenses/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-12 13:12:27.000000 hvpy-1.1.0/licenses/TEMPLATE_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-12 13:12:27.000000 hvpy-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-07-12 13:12:43.471241 hvpy-1.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      567 2023-07-12 13:12:27.000000 hvpy-1.1.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-12 13:12:27.000000 hvpy-1.1.0/tox.ini
```

### Comparing `hvpy-1.0.1/.github/workflows/ci.yml` & `hvpy-1.1.0/.github/workflows/ci.yml`

 * *Files 6% similar despite different names*

```diff
@@ -20,30 +20,41 @@
 
 jobs:
   core:
     uses: OpenAstronomy/github-actions-workflows/.github/workflows/tox.yml@main
     with:
       submodules: false
       coverage: codecov
+      toxdeps: tox-pypi-filter
       envs: |
-        - linux: py310
+        - linux: py311
         - linux: codestyle
   test:
     needs: [core]
     uses: OpenAstronomy/github-actions-workflows/.github/workflows/tox.yml@main
     with:
       submodules: false
       coverage: codecov
+      toxdeps: tox-pypi-filter
+      envs: |
+        - linux: py38
+        - macos: py310
+        - windows: py39
+  docs:
+    needs: [test]
+    uses: OpenAstronomy/github-actions-workflows/.github/workflows/tox.yml@main
+    with:
+      submodules: false
+      coverage: codecov
+      toxdeps: tox-pypi-filter
       libraries: |
         apt:
           - libopenjp2-7
           - graphviz
       envs: |
-        - macos: py38
-        - windows: py39
         - linux: build_docs
   publish:
     # Build wheels when pushing to any branch except main
     # publish.yml will only publish if tagged ^v.*
     if: |
       (
         github.event_name != 'pull_request' && (
@@ -54,11 +65,11 @@
         github.event_name == 'pull_request' &&
         contains(github.event.pull_request.labels.*.name, 'Run publish')
       )
     needs: [test]
     uses: OpenAstronomy/github-actions-workflows/.github/workflows/publish_pure_python.yml@v1
     with:
       test_extras: 'all,tests'
-      test_command: 'HELIOVIEWER_API_URL=https://api.beta.helioviewer.org/v2/ pytest -p no:warnings --doctest-rst -m "not mpl_image_compare" --pyargs hvpy'
+      test_command: 'HELIOVIEWER_API_URL=https://api.beta.helioviewer.org/v2/ pytest -p no:warnings --doctest-rst --pyargs hvpy'
       submodules: false
     secrets:
       pypi_token: ${{ secrets.pypi_token }}
```

### Comparing `hvpy-1.0.1/.gitignore` & `hvpy-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hvpy-1.0.1/.pre-commit-config.yaml` & `hvpy-1.1.0/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 repos:
   - repo: https://github.com/myint/docformatter
-    rev: v1.5.0
+    rev: v1.7.4
     hooks:
       - id: docformatter
         args: [--in-place, --pre-summary-newline, --make-summary-multi]
   - repo: https://github.com/myint/autoflake
-    rev: v1.7.6
+    rev: v2.2.0
     hooks:
       - id: autoflake
         args: ['--in-place', '--remove-all-unused-imports', '--remove-unused-variable']
         exclude: ".*(.fits|.fts|.fit|.txt|tca.*|extern.*|.rst|.md|__init__.py)$"
   - repo: https://github.com/psf/black
-    rev: 22.10.0
+    rev: 23.3.0
     hooks:
     - id: black
       exclude: ".*(.fits|.fts|.fit|.txt|.csv)$"
   - repo: https://github.com/timothycrosley/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
     - id: isort
       exclude: ".*(.fits|.fts|.fit|.txt|.csv|__init__.py)$"
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
     - id: check-ast
     - id: check-case-conflict
     - id: trailing-whitespace
       exclude: ".*(.fits|.fts|.fit|.txt|.csv)$"
     - id: mixed-line-ending
       exclude: ".*(.fits|.fts|.fit|.txt|.csv)$"
     - id: end-of-file-fixer
       exclude: ".*(.fits|.fts|.fit|.txt|.csv)$"
     - id: check-yaml
     - id: debug-statements
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: 'v0.982'
+    rev: 'v1.4.1'
     hooks:
     - id: mypy
       additional_dependencies: [types-requests==2.28.0]
```

### Comparing `hvpy-1.0.1/LICENSE` & `hvpy-1.1.0/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 2-Clause License
 
-Copyright (c) 2022, Helioviewer Project
+Copyright (c) 2022-2023, Helioviewer Project
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `hvpy-1.0.1/PKG-INFO` & `hvpy-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hvpy
-Version: 1.0.1
+Version: 1.1.0
 Summary: Helioviewer Python API Wrapper
 Home-page: https://helioviewer.org/
 Author: The Helioviewer Project
 Author-email: contact@helioviewer.org
 License: BSD 2-Clause
 Keywords: solar physics,solar,science,sun,data,helioviewer
 Platform: any
@@ -14,14 +14,15 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.8
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: licenses/LICENSE.rst
 
 Helioviewer Python API Wrapper
```

### Comparing `hvpy-1.0.1/README.rst` & `hvpy-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `hvpy-1.0.1/docs/Makefile` & `hvpy-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hvpy-1.0.1/docs/conf.py` & `hvpy-1.1.0/docs/conf.py`

 * *Files 22% similar despite different names*

```diff
@@ -40,24 +40,19 @@
     dtype, target = line.split(None, 1)
     target = target.strip()
     nitpick_ignore.append((dtype, target))
 
 # -- Options for intersphinx extension -----------------------------------------
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3/", None),
-    "numpy": ("https://numpy.org/doc/stable/", None),
-    "scipy": ("https://docs.scipy.org/doc/scipy/reference/", None),
-    "matplotlib": ("https://matplotlib.org/stable", None),
-    "aiapy": ("https://aiapy.readthedocs.io/en/stable/", None),
-    "astropy": ("https://docs.astropy.org/en/stable/", None),
     "requests": ("https://requests.readthedocs.io/en/stable/", None),
+    "pydantic": ("https://docs.pydantic.dev/latest/", None),
 }
 
 # -- Options for HTML output ---------------------------------------------------
 # The theme to use for HTML and HTML Help pages.
 html_theme = "sphinx_book_theme"
 html_theme_options = {
     "repository_url": "https://github.com/Helioviewer-Project/python-api/",
     "use_repository_button": True,
-    "extra_navbar": "",
 }
 html_title = "hvpy"
```

### Comparing `hvpy-1.0.1/docs/dev_guide.rst` & `hvpy-1.1.0/docs/dev_guide.rst`

 * *Files identical despite different names*

### Comparing `hvpy-1.0.1/docs/guide.rst` & `hvpy-1.1.0/docs/guide.rst`

 * *Files identical despite different names*

### Comparing `hvpy-1.0.1/docs/index.rst` & `hvpy-1.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `hvpy-1.0.1/docs/installation.rst` & `hvpy-1.1.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `hvpy-1.0.1/docs/make.bat` & `hvpy-1.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hvpy-1.0.1/hvpy/api_groups/communications/get_news_feed.py` & `hvpy-1.1.0/hvpy/api_groups/communications/get_news_feed.py`

 * *Files identical despite different names*

### Comparing `hvpy-1.0.1/hvpy/api_groups/communications/shorten_url.py` & `hvpy-1.1.0/hvpy/api_groups/communications/shorten_url.py`

 * *Files identical despite different names*

### Comparing `hvpy-1.0.1/hvpy/api_groups/communications/tests/test_shorten_url.py` & `hvpy-1.1.0/hvpy/api_groups/communications/tests/test_shorten_url.py`

 * *Files identical despite different names*

### Comparing `hvpy-1.0.1/hvpy/api_groups/jpeg2000/get_jp2_header.py` & `hvpy-1.1.0/hvpy/api_groups/jpeg2000/get_jp2_header.py`

 * *Files identical despite different names*

### Comparing `hvpy-1.0.1/hvpy/api_groups/jpeg2000/get_jp2_image.py` & `hvpy-1.1.0/hvpy/api_groups/official_clients/get_closest_image.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,52 +1,45 @@
-from typing import Union
+from typing import Union, Optional
 from datetime import datetime
 
-from pydantic import Field, validator
+from pydantic import field_validator
 
 from hvpy.datasource import DataSource
 from hvpy.io import HvpyParameters, OutputType
 from hvpy.utils import _data_source_to_int, convert_date_to_isoformat
 
 
-class getJP2ImageInputParameters(HvpyParameters):
+class getClosestImageInputParameters(HvpyParameters):
     """
-    Handles the input parameters of the ``getJP2Image`` API.
+    Handles the input parameters of the ``getClosestImage`` API.
 
     .. {Shared}
     Attributes
     ----------
     date
-        Desired datetime of the JP2 image.
+        Datetime of the image.
     sourceId
         Unique image datasource identifier.
-    jpip
-        Returns a JPIP URI instead of the binary data of the image if set to True.
-        Default is `False`, optional.
-    json
-        Returns the JSON if set to `True`.
-        Default is `False`, optional.
+    callback
+        Wrap the response object in a function call of your choosing.
+        Default is `None` (no wrapping), optional.
 
     References
     ----------
-    * `<https://api.helioviewer.org/docs/v2/api/api_groups/jpeg2000.html#getjp2image>`__
+    * `<https://api.helioviewer.org/docs/v2/api/api_groups/official_clients.html#getclosestimage>`__
 
     .. {Shared}
     """
 
     date: datetime
     sourceId: Union[int, DataSource]
-    jpip: bool = False
-    Json: bool = Field(False, alias="json")
-    _date_validator = validator("date", allow_reuse=True)(convert_date_to_isoformat)
-    _source_id_validator = validator("sourceId", allow_reuse=True)(_data_source_to_int)
+    callback: Optional[str] = None
+    _date_validator = field_validator("date")(convert_date_to_isoformat)
+    _source_id_validator = field_validator("sourceId")(_data_source_to_int)
 
     def get_output_type(self) -> OutputType:
         """
         Returns the output type of the API call.
         """
-        if self.Json and self.jpip:
+        if self.callback is None:
             return OutputType.JSON
-        elif not self.Json and self.jpip:
-            return OutputType.STRING
-        else:
-            return OutputType.RAW
+        return OutputType.STRING
```

### Comparing `hvpy-1.0.1/hvpy/api_groups/jpeg2000/get_jpx.py` & `hvpy-1.1.0/hvpy/api_groups/jpeg2000/get_jpx.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Union, Optional
 from datetime import datetime
 
-from pydantic import validator
+from pydantic import field_validator
 
 from hvpy.datasource import DataSource
 from hvpy.io import HvpyParameters, OutputType
 from hvpy.utils import _data_source_to_int, convert_date_to_isoformat
 
 
 class getJPXInputParameters(HvpyParameters):
@@ -46,16 +46,16 @@
     startTime: datetime
     endTime: datetime
     sourceId: Union[int, DataSource]
     linked: bool = True
     verbose: bool = False
     jpip: bool = False
     cadence: Optional[int] = None
-    _date_validator = validator("startTime", "endTime", allow_reuse=True)(convert_date_to_isoformat)
-    _source_id_validator = validator("sourceId", allow_reuse=True)(_data_source_to_int)
+    _date_validator = field_validator("startTime", "endTime")(convert_date_to_isoformat)
+    _source_id_validator = field_validator("sourceId")(_data_source_to_int)
 
     def get_output_type(self) -> OutputType:
         """
         Returns the output type of the API call.
         """
         if not self.jpip and not self.verbose:
             return OutputType.RAW
```

### Comparing `hvpy-1.0.1/hvpy/api_groups/jpeg2000/get_jpx_closest_to_mid_point.py` & `hvpy-1.1.0/hvpy/api_groups/jpeg2000/get_jpx_closest_to_mid_point.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List, Union
 from datetime import datetime
 
-from pydantic import validator
+from pydantic import field_validator
 
 from hvpy.datasource import DataSource
 from hvpy.io import HvpyParameters, OutputType
 from hvpy.utils import _data_source_to_int, convert_date_to_unix
 
 
 class getJPXClosestToMidPointInputParameters(HvpyParameters):
@@ -40,16 +40,16 @@
 
     startTimes: List[datetime]
     endTimes: List[datetime]
     sourceId: Union[int, DataSource]
     linked: bool = True
     verbose: bool = False
     jpip: bool = False
-    _date_validator = validator("startTimes", "endTimes", allow_reuse=True)(convert_date_to_unix)
-    _source_id_validator = validator("sourceId", allow_reuse=True)(_data_source_to_int)
+    _date_validator = field_validator("startTimes", "endTimes")(convert_date_to_unix)
+    _source_id_validator = field_validator("sourceId")(_data_source_to_int)
 
     def get_output_type(self) -> OutputType:
         """
         Returns the output type of the API call.
         """
         if not self.jpip and not self.verbose:
             return OutputType.RAW
```

### Comparing `hvpy-1.0.1/hvpy/api_groups/jpeg2000/tests/test_get_jp2_header.py` & `hvpy-1.1.0/hvpy/api_groups/jpeg2000/tests/test_get_jp2_header.py`

 * *Files identical despite different names*

### Comparing `hvpy-1.0.1/hvpy/api_groups/jpeg2000/tests/test_get_jp2_image.py` & `hvpy-1.1.0/hvpy/api_groups/jpeg2000/tests/test_get_jp2_image.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 from hvpy.api_groups.jpeg2000.get_jp2_image import getJP2ImageInputParameters
 from hvpy.datasource import DataSource
 
 
 def test_str_response(date):
     response = getJP2Image(date=date, sourceId=DataSource.AIA_335, jpip=True, json=False)
     assert isinstance(response, str)
-    assert response.startswith("jpip://")
+    assert response.startswith("jpips://")
 
 
 def test_json_response(date):
     response = getJP2Image(date=date, sourceId=14, jpip=True, json=True)
     assert isinstance(response, dict)
     assert "uri" in response
-    assert response["uri"].startswith("jpip://")
+    assert response["uri"].startswith("jpips://")
 
 
 def test_raw_response(date):
     response = getJP2Image(date=date, sourceId=DataSource.AIA_335, jpip=False, json=False)
     assert isinstance(response, bytes)
```

### Comparing `hvpy-1.0.1/hvpy/api_groups/jpeg2000/tests/test_get_jpx.py` & `hvpy-1.1.0/hvpy/api_groups/jpeg2000/tests/test_get_jpx.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,29 +25,29 @@
         sourceId=DataSource.AIA_335,
         linked=False,
         verbose=False,
         jpip=True,
         cadence=60,
     )
     assert isinstance(response, str)
-    assert response.startswith("jpip://")
+    assert response.startswith("jpips://")
 
 
 def test_json_response(start_time, end_time):
     response = getJPX(
         startTime=start_time,
         endTime=end_time,
         sourceId=14,
         linked=False,
         verbose=True,
         jpip=True,
         cadence=60,
     )
     assert isinstance(response, dict)
-    assert response["uri"].startswith("jpip://")
+    assert response["uri"].startswith("jpips://")
 
     response = getJPX(
         startTime=start_time,
         endTime=end_time,
         sourceId=14,
         linked=False,
         verbose=True,
```

### Comparing `hvpy-1.0.1/hvpy/api_groups/jpeg2000/tests/test_get_jpx_closest_to_mid_point.py` & `hvpy-1.1.0/hvpy/api_groups/jpeg2000/tests/test_get_jpx_closest_to_mid_point.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,28 +23,28 @@
         endTimes=end_times,
         sourceId=14,
         linked=False,
         verbose=False,
         jpip=True,
     )
     assert isinstance(response, str)
-    assert response.startswith("jpip://")
+    assert response.startswith("jpips://")
 
 
 def test_json_response(start_times, end_times):
     response = getJPXClosestToMidPoint(
         startTimes=start_times,
         endTimes=end_times,
         sourceId=DataSource.AIA_335,
         linked=False,
         verbose=True,
         jpip=True,
     )
     assert isinstance(response, dict)
-    assert response["uri"].startswith("jpip://")
+    assert response["uri"].startswith("jpips://")
 
     response = getJPXClosestToMidPoint(
         startTimes=start_times,
         endTimes=end_times,
         sourceId=14,
         linked=False,
         verbose=True,
```

### Comparing `hvpy-1.0.1/hvpy/api_groups/movies/download_movie.py` & `hvpy-1.1.0/hvpy/api_groups/movies/download_movie.py`

 * *Files identical despite different names*

### Comparing `hvpy-1.0.1/hvpy/api_groups/movies/get_movie_status.py` & `hvpy-1.1.0/hvpy/api_groups/movies/get_movie_status.py`

 * *Files identical despite different names*

### Comparing `hvpy-1.0.1/hvpy/api_groups/movies/queue_movie.py` & `hvpy-1.1.0/hvpy/api_groups/movies/queue_movie.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional
 from datetime import datetime
 
-from pydantic import validator
+from pydantic import field_validator
 
 from hvpy.io import HvpyParameters, OutputType
 from hvpy.utils import convert_date_to_isoformat
 
 
 class queueMovieInputParameters(HvpyParameters):
     """
@@ -130,16 +130,14 @@
     x2: Optional[str] = None
     y2: Optional[str] = None
     callback: Optional[str] = None
     size: int = 0
     movieIcons: Optional[int] = None
     followViewport: Optional[int] = None
     reqObservationDate: Optional[datetime] = None
-    _date_validator = validator("startTime", "endTime", "reqObservationDate", allow_reuse=True)(
-        convert_date_to_isoformat
-    )
+    _date_validator = field_validator("startTime", "endTime", "reqObservationDate")(convert_date_to_isoformat)
 
     def get_output_type(self) -> OutputType:
         """
         Returns the output type of the API call.
         """
         return OutputType.JSON
```

### Comparing `hvpy-1.0.1/hvpy/api_groups/movies/re_queue_movie.py` & `hvpy-1.1.0/hvpy/api_groups/movies/re_queue_movie.py`

 * *Files identical despite different names*

### Comparing `hvpy-1.0.1/hvpy/api_groups/movies/tests/test_download_movie.py` & `hvpy-1.1.0/hvpy/api_groups/movies/tests/test_download_movie.py`

 * *Files identical despite different names*

### Comparing `hvpy-1.0.1/hvpy/api_groups/movies/tests/test_get_movie_status.py` & `hvpy-1.1.0/hvpy/api_groups/movies/tests/test_get_movie_status.py`

 * *Files identical despite different names*

### Comparing `hvpy-1.0.1/hvpy/api_groups/movies/tests/test_queue_movie.py` & `hvpy-1.1.0/hvpy/api_groups/movies/tests/test_queue_movie.py`

 * *Files identical despite different names*

### Comparing `hvpy-1.0.1/hvpy/api_groups/movies/tests/test_re_queue_movie.py` & `hvpy-1.1.0/hvpy/api_groups/movies/tests/test_re_queue_movie.py`

 * *Files identical despite different names*

### Comparing `hvpy-1.0.1/hvpy/api_groups/official_clients/get_closest_image.py` & `hvpy-1.1.0/hvpy/api_groups/official_clients/get_data_sources.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,41 @@
-from typing import Union, Optional
-from datetime import datetime
+from typing import Optional
 
-from pydantic import validator
-
-from hvpy.datasource import DataSource
 from hvpy.io import HvpyParameters, OutputType
-from hvpy.utils import _data_source_to_int, convert_date_to_isoformat
 
 
-class getClosestImageInputParameters(HvpyParameters):
+class getDataSourcesInputParameters(HvpyParameters):
     """
-    Handles the input parameters of the ``getClosestImage`` API.
+    Handles the input parameters of the ``getDataSources`` API.
 
     .. {Shared}
     Attributes
     ----------
-    date
-        Datetime of the image.
-    sourceId
-        Unique image datasource identifier.
+    verbose
+        Output the hierarchical list of available datasources in a format that is compatible with the JHelioviewer desktop client.
+        Default is `False`, optional.
+    enable
+        Comma-separated list of observatories to enable.
+        Default is `None` (all observatories are enabled), optional.
     callback
         Wrap the response object in a function call of your choosing.
         Default is `None` (no wrapping), optional.
 
     References
     ----------
-    * `<https://api.helioviewer.org/docs/v2/api/api_groups/official_clients.html#getclosestimage>`__
+    * `<https://api.helioviewer.org/docs/v2/api/api_groups/official_clients.html#getdatasources>`__
 
     .. {Shared}
     """
 
-    date: datetime
-    sourceId: Union[int, DataSource]
+    verbose: bool = False
+    enable: Optional[str] = None
     callback: Optional[str] = None
-    _date_validator = validator("date", allow_reuse=True)(convert_date_to_isoformat)
-    _source_id_validator = validator("sourceId", allow_reuse=True)(_data_source_to_int)
 
     def get_output_type(self) -> OutputType:
         """
         Returns the output type of the API call.
         """
-        if self.callback is None:
+        if self.callback:
+            return OutputType.STRING
+        else:
             return OutputType.JSON
-        return OutputType.STRING
```

### Comparing `hvpy-1.0.1/hvpy/api_groups/official_clients/tests/test_get_closest_image.py` & `hvpy-1.1.0/hvpy/api_groups/official_clients/tests/test_get_closest_image.py`

 * *Files identical despite different names*

### Comparing `hvpy-1.0.1/hvpy/api_groups/screenshots/download_screenshot.py` & `hvpy-1.1.0/hvpy/api_groups/screenshots/download_screenshot.py`

 * *Files identical despite different names*

### Comparing `hvpy-1.0.1/hvpy/api_groups/screenshots/get_tile.py` & `hvpy-1.1.0/hvpy/api_groups/screenshots/get_tile.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional
 from datetime import datetime
 
-from pydantic import validator
+from pydantic import field_validator
 
 from hvpy.io import HvpyParameters, OutputType
 from hvpy.utils import convert_date_to_isoformat
 
 
 class getTileInputParameters(HvpyParameters):
     """
@@ -61,14 +61,14 @@
     y: int
     imageScale: int
     difference: Optional[int] = None
     diffCount: Optional[int] = None
     diffTime: Optional[int] = None
     baseDiffTime: Optional[datetime] = None
 
-    _date_vaidator = validator("baseDiffTime", allow_reuse=True)(convert_date_to_isoformat)
+    _date_vaidator = field_validator("baseDiffTime")(convert_date_to_isoformat)
 
     def get_output_type(self) -> OutputType:
         """
         Returns the output type of the API call.
         """
         return OutputType.RAW
```

### Comparing `hvpy-1.0.1/hvpy/api_groups/screenshots/take_screenshot.py` & `hvpy-1.1.0/hvpy/api_groups/screenshots/take_screenshot.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional
 from datetime import datetime
 
-from pydantic import validator
+from pydantic import field_validator
 
 from hvpy.io import HvpyParameters, OutputType
 from hvpy.utils import convert_date_to_isoformat
 
 
 class takeScreenshotInputParameters(HvpyParameters):
     """
@@ -94,25 +94,25 @@
     layers: str
     events: Optional[str] = None
     eventLabels: bool = False
     scale: bool = False
     scaleType: Optional[str] = None
     scaleX: Optional[int] = None
     scaleY: Optional[int] = None
-    width: Optional[str] = None
-    height: Optional[str] = None
-    x0: Optional[str] = None
-    y0: Optional[str] = None
-    x1: Optional[str] = None
-    y1: Optional[str] = None
-    x2: Optional[str] = None
-    y2: Optional[str] = None
+    width: Optional[int] = None
+    height: Optional[int] = None
+    x0: Optional[int] = None
+    y0: Optional[int] = None
+    x1: Optional[int] = None
+    y1: Optional[int] = None
+    x2: Optional[int] = None
+    y2: Optional[int] = None
     display: bool = False
     watermark: bool = False
     callback: Optional[str] = None
-    _date_vaidator = validator("date", allow_reuse=True)(convert_date_to_isoformat)
+    _date_vaidator = field_validator("date")(convert_date_to_isoformat)
 
     def get_output_type(self) -> OutputType:
         """
         Returns the output type of the API call.
         """
         return OutputType.RAW if self.display else OutputType.JSON
```

### Comparing `hvpy-1.0.1/hvpy/api_groups/screenshots/tests/test_download_screenshot.py` & `hvpy-1.1.0/hvpy/api_groups/screenshots/tests/test_download_screenshot.py`

 * *Files identical despite different names*

### Comparing `hvpy-1.0.1/hvpy/api_groups/screenshots/tests/test_get_tile.py` & `hvpy-1.1.0/hvpy/api_groups/screenshots/tests/test_get_tile.py`

 * *Files identical despite different names*

### Comparing `hvpy-1.0.1/hvpy/api_groups/screenshots/tests/test_take_screenshot.py` & `hvpy-1.1.0/hvpy/api_groups/screenshots/tests/test_take_screenshot.py`

 * *Files identical despite different names*

### Comparing `hvpy-1.0.1/hvpy/config.py` & `hvpy-1.1.0/hvpy/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-from pydantic import BaseSettings, Field
+from pydantic import Field
+from pydantic_settings import BaseSettings, SettingsConfigDict
 
 __all__ = ["LiveSettings", "set_api_url", "get_api_url"]
 
 
 class Settings(BaseSettings):
-    api_url: str = Field("https://api.helioviewer.org/v2/", env="HELIOVIEWER_API_URL")
+    model_config = SettingsConfigDict(env_prefix="HELIOVIEWER_")
+    api_url: str = Field("https://api.helioviewer.org/v2/")
 
 
 def get_api_url() -> str:
     """
     Returns the API URL.
     """
     from hvpy.config import LiveSettings
```

### Comparing `hvpy-1.0.1/hvpy/conftest.py` & `hvpy-1.1.0/hvpy/conftest.py`

 * *Files identical despite different names*

### Comparing `hvpy-1.0.1/hvpy/core.py` & `hvpy-1.1.0/hvpy/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,10 +43,10 @@
         The input parameters.
 
     Returns
     -------
     Union[bytes, str, Dict[str, Any]]
         Parsed response from the API.
     """
-    response = requests.get(input_parameters.url, params=input_parameters.dict())
+    response = requests.get(input_parameters.url, params=input_parameters.model_dump())
     response.raise_for_status()
     return parse_response(response, input_parameters.get_output_type())
```

### Comparing `hvpy-1.0.1/hvpy/datasource.py` & `hvpy-1.1.0/hvpy/datasource.py`

 * *Files 4% similar despite different names*

```diff
@@ -434,40 +434,75 @@
     """
 
     EUI_HRI_1216 = 87
     """
     Solar Orbiter instrument HRI, measurement 1216.
     """
 
-    SUVI_94 = 88
+    IRIS_SJI_1330 = 88
+    """
+    IRIS Slit Jaw Imager, measurement 1330.
+    """
+
+    IRIS_SJI_2796 = 89
+    """
+    IRIS Slit Jaw Imager, measurement 2796.
+    """
+
+    IRIS_SJI_1400 = 90
+    """
+    IRIS Slit Jaw Imager, measurement 1400.
+    """
+
+    IRIS_SJI_2832 = 92
+    """
+    IRIS Slit Jaw Imager, measurement 2832.
+    """
+
+    GONG_MAGNETOGRAM = 37
+    """
+    NSO GONG Magnetograms.
+    """
+
+    GONG_H_ALPHA = 94
+    """
+    NSO GONG H-Alpha.
+    """
+
+    GONG_FARSIDE = 95
+    """
+    NSO GONG Farside.
+    """
+
+    SUVI_94 = 2000
     """
     GOES-R instrument SUVI, measurement 94.
     """
 
-    SUVI_131 = 89
+    SUVI_131 = 2001
     """
     GOES-R instrument SUVI, measurement 131.
     """
 
-    SUVI_171 = 90
+    SUVI_171 = 2002
     """
     GOES-R instrument SUVI, measurement 171.
     """
 
-    SUVI_195 = 91
+    SUVI_195 = 2003
     """
     GOES-R instrument SUVI, measurement 195.
     """
 
-    SUVI_284 = 92
+    SUVI_284 = 2004
     """
     GOES-R instrument SUVI, measurement 284.
     """
 
-    SUVI_304 = 93
+    SUVI_304 = 2005
     """
     GOES-R instrument SUVI, measurement 304.
     """
 
     XRT_ANY_ANY = 10001
     """
     Hinode instrument XRT any/any.
```

### Comparing `hvpy-1.0.1/hvpy/event.py` & `hvpy-1.1.0/hvpy/event.py`

 * *Files identical despite different names*

### Comparing `hvpy-1.0.1/hvpy/facade.py` & `hvpy-1.1.0/hvpy/facade.py`

 * *Files 12% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     ----------
     {Insert}
     Examples
     --------
     >>> from hvpy import getJP2Image
     >>> from datetime import datetime, timedelta
     >>> getJP2Image(date=datetime.today(), sourceId=14, jpip=True)
-    'jpip://...'
+    'jpips://...'
     """
     params = getJP2ImageInputParameters(date=date, sourceId=sourceId, jpip=jpip, json=json)
     return execute_api_call(input_parameters=params)
 
 
 @_add_shared_docstring(getJP2HeaderInputParameters)
 def getJP2Header(
@@ -61,15 +61,15 @@
 
     Parameters
     ----------
     {Insert}
     Examples
     --------
     >>> from hvpy import getJP2Header
-    >>> getJP2Header(id=7654321,callback="xml_header")
+    >>> getJP2Header(id=7654321, callback="xml_header")
     'xml_header(\\\'<?xml version="1.0" encoding="utf-8"?><meta><fits>...')'
     """
     params = getJP2HeaderInputParameters(id=id, callback=callback)
     return execute_api_call(input_parameters=params)
 
 
 @_add_shared_docstring(getJPXClosestToMidPointInputParameters)
@@ -95,15 +95,15 @@
     >>> getJPXClosestToMidPoint(
     ...     startTimes=[datetime.today() - timedelta(days=15, minutes=5), datetime.today() - timedelta(days=16, minutes=5)],
     ...     endTimes=[datetime.today() - timedelta(days=15), datetime.today() - timedelta(days=16)],
     ...     sourceId=14,
     ...     linked=False,
     ...     jpip=True
     ... )
-    'jpip://beta.helioviewer.org:8090/movies/SDO_AIA_335_...jpxmid'
+    'jpips://beta.helioviewer.org:8092/movies/...jpxmid'
     """
     params = getJPXClosestToMidPointInputParameters(
         startTimes=startTimes,
         endTimes=endTimes,
         sourceId=sourceId,
         linked=linked,
         verbose=verbose,
@@ -136,15 +136,15 @@
     >>> getJPX(startTime=datetime.today() - timedelta(days=15, minutes=5),
     ...        endTime=datetime.today() - timedelta(days=15),
     ...        sourceId=14,
     ...        linked=False,
     ...        jpip=True,
     ...        verbose=False,
     ...        cadence=60)
-    'jpip://beta.helioviewer.org:8090/movies/...'
+    'jpips://beta.helioviewer.org:8092/movies/...'
     """
     params = getJPXInputParameters(
         startTime=startTime,
         endTime=endTime,
         sourceId=sourceId,
         linked=linked,
         verbose=verbose,
@@ -163,15 +163,15 @@
     Parameters
     ----------
     {Insert}
     Examples
     --------
     >>> from hvpy import getStatus
     >>> getStatus()
-    {'AIA': ..., 'COSMO': ..., 'EUI': ..., 'HMI': ..., 'LASCO': ..., 'SECCHI': ..., 'SWAP': ..., 'XRT': ...}
+    {'AIA': ..., ...}
     """
     params = getStatusInputParameters()
     return execute_api_call(input_parameters=params)
 
 
 @_add_shared_docstring(getClosestImageInputParameters)
 def getClosestImage(
@@ -213,15 +213,15 @@
     Parameters
     ----------
     {Insert}
     Examples
     --------
     >>> from hvpy import getDataSources
     >>> getDataSources()
-    {'GOES-R': {'SUVI': {...: {'sourceId': ..., 'nickname': 'GOES-R SUVI 94', 'layeringOrder': 1, 'start': ..., 'end': ..., 'uiLabels': [{'label': 'Observatory', 'name': 'GOES-R'}, {'label': 'Detector', 'name': 'SUVI'}, ...}
+    {'GOES-R': {'SUVI': {'94': {'sourceId': 2000, 'nickname': 'GOES-R SUVI 94', 'layeringOrder': 1, 'start': '...', 'end': '...', 'uiLabels': [{'label': 'Observatory', 'name': 'GOES-R'}, {'label': 'Instrument', 'name': 'SUVI'}, {'label': 'Measurement', 'name': '94'}]}...
     """
     params = getDataSourcesInputParameters(
         verbose=verbose,
         enable=enable,
         callback=callback,
     )
     return execute_api_call(input_parameters=params)
@@ -234,22 +234,22 @@
     layers: str,
     events: Optional[str] = None,
     eventLabels: bool = False,
     scale: bool = False,
     scaleType: Optional[str] = None,
     scaleX: Optional[int] = None,
     scaleY: Optional[int] = None,
-    width: Optional[str] = None,
-    height: Optional[str] = None,
-    x0: Optional[str] = None,
-    y0: Optional[str] = None,
-    x1: Optional[str] = None,
-    y1: Optional[str] = None,
-    x2: Optional[str] = None,
-    y2: Optional[str] = None,
+    width: Optional[int] = None,
+    height: Optional[int] = None,
+    x0: Optional[int] = None,
+    y0: Optional[int] = None,
+    x1: Optional[int] = None,
+    y1: Optional[int] = None,
+    x2: Optional[int] = None,
+    y2: Optional[int] = None,
     display: bool = False,
     watermark: bool = False,
     callback: Optional[str] = None,
 ):
     """
     Generate a custom screenshot.
 
@@ -328,22 +328,22 @@
     maxFrames: Optional[str] = None,
     scale: Optional[bool] = None,
     scaleType: Optional[str] = None,
     scaleX: Optional[float] = None,
     scaleY: Optional[float] = None,
     movieLength: Optional[float] = None,
     watermark: bool = True,
-    width: Optional[str] = None,
-    height: Optional[str] = None,
-    x0: Optional[str] = None,
-    y0: Optional[str] = None,
-    x1: Optional[str] = None,
-    y1: Optional[str] = None,
-    x2: Optional[str] = None,
-    y2: Optional[str] = None,
+    width: Optional[int] = None,
+    height: Optional[int] = None,
+    x0: Optional[int] = None,
+    y0: Optional[int] = None,
+    x1: Optional[int] = None,
+    y1: Optional[int] = None,
+    x2: Optional[int] = None,
+    y2: Optional[int] = None,
     callback: Optional[str] = None,
     size: int = 0,
     movieIcons: Optional[int] = None,
     followViewport: Optional[int] = None,
     reqObservationDate: Optional[datetime] = None,
 ) -> Union[bytes, str, Dict[str, Any]]:
     """
@@ -408,16 +408,16 @@
     Re-generate a custom movie that is no longer cached on the server.
 
     Parameters
     ----------
     {Insert}
     Examples
     --------
-    >>> from hvpy import reQueueMovie        # doctest: +SKIP
-    >>> reQueueMovie(id="gxRN5", force=True) # doctest: +SKIP
+    >>> from hvpy import reQueueMovie
+    >>> reQueueMovie(id="gxRN5", force=True)  # doctest: +SKIP
     {'id': 'gxRN5', 'eta': 274, 'queue': 0, 'token': '...'}
     """
     params = reQueueMovieInputParameters(
         id=id,
         force=force,
     )
     return execute_api_call(input_parameters=params)
@@ -436,15 +436,15 @@
 
     Parameters
     ----------
     {Insert}
     Examples
     --------
     >>> from hvpy import getMovieStatus
-    >>> getMovieStatus(id="h2n6n", format="mp4")
+    >>> getMovieStatus(id="h2n6n", format="mp4")  # doctest: +SKIP
     {'frameRate': ..., 'numFrames': ..., 'startDate': '...', 'status': ..., 'endDate': '...', 'width': ..., 'height': ..., 'title': '...', 'thumbnails': {'icon': '...', 'small': '...', 'medium': '...', 'large': '...', 'full': '...'}, 'url': '...', 'statusLabel': 'Completed'}
     """
     params = getMovieStatusInputParameters(
         id=id,
         format=format,
         verbose=verbose,
         callback=callback,
```

### Comparing `hvpy-1.0.1/hvpy/helpers.py` & `hvpy-1.1.0/hvpy/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,22 +27,22 @@
     maxFrames: Optional[str] = None,
     scale: Optional[bool] = None,
     scaleType: Optional[str] = None,
     scaleX: Optional[float] = None,
     scaleY: Optional[float] = None,
     movieLength: Optional[float] = None,
     watermark: bool = True,
-    width: Optional[str] = None,
-    height: Optional[str] = None,
-    x0: Optional[str] = None,
-    y0: Optional[str] = None,
-    x1: Optional[str] = None,
-    y1: Optional[str] = None,
-    x2: Optional[str] = None,
-    y2: Optional[str] = None,
+    width: Optional[int] = None,
+    height: Optional[int] = None,
+    x0: Optional[int] = None,
+    y0: Optional[int] = None,
+    x1: Optional[int] = None,
+    y1: Optional[int] = None,
+    x2: Optional[int] = None,
+    y2: Optional[int] = None,
     size: int = 0,
     movieIcons: Optional[int] = None,
     followViewport: Optional[int] = None,
     reqObservationDate: Optional[datetime] = None,
     overwrite: bool = False,
     filename: Optional[Union[str, Path]] = None,
     hq: bool = False,
@@ -137,22 +137,22 @@
     layers: str,
     events: Optional[str] = None,
     eventLabels: bool = False,
     scale: bool = False,
     scaleType: Optional[str] = None,
     scaleX: Optional[int] = None,
     scaleY: Optional[int] = None,
-    width: Optional[str] = None,
-    height: Optional[str] = None,
-    x0: Optional[str] = None,
-    y0: Optional[str] = None,
-    x1: Optional[str] = None,
-    y1: Optional[str] = None,
-    x2: Optional[str] = None,
-    y2: Optional[str] = None,
+    width: Optional[int] = None,
+    height: Optional[int] = None,
+    x0: Optional[int] = None,
+    y0: Optional[int] = None,
+    x1: Optional[int] = None,
+    y1: Optional[int] = None,
+    x2: Optional[int] = None,
+    y2: Optional[int] = None,
     watermark: bool = False,
     overwrite: bool = False,
     filename: Optional[Union[str, Path]] = None,
 ) -> Path:
     """
     Automatically creates a screenshot using `takeScreenshot`,
     `downloadScreenshot` functions.
```

### Comparing `hvpy-1.0.1/hvpy/io.py` & `hvpy-1.1.0/hvpy/io.py`

 * *Files 24% similar despite different names*

```diff
@@ -24,21 +24,26 @@
 
 
 class HvpyParameters(BaseModel):
     """
     Base model for all Helioviewer API parameters.
     """
 
-    def dict(self) -> Dict[str, Any]:  # type: ignore
+    def model_dump(self) -> Dict[str, Any]:
         # pydantic doesn't allow using lowercase 'json' as a field
-        d = super().dict()
-        if "Json" in d:
-            d["json"] = d["Json"]
-            del d["Json"]
-        return d
+        import warnings
+
+        with warnings.catch_warnings():
+            # Our datetime fields are strings(???) and pydantic complains about that
+            warnings.simplefilter("ignore")
+            dump = super().model_dump()
+        if "Json" in dump:
+            dump["json"] = dump["Json"]
+            del dump["Json"]
+        return dump
 
     def get_output_type(self) -> OutputType:
         """
         Works out the return type of the API call.
 
         This by default is RAW, subclasses should redefine this.
```

### Comparing `hvpy-1.0.1/hvpy/parameters.py` & `hvpy-1.1.0/hvpy/parameters.py`

 * *Files identical despite different names*

### Comparing `hvpy-1.0.1/hvpy/tests/test_datasources.py` & `hvpy-1.1.0/hvpy/tests/test_datasources.py`

 * *Files identical despite different names*

### Comparing `hvpy-1.0.1/hvpy/tests/test_event.py` & `hvpy-1.1.0/hvpy/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `hvpy-1.0.1/hvpy/tests/test_helper.py` & `hvpy-1.1.0/hvpy/tests/test_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             startTime=start_time,
             endTime=end_time,
             layers=create_layers([(DataSource.AIA_171, 100)]),
             events=create_events(["AR"]),
             eventsLabels=True,
             imageScale=1,
             filename=f1,
-            timeout=0.5,
+            timeout=0.01,
         )
 
 
 def test_error_handling2(tmp_path):
     f1 = tmp_path / "movie"
     with pytest.raises(RuntimeError):
         createMovie(
```

### Comparing `hvpy-1.0.1/hvpy/tests/test_io.py` & `hvpy-1.1.0/hvpy/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `hvpy-1.0.1/hvpy/tests/test_utils.py` & `hvpy-1.1.0/hvpy/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `hvpy-1.0.1/hvpy/utils.py` & `hvpy-1.1.0/hvpy/utils.py`

 * *Files identical despite different names*

### Comparing `hvpy-1.0.1/hvpy.egg-info/PKG-INFO` & `hvpy-1.1.0/hvpy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hvpy
-Version: 1.0.1
+Version: 1.1.0
 Summary: Helioviewer Python API Wrapper
 Home-page: https://helioviewer.org/
 Author: The Helioviewer Project
 Author-email: contact@helioviewer.org
 License: BSD 2-Clause
 Keywords: solar physics,solar,science,sun,data,helioviewer
 Platform: any
@@ -14,14 +14,15 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.8
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: licenses/LICENSE.rst
 
 Helioviewer Python API Wrapper
```

### Comparing `hvpy-1.0.1/hvpy.egg-info/SOURCES.txt` & `hvpy-1.1.0/hvpy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 .readthedocs.yaml
 LICENSE
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
+.github/dependabot.yml
 .github/workflows/ci.yml
+.github/workflows/cron.yml
 docs/Makefile
 docs/api.rst
 docs/conf.py
 docs/dev_guide.rst
 docs/guide.rst
 docs/index.rst
 docs/installation.rst
```

### Comparing `hvpy-1.0.1/licenses/LICENSE.rst` & `hvpy-1.1.0/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `hvpy-1.0.1/licenses/TEMPLATE_LICENSE.rst` & `hvpy-1.1.0/licenses/TEMPLATE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `hvpy-1.0.1/setup.cfg` & `hvpy-1.1.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -18,33 +18,36 @@
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Scientific/Engineering :: Physics
 
 [options]
 zip_safe = True
 packages = find:
 include_package_data = True
 python_requires = >=3.8
 setup_requires = 
 	setuptools_scm
 install_requires = 
 	requests>=2.27.0
-	pydantic>=1.9.1
+	pydantic>=2.0.0
+	pydantic-settings>=2.0.0
 
 [options.extras_require]
 tests = 
 	pytest-astropy>=0.10
+	pytest-timeout
 	pytest>=6.0
 docs = 
-	sphinx<5.1.0
+	sphinx<6.0.0
 	sphinx-autodoc-typehints
 	sphinx-automodapi
 	sphinx-book-theme
 
 [tool:pytest]
 testpaths = "hvpy" "docs"
 norecursedirs = ".tox" "build" "docs[\/]_build" "docs[\/]generated" "*.egg-info" "examples" ".jupyter" ".history"
```

### Comparing `hvpy-1.0.1/setup.py` & `hvpy-1.1.0/setup.py`

 * *Files identical despite different names*


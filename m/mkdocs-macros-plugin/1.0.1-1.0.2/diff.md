# Comparing `tmp/mkdocs-macros-plugin-1.0.1.tar.gz` & `tmp/mkdocs-macros-plugin-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-macros-plugin-1.0.1.tar", last modified: Thu May 25 12:11:51 2023, max compression
+gzip compressed data, was "mkdocs-macros-plugin-1.0.2.tar", last modified: Wed Jul 12 10:57:08 2023, max compression
```

## Comparing `mkdocs-macros-plugin-1.0.1.tar` & `mkdocs-macros-plugin-1.0.2.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:51.000000 mkdocs-macros-plugin-1.0.1/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:26.000000 mkdocs-macros-plugin-1.0.1/.github/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:34.000000 mkdocs-macros-plugin-1.0.1/.github/workflows/
--rw-r--r--   0 laurent    (501) staff       (20)      457 2020-03-10 06:37:22.000000 mkdocs-macros-plugin-1.0.1/.github/workflows/greetings.yml
--rw-r--r--   0 laurent    (501) staff       (20)      423 2022-07-22 15:00:04.000000 mkdocs-macros-plugin-1.0.1/.gitignore
--rw-r--r--   0 laurent    (501) staff       (20)      601 2021-04-23 13:52:57.000000 mkdocs-macros-plugin-1.0.1/.readthedocs.yml
--rw-r--r--   0 laurent    (501) staff       (20)     4360 2023-04-23 11:03:28.000000 mkdocs-macros-plugin-1.0.1/CHANGELOG.md
--rw-r--r--   0 laurent    (501) staff       (20)     1134 2021-11-23 01:28:45.000000 mkdocs-macros-plugin-1.0.1/LICENSE.md
--rw-r--r--   0 laurent    (501) staff       (20)       64 2020-11-22 09:50:49.000000 mkdocs-macros-plugin-1.0.1/MANIFEST.in
--rw-r--r--   0 laurent    (501) staff       (20)     7462 2023-05-25 12:11:51.000000 mkdocs-macros-plugin-1.0.1/PKG-INFO
--rw-r--r--   0 laurent    (501) staff       (20)     6692 2022-07-22 15:00:04.000000 mkdocs-macros-plugin-1.0.1/README.md
--rw-r--r--   0 laurent    (501) staff       (20)   249520 2020-02-24 19:02:56.000000 mkdocs-macros-plugin-1.0.1/macros_info.png
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:38.000000 mkdocs-macros-plugin-1.0.1/mkdocs_macros/
--rw-rw-r--   0 laurent    (501) staff       (20)      234 2021-01-04 17:04:12.000000 mkdocs-macros-plugin-1.0.1/mkdocs_macros/__init__.py
--rw-r--r--   0 laurent    (501) staff       (20)    11781 2023-04-24 12:12:46.000000 mkdocs-macros-plugin-1.0.1/mkdocs_macros/context.py
--rw-r--r--   0 laurent    (501) staff       (20)     1073 2022-07-22 15:00:04.000000 mkdocs-macros-plugin-1.0.1/mkdocs_macros/errors.py
--rw-r--r--   0 laurent    (501) staff       (20)     1604 2023-04-22 15:06:54.000000 mkdocs-macros-plugin-1.0.1/mkdocs_macros/macros_info.md
--rw-r--r--   0 laurent    (501) staff       (20)    26748 2023-04-23 08:50:05.000000 mkdocs-macros-plugin-1.0.1/mkdocs_macros/plugin.py
--rwxr-xr-x   0 laurent    (501) staff       (20)     6562 2022-03-16 08:10:30.000000 mkdocs-macros-plugin-1.0.1/mkdocs_macros/util.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:42.000000 mkdocs-macros-plugin-1.0.1/mkdocs_macros_plugin.egg-info/
--rw-r--r--   0 laurent    (501) staff       (20)     7462 2023-05-25 12:11:24.000000 mkdocs-macros-plugin-1.0.1/mkdocs_macros_plugin.egg-info/PKG-INFO
--rw-r--r--   0 laurent    (501) staff       (20)     1759 2023-05-25 12:11:26.000000 mkdocs-macros-plugin-1.0.1/mkdocs_macros_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 laurent    (501) staff       (20)        1 2023-05-25 12:11:24.000000 mkdocs-macros-plugin-1.0.1/mkdocs_macros_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 laurent    (501) staff       (20)       60 2023-05-25 12:11:24.000000 mkdocs-macros-plugin-1.0.1/mkdocs_macros_plugin.egg-info/entry_points.txt
--rw-r--r--   0 laurent    (501) staff       (20)      132 2023-05-25 12:11:24.000000 mkdocs-macros-plugin-1.0.1/mkdocs_macros_plugin.egg-info/requires.txt
--rw-r--r--   0 laurent    (501) staff       (20)       14 2023-05-25 12:11:24.000000 mkdocs-macros-plugin-1.0.1/mkdocs_macros_plugin.egg-info/top_level.txt
--rw-r--r--   0 laurent    (501) staff       (20)       38 2023-05-25 12:11:51.000000 mkdocs-macros-plugin-1.0.1/setup.cfg
--rw-r--r--   0 laurent    (501) staff       (20)     1923 2023-05-25 12:05:14.000000 mkdocs-macros-plugin-1.0.1/setup.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:42.000000 mkdocs-macros-plugin-1.0.1/test/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:43.000000 mkdocs-macros-plugin-1.0.1/test/debug/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:43.000000 mkdocs-macros-plugin-1.0.1/test/debug/docs/
--rw-r--r--   0 laurent    (501) staff       (20)      129 2022-03-12 15:07:17.000000 mkdocs-macros-plugin-1.0.1/test/debug/docs/index.md
--rw-r--r--   0 laurent    (501) staff       (20)      223 2022-03-12 15:07:17.000000 mkdocs-macros-plugin-1.0.1/test/debug/mkdocs.yml
--rw-rw-r--   0 laurent    (501) staff       (20)     1277 2020-02-23 06:57:46.000000 mkdocs-macros-plugin-1.0.1/test/main_sample.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:44.000000 mkdocs-macros-plugin-1.0.1/test/module/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:44.000000 mkdocs-macros-plugin-1.0.1/test/module/docs/
--rw-r--r--   0 laurent    (501) staff       (20)      346 2022-03-25 19:56:02.000000 mkdocs-macros-plugin-1.0.1/test/module/docs/environment.md
--rw-r--r--   0 laurent    (501) staff       (20)     2372 2022-03-16 08:05:31.000000 mkdocs-macros-plugin-1.0.1/test/module/docs/index.md
--rw-r--r--   0 laurent    (501) staff       (20)      357 2021-04-21 16:34:52.000000 mkdocs-macros-plugin-1.0.1/test/module/docs/literal.md
--rw-r--r--   0 laurent    (501) staff       (20)      128 2020-05-15 07:15:24.000000 mkdocs-macros-plugin-1.0.1/test/module/docs/other.md
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:45.000000 mkdocs-macros-plugin-1.0.1/test/module/include/
--rw-r--r--   0 laurent    (501) staff       (20)       68 2021-06-19 05:35:28.000000 mkdocs-macros-plugin-1.0.1/test/module/include/foo.md
--rw-r--r--   0 laurent    (501) staff       (20)     2023 2023-04-23 08:53:11.000000 mkdocs-macros-plugin-1.0.1/test/module/main.py
--rw-r--r--   0 laurent    (501) staff       (20)      498 2022-03-25 19:55:51.000000 mkdocs-macros-plugin-1.0.1/test/module/mkdocs.yml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:45.000000 mkdocs-macros-plugin-1.0.1/test/module_dir/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:46.000000 mkdocs-macros-plugin-1.0.1/test/module_dir/docs/
--rw-r--r--   0 laurent    (501) staff       (20)      237 2022-03-25 19:54:47.000000 mkdocs-macros-plugin-1.0.1/test/module_dir/docs/environment.md
--rw-r--r--   0 laurent    (501) staff       (20)      529 2020-09-25 16:29:39.000000 mkdocs-macros-plugin-1.0.1/test/module_dir/docs/index.md
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:46.000000 mkdocs-macros-plugin-1.0.1/test/module_dir/include/
--rw-r--r--   0 laurent    (501) staff       (20)       68 2020-03-02 21:15:58.000000 mkdocs-macros-plugin-1.0.1/test/module_dir/include/foo.md
--rw-r--r--   0 laurent    (501) staff       (20)      281 2020-09-25 16:31:43.000000 mkdocs-macros-plugin-1.0.1/test/module_dir/mkdocs.yml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:46.000000 mkdocs-macros-plugin-1.0.1/test/module_dir/mymodule/
--rw-r--r--   0 laurent    (501) staff       (20)      685 2021-06-19 08:12:07.000000 mkdocs-macros-plugin-1.0.1/test/module_dir/mymodule/__init__.py
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:47.000000 mkdocs-macros-plugin-1.0.1/test/new_syntax/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:47.000000 mkdocs-macros-plugin-1.0.1/test/new_syntax/docs/
--rw-r--r--   0 laurent    (501) staff       (20)      160 2020-09-28 06:50:54.000000 mkdocs-macros-plugin-1.0.1/test/new_syntax/docs/index.md
--rw-r--r--   0 laurent    (501) staff       (20)      138 2020-03-22 11:26:31.000000 mkdocs-macros-plugin-1.0.1/test/new_syntax/main.py
--rw-r--r--   0 laurent    (501) staff       (20)      336 2020-09-28 06:42:49.000000 mkdocs-macros-plugin-1.0.1/test/new_syntax/mkdocs.yml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:48.000000 mkdocs-macros-plugin-1.0.1/test/opt-in/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:48.000000 mkdocs-macros-plugin-1.0.1/test/opt-in/docs/
--rw-r--r--   0 laurent    (501) staff       (20)       62 2023-04-22 10:48:15.000000 mkdocs-macros-plugin-1.0.1/test/opt-in/docs/index.md
--rw-r--r--   0 laurent    (501) staff       (20)       93 2023-04-22 10:49:04.000000 mkdocs-macros-plugin-1.0.1/test/opt-in/docs/page_with_macros.md
--rw-r--r--   0 laurent    (501) staff       (20)      257 2023-04-22 13:36:25.000000 mkdocs-macros-plugin-1.0.1/test/opt-in/mkdocs.yml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:48.000000 mkdocs-macros-plugin-1.0.1/test/opt-out/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:48.000000 mkdocs-macros-plugin-1.0.1/test/opt-out/docs/
--rw-r--r--   0 laurent    (501) staff       (20)      160 2023-04-22 11:13:20.000000 mkdocs-macros-plugin-1.0.1/test/opt-out/docs/index.md
--rw-r--r--   0 laurent    (501) staff       (20)       93 2023-04-22 10:49:04.000000 mkdocs-macros-plugin-1.0.1/test/opt-out/docs/page_with_macros.md
--rw-r--r--   0 laurent    (501) staff       (20)      255 2023-04-22 13:35:37.000000 mkdocs-macros-plugin-1.0.1/test/opt-out/mkdocs.yml
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:48.000000 mkdocs-macros-plugin-1.0.1/test/simple/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:48.000000 mkdocs-macros-plugin-1.0.1/test/simple/docs/
--rw-r--r--   0 laurent    (501) staff       (20)       21 2020-03-04 11:55:35.000000 mkdocs-macros-plugin-1.0.1/test/simple/docs/index.md
--rw-r--r--   0 laurent    (501) staff       (20)      138 2020-09-15 20:07:40.000000 mkdocs-macros-plugin-1.0.1/test/simple/main_old.py
--rw-r--r--   0 laurent    (501) staff       (20)       92 2020-02-24 18:30:04.000000 mkdocs-macros-plugin-1.0.1/test/simple/mkdocs.yml
--rwxr-xr-x   0 laurent    (501) staff       (20)     1119 2020-10-03 09:23:32.000000 mkdocs-macros-plugin-1.0.1/update_pypi.sh
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:49.000000 mkdocs-macros-plugin-1.0.1/webdoc/
-drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-05-25 12:11:51.000000 mkdocs-macros-plugin-1.0.1/webdoc/docs/
--rw-r--r--   0 laurent    (501) staff       (20)     7677 2023-04-24 07:59:08.000000 mkdocs-macros-plugin-1.0.1/webdoc/docs/advanced.md
--rw-r--r--   0 laurent    (501) staff       (20)       50 2021-04-23 09:53:10.000000 mkdocs-macros-plugin-1.0.1/webdoc/docs/changelog.md
--rw-r--r--   0 laurent    (501) staff       (20)     2338 2021-04-24 11:27:05.000000 mkdocs-macros-plugin-1.0.1/webdoc/docs/contribute.md
--rw-r--r--   0 laurent    (501) staff       (20)    23462 2020-05-15 08:53:26.000000 mkdocs-macros-plugin-1.0.1/webdoc/docs/dog-eating.jpg
--rw-r--r--   0 laurent    (501) staff       (20)     3998 2022-01-26 01:22:27.000000 mkdocs-macros-plugin-1.0.1/webdoc/docs/git_info.md
--rw-r--r--   0 laurent    (501) staff       (20)      960 2021-11-23 01:28:45.000000 mkdocs-macros-plugin-1.0.1/webdoc/docs/help.md
--rw-r--r--   0 laurent    (501) staff       (20)     9232 2023-04-24 07:30:46.000000 mkdocs-macros-plugin-1.0.1/webdoc/docs/index.md
--rw-r--r--   0 laurent    (501) staff       (20)     1081 2020-03-10 08:29:58.000000 mkdocs-macros-plugin-1.0.1/webdoc/docs/license.md
--rw-r--r--   0 laurent    (501) staff       (20)    13954 2023-04-23 09:30:47.000000 mkdocs-macros-plugin-1.0.1/webdoc/docs/macros.md
--rw-r--r--   0 laurent    (501) staff       (20)   249520 2020-03-10 08:57:11.000000 mkdocs-macros-plugin-1.0.1/webdoc/docs/macros_info.png
--rw-r--r--   0 laurent    (501) staff       (20)     6724 2023-04-22 15:25:41.000000 mkdocs-macros-plugin-1.0.1/webdoc/docs/pages.md
--rw-r--r--   0 laurent    (501) staff       (20)     5693 2021-09-09 06:43:39.000000 mkdocs-macros-plugin-1.0.1/webdoc/docs/pluglets.md
--rw-r--r--   0 laurent    (501) staff       (20)    10756 2023-04-23 11:02:22.000000 mkdocs-macros-plugin-1.0.1/webdoc/docs/post_production.md
--rw-r--r--   0 laurent    (501) staff       (20)     9834 2023-04-23 14:23:38.000000 mkdocs-macros-plugin-1.0.1/webdoc/docs/rendering.md
--rw-r--r--   0 laurent    (501) staff       (20)     7974 2021-04-19 13:34:36.000000 mkdocs-macros-plugin-1.0.1/webdoc/docs/tips.md
--rw-r--r--   0 laurent    (501) staff       (20)    10171 2023-04-23 19:17:25.000000 mkdocs-macros-plugin-1.0.1/webdoc/docs/troubleshooting.md
--rw-r--r--   0 laurent    (501) staff       (20)     7478 2022-01-26 01:35:47.000000 mkdocs-macros-plugin-1.0.1/webdoc/docs/why.md
--rw-r--r--   0 laurent    (501) staff       (20)       51 2021-04-23 13:51:49.000000 mkdocs-macros-plugin-1.0.1/webdoc/extra_requirements.txt
--rw-r--r--   0 laurent    (501) staff       (20)     1383 2023-04-23 14:27:56.000000 mkdocs-macros-plugin-1.0.1/webdoc/mkdocs.yml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:08.000000 mkdocs-macros-plugin-1.0.2/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:07.000000 mkdocs-macros-plugin-1.0.2/.github/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:07.000000 mkdocs-macros-plugin-1.0.2/.github/workflows/
+-rw-r--r--   0 laurent    (501) staff       (20)      457 2020-03-10 06:37:22.000000 mkdocs-macros-plugin-1.0.2/.github/workflows/greetings.yml
+-rw-r--r--   0 laurent    (501) staff       (20)      423 2022-07-22 15:00:04.000000 mkdocs-macros-plugin-1.0.2/.gitignore
+-rw-r--r--   0 laurent    (501) staff       (20)      601 2021-04-23 13:52:57.000000 mkdocs-macros-plugin-1.0.2/.readthedocs.yml
+-rw-r--r--   0 laurent    (501) staff       (20)     4611 2023-07-02 17:49:04.000000 mkdocs-macros-plugin-1.0.2/CHANGELOG.md
+-rw-r--r--   0 laurent    (501) staff       (20)     1134 2021-11-23 01:28:45.000000 mkdocs-macros-plugin-1.0.2/LICENSE.md
+-rw-r--r--   0 laurent    (501) staff       (20)       64 2020-11-22 09:50:49.000000 mkdocs-macros-plugin-1.0.2/MANIFEST.in
+-rw-r--r--   0 laurent    (501) staff       (20)     7462 2023-07-12 10:57:08.000000 mkdocs-macros-plugin-1.0.2/PKG-INFO
+-rw-r--r--   0 laurent    (501) staff       (20)     6692 2022-07-22 15:00:04.000000 mkdocs-macros-plugin-1.0.2/README.md
+-rw-r--r--   0 laurent    (501) staff       (20)   249520 2020-02-24 19:02:56.000000 mkdocs-macros-plugin-1.0.2/macros_info.png
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:07.000000 mkdocs-macros-plugin-1.0.2/mkdocs_macros/
+-rw-rw-r--   0 laurent    (501) staff       (20)      234 2021-01-04 17:04:12.000000 mkdocs-macros-plugin-1.0.2/mkdocs_macros/__init__.py
+-rw-r--r--   0 laurent    (501) staff       (20)    11781 2023-07-03 06:44:13.000000 mkdocs-macros-plugin-1.0.2/mkdocs_macros/context.py
+-rw-r--r--   0 laurent    (501) staff       (20)     1073 2022-07-22 15:00:04.000000 mkdocs-macros-plugin-1.0.2/mkdocs_macros/errors.py
+-rw-r--r--   0 laurent    (501) staff       (20)     1604 2023-04-22 15:06:54.000000 mkdocs-macros-plugin-1.0.2/mkdocs_macros/macros_info.md
+-rw-r--r--   0 laurent    (501) staff       (20)    27055 2023-07-02 14:52:08.000000 mkdocs-macros-plugin-1.0.2/mkdocs_macros/plugin.py
+-rwxr-xr-x   0 laurent    (501) staff       (20)     6562 2022-03-16 08:10:30.000000 mkdocs-macros-plugin-1.0.2/mkdocs_macros/util.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:07.000000 mkdocs-macros-plugin-1.0.2/mkdocs_macros_plugin.egg-info/
+-rw-r--r--   0 laurent    (501) staff       (20)     7462 2023-07-12 10:57:04.000000 mkdocs-macros-plugin-1.0.2/mkdocs_macros_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 laurent    (501) staff       (20)     1759 2023-07-12 10:57:07.000000 mkdocs-macros-plugin-1.0.2/mkdocs_macros_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 laurent    (501) staff       (20)        1 2023-07-12 10:57:05.000000 mkdocs-macros-plugin-1.0.2/mkdocs_macros_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 laurent    (501) staff       (20)       60 2023-07-12 10:57:05.000000 mkdocs-macros-plugin-1.0.2/mkdocs_macros_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 laurent    (501) staff       (20)      132 2023-07-12 10:57:05.000000 mkdocs-macros-plugin-1.0.2/mkdocs_macros_plugin.egg-info/requires.txt
+-rw-r--r--   0 laurent    (501) staff       (20)       14 2023-07-12 10:57:05.000000 mkdocs-macros-plugin-1.0.2/mkdocs_macros_plugin.egg-info/top_level.txt
+-rw-r--r--   0 laurent    (501) staff       (20)       38 2023-07-12 10:57:08.000000 mkdocs-macros-plugin-1.0.2/setup.cfg
+-rw-r--r--   0 laurent    (501) staff       (20)     1923 2023-07-02 17:49:16.000000 mkdocs-macros-plugin-1.0.2/setup.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:07.000000 mkdocs-macros-plugin-1.0.2/test/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:07.000000 mkdocs-macros-plugin-1.0.2/test/debug/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:07.000000 mkdocs-macros-plugin-1.0.2/test/debug/docs/
+-rw-r--r--   0 laurent    (501) staff       (20)      129 2022-03-12 15:07:17.000000 mkdocs-macros-plugin-1.0.2/test/debug/docs/index.md
+-rw-r--r--   0 laurent    (501) staff       (20)      223 2022-03-12 15:07:17.000000 mkdocs-macros-plugin-1.0.2/test/debug/mkdocs.yml
+-rw-rw-r--   0 laurent    (501) staff       (20)     1277 2020-02-23 06:57:46.000000 mkdocs-macros-plugin-1.0.2/test/main_sample.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:07.000000 mkdocs-macros-plugin-1.0.2/test/module/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:07.000000 mkdocs-macros-plugin-1.0.2/test/module/docs/
+-rw-r--r--   0 laurent    (501) staff       (20)      361 2023-07-02 09:57:52.000000 mkdocs-macros-plugin-1.0.2/test/module/docs/environment.md
+-rw-r--r--   0 laurent    (501) staff       (20)     2372 2023-07-02 09:55:13.000000 mkdocs-macros-plugin-1.0.2/test/module/docs/index.md
+-rw-r--r--   0 laurent    (501) staff       (20)      357 2021-04-21 16:34:52.000000 mkdocs-macros-plugin-1.0.2/test/module/docs/literal.md
+-rw-r--r--   0 laurent    (501) staff       (20)      165 2023-07-02 13:51:07.000000 mkdocs-macros-plugin-1.0.2/test/module/docs/other.md
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:07.000000 mkdocs-macros-plugin-1.0.2/test/module/include/
+-rw-r--r--   0 laurent    (501) staff       (20)       68 2021-06-19 05:35:28.000000 mkdocs-macros-plugin-1.0.2/test/module/include/foo.md
+-rw-r--r--   0 laurent    (501) staff       (20)     2023 2023-04-23 08:53:11.000000 mkdocs-macros-plugin-1.0.2/test/module/main.py
+-rw-r--r--   0 laurent    (501) staff       (20)      518 2023-07-02 10:41:31.000000 mkdocs-macros-plugin-1.0.2/test/module/mkdocs.yml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:08.000000 mkdocs-macros-plugin-1.0.2/test/module_dir/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:08.000000 mkdocs-macros-plugin-1.0.2/test/module_dir/docs/
+-rw-r--r--   0 laurent    (501) staff       (20)      237 2022-03-25 19:54:47.000000 mkdocs-macros-plugin-1.0.2/test/module_dir/docs/environment.md
+-rw-r--r--   0 laurent    (501) staff       (20)      529 2023-07-02 09:54:23.000000 mkdocs-macros-plugin-1.0.2/test/module_dir/docs/index.md
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:08.000000 mkdocs-macros-plugin-1.0.2/test/module_dir/include/
+-rw-r--r--   0 laurent    (501) staff       (20)       68 2020-03-02 21:15:58.000000 mkdocs-macros-plugin-1.0.2/test/module_dir/include/foo.md
+-rw-r--r--   0 laurent    (501) staff       (20)      281 2020-09-25 16:31:43.000000 mkdocs-macros-plugin-1.0.2/test/module_dir/mkdocs.yml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:08.000000 mkdocs-macros-plugin-1.0.2/test/module_dir/mymodule/
+-rw-r--r--   0 laurent    (501) staff       (20)      685 2021-06-19 08:12:07.000000 mkdocs-macros-plugin-1.0.2/test/module_dir/mymodule/__init__.py
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:08.000000 mkdocs-macros-plugin-1.0.2/test/new_syntax/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:08.000000 mkdocs-macros-plugin-1.0.2/test/new_syntax/docs/
+-rw-r--r--   0 laurent    (501) staff       (20)      160 2020-09-28 06:50:54.000000 mkdocs-macros-plugin-1.0.2/test/new_syntax/docs/index.md
+-rw-r--r--   0 laurent    (501) staff       (20)      138 2020-03-22 11:26:31.000000 mkdocs-macros-plugin-1.0.2/test/new_syntax/main.py
+-rw-r--r--   0 laurent    (501) staff       (20)      336 2020-09-28 06:42:49.000000 mkdocs-macros-plugin-1.0.2/test/new_syntax/mkdocs.yml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:08.000000 mkdocs-macros-plugin-1.0.2/test/opt-in/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:08.000000 mkdocs-macros-plugin-1.0.2/test/opt-in/docs/
+-rw-r--r--   0 laurent    (501) staff       (20)       62 2023-04-22 10:48:15.000000 mkdocs-macros-plugin-1.0.2/test/opt-in/docs/index.md
+-rw-r--r--   0 laurent    (501) staff       (20)       93 2023-04-22 10:49:04.000000 mkdocs-macros-plugin-1.0.2/test/opt-in/docs/page_with_macros.md
+-rw-r--r--   0 laurent    (501) staff       (20)      257 2023-04-22 13:36:25.000000 mkdocs-macros-plugin-1.0.2/test/opt-in/mkdocs.yml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:08.000000 mkdocs-macros-plugin-1.0.2/test/opt-out/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:08.000000 mkdocs-macros-plugin-1.0.2/test/opt-out/docs/
+-rw-r--r--   0 laurent    (501) staff       (20)      160 2023-04-22 11:13:20.000000 mkdocs-macros-plugin-1.0.2/test/opt-out/docs/index.md
+-rw-r--r--   0 laurent    (501) staff       (20)       93 2023-04-22 10:49:04.000000 mkdocs-macros-plugin-1.0.2/test/opt-out/docs/page_with_macros.md
+-rw-r--r--   0 laurent    (501) staff       (20)      255 2023-04-22 13:35:37.000000 mkdocs-macros-plugin-1.0.2/test/opt-out/mkdocs.yml
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:08.000000 mkdocs-macros-plugin-1.0.2/test/simple/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:08.000000 mkdocs-macros-plugin-1.0.2/test/simple/docs/
+-rw-r--r--   0 laurent    (501) staff       (20)       21 2020-03-04 11:55:35.000000 mkdocs-macros-plugin-1.0.2/test/simple/docs/index.md
+-rw-r--r--   0 laurent    (501) staff       (20)      138 2020-09-15 20:07:40.000000 mkdocs-macros-plugin-1.0.2/test/simple/main_old.py
+-rw-r--r--   0 laurent    (501) staff       (20)       92 2020-02-24 18:30:04.000000 mkdocs-macros-plugin-1.0.2/test/simple/mkdocs.yml
+-rwxr-xr-x   0 laurent    (501) staff       (20)     1119 2020-10-03 09:23:32.000000 mkdocs-macros-plugin-1.0.2/update_pypi.sh
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:08.000000 mkdocs-macros-plugin-1.0.2/webdoc/
+drwxr-xr-x   0 laurent    (501) staff       (20)        0 2023-07-12 10:57:08.000000 mkdocs-macros-plugin-1.0.2/webdoc/docs/
+-rw-r--r--   0 laurent    (501) staff       (20)     7677 2023-04-24 07:59:08.000000 mkdocs-macros-plugin-1.0.2/webdoc/docs/advanced.md
+-rw-r--r--   0 laurent    (501) staff       (20)       50 2021-04-23 09:53:10.000000 mkdocs-macros-plugin-1.0.2/webdoc/docs/changelog.md
+-rw-r--r--   0 laurent    (501) staff       (20)     2338 2021-04-24 11:27:05.000000 mkdocs-macros-plugin-1.0.2/webdoc/docs/contribute.md
+-rw-r--r--   0 laurent    (501) staff       (20)    23462 2020-05-15 08:53:26.000000 mkdocs-macros-plugin-1.0.2/webdoc/docs/dog-eating.jpg
+-rw-r--r--   0 laurent    (501) staff       (20)     3998 2022-01-26 01:22:27.000000 mkdocs-macros-plugin-1.0.2/webdoc/docs/git_info.md
+-rw-r--r--   0 laurent    (501) staff       (20)      960 2021-11-23 01:28:45.000000 mkdocs-macros-plugin-1.0.2/webdoc/docs/help.md
+-rw-r--r--   0 laurent    (501) staff       (20)     9232 2023-04-24 07:30:46.000000 mkdocs-macros-plugin-1.0.2/webdoc/docs/index.md
+-rw-r--r--   0 laurent    (501) staff       (20)     1081 2020-03-10 08:29:58.000000 mkdocs-macros-plugin-1.0.2/webdoc/docs/license.md
+-rw-r--r--   0 laurent    (501) staff       (20)    13954 2023-04-23 09:30:47.000000 mkdocs-macros-plugin-1.0.2/webdoc/docs/macros.md
+-rw-r--r--   0 laurent    (501) staff       (20)   249520 2020-03-10 08:57:11.000000 mkdocs-macros-plugin-1.0.2/webdoc/docs/macros_info.png
+-rw-r--r--   0 laurent    (501) staff       (20)     7420 2023-07-03 05:17:35.000000 mkdocs-macros-plugin-1.0.2/webdoc/docs/pages.md
+-rw-r--r--   0 laurent    (501) staff       (20)     5693 2021-09-09 06:43:39.000000 mkdocs-macros-plugin-1.0.2/webdoc/docs/pluglets.md
+-rw-r--r--   0 laurent    (501) staff       (20)    10756 2023-04-23 11:02:22.000000 mkdocs-macros-plugin-1.0.2/webdoc/docs/post_production.md
+-rw-r--r--   0 laurent    (501) staff       (20)     9834 2023-04-23 14:23:38.000000 mkdocs-macros-plugin-1.0.2/webdoc/docs/rendering.md
+-rw-r--r--   0 laurent    (501) staff       (20)     8741 2023-07-02 18:14:07.000000 mkdocs-macros-plugin-1.0.2/webdoc/docs/tips.md
+-rw-r--r--   0 laurent    (501) staff       (20)    10171 2023-04-23 19:17:25.000000 mkdocs-macros-plugin-1.0.2/webdoc/docs/troubleshooting.md
+-rw-r--r--   0 laurent    (501) staff       (20)     7478 2022-01-26 01:35:47.000000 mkdocs-macros-plugin-1.0.2/webdoc/docs/why.md
+-rw-r--r--   0 laurent    (501) staff       (20)       51 2021-04-23 13:51:49.000000 mkdocs-macros-plugin-1.0.2/webdoc/extra_requirements.txt
+-rw-r--r--   0 laurent    (501) staff       (20)     1383 2023-04-23 14:27:56.000000 mkdocs-macros-plugin-1.0.2/webdoc/mkdocs.yml
```

### Comparing `mkdocs-macros-plugin-1.0.1/.readthedocs.yml` & `mkdocs-macros-plugin-1.0.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.1/CHANGELOG.md` & `mkdocs-macros-plugin-1.0.2/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 # Changelog: mkdocs-macros
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/) and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
-## 1.1.0-alpha, 2024-04-23
+## 1.0.2, 2023-07-02
+* Added: it is now possible to use macros in page titles, in the
+    nav section of the yaml file, or in the level 1 titles; 
+    the macros are correctly interpreted in the navigation part
+    of the page.
+
+## 1.0.1, 2023-05-25
+
+## 1.0.0-alpha, 2023-04-23
 
 * Improved user guide, with introduction of two new pages:
     "Controlling macro rendering" and "Post production".
 
 * Fixed: (#158) In modules, `on_pre_page_macros()`, the `env.markdown` 
     attribute is now available to create a header or footer.
```

### Comparing `mkdocs-macros-plugin-1.0.1/LICENSE.md` & `mkdocs-macros-plugin-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.1/PKG-INFO` & `mkdocs-macros-plugin-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-macros-plugin
-Version: 1.0.1
+Version: 1.0.2
 Summary: Unleash the power of MkDocs with macros and variables
 Home-page: https://github.com/fralau/mkdocs_macros_plugin
 Author: Laurent Franceschbetti
 Author-email: info@settlenext.com
 License: MIT
 Keywords: mkdocs python markdown macros
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mkdocs-macros-plugin-1.0.1/README.md` & `mkdocs-macros-plugin-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.1/macros_info.png` & `mkdocs-macros-plugin-1.0.2/macros_info.png`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.1/mkdocs_macros/context.py` & `mkdocs-macros-plugin-1.0.2/mkdocs_macros/context.py`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.1/mkdocs_macros/errors.py` & `mkdocs-macros-plugin-1.0.2/mkdocs_macros/errors.py`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.1/mkdocs_macros/macros_info.md` & `mkdocs-macros-plugin-1.0.2/mkdocs_macros/macros_info.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.1/mkdocs_macros/plugin.py` & `mkdocs-macros-plugin-1.0.2/mkdocs_macros/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -484,15 +484,19 @@
         """
 
         # Process meta_variables
         # ----------------------
         # copy the page variables and update with the meta data
         # in the YAML header:
         page_variables = copy(self.variables)
-        meta_variables = self.variables['page'].meta
+        try:
+            meta_variables = self.variables['page'].meta
+        except KeyError as e:
+            # this is a premature rendering, no meta variables in the page
+            meta_variables = {}
         # Warning this is ternary logique (True, False, None: nothing said)
         ignore_macros = None
         render_macros = None
         
         if meta_variables:
             # determine whether the page will be rendered or not
             # the two formulations are accepted
@@ -714,14 +718,18 @@
             for func in self.pre_macro_functions:
                 func(self)
             # render the macros
             self.markdown = self.render(
                 markdown=self.markdown,
                 # page=page,
             )
+            # Convert macros in the title from render (if exists)
+            # to answer 144
+            page.title = self.render(markdown=page.title)
+
             # execute the post-macro functions in the various modules
             for func in self.post_macro_functions:
                 func(self)
             return self.markdown
 
     def on_post_build(self, config: config_options.Config):
         """
```

### Comparing `mkdocs-macros-plugin-1.0.1/mkdocs_macros/util.py` & `mkdocs-macros-plugin-1.0.2/mkdocs_macros/util.py`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.1/mkdocs_macros_plugin.egg-info/PKG-INFO` & `mkdocs-macros-plugin-1.0.2/mkdocs_macros_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-macros-plugin
-Version: 1.0.1
+Version: 1.0.2
 Summary: Unleash the power of MkDocs with macros and variables
 Home-page: https://github.com/fralau/mkdocs_macros_plugin
 Author: Laurent Franceschbetti
 Author-email: info@settlenext.com
 License: MIT
 Keywords: mkdocs python markdown macros
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mkdocs-macros-plugin-1.0.1/mkdocs_macros_plugin.egg-info/SOURCES.txt` & `mkdocs-macros-plugin-1.0.2/mkdocs_macros_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.1/setup.py` & `mkdocs-macros-plugin-1.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from setuptools import setup, find_packages
 
 
 # --------------------
 # Initialization
 # --------------------
 
-VERSION_NUMBER = '1.0.1'
+VERSION_NUMBER = '1.0.2'
 
 # required if you want to run document/test
 # pip install 'mkdocs-macros-plugin[test]'
 TEST_REQUIRE = ['mkdocs-macros-test', 'mkdocs-material>=6.2',
                 'mkdocs-include-markdown-plugin']
 
 # --------------------
```

### Comparing `mkdocs-macros-plugin-1.0.1/test/main_sample.py` & `mkdocs-macros-plugin-1.0.2/test/main_sample.py`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.1/test/module/docs/index.md` & `mkdocs-macros-plugin-1.0.2/test/module/docs/index.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.1/test/module/main.py` & `mkdocs-macros-plugin-1.0.2/test/module/main.py`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.1/test/module_dir/docs/index.md` & `mkdocs-macros-plugin-1.0.2/test/module_dir/docs/index.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.1/test/module_dir/mymodule/__init__.py` & `mkdocs-macros-plugin-1.0.2/test/module_dir/mymodule/__init__.py`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.1/update_pypi.sh` & `mkdocs-macros-plugin-1.0.2/update_pypi.sh`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.1/webdoc/docs/advanced.md` & `mkdocs-macros-plugin-1.0.2/webdoc/docs/advanced.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.1/webdoc/docs/contribute.md` & `mkdocs-macros-plugin-1.0.2/webdoc/docs/contribute.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.1/webdoc/docs/dog-eating.jpg` & `mkdocs-macros-plugin-1.0.2/webdoc/docs/dog-eating.jpg`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.1/webdoc/docs/git_info.md` & `mkdocs-macros-plugin-1.0.2/webdoc/docs/git_info.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.1/webdoc/docs/help.md` & `mkdocs-macros-plugin-1.0.2/webdoc/docs/help.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.1/webdoc/docs/index.md` & `mkdocs-macros-plugin-1.0.2/webdoc/docs/index.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.1/webdoc/docs/license.md` & `mkdocs-macros-plugin-1.0.2/webdoc/docs/license.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.1/webdoc/docs/macros.md` & `mkdocs-macros-plugin-1.0.2/webdoc/docs/macros.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.1/webdoc/docs/macros_info.png` & `mkdocs-macros-plugin-1.0.2/webdoc/docs/macros_info.png`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.1/webdoc/docs/pages.md` & `mkdocs-macros-plugin-1.0.2/webdoc/docs/pages.md`

 * *Files 3% similar despite different names*

```diff
@@ -86,14 +86,16 @@
 The price of the product is {{ price }}.
 
 See [more information on the website]({{ company.website }}).
 
 See <a href="{{ company.website }}">more information on the website</a>.
 ```
 
+!!! Note "Literals"
+    Only literals (strings or numbers) can be used in the `extra` section.
 
 Local (page-level) variables and macros
 ---------------------------------------
 
 If you really need a variable or macro that needs to remain **local** to
 the markdown page, you can use a standard Jinja2 declaration.
 
@@ -119,22 +121,33 @@
 
 Then you can access the content of the YAML header in two ways:
 
 1. By name e.g. `{{ title }}` and `{{ bottles.whine }}`
 1. Explicitly, i.e. using the dot notation, e.g. 
 `{{ page.meta.title }}` and `{{ page.meta.bottles.whine }}`.
 
+If used, the `title` variable will be used for the page's title and
+in the navigation of the website (unless specified in the config file). It does not alter the content of the page itself. 
 
+!!! Note "Literals or macros"
+    Only use literals in the header (strings or numbers).
 
-!!! Tip
+    _As of 1.0.2_ The only exception is the `title` field: macros used there will be rendered just after the page content itself.
+    E.g. (supposing that product_name is an existing variable):
+    
+    ```
+    title: Description of {{ product_name }}
+    ```
+
+!!! Tip "Displaying the content of variables"
     `{{ page.meta }}` gives the content of the header.
     If you wish to have it typed in a nice tabular form, you can use:
     `{{ context(page.meta) | pretty }}`
 
-!!! Warning "Caution"
+!!! Warning "Caution: overwriting variables"
     If variables in the metadata have the same name as variables
     already defined (suche as `extra`, `config`, etc.) those will
     be overwritten, but for this page only.
 
 ### Using the `set` keyword
 
 Variables can be defined in the template with the `set` keyword, e.g.:
```

#### html2text {}

```diff
@@ -35,43 +35,51 @@
 Python module To discover what each of these objects contain, you can use the
 `pretty` filter provided with the plugin, e.g.: {{ context(page) | pretty }}
 Configuration variables ----------------------- To easily and quickly define
 custom variables, declare them in you `mkdocs.yml` file: ``` {.yaml} extra:
 price: 12.50 company: name: Acme address: .... website: www.acme.com ``` In
 your markdown file: ``` {.markdown} The price of the product is {{ price }}.
 See [more information on the website]({{ company.website }}). See more
-information_on_the_website. ``` Local (page-level) variables and macros -------
--------------------------------- If you really need a variable or macro that
-needs to remain **local** to the markdown page, you can use a standard Jinja2
-declaration. !!! Warning Note that the `context()` macro (for listing
-variables) will **not** display variables defined at page level. ### In the
-YAML header of the page Variables defined in the YAML header of the page are
-accessible as themselves and via the `page.meta` object. For example, if the
-the header is as follows: ```yaml --- title: My special title bottles: whine:
-500 beer: 123 --- ``` Then you can access the content of the YAML header in two
-ways: 1. By name e.g. `{{ title }}` and `{{ bottles.whine }}` 1. Explicitly,
-i.e. using the dot notation, e.g. `{{ page.meta.title }}` and `{
-{ page.meta.bottles.whine }}`. !!! Tip `{{ page.meta }}` gives the content of
-the header. If you wish to have it typed in a nice tabular form, you can use: `
-{{ context(page.meta) | pretty }}` !!! Warning "Caution" If variables in the
-metadata have the same name as variables already defined (suche as `extra`,
-`config`, etc.) those will be overwritten, but for this page only. ### Using
-the `set` keyword Variables can be defined in the template with the `set`
-keyword, e.g.: ``` {.jinja2} {% set acme = 'Acme Company Ltd' %} Please buy the
-great products from {{ acme }}! ``` Contrary to variables defined in the
-`extra` section of the `mkdocs.yml` file, they are accessible only within the
-specific page. They are not accessible from the python code. !!! Tip If you
-need reference information on the page, there is a `page` object e.g.: `{
-{ page.title }}`, `{{ page.url }}`, `{{ page.is_homepage }}`, etc. ### Page-
-level macros It is possible to write **Jinja2 macros** written with the Jinja2
-syntax (instead of a Python module). This allows you benefit from the power of
-that language for the manipulation of strings. Here is an example of Jinja2
-macro, from the official documentation: ``` {.jinja2} {% macro input(name,
-value='', type='text', size=20) -%} [Unknown INPUT type] {%- endmacro %} ```
-Which can be called (within the page) as: ``` {.jinja2}
+information_on_the_website. ``` !!! Note "Literals" Only literals (strings or
+numbers) can be used in the `extra` section. Local (page-level) variables and
+macros --------------------------------------- If you really need a variable or
+macro that needs to remain **local** to the markdown page, you can use a
+standard Jinja2 declaration. !!! Warning Note that the `context()` macro (for
+listing variables) will **not** display variables defined at page level. ### In
+the YAML header of the page Variables defined in the YAML header of the page
+are accessible as themselves and via the `page.meta` object. For example, if
+the the header is as follows: ```yaml --- title: My special title bottles:
+whine: 500 beer: 123 --- ``` Then you can access the content of the YAML header
+in two ways: 1. By name e.g. `{{ title }}` and `{{ bottles.whine }}` 1.
+Explicitly, i.e. using the dot notation, e.g. `{{ page.meta.title }}` and `{
+{ page.meta.bottles.whine }}`. If used, the `title` variable will be used for
+the page's title and in the navigation of the website (unless specified in the
+config file). It does not alter the content of the page itself. !!! Note
+"Literals or macros" Only use literals in the header (strings or numbers). _As
+of 1.0.2_ The only exception is the `title` field: macros used there will be
+rendered just after the page content itself. E.g. (supposing that product_name
+is an existing variable): ``` title: Description of {{ product_name }} ``` !!!
+Tip "Displaying the content of variables" `{{ page.meta }}` gives the content
+of the header. If you wish to have it typed in a nice tabular form, you can
+use: `{{ context(page.meta) | pretty }}` !!! Warning "Caution: overwriting
+variables" If variables in the metadata have the same name as variables already
+defined (suche as `extra`, `config`, etc.) those will be overwritten, but for
+this page only. ### Using the `set` keyword Variables can be defined in the
+template with the `set` keyword, e.g.: ``` {.jinja2} {% set acme = 'Acme
+Company Ltd' %} Please buy the great products from {{ acme }}! ``` Contrary to
+variables defined in the `extra` section of the `mkdocs.yml` file, they are
+accessible only within the specific page. They are not accessible from the
+python code. !!! Tip If you need reference information on the page, there is a
+`page` object e.g.: `{{ page.title }}`, `{{ page.url }}`, `{{ page.is_homepage
+}}`, etc. ### Page-level macros It is possible to write **Jinja2 macros**
+written with the Jinja2 syntax (instead of a Python module). This allows you
+benefit from the power of that language for the manipulation of strings. Here
+is an example of Jinja2 macro, from the official documentation: ``` {.jinja2}
+{% macro input(name, value='', type='text', size=20) -%} [Unknown INPUT type]
+{%- endmacro %} ``` Which can be called (within the page) as: ``` {.jinja2}
 {{ input('username') }}
 {{ input('password', type='password') }}
 ``` !!! Note All definitions will remain **local** to the page. It is possible
 to define Jinja2 macros in a separate file, and to import them from there in
 any page, using the `{% import ..}` directive. See explanations under [Advanced
 Usage](../advanced/#importing-macros-from-a-separate-file). Conditionals,
 loops, etc. ------------------------- With the macros plugin, you may use the
```

### Comparing `mkdocs-macros-plugin-1.0.1/webdoc/docs/pluglets.md` & `mkdocs-macros-plugin-1.0.2/webdoc/docs/pluglets.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.1/webdoc/docs/post_production.md` & `mkdocs-macros-plugin-1.0.2/webdoc/docs/post_production.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.1/webdoc/docs/rendering.md` & `mkdocs-macros-plugin-1.0.2/webdoc/docs/rendering.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.1/webdoc/docs/tips.md` & `mkdocs-macros-plugin-1.0.2/webdoc/docs/tips.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,37 @@
 Tips and Tricks
 ===============
 
+Can I use macros in page titles?
+--------------------------------
+_New in 1.0.2_
+
+Yes. You can use a macro in the title of the page in:
+
+1. The `nav` section of the config file 
+1. As the metadata `title` in the yaml header of the page.
+1. Directly as the header 1 of the page, e.g.  
+`#Environment at {{unit_price}}"`.
+
+For example, in `nav`section of the config file,
+e.g. 
+
+```yaml
+nav:
+    - Home: index.md
+    - Environment at {{ unit_price}}: environment.md
+    - Second:
+        - Also for {{ unit_price}}: other.md
+    - Not interpreted: literal.md
+```
+
+!!! Note "Rendering"
+    The macros in the title are rendered _just after_ those in the markdown
+    file. Hence they benefit from the whole context (variables, functions, filters) available in the page.
+
 How can I get the project's document directory?
 -------------------------------------
 
 This would be the main directory where the project's 
 markdown pages are located.
 
 From a markdown page:
```

### Comparing `mkdocs-macros-plugin-1.0.1/webdoc/docs/troubleshooting.md` & `mkdocs-macros-plugin-1.0.2/webdoc/docs/troubleshooting.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.1/webdoc/docs/why.md` & `mkdocs-macros-plugin-1.0.2/webdoc/docs/why.md`

 * *Files identical despite different names*

### Comparing `mkdocs-macros-plugin-1.0.1/webdoc/mkdocs.yml` & `mkdocs-macros-plugin-1.0.2/webdoc/mkdocs.yml`

 * *Files identical despite different names*


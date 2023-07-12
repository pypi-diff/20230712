# Comparing `tmp/nio-bot-1.0.0.tar.gz` & `tmp/nio-bot-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nio-bot-1.0.0.tar", last modified: Wed Jul 12 12:39:54 2023, max compression
+gzip compressed data, was "nio-bot-1.0.1.tar", last modified: Wed Jul 12 13:39:27 2023, max compression
```

## Comparing `nio-bot-1.0.0.tar` & `nio-bot-1.0.1.tar`

### file list

```diff
@@ -1,69 +1,70 @@
-drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 12:39:54.627895 nio-bot-1.0.0/
-drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 12:39:54.617895 nio-bot-1.0.0/.github/
-drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 12:39:54.617895 nio-bot-1.0.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 nex       (1000) nex       (1000)      797 2023-06-29 20:01:59.000000 nio-bot-1.0.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 nex       (1000) nex       (1000)      609 2023-06-29 20:01:59.000000 nio-bot-1.0.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 nex       (1000) nex       (1000)     7062 2023-07-12 12:39:09.000000 nio-bot-1.0.0/.gitignore
-drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 12:39:54.621229 nio-bot-1.0.0/.idea/
--rw-r--r--   0 nex       (1000) nex       (1000)      176 2023-06-08 18:22:57.000000 nio-bot-1.0.0/.idea/.gitignore
-drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 12:39:54.621229 nio-bot-1.0.0/.idea/inspectionProfiles/
--rw-r--r--   0 nex       (1000) nex       (1000)     3647 2023-06-08 18:25:30.000000 nio-bot-1.0.0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 nex       (1000) nex       (1000)      174 2023-06-08 18:25:30.000000 nio-bot-1.0.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 nex       (1000) nex       (1000)      185 2023-06-08 18:47:53.000000 nio-bot-1.0.0/.idea/markdown.xml
--rw-r--r--   0 nex       (1000) nex       (1000)      337 2023-06-08 18:25:30.000000 nio-bot-1.0.0/.idea/misc.xml
--rw-r--r--   0 nex       (1000) nex       (1000)      266 2023-06-08 18:25:30.000000 nio-bot-1.0.0/.idea/modules.xml
--rw-r--r--   0 nex       (1000) nex       (1000)      426 2023-06-13 20:35:20.000000 nio-bot-1.0.0/.idea/nio-bot.iml
--rw-r--r--   0 nex       (1000) nex       (1000)      180 2023-06-12 20:15:29.000000 nio-bot-1.0.0/.idea/vcs.xml
--rw-r--r--   0 nex       (1000) nex       (1000)    35149 2023-06-12 20:12:46.000000 nio-bot-1.0.0/LICENSE
--rw-r--r--   0 nex       (1000) nex       (1000)     8268 2023-07-12 12:39:54.627895 nio-bot-1.0.0/PKG-INFO
--rw-r--r--   0 nex       (1000) nex       (1000)     7969 2023-06-29 12:18:06.000000 nio-bot-1.0.0/README.md
-drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 12:39:54.621229 nio-bot-1.0.0/docs/
-drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 12:39:54.621229 nio-bot-1.0.0/docs/guides/
--rw-r--r--   0 nex       (1000) nex       (1000)    14023 2023-07-05 11:52:24.000000 nio-bot-1.0.0/docs/guides/getting-started.md
--rw-r--r--   0 nex       (1000) nex       (1000)     1412 2023-07-03 21:42:38.000000 nio-bot-1.0.0/docs/index.md
-drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 12:39:54.621229 nio-bot-1.0.0/docs/reference/
--rw-r--r--   0 nex       (1000) nex       (1000)       36 2023-07-04 10:54:58.000000 nio-bot-1.0.0/docs/reference/attachment.md
--rw-r--r--   0 nex       (1000) nex       (1000)       27 2023-07-11 19:15:48.000000 nio-bot-1.0.0/docs/reference/client.md
--rw-r--r--   0 nex       (1000) nex       (1000)      100 2023-07-03 19:05:59.000000 nio-bot-1.0.0/docs/reference/commands.md
--rw-r--r--   0 nex       (1000) nex       (1000)      708 2023-07-03 20:33:05.000000 nio-bot-1.0.0/docs/reference/context.md
--rw-r--r--   0 nex       (1000) nex       (1000)       35 2023-07-03 19:08:54.000000 nio-bot-1.0.0/docs/reference/exceptions.md
-drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 12:39:54.624562 nio-bot-1.0.0/docs/reference/utils/
--rw-r--r--   0 nex       (1000) nex       (1000)      229 2023-07-04 20:00:25.000000 nio-bot-1.0.0/docs/reference/utils/federation.md
--rw-r--r--   0 nex       (1000) nex       (1000)     2764 2023-07-03 21:01:45.000000 nio-bot-1.0.0/docs/reference/utils/help_command.md
--rw-r--r--   0 nex       (1000) nex       (1000)     2236 2023-07-04 09:49:11.000000 nio-bot-1.0.0/docs/reference/utils/parsers.md
--rw-r--r--   0 nex       (1000) nex       (1000)      707 2023-07-04 19:56:41.000000 nio-bot-1.0.0/docs/reference/utils/string_view.md
--rw-r--r--   0 nex       (1000) nex       (1000)     2346 2023-07-03 21:31:35.000000 nio-bot-1.0.0/docs/reference/utils/typing.md
--rw-r--r--   0 nex       (1000) nex       (1000)     1960 2023-07-04 10:48:38.000000 nio-bot-1.0.0/docs/reference/utils/unblock.md
-drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 12:39:54.624562 nio-bot-1.0.0/examples/
--rw-r--r--   0 nex       (1000) nex       (1000)     1636 2023-06-13 20:43:23.000000 nio-bot-1.0.0/examples/access_token.py
--rw-r--r--   0 nex       (1000) nex       (1000)     1605 2023-06-13 20:35:19.000000 nio-bot-1.0.0/examples/hello_world.py
--rw-r--r--   0 nex       (1000) nex       (1000)     1210 2023-06-15 08:59:25.000000 nio-bot-1.0.0/examples/uploading.py
--rw-r--r--   0 nex       (1000) nex       (1000)     1243 2023-07-04 21:28:18.000000 nio-bot-1.0.0/mkdocs.yml
--rw-r--r--   0 nex       (1000) nex       (1000)      781 2023-07-04 21:26:46.000000 nio-bot-1.0.0/pyproject.toml
--rw-r--r--   0 nex       (1000) nex       (1000)       91 2023-07-04 18:30:33.000000 nio-bot-1.0.0/requirements.txt
--rw-r--r--   0 nex       (1000) nex       (1000)       38 2023-07-12 12:39:54.627895 nio-bot-1.0.0/setup.cfg
-drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 12:39:54.617895 nio-bot-1.0.0/src/
-drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 12:39:54.624562 nio-bot-1.0.0/src/nio_bot.egg-info/
--rw-r--r--   0 nex       (1000) nex       (1000)     8268 2023-07-12 12:39:54.000000 nio-bot-1.0.0/src/nio_bot.egg-info/PKG-INFO
--rw-r--r--   0 nex       (1000) nex       (1000)     1409 2023-07-12 12:39:54.000000 nio-bot-1.0.0/src/nio_bot.egg-info/SOURCES.txt
--rw-r--r--   0 nex       (1000) nex       (1000)        1 2023-07-12 12:39:54.000000 nio-bot-1.0.0/src/nio_bot.egg-info/dependency_links.txt
--rw-r--r--   0 nex       (1000) nex       (1000)       58 2023-07-12 12:39:54.000000 nio-bot-1.0.0/src/nio_bot.egg-info/entry_points.txt
--rw-r--r--   0 nex       (1000) nex       (1000)      203 2023-07-12 12:39:54.000000 nio-bot-1.0.0/src/nio_bot.egg-info/requires.txt
--rw-r--r--   0 nex       (1000) nex       (1000)        7 2023-07-12 12:39:54.000000 nio-bot-1.0.0/src/nio_bot.egg-info/top_level.txt
-drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 12:39:54.624562 nio-bot-1.0.0/src/niobot/
--rw-r--r--   0 nex       (1000) nex       (1000)      806 2023-07-12 12:39:09.000000 nio-bot-1.0.0/src/niobot/__init__.py
--rw-r--r--   0 nex       (1000) nex       (1000)    13336 2023-07-12 12:39:09.000000 nio-bot-1.0.0/src/niobot/__main__.py
--rw-r--r--   0 nex       (1000) nex       (1000)      160 2023-07-12 12:39:54.000000 nio-bot-1.0.0/src/niobot/__version__.py
--rw-r--r--   0 nex       (1000) nex       (1000)    31604 2023-07-12 12:39:09.000000 nio-bot-1.0.0/src/niobot/attachment.py
--rw-r--r--   0 nex       (1000) nex       (1000)    32431 2023-07-12 12:39:09.000000 nio-bot-1.0.0/src/niobot/client.py
--rw-r--r--   0 nex       (1000) nex       (1000)    12273 2023-07-12 12:39:09.000000 nio-bot-1.0.0/src/niobot/commands.py
--rw-r--r--   0 nex       (1000) nex       (1000)     5146 2023-07-12 12:39:09.000000 nio-bot-1.0.0/src/niobot/context.py
--rw-r--r--   0 nex       (1000) nex       (1000)     3952 2023-07-12 12:39:09.000000 nio-bot-1.0.0/src/niobot/exceptions.py
-drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 12:39:54.627895 nio-bot-1.0.0/src/niobot/utils/
--rw-r--r--   0 nex       (1000) nex       (1000)      777 2023-07-03 20:38:45.000000 nio-bot-1.0.0/src/niobot/utils/__init__.py
--rw-r--r--   0 nex       (1000) nex       (1000)     1531 2023-07-12 12:39:09.000000 nio-bot-1.0.0/src/niobot/utils/federation.py
--rw-r--r--   0 nex       (1000) nex       (1000)     5027 2023-07-12 12:39:09.000000 nio-bot-1.0.0/src/niobot/utils/help_command.py
--rw-r--r--   0 nex       (1000) nex       (1000)     3535 2023-06-28 19:12:30.000000 nio-bot-1.0.0/src/niobot/utils/parsers.py
--rw-r--r--   0 nex       (1000) nex       (1000)     3467 2023-07-04 19:58:56.000000 nio-bot-1.0.0/src/niobot/utils/string_view.py
--rw-r--r--   0 nex       (1000) nex       (1000)     1553 2023-07-03 21:16:02.000000 nio-bot-1.0.0/src/niobot/utils/typing.py
--rw-r--r--   0 nex       (1000) nex       (1000)     2071 2023-07-04 10:53:34.000000 nio-bot-1.0.0/src/niobot/utils/unblocking.py
+drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 13:39:27.061500 nio-bot-1.0.1/
+drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 13:39:27.054833 nio-bot-1.0.1/.github/
+drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 13:39:27.058166 nio-bot-1.0.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 nex       (1000) nex       (1000)      797 2023-06-29 20:01:59.000000 nio-bot-1.0.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 nex       (1000) nex       (1000)      609 2023-06-29 20:01:59.000000 nio-bot-1.0.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 nex       (1000) nex       (1000)     7062 2023-07-12 12:39:09.000000 nio-bot-1.0.1/.gitignore
+drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 13:39:27.058166 nio-bot-1.0.1/.idea/
+-rw-r--r--   0 nex       (1000) nex       (1000)      176 2023-06-08 18:22:57.000000 nio-bot-1.0.1/.idea/.gitignore
+drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 13:39:27.058166 nio-bot-1.0.1/.idea/inspectionProfiles/
+-rw-r--r--   0 nex       (1000) nex       (1000)     3647 2023-06-08 18:25:30.000000 nio-bot-1.0.1/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 nex       (1000) nex       (1000)      174 2023-06-08 18:25:30.000000 nio-bot-1.0.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 nex       (1000) nex       (1000)      185 2023-06-08 18:47:53.000000 nio-bot-1.0.1/.idea/markdown.xml
+-rw-r--r--   0 nex       (1000) nex       (1000)      337 2023-06-08 18:25:30.000000 nio-bot-1.0.1/.idea/misc.xml
+-rw-r--r--   0 nex       (1000) nex       (1000)      266 2023-06-08 18:25:30.000000 nio-bot-1.0.1/.idea/modules.xml
+-rw-r--r--   0 nex       (1000) nex       (1000)      426 2023-06-13 20:35:20.000000 nio-bot-1.0.1/.idea/nio-bot.iml
+-rw-r--r--   0 nex       (1000) nex       (1000)      180 2023-06-12 20:15:29.000000 nio-bot-1.0.1/.idea/vcs.xml
+-rw-r--r--   0 nex       (1000) nex       (1000)    35149 2023-06-12 20:12:46.000000 nio-bot-1.0.1/LICENSE
+-rw-r--r--   0 nex       (1000) nex       (1000)     9023 2023-07-12 13:39:27.061500 nio-bot-1.0.1/PKG-INFO
+-rw-r--r--   0 nex       (1000) nex       (1000)     8276 2023-07-12 13:13:04.000000 nio-bot-1.0.1/README.md
+drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 13:39:27.058166 nio-bot-1.0.1/docs/
+drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 13:39:27.058166 nio-bot-1.0.1/docs/guides/
+-rw-r--r--   0 nex       (1000) nex       (1000)    14023 2023-07-05 11:52:24.000000 nio-bot-1.0.1/docs/guides/getting-started.md
+-rw-r--r--   0 nex       (1000) nex       (1000)     1412 2023-07-03 21:42:38.000000 nio-bot-1.0.1/docs/index.md
+drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 13:39:27.058166 nio-bot-1.0.1/docs/reference/
+-rw-r--r--   0 nex       (1000) nex       (1000)       36 2023-07-04 10:54:58.000000 nio-bot-1.0.1/docs/reference/attachment.md
+-rw-r--r--   0 nex       (1000) nex       (1000)       27 2023-07-11 19:15:48.000000 nio-bot-1.0.1/docs/reference/client.md
+-rw-r--r--   0 nex       (1000) nex       (1000)      100 2023-07-03 19:05:59.000000 nio-bot-1.0.1/docs/reference/commands.md
+-rw-r--r--   0 nex       (1000) nex       (1000)      708 2023-07-03 20:33:05.000000 nio-bot-1.0.1/docs/reference/context.md
+-rw-r--r--   0 nex       (1000) nex       (1000)       35 2023-07-03 19:08:54.000000 nio-bot-1.0.1/docs/reference/exceptions.md
+drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 13:39:27.058166 nio-bot-1.0.1/docs/reference/utils/
+-rw-r--r--   0 nex       (1000) nex       (1000)      229 2023-07-04 20:00:25.000000 nio-bot-1.0.1/docs/reference/utils/federation.md
+-rw-r--r--   0 nex       (1000) nex       (1000)     2764 2023-07-03 21:01:45.000000 nio-bot-1.0.1/docs/reference/utils/help_command.md
+-rw-r--r--   0 nex       (1000) nex       (1000)     2236 2023-07-04 09:49:11.000000 nio-bot-1.0.1/docs/reference/utils/parsers.md
+-rw-r--r--   0 nex       (1000) nex       (1000)      707 2023-07-04 19:56:41.000000 nio-bot-1.0.1/docs/reference/utils/string_view.md
+-rw-r--r--   0 nex       (1000) nex       (1000)     2346 2023-07-03 21:31:35.000000 nio-bot-1.0.1/docs/reference/utils/typing.md
+-rw-r--r--   0 nex       (1000) nex       (1000)     1960 2023-07-04 10:48:38.000000 nio-bot-1.0.1/docs/reference/utils/unblock.md
+drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 13:39:27.058166 nio-bot-1.0.1/examples/
+-rw-r--r--   0 nex       (1000) nex       (1000)     1636 2023-06-13 20:43:23.000000 nio-bot-1.0.1/examples/access_token.py
+-rw-r--r--   0 nex       (1000) nex       (1000)     1605 2023-06-13 20:35:19.000000 nio-bot-1.0.1/examples/hello_world.py
+-rw-r--r--   0 nex       (1000) nex       (1000)     1210 2023-06-15 08:59:25.000000 nio-bot-1.0.1/examples/uploading.py
+-rw-r--r--   0 nex       (1000) nex       (1000)     1243 2023-07-04 21:28:18.000000 nio-bot-1.0.1/mkdocs.yml
+-rw-r--r--   0 nex       (1000) nex       (1000)     1208 2023-07-12 13:39:10.000000 nio-bot-1.0.1/pyproject.toml
+-rw-r--r--   0 nex       (1000) nex       (1000)       91 2023-07-04 18:30:33.000000 nio-bot-1.0.1/requirements.txt
+-rw-r--r--   0 nex       (1000) nex       (1000)       38 2023-07-12 13:39:27.061500 nio-bot-1.0.1/setup.cfg
+-rw-r--r--   0 nex       (1000) nex       (1000)       80 2023-07-12 13:39:10.000000 nio-bot-1.0.1/setup.py
+drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 13:39:27.054833 nio-bot-1.0.1/src/
+drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 13:39:27.058166 nio-bot-1.0.1/src/nio_bot.egg-info/
+-rw-r--r--   0 nex       (1000) nex       (1000)     9023 2023-07-12 13:39:27.000000 nio-bot-1.0.1/src/nio_bot.egg-info/PKG-INFO
+-rw-r--r--   0 nex       (1000) nex       (1000)     1418 2023-07-12 13:39:27.000000 nio-bot-1.0.1/src/nio_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 nex       (1000) nex       (1000)        1 2023-07-12 13:39:27.000000 nio-bot-1.0.1/src/nio_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 nex       (1000) nex       (1000)       52 2023-07-12 13:39:27.000000 nio-bot-1.0.1/src/nio_bot.egg-info/entry_points.txt
+-rw-r--r--   0 nex       (1000) nex       (1000)      203 2023-07-12 13:39:27.000000 nio-bot-1.0.1/src/nio_bot.egg-info/requires.txt
+-rw-r--r--   0 nex       (1000) nex       (1000)        7 2023-07-12 13:39:27.000000 nio-bot-1.0.1/src/nio_bot.egg-info/top_level.txt
+drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 13:39:27.061500 nio-bot-1.0.1/src/niobot/
+-rw-r--r--   0 nex       (1000) nex       (1000)      806 2023-07-12 12:39:09.000000 nio-bot-1.0.1/src/niobot/__init__.py
+-rw-r--r--   0 nex       (1000) nex       (1000)    13336 2023-07-12 12:39:09.000000 nio-bot-1.0.1/src/niobot/__main__.py
+-rw-r--r--   0 nex       (1000) nex       (1000)      160 2023-07-12 13:39:26.000000 nio-bot-1.0.1/src/niobot/__version__.py
+-rw-r--r--   0 nex       (1000) nex       (1000)    31671 2023-07-12 13:02:33.000000 nio-bot-1.0.1/src/niobot/attachment.py
+-rw-r--r--   0 nex       (1000) nex       (1000)    32431 2023-07-12 12:39:09.000000 nio-bot-1.0.1/src/niobot/client.py
+-rw-r--r--   0 nex       (1000) nex       (1000)    12273 2023-07-12 12:39:09.000000 nio-bot-1.0.1/src/niobot/commands.py
+-rw-r--r--   0 nex       (1000) nex       (1000)     5146 2023-07-12 12:39:09.000000 nio-bot-1.0.1/src/niobot/context.py
+-rw-r--r--   0 nex       (1000) nex       (1000)     3952 2023-07-12 12:39:09.000000 nio-bot-1.0.1/src/niobot/exceptions.py
+drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 13:39:27.061500 nio-bot-1.0.1/src/niobot/utils/
+-rw-r--r--   0 nex       (1000) nex       (1000)      777 2023-07-03 20:38:45.000000 nio-bot-1.0.1/src/niobot/utils/__init__.py
+-rw-r--r--   0 nex       (1000) nex       (1000)     1531 2023-07-12 12:39:09.000000 nio-bot-1.0.1/src/niobot/utils/federation.py
+-rw-r--r--   0 nex       (1000) nex       (1000)     5027 2023-07-12 12:39:09.000000 nio-bot-1.0.1/src/niobot/utils/help_command.py
+-rw-r--r--   0 nex       (1000) nex       (1000)     3535 2023-06-28 19:12:30.000000 nio-bot-1.0.1/src/niobot/utils/parsers.py
+-rw-r--r--   0 nex       (1000) nex       (1000)     3467 2023-07-04 19:58:56.000000 nio-bot-1.0.1/src/niobot/utils/string_view.py
+-rw-r--r--   0 nex       (1000) nex       (1000)     1553 2023-07-03 21:16:02.000000 nio-bot-1.0.1/src/niobot/utils/typing.py
+-rw-r--r--   0 nex       (1000) nex       (1000)     2071 2023-07-04 10:53:34.000000 nio-bot-1.0.1/src/niobot/utils/unblocking.py
```

### Comparing `nio-bot-1.0.0/.github/ISSUE_TEMPLATE/bug_report.md` & `nio-bot-1.0.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/.github/ISSUE_TEMPLATE/feature_request.md` & `nio-bot-1.0.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/.gitignore` & `nio-bot-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/.idea/inspectionProfiles/Project_Default.xml` & `nio-bot-1.0.1/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/LICENSE` & `nio-bot-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/PKG-INFO` & `nio-bot-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,74 +1,84 @@
 Metadata-Version: 2.1
 Name: nio-bot
-Version: 1.0.0
+Version: 1.0.1
 Summary: Making matrix bots simple
 Author-email: Nexus <packages@nexy7574.co.uk>
 License: GNU GPLv3
+Project-URL: homepage, https://github.com/EEKIM10/niobot
+Project-URL: repository, https://github.com/EEKIM10/niobot
+Project-URL: documentation, https://eekim10.github.io/niobot/
+Project-URL: changelog, https://github.com/EEKIM10/niobot/releases
+Project-URL: tracker, https://github.com/EEKIM10/niobot/issues
+Project-URL: support, https://matrix.to/#/#niobot:nexy7574.co.uk
+Keywords: nio,matrix-nio,matrix,bot,botlib,niobot,framework,library,python
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: e2ee
 Provides-Extra: cli
 Provides-Extra: dev
 License-File: LICENSE
 
-<details>
-    <summary>Version information & warning</summary>
-This library does not currently have a "stable" version, as such all versions will be <code>0.1.dev&lt;Commit Number&gt;+g&lt;Commit Hash&gt;</code>.
-In order to pin to a specific version you should use the following in a requirements.txt or equivalent:
-    
-```
-matrix-nio @ git+https://github.com/EEKIM10/niobot.git@<commit number>
-# or for e2ee
-matrix-nio[e2ee] @ git+https://github.com/EEKIM10/niobot.git@<commit number>
-```
-
-Please remember, until there is a "stable" version, all commits will be pushed to main! Version pinning is highly
-recommended.
-</details>
-
 # NioBot
 A simple, easy to use python Matrix bot library, based on the excellent 
 [matrix-nio](https://pypi.org/project/matrix-nio/) library.
 
 NioBot is designed to have a similar (as similar as reasonably possible) design and feel to the
 [discord.py](https://pypi.org/project/discord.py) library, which should hopefully give it a familiar feel if you're
 coming from a discord background.
 
 Please note that there *will* be teething problems, and as such some advanced features may not be
 available, as with any client.
 
 ## Need help?
-look at [examples](/examples), open an issue, or [contact me on matrix](https://matrix.to/#/@nex:nexy7574.co.uk)
-
-## Examples
-You can see the [examples](/examples) directory, which contains a few examples of how to use NioBot.
-Note that these examples are not tested and will need some tweaking.
+Take a look at the [docs!](https://eekim10.github.io/niobot)
 
 ---
 
 Alternatively, take a look at my [dev bot](https://github.com/EEKIM10/niobot-test), which is a bot that I use to test
 features of nio-bot before they're released.
 This bot is very advanced as, since I developed the library, I know exactly how it works, and will have bleeding-edge
 features built into it, which a lot of users may not use yet.
 
 It is, however, a great example of how an advanced, full feature bot can be created using this library.
 
 You can see it live [here](https://matrix.to/#/@jimmy-bot:nexy7574.co.uk)
 (DM it, the prefix is ?, and full end-to-end encryption is supported. Average response time is ~300-500ms)
 
 ## Installation
+### Versions
+NioBot uses SemVer (semantic versioning) for versioning. This means that the version number is split into three parts:
+`Major`, `Minor` and `Patch`. As per the versioning, `Major` versions are not guaranteed to be backwards compatible,
+however `Minor` and `Patch` versions are.
+
+This means that there will always be a new `Major` increment when a backwards incompatible change is made, and a new
+`Minor` increment when a backwards compatible change is made. `Patch` versions are almost always bug fixes, and are
+always backwards compatible. If a bug fix is not backwards compatible, a new `Major` version will be released.
+
+Major changes may be pushed into their own branches for "feature previews". These branches will be prefixed with
+`feature/`, and will be merged into `master` when they are ready for release. For example, `feature/my-thing`,
+which means you can install it using `niobot @ git+https://github.com/EEKIM10/niobot.git@feature/my-thing`.
+This minimises the number of breaking releases.
+
+### Release versions
+You can use the [PyPi](https://pypi.org/project/niobot) releases:
+```python
+niobot==1.0.0  # or whatever version
+# Or to install it with extras
+niobot[e2ee,cli]==1.0.0
+```
+
+### Development (master branch)
 You should use requirements.txt:
 ```python
 matrix-nio @ git+https://github.com/EEKIM10/niobot.git
 # Or with e2ee support (note you will need libolm)
 matrix-nio[e2ee] @ git+https://github.com/EEKIM10/niobot.git
 ```
-You can figure out how to install it in other ways. See the start of this README for more information on version
-pinning.
+You can figure out how to install it in other ways.
 
 ## Features
 NioBot aims to be as easy to use as possible, so form is preferred over function.
 Some features you'd normally expect may not be implemented (yet, feel free to open a pull request!) or may not work as 
 intended or how you'd expect, however as with any matrix client.
 
 However, like any good client, NioBot tries to adhere to the 
@@ -122,42 +132,42 @@
 |- main.py  (your bot file, the bit that runs your bot)
 |- modules
     |- ping.py
 ```
 
 In main.py, you'll put some similar code:
 ```python
-import niolib
+import niobot
 
-bot = niolib.Bot(...)
+bot = niobot.Bot(...)
 bot.mount_module("modules.ping")  # mounts the ping module
 
 bot.run(password="password")
 ```
 
 When you call `mount_module`, it effectively calls `import module` under the hood, and then does one of the following:
 
 1. Calls the `module.setup(bot)` function, if it exists
 2. Discovers all classes that subclass `niolib.Module` in the module, and calls their `__setup__`, adding all commands
 registered under that class
 
 Take the following file as ping.py:
 ```python
-import niolib
+import niobot
 
 
 class MyPingModule(niolib.Module):
     # This class is a subclass of niolib.Module, so it will be automatically discovered and loaded
     # It also has two attributes defined that you can use:
     # * self.bot: the instance of the bot
     # * self.log: An instance of logging.Logger, which you can use to log messages to the console or log file.
     #   It is recommended to use this instead of print().
     
     # Now we will define a command
-    @niolib.command()
+    @niobot.command()
     async def ping(self, ctx: niolib.Context):
         """Shows the latency"""
         roundtrip = (time.time() * 1000 - ctx.event.server_timestamp)
         await ctx.reply("Pong! Took {:,.2f}ms".format(roundtrip))
 ```
 
 Notice how here, we use `@niolib.command`, instead of `@bot.command`? They work the same, however
```

### Comparing `nio-bot-1.0.0/README.md` & `nio-bot-1.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,64 @@
-<details>
-    <summary>Version information & warning</summary>
-This library does not currently have a "stable" version, as such all versions will be <code>0.1.dev&lt;Commit Number&gt;+g&lt;Commit Hash&gt;</code>.
-In order to pin to a specific version you should use the following in a requirements.txt or equivalent:
-    
-```
-matrix-nio @ git+https://github.com/EEKIM10/niobot.git@<commit number>
-# or for e2ee
-matrix-nio[e2ee] @ git+https://github.com/EEKIM10/niobot.git@<commit number>
-```
-
-Please remember, until there is a "stable" version, all commits will be pushed to main! Version pinning is highly
-recommended.
-</details>
-
 # NioBot
 A simple, easy to use python Matrix bot library, based on the excellent 
 [matrix-nio](https://pypi.org/project/matrix-nio/) library.
 
 NioBot is designed to have a similar (as similar as reasonably possible) design and feel to the
 [discord.py](https://pypi.org/project/discord.py) library, which should hopefully give it a familiar feel if you're
 coming from a discord background.
 
 Please note that there *will* be teething problems, and as such some advanced features may not be
 available, as with any client.
 
 ## Need help?
-look at [examples](/examples), open an issue, or [contact me on matrix](https://matrix.to/#/@nex:nexy7574.co.uk)
-
-## Examples
-You can see the [examples](/examples) directory, which contains a few examples of how to use NioBot.
-Note that these examples are not tested and will need some tweaking.
+Take a look at the [docs!](https://eekim10.github.io/niobot)
 
 ---
 
 Alternatively, take a look at my [dev bot](https://github.com/EEKIM10/niobot-test), which is a bot that I use to test
 features of nio-bot before they're released.
 This bot is very advanced as, since I developed the library, I know exactly how it works, and will have bleeding-edge
 features built into it, which a lot of users may not use yet.
 
 It is, however, a great example of how an advanced, full feature bot can be created using this library.
 
 You can see it live [here](https://matrix.to/#/@jimmy-bot:nexy7574.co.uk)
 (DM it, the prefix is ?, and full end-to-end encryption is supported. Average response time is ~300-500ms)
 
 ## Installation
+### Versions
+NioBot uses SemVer (semantic versioning) for versioning. This means that the version number is split into three parts:
+`Major`, `Minor` and `Patch`. As per the versioning, `Major` versions are not guaranteed to be backwards compatible,
+however `Minor` and `Patch` versions are.
+
+This means that there will always be a new `Major` increment when a backwards incompatible change is made, and a new
+`Minor` increment when a backwards compatible change is made. `Patch` versions are almost always bug fixes, and are
+always backwards compatible. If a bug fix is not backwards compatible, a new `Major` version will be released.
+
+Major changes may be pushed into their own branches for "feature previews". These branches will be prefixed with
+`feature/`, and will be merged into `master` when they are ready for release. For example, `feature/my-thing`,
+which means you can install it using `niobot @ git+https://github.com/EEKIM10/niobot.git@feature/my-thing`.
+This minimises the number of breaking releases.
+
+### Release versions
+You can use the [PyPi](https://pypi.org/project/niobot) releases:
+```python
+niobot==1.0.0  # or whatever version
+# Or to install it with extras
+niobot[e2ee,cli]==1.0.0
+```
+
+### Development (master branch)
 You should use requirements.txt:
 ```python
 matrix-nio @ git+https://github.com/EEKIM10/niobot.git
 # Or with e2ee support (note you will need libolm)
 matrix-nio[e2ee] @ git+https://github.com/EEKIM10/niobot.git
 ```
-You can figure out how to install it in other ways. See the start of this README for more information on version
-pinning.
+You can figure out how to install it in other ways.
 
 ## Features
 NioBot aims to be as easy to use as possible, so form is preferred over function.
 Some features you'd normally expect may not be implemented (yet, feel free to open a pull request!) or may not work as 
 intended or how you'd expect, however as with any matrix client.
 
 However, like any good client, NioBot tries to adhere to the 
@@ -109,42 +112,42 @@
 |- main.py  (your bot file, the bit that runs your bot)
 |- modules
     |- ping.py
 ```
 
 In main.py, you'll put some similar code:
 ```python
-import niolib
+import niobot
 
-bot = niolib.Bot(...)
+bot = niobot.Bot(...)
 bot.mount_module("modules.ping")  # mounts the ping module
 
 bot.run(password="password")
 ```
 
 When you call `mount_module`, it effectively calls `import module` under the hood, and then does one of the following:
 
 1. Calls the `module.setup(bot)` function, if it exists
 2. Discovers all classes that subclass `niolib.Module` in the module, and calls their `__setup__`, adding all commands
 registered under that class
 
 Take the following file as ping.py:
 ```python
-import niolib
+import niobot
 
 
 class MyPingModule(niolib.Module):
     # This class is a subclass of niolib.Module, so it will be automatically discovered and loaded
     # It also has two attributes defined that you can use:
     # * self.bot: the instance of the bot
     # * self.log: An instance of logging.Logger, which you can use to log messages to the console or log file.
     #   It is recommended to use this instead of print().
     
     # Now we will define a command
-    @niolib.command()
+    @niobot.command()
     async def ping(self, ctx: niolib.Context):
         """Shows the latency"""
         roundtrip = (time.time() * 1000 - ctx.event.server_timestamp)
         await ctx.reply("Pong! Took {:,.2f}ms".format(roundtrip))
 ```
 
 Notice how here, we use `@niolib.command`, instead of `@bot.command`? They work the same, however
```

### Comparing `nio-bot-1.0.0/docs/guides/getting-started.md` & `nio-bot-1.0.1/docs/guides/getting-started.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/docs/index.md` & `nio-bot-1.0.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/docs/reference/context.md` & `nio-bot-1.0.1/docs/reference/context.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/docs/reference/utils/help_command.md` & `nio-bot-1.0.1/docs/reference/utils/help_command.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/docs/reference/utils/parsers.md` & `nio-bot-1.0.1/docs/reference/utils/parsers.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/docs/reference/utils/string_view.md` & `nio-bot-1.0.1/docs/reference/utils/string_view.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/docs/reference/utils/typing.md` & `nio-bot-1.0.1/docs/reference/utils/typing.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/docs/reference/utils/unblock.md` & `nio-bot-1.0.1/docs/reference/utils/unblock.md`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/examples/access_token.py` & `nio-bot-1.0.1/examples/access_token.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/examples/hello_world.py` & `nio-bot-1.0.1/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/examples/uploading.py` & `nio-bot-1.0.1/examples/uploading.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/mkdocs.yml` & `nio-bot-1.0.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/src/nio_bot.egg-info/PKG-INFO` & `nio-bot-1.0.1/src/nio_bot.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,74 +1,84 @@
 Metadata-Version: 2.1
 Name: nio-bot
-Version: 1.0.0
+Version: 1.0.1
 Summary: Making matrix bots simple
 Author-email: Nexus <packages@nexy7574.co.uk>
 License: GNU GPLv3
+Project-URL: homepage, https://github.com/EEKIM10/niobot
+Project-URL: repository, https://github.com/EEKIM10/niobot
+Project-URL: documentation, https://eekim10.github.io/niobot/
+Project-URL: changelog, https://github.com/EEKIM10/niobot/releases
+Project-URL: tracker, https://github.com/EEKIM10/niobot/issues
+Project-URL: support, https://matrix.to/#/#niobot:nexy7574.co.uk
+Keywords: nio,matrix-nio,matrix,bot,botlib,niobot,framework,library,python
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: e2ee
 Provides-Extra: cli
 Provides-Extra: dev
 License-File: LICENSE
 
-<details>
-    <summary>Version information & warning</summary>
-This library does not currently have a "stable" version, as such all versions will be <code>0.1.dev&lt;Commit Number&gt;+g&lt;Commit Hash&gt;</code>.
-In order to pin to a specific version you should use the following in a requirements.txt or equivalent:
-    
-```
-matrix-nio @ git+https://github.com/EEKIM10/niobot.git@<commit number>
-# or for e2ee
-matrix-nio[e2ee] @ git+https://github.com/EEKIM10/niobot.git@<commit number>
-```
-
-Please remember, until there is a "stable" version, all commits will be pushed to main! Version pinning is highly
-recommended.
-</details>
-
 # NioBot
 A simple, easy to use python Matrix bot library, based on the excellent 
 [matrix-nio](https://pypi.org/project/matrix-nio/) library.
 
 NioBot is designed to have a similar (as similar as reasonably possible) design and feel to the
 [discord.py](https://pypi.org/project/discord.py) library, which should hopefully give it a familiar feel if you're
 coming from a discord background.
 
 Please note that there *will* be teething problems, and as such some advanced features may not be
 available, as with any client.
 
 ## Need help?
-look at [examples](/examples), open an issue, or [contact me on matrix](https://matrix.to/#/@nex:nexy7574.co.uk)
-
-## Examples
-You can see the [examples](/examples) directory, which contains a few examples of how to use NioBot.
-Note that these examples are not tested and will need some tweaking.
+Take a look at the [docs!](https://eekim10.github.io/niobot)
 
 ---
 
 Alternatively, take a look at my [dev bot](https://github.com/EEKIM10/niobot-test), which is a bot that I use to test
 features of nio-bot before they're released.
 This bot is very advanced as, since I developed the library, I know exactly how it works, and will have bleeding-edge
 features built into it, which a lot of users may not use yet.
 
 It is, however, a great example of how an advanced, full feature bot can be created using this library.
 
 You can see it live [here](https://matrix.to/#/@jimmy-bot:nexy7574.co.uk)
 (DM it, the prefix is ?, and full end-to-end encryption is supported. Average response time is ~300-500ms)
 
 ## Installation
+### Versions
+NioBot uses SemVer (semantic versioning) for versioning. This means that the version number is split into three parts:
+`Major`, `Minor` and `Patch`. As per the versioning, `Major` versions are not guaranteed to be backwards compatible,
+however `Minor` and `Patch` versions are.
+
+This means that there will always be a new `Major` increment when a backwards incompatible change is made, and a new
+`Minor` increment when a backwards compatible change is made. `Patch` versions are almost always bug fixes, and are
+always backwards compatible. If a bug fix is not backwards compatible, a new `Major` version will be released.
+
+Major changes may be pushed into their own branches for "feature previews". These branches will be prefixed with
+`feature/`, and will be merged into `master` when they are ready for release. For example, `feature/my-thing`,
+which means you can install it using `niobot @ git+https://github.com/EEKIM10/niobot.git@feature/my-thing`.
+This minimises the number of breaking releases.
+
+### Release versions
+You can use the [PyPi](https://pypi.org/project/niobot) releases:
+```python
+niobot==1.0.0  # or whatever version
+# Or to install it with extras
+niobot[e2ee,cli]==1.0.0
+```
+
+### Development (master branch)
 You should use requirements.txt:
 ```python
 matrix-nio @ git+https://github.com/EEKIM10/niobot.git
 # Or with e2ee support (note you will need libolm)
 matrix-nio[e2ee] @ git+https://github.com/EEKIM10/niobot.git
 ```
-You can figure out how to install it in other ways. See the start of this README for more information on version
-pinning.
+You can figure out how to install it in other ways.
 
 ## Features
 NioBot aims to be as easy to use as possible, so form is preferred over function.
 Some features you'd normally expect may not be implemented (yet, feel free to open a pull request!) or may not work as 
 intended or how you'd expect, however as with any matrix client.
 
 However, like any good client, NioBot tries to adhere to the 
@@ -122,42 +132,42 @@
 |- main.py  (your bot file, the bit that runs your bot)
 |- modules
     |- ping.py
 ```
 
 In main.py, you'll put some similar code:
 ```python
-import niolib
+import niobot
 
-bot = niolib.Bot(...)
+bot = niobot.Bot(...)
 bot.mount_module("modules.ping")  # mounts the ping module
 
 bot.run(password="password")
 ```
 
 When you call `mount_module`, it effectively calls `import module` under the hood, and then does one of the following:
 
 1. Calls the `module.setup(bot)` function, if it exists
 2. Discovers all classes that subclass `niolib.Module` in the module, and calls their `__setup__`, adding all commands
 registered under that class
 
 Take the following file as ping.py:
 ```python
-import niolib
+import niobot
 
 
 class MyPingModule(niolib.Module):
     # This class is a subclass of niolib.Module, so it will be automatically discovered and loaded
     # It also has two attributes defined that you can use:
     # * self.bot: the instance of the bot
     # * self.log: An instance of logging.Logger, which you can use to log messages to the console or log file.
     #   It is recommended to use this instead of print().
     
     # Now we will define a command
-    @niolib.command()
+    @niobot.command()
     async def ping(self, ctx: niolib.Context):
         """Shows the latency"""
         roundtrip = (time.time() * 1000 - ctx.event.server_timestamp)
         await ctx.reply("Pong! Took {:,.2f}ms".format(roundtrip))
 ```
 
 Notice how here, we use `@niolib.command`, instead of `@bot.command`? They work the same, however
```

### Comparing `nio-bot-1.0.0/src/nio_bot.egg-info/SOURCES.txt` & `nio-bot-1.0.1/src/nio_bot.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 .gitignore
 LICENSE
 README.md
 mkdocs.yml
 pyproject.toml
 requirements.txt
+setup.py
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .idea/.gitignore
 .idea/markdown.xml
 .idea/misc.xml
 .idea/modules.xml
 .idea/nio-bot.iml
```

### Comparing `nio-bot-1.0.0/src/niobot/__init__.py` & `nio-bot-1.0.1/src/niobot/__init__.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/src/niobot/__main__.py` & `nio-bot-1.0.1/src/niobot/__main__.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/src/niobot/attachment.py` & `nio-bot-1.0.1/src/niobot/attachment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Matrix file attachments. Full e2ee support is implemented.
 
 !!! danger "You need FFMPEG for this to work"
     In order for most attachment-related operations, you must have `ffprobe` in your $PATH.
-    As a matter of fact,
+    As a matter of fact, the library will not load any attachment-related classes without it.
 """
 import abc
 import tempfile
 import warnings
 
 import nio
 import subprocess
@@ -26,19 +26,19 @@
 from .utils import run_blocking
 from .exceptions import MediaUploadException, MetadataDetectionException, MediaCodecWarning
 
 if typing.TYPE_CHECKING:
     from .client import NioBot
 
 if not shutil.which("ffmpeg"):
-    raise RuntimeError(
+    raise ImportError(
         "ffmpeg is not installed. You must install it to use this library. If its installed, is it in PATH?"
     )
 if not shutil.which("ffprobe"):
-    raise RuntimeError(
+    raise ImportError(
         "ffprobe is not installed. You must install it to use this library. If its installed, is it in PATH?"
     )
 
 
 log = logging.getLogger(__name__)
```

### Comparing `nio-bot-1.0.0/src/niobot/client.py` & `nio-bot-1.0.1/src/niobot/client.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/src/niobot/commands.py` & `nio-bot-1.0.1/src/niobot/commands.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/src/niobot/context.py` & `nio-bot-1.0.1/src/niobot/context.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/src/niobot/exceptions.py` & `nio-bot-1.0.1/src/niobot/exceptions.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/src/niobot/utils/__init__.py` & `nio-bot-1.0.1/src/niobot/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/src/niobot/utils/federation.py` & `nio-bot-1.0.1/src/niobot/utils/federation.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/src/niobot/utils/help_command.py` & `nio-bot-1.0.1/src/niobot/utils/help_command.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/src/niobot/utils/parsers.py` & `nio-bot-1.0.1/src/niobot/utils/parsers.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/src/niobot/utils/string_view.py` & `nio-bot-1.0.1/src/niobot/utils/string_view.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/src/niobot/utils/typing.py` & `nio-bot-1.0.1/src/niobot/utils/typing.py`

 * *Files identical despite different names*

### Comparing `nio-bot-1.0.0/src/niobot/utils/unblocking.py` & `nio-bot-1.0.1/src/niobot/utils/unblocking.py`

 * *Files identical despite different names*


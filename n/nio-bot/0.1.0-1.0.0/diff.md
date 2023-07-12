# Comparing `tmp/nio-bot-0.1.0.tar.gz` & `tmp/nio-bot-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nio-bot-0.1.0.tar", last modified: Wed Jul  5 18:15:04 2023, max compression
+gzip compressed data, was "nio-bot-1.0.0.tar", last modified: Wed Jul 12 12:39:54 2023, max compression
```

## Comparing `nio-bot-0.1.0.tar` & `nio-bot-1.0.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-05 18:15:04.672064 nio-bot-0.1.0/
-drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-05 18:15:04.658731 nio-bot-0.1.0/.github/
-drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-05 18:15:04.662064 nio-bot-0.1.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 nex       (1000) nex       (1000)      797 2023-06-29 20:01:59.000000 nio-bot-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 nex       (1000) nex       (1000)      609 2023-06-29 20:01:59.000000 nio-bot-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 nex       (1000) nex       (1000)     6960 2023-06-26 20:08:05.000000 nio-bot-0.1.0/.gitignore
-drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-05 18:15:04.662064 nio-bot-0.1.0/.idea/
--rw-r--r--   0 nex       (1000) nex       (1000)      176 2023-06-08 18:22:57.000000 nio-bot-0.1.0/.idea/.gitignore
-drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-05 18:15:04.662064 nio-bot-0.1.0/.idea/inspectionProfiles/
--rw-r--r--   0 nex       (1000) nex       (1000)     3647 2023-06-08 18:25:30.000000 nio-bot-0.1.0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 nex       (1000) nex       (1000)      174 2023-06-08 18:25:30.000000 nio-bot-0.1.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 nex       (1000) nex       (1000)      185 2023-06-08 18:47:53.000000 nio-bot-0.1.0/.idea/markdown.xml
--rw-r--r--   0 nex       (1000) nex       (1000)      337 2023-06-08 18:25:30.000000 nio-bot-0.1.0/.idea/misc.xml
--rw-r--r--   0 nex       (1000) nex       (1000)      266 2023-06-08 18:25:30.000000 nio-bot-0.1.0/.idea/modules.xml
--rw-r--r--   0 nex       (1000) nex       (1000)      426 2023-06-13 20:35:20.000000 nio-bot-0.1.0/.idea/nio-bot.iml
--rw-r--r--   0 nex       (1000) nex       (1000)      180 2023-06-12 20:15:29.000000 nio-bot-0.1.0/.idea/vcs.xml
--rw-r--r--   0 nex       (1000) nex       (1000)    35149 2023-06-12 20:12:46.000000 nio-bot-0.1.0/LICENSE
--rw-r--r--   0 nex       (1000) nex       (1000)     8268 2023-07-05 18:15:04.672064 nio-bot-0.1.0/PKG-INFO
--rw-r--r--   0 nex       (1000) nex       (1000)     7969 2023-06-29 12:18:06.000000 nio-bot-0.1.0/README.md
-drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-05 18:15:04.662064 nio-bot-0.1.0/docs/
-drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-05 18:15:04.662064 nio-bot-0.1.0/docs/guides/
--rw-r--r--   0 nex       (1000) nex       (1000)    14023 2023-07-05 11:52:24.000000 nio-bot-0.1.0/docs/guides/getting-started.md
--rw-r--r--   0 nex       (1000) nex       (1000)     1412 2023-07-03 21:42:38.000000 nio-bot-0.1.0/docs/index.md
-drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-05 18:15:04.662064 nio-bot-0.1.0/docs/reference/
--rw-r--r--   0 nex       (1000) nex       (1000)       36 2023-07-04 10:54:58.000000 nio-bot-0.1.0/docs/reference/attachment.md
--rw-r--r--   0 nex       (1000) nex       (1000)       27 2023-07-03 18:52:57.000000 nio-bot-0.1.0/docs/reference/client.md
--rw-r--r--   0 nex       (1000) nex       (1000)      100 2023-07-03 19:05:59.000000 nio-bot-0.1.0/docs/reference/commands.md
--rw-r--r--   0 nex       (1000) nex       (1000)      708 2023-07-03 20:33:05.000000 nio-bot-0.1.0/docs/reference/context.md
--rw-r--r--   0 nex       (1000) nex       (1000)       35 2023-07-03 19:08:54.000000 nio-bot-0.1.0/docs/reference/exceptions.md
-drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-05 18:15:04.665398 nio-bot-0.1.0/docs/reference/utils/
--rw-r--r--   0 nex       (1000) nex       (1000)      229 2023-07-04 20:00:25.000000 nio-bot-0.1.0/docs/reference/utils/federation.md
--rw-r--r--   0 nex       (1000) nex       (1000)     2764 2023-07-03 21:01:45.000000 nio-bot-0.1.0/docs/reference/utils/help_command.md
--rw-r--r--   0 nex       (1000) nex       (1000)     2236 2023-07-04 09:49:11.000000 nio-bot-0.1.0/docs/reference/utils/parsers.md
--rw-r--r--   0 nex       (1000) nex       (1000)      707 2023-07-04 19:56:41.000000 nio-bot-0.1.0/docs/reference/utils/string_view.md
--rw-r--r--   0 nex       (1000) nex       (1000)     2346 2023-07-03 21:31:35.000000 nio-bot-0.1.0/docs/reference/utils/typing.md
--rw-r--r--   0 nex       (1000) nex       (1000)     1960 2023-07-04 10:48:38.000000 nio-bot-0.1.0/docs/reference/utils/unblock.md
-drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-05 18:15:04.665398 nio-bot-0.1.0/examples/
--rw-r--r--   0 nex       (1000) nex       (1000)     1636 2023-06-13 20:43:23.000000 nio-bot-0.1.0/examples/access_token.py
--rw-r--r--   0 nex       (1000) nex       (1000)     1605 2023-06-13 20:35:19.000000 nio-bot-0.1.0/examples/hello_world.py
--rw-r--r--   0 nex       (1000) nex       (1000)     1210 2023-06-15 08:59:25.000000 nio-bot-0.1.0/examples/uploading.py
--rw-r--r--   0 nex       (1000) nex       (1000)     1243 2023-07-04 21:28:18.000000 nio-bot-0.1.0/mkdocs.yml
--rw-r--r--   0 nex       (1000) nex       (1000)      781 2023-07-04 21:26:46.000000 nio-bot-0.1.0/pyproject.toml
--rw-r--r--   0 nex       (1000) nex       (1000)       91 2023-07-04 18:30:33.000000 nio-bot-0.1.0/requirements.txt
--rw-r--r--   0 nex       (1000) nex       (1000)       38 2023-07-05 18:15:04.672064 nio-bot-0.1.0/setup.cfg
-drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-05 18:15:04.658731 nio-bot-0.1.0/src/
-drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-05 18:15:04.665398 nio-bot-0.1.0/src/nio_bot.egg-info/
--rw-r--r--   0 nex       (1000) nex       (1000)     8268 2023-07-05 18:15:04.000000 nio-bot-0.1.0/src/nio_bot.egg-info/PKG-INFO
--rw-r--r--   0 nex       (1000) nex       (1000)     1409 2023-07-05 18:15:04.000000 nio-bot-0.1.0/src/nio_bot.egg-info/SOURCES.txt
--rw-r--r--   0 nex       (1000) nex       (1000)        1 2023-07-05 18:15:04.000000 nio-bot-0.1.0/src/nio_bot.egg-info/dependency_links.txt
--rw-r--r--   0 nex       (1000) nex       (1000)       58 2023-07-05 18:15:04.000000 nio-bot-0.1.0/src/nio_bot.egg-info/entry_points.txt
--rw-r--r--   0 nex       (1000) nex       (1000)      203 2023-07-05 18:15:04.000000 nio-bot-0.1.0/src/nio_bot.egg-info/requires.txt
--rw-r--r--   0 nex       (1000) nex       (1000)        7 2023-07-05 18:15:04.000000 nio-bot-0.1.0/src/nio_bot.egg-info/top_level.txt
-drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-05 18:15:04.668731 nio-bot-0.1.0/src/niobot/
--rw-r--r--   0 nex       (1000) nex       (1000)      753 2023-07-03 21:18:06.000000 nio-bot-0.1.0/src/niobot/__init__.py
--rw-r--r--   0 nex       (1000) nex       (1000)    13112 2023-07-04 20:36:37.000000 nio-bot-0.1.0/src/niobot/__main__.py
--rw-r--r--   0 nex       (1000) nex       (1000)      160 2023-07-05 18:15:04.000000 nio-bot-0.1.0/src/niobot/__version__.py
--rw-r--r--   0 nex       (1000) nex       (1000)    15152 2023-07-05 18:02:06.000000 nio-bot-0.1.0/src/niobot/attachment.py
--rw-r--r--   0 nex       (1000) nex       (1000)    29593 2023-07-03 21:02:42.000000 nio-bot-0.1.0/src/niobot/client.py
--rw-r--r--   0 nex       (1000) nex       (1000)     9530 2023-07-05 17:32:31.000000 nio-bot-0.1.0/src/niobot/commands.py
--rw-r--r--   0 nex       (1000) nex       (1000)     4664 2023-07-05 17:32:31.000000 nio-bot-0.1.0/src/niobot/context.py
--rw-r--r--   0 nex       (1000) nex       (1000)     2981 2023-07-03 20:00:21.000000 nio-bot-0.1.0/src/niobot/exceptions.py
-drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-05 18:15:04.668731 nio-bot-0.1.0/src/niobot/utils/
--rw-r--r--   0 nex       (1000) nex       (1000)      777 2023-07-03 20:38:45.000000 nio-bot-0.1.0/src/niobot/utils/__init__.py
--rw-r--r--   0 nex       (1000) nex       (1000)     1533 2023-07-04 20:12:47.000000 nio-bot-0.1.0/src/niobot/utils/federation.py
--rw-r--r--   0 nex       (1000) nex       (1000)     5045 2023-07-03 21:05:05.000000 nio-bot-0.1.0/src/niobot/utils/help_command.py
--rw-r--r--   0 nex       (1000) nex       (1000)     3535 2023-06-28 19:12:30.000000 nio-bot-0.1.0/src/niobot/utils/parsers.py
--rw-r--r--   0 nex       (1000) nex       (1000)     3467 2023-07-04 19:58:56.000000 nio-bot-0.1.0/src/niobot/utils/string_view.py
--rw-r--r--   0 nex       (1000) nex       (1000)     1553 2023-07-03 21:16:02.000000 nio-bot-0.1.0/src/niobot/utils/typing.py
--rw-r--r--   0 nex       (1000) nex       (1000)     2071 2023-07-04 10:53:34.000000 nio-bot-0.1.0/src/niobot/utils/unblocking.py
+drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 12:39:54.627895 nio-bot-1.0.0/
+drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 12:39:54.617895 nio-bot-1.0.0/.github/
+drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 12:39:54.617895 nio-bot-1.0.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 nex       (1000) nex       (1000)      797 2023-06-29 20:01:59.000000 nio-bot-1.0.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 nex       (1000) nex       (1000)      609 2023-06-29 20:01:59.000000 nio-bot-1.0.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 nex       (1000) nex       (1000)     7062 2023-07-12 12:39:09.000000 nio-bot-1.0.0/.gitignore
+drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 12:39:54.621229 nio-bot-1.0.0/.idea/
+-rw-r--r--   0 nex       (1000) nex       (1000)      176 2023-06-08 18:22:57.000000 nio-bot-1.0.0/.idea/.gitignore
+drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 12:39:54.621229 nio-bot-1.0.0/.idea/inspectionProfiles/
+-rw-r--r--   0 nex       (1000) nex       (1000)     3647 2023-06-08 18:25:30.000000 nio-bot-1.0.0/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 nex       (1000) nex       (1000)      174 2023-06-08 18:25:30.000000 nio-bot-1.0.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 nex       (1000) nex       (1000)      185 2023-06-08 18:47:53.000000 nio-bot-1.0.0/.idea/markdown.xml
+-rw-r--r--   0 nex       (1000) nex       (1000)      337 2023-06-08 18:25:30.000000 nio-bot-1.0.0/.idea/misc.xml
+-rw-r--r--   0 nex       (1000) nex       (1000)      266 2023-06-08 18:25:30.000000 nio-bot-1.0.0/.idea/modules.xml
+-rw-r--r--   0 nex       (1000) nex       (1000)      426 2023-06-13 20:35:20.000000 nio-bot-1.0.0/.idea/nio-bot.iml
+-rw-r--r--   0 nex       (1000) nex       (1000)      180 2023-06-12 20:15:29.000000 nio-bot-1.0.0/.idea/vcs.xml
+-rw-r--r--   0 nex       (1000) nex       (1000)    35149 2023-06-12 20:12:46.000000 nio-bot-1.0.0/LICENSE
+-rw-r--r--   0 nex       (1000) nex       (1000)     8268 2023-07-12 12:39:54.627895 nio-bot-1.0.0/PKG-INFO
+-rw-r--r--   0 nex       (1000) nex       (1000)     7969 2023-06-29 12:18:06.000000 nio-bot-1.0.0/README.md
+drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 12:39:54.621229 nio-bot-1.0.0/docs/
+drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 12:39:54.621229 nio-bot-1.0.0/docs/guides/
+-rw-r--r--   0 nex       (1000) nex       (1000)    14023 2023-07-05 11:52:24.000000 nio-bot-1.0.0/docs/guides/getting-started.md
+-rw-r--r--   0 nex       (1000) nex       (1000)     1412 2023-07-03 21:42:38.000000 nio-bot-1.0.0/docs/index.md
+drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 12:39:54.621229 nio-bot-1.0.0/docs/reference/
+-rw-r--r--   0 nex       (1000) nex       (1000)       36 2023-07-04 10:54:58.000000 nio-bot-1.0.0/docs/reference/attachment.md
+-rw-r--r--   0 nex       (1000) nex       (1000)       27 2023-07-11 19:15:48.000000 nio-bot-1.0.0/docs/reference/client.md
+-rw-r--r--   0 nex       (1000) nex       (1000)      100 2023-07-03 19:05:59.000000 nio-bot-1.0.0/docs/reference/commands.md
+-rw-r--r--   0 nex       (1000) nex       (1000)      708 2023-07-03 20:33:05.000000 nio-bot-1.0.0/docs/reference/context.md
+-rw-r--r--   0 nex       (1000) nex       (1000)       35 2023-07-03 19:08:54.000000 nio-bot-1.0.0/docs/reference/exceptions.md
+drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 12:39:54.624562 nio-bot-1.0.0/docs/reference/utils/
+-rw-r--r--   0 nex       (1000) nex       (1000)      229 2023-07-04 20:00:25.000000 nio-bot-1.0.0/docs/reference/utils/federation.md
+-rw-r--r--   0 nex       (1000) nex       (1000)     2764 2023-07-03 21:01:45.000000 nio-bot-1.0.0/docs/reference/utils/help_command.md
+-rw-r--r--   0 nex       (1000) nex       (1000)     2236 2023-07-04 09:49:11.000000 nio-bot-1.0.0/docs/reference/utils/parsers.md
+-rw-r--r--   0 nex       (1000) nex       (1000)      707 2023-07-04 19:56:41.000000 nio-bot-1.0.0/docs/reference/utils/string_view.md
+-rw-r--r--   0 nex       (1000) nex       (1000)     2346 2023-07-03 21:31:35.000000 nio-bot-1.0.0/docs/reference/utils/typing.md
+-rw-r--r--   0 nex       (1000) nex       (1000)     1960 2023-07-04 10:48:38.000000 nio-bot-1.0.0/docs/reference/utils/unblock.md
+drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 12:39:54.624562 nio-bot-1.0.0/examples/
+-rw-r--r--   0 nex       (1000) nex       (1000)     1636 2023-06-13 20:43:23.000000 nio-bot-1.0.0/examples/access_token.py
+-rw-r--r--   0 nex       (1000) nex       (1000)     1605 2023-06-13 20:35:19.000000 nio-bot-1.0.0/examples/hello_world.py
+-rw-r--r--   0 nex       (1000) nex       (1000)     1210 2023-06-15 08:59:25.000000 nio-bot-1.0.0/examples/uploading.py
+-rw-r--r--   0 nex       (1000) nex       (1000)     1243 2023-07-04 21:28:18.000000 nio-bot-1.0.0/mkdocs.yml
+-rw-r--r--   0 nex       (1000) nex       (1000)      781 2023-07-04 21:26:46.000000 nio-bot-1.0.0/pyproject.toml
+-rw-r--r--   0 nex       (1000) nex       (1000)       91 2023-07-04 18:30:33.000000 nio-bot-1.0.0/requirements.txt
+-rw-r--r--   0 nex       (1000) nex       (1000)       38 2023-07-12 12:39:54.627895 nio-bot-1.0.0/setup.cfg
+drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 12:39:54.617895 nio-bot-1.0.0/src/
+drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 12:39:54.624562 nio-bot-1.0.0/src/nio_bot.egg-info/
+-rw-r--r--   0 nex       (1000) nex       (1000)     8268 2023-07-12 12:39:54.000000 nio-bot-1.0.0/src/nio_bot.egg-info/PKG-INFO
+-rw-r--r--   0 nex       (1000) nex       (1000)     1409 2023-07-12 12:39:54.000000 nio-bot-1.0.0/src/nio_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 nex       (1000) nex       (1000)        1 2023-07-12 12:39:54.000000 nio-bot-1.0.0/src/nio_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 nex       (1000) nex       (1000)       58 2023-07-12 12:39:54.000000 nio-bot-1.0.0/src/nio_bot.egg-info/entry_points.txt
+-rw-r--r--   0 nex       (1000) nex       (1000)      203 2023-07-12 12:39:54.000000 nio-bot-1.0.0/src/nio_bot.egg-info/requires.txt
+-rw-r--r--   0 nex       (1000) nex       (1000)        7 2023-07-12 12:39:54.000000 nio-bot-1.0.0/src/nio_bot.egg-info/top_level.txt
+drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 12:39:54.624562 nio-bot-1.0.0/src/niobot/
+-rw-r--r--   0 nex       (1000) nex       (1000)      806 2023-07-12 12:39:09.000000 nio-bot-1.0.0/src/niobot/__init__.py
+-rw-r--r--   0 nex       (1000) nex       (1000)    13336 2023-07-12 12:39:09.000000 nio-bot-1.0.0/src/niobot/__main__.py
+-rw-r--r--   0 nex       (1000) nex       (1000)      160 2023-07-12 12:39:54.000000 nio-bot-1.0.0/src/niobot/__version__.py
+-rw-r--r--   0 nex       (1000) nex       (1000)    31604 2023-07-12 12:39:09.000000 nio-bot-1.0.0/src/niobot/attachment.py
+-rw-r--r--   0 nex       (1000) nex       (1000)    32431 2023-07-12 12:39:09.000000 nio-bot-1.0.0/src/niobot/client.py
+-rw-r--r--   0 nex       (1000) nex       (1000)    12273 2023-07-12 12:39:09.000000 nio-bot-1.0.0/src/niobot/commands.py
+-rw-r--r--   0 nex       (1000) nex       (1000)     5146 2023-07-12 12:39:09.000000 nio-bot-1.0.0/src/niobot/context.py
+-rw-r--r--   0 nex       (1000) nex       (1000)     3952 2023-07-12 12:39:09.000000 nio-bot-1.0.0/src/niobot/exceptions.py
+drwxr-xr-x   0 nex       (1000) nex       (1000)        0 2023-07-12 12:39:54.627895 nio-bot-1.0.0/src/niobot/utils/
+-rw-r--r--   0 nex       (1000) nex       (1000)      777 2023-07-03 20:38:45.000000 nio-bot-1.0.0/src/niobot/utils/__init__.py
+-rw-r--r--   0 nex       (1000) nex       (1000)     1531 2023-07-12 12:39:09.000000 nio-bot-1.0.0/src/niobot/utils/federation.py
+-rw-r--r--   0 nex       (1000) nex       (1000)     5027 2023-07-12 12:39:09.000000 nio-bot-1.0.0/src/niobot/utils/help_command.py
+-rw-r--r--   0 nex       (1000) nex       (1000)     3535 2023-06-28 19:12:30.000000 nio-bot-1.0.0/src/niobot/utils/parsers.py
+-rw-r--r--   0 nex       (1000) nex       (1000)     3467 2023-07-04 19:58:56.000000 nio-bot-1.0.0/src/niobot/utils/string_view.py
+-rw-r--r--   0 nex       (1000) nex       (1000)     1553 2023-07-03 21:16:02.000000 nio-bot-1.0.0/src/niobot/utils/typing.py
+-rw-r--r--   0 nex       (1000) nex       (1000)     2071 2023-07-04 10:53:34.000000 nio-bot-1.0.0/src/niobot/utils/unblocking.py
```

### Comparing `nio-bot-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md` & `nio-bot-1.0.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `nio-bot-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md` & `nio-bot-1.0.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `nio-bot-0.1.0/.gitignore` & `nio-bot-1.0.0/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -332,7 +332,9 @@
 .history
 .ionide
 
 # End of https://www.toptal.com/developers/gitignore/api/python,venv,visualstudiocode,git,pycharm
 
 src/niobot/__version__.py
 # Setuptools tells us to explicitly ignore this
+/niobot
+# ^ I symlink /src/niobot to /niobot for docs so I don't have to remember to `cd` into `src.`
```

### Comparing `nio-bot-0.1.0/.idea/inspectionProfiles/Project_Default.xml` & `nio-bot-1.0.0/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `nio-bot-0.1.0/LICENSE` & `nio-bot-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nio-bot-0.1.0/PKG-INFO` & `nio-bot-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nio-bot
-Version: 0.1.0
+Version: 1.0.0
 Summary: Making matrix bots simple
 Author-email: Nexus <packages@nexy7574.co.uk>
 License: GNU GPLv3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: e2ee
 Provides-Extra: cli
```

### Comparing `nio-bot-0.1.0/README.md` & `nio-bot-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `nio-bot-0.1.0/docs/guides/getting-started.md` & `nio-bot-1.0.0/docs/guides/getting-started.md`

 * *Files identical despite different names*

### Comparing `nio-bot-0.1.0/docs/index.md` & `nio-bot-1.0.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `nio-bot-0.1.0/docs/reference/context.md` & `nio-bot-1.0.0/docs/reference/context.md`

 * *Files identical despite different names*

### Comparing `nio-bot-0.1.0/docs/reference/utils/help_command.md` & `nio-bot-1.0.0/docs/reference/utils/help_command.md`

 * *Files identical despite different names*

### Comparing `nio-bot-0.1.0/docs/reference/utils/parsers.md` & `nio-bot-1.0.0/docs/reference/utils/parsers.md`

 * *Files identical despite different names*

### Comparing `nio-bot-0.1.0/docs/reference/utils/string_view.md` & `nio-bot-1.0.0/docs/reference/utils/string_view.md`

 * *Files identical despite different names*

### Comparing `nio-bot-0.1.0/docs/reference/utils/typing.md` & `nio-bot-1.0.0/docs/reference/utils/typing.md`

 * *Files identical despite different names*

### Comparing `nio-bot-0.1.0/docs/reference/utils/unblock.md` & `nio-bot-1.0.0/docs/reference/utils/unblock.md`

 * *Files identical despite different names*

### Comparing `nio-bot-0.1.0/examples/access_token.py` & `nio-bot-1.0.0/examples/access_token.py`

 * *Files identical despite different names*

### Comparing `nio-bot-0.1.0/examples/hello_world.py` & `nio-bot-1.0.0/examples/hello_world.py`

 * *Files identical despite different names*

### Comparing `nio-bot-0.1.0/examples/uploading.py` & `nio-bot-1.0.0/examples/uploading.py`

 * *Files identical despite different names*

### Comparing `nio-bot-0.1.0/mkdocs.yml` & `nio-bot-1.0.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `nio-bot-0.1.0/pyproject.toml` & `nio-bot-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nio-bot-0.1.0/src/nio_bot.egg-info/PKG-INFO` & `nio-bot-1.0.0/src/nio_bot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nio-bot
-Version: 0.1.0
+Version: 1.0.0
 Summary: Making matrix bots simple
 Author-email: Nexus <packages@nexy7574.co.uk>
 License: GNU GPLv3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: e2ee
 Provides-Extra: cli
```

### Comparing `nio-bot-0.1.0/src/nio_bot.egg-info/SOURCES.txt` & `nio-bot-1.0.0/src/nio_bot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nio-bot-0.1.0/src/niobot/__init__.py` & `nio-bot-1.0.0/src/niobot/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,28 @@
+from nio import *
 from . import utils
 from .utils import *
 from .client import *
-from .attachment import *
 from .commands import *
 from .context import *
 from .exceptions import *
-
-
+try:
+    from .attachment import *
+    ATTACHMENTS_AVAILABLE = True
+except ImportError:
+    pass
+    ATTACHMENTS_AVAILABLE = False
 
 try:
     import __version__ as version_meta
 except ImportError:
     class __VersionMeta:
         __version__ = "0.0.dev0+gFFFFFF"
         __version_tuple__ = (0, 0, "dev0", "gFFFFFF")
-    version_meta = __VersionMeta
+    version_meta = __VersionMeta()
 
 __author__ = "Nexus <pip@nexy7574.co.uk>"
 __license__ = "GNU GPLv3"
 __url__ = "https://github.com/EEKIM10/niobot"
 __title__ = "niobot"
 __description__ = "A Matrix bot framework written in Python built on matrix-nio."
-
-
-def __user_agent__() -> str:
-    """Returns the user agent for the bot"""
-    return f"Mozilla/5.0 {__title__}/{version_meta.__version__} ({__url__})"
+__user_agent__ = f"Mozilla/5.0 {__title__}/{version_meta.__version__} ({__url__})"
```

### Comparing `nio-bot-0.1.0/src/niobot/__main__.py` & `nio-bot-1.0.0/src/niobot/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import asyncio
 import datetime
 import os
+import pathlib
 import re
 import sys
 import logging
 
 import niobot
 import importlib.metadata
 
@@ -116,23 +117,28 @@
             logger.critical("Failed to resolve nio version information via pip.")
             nio_version = "0.0.0"
         else:
             logger.debug("Successfully resolved nio version information via pip.")
             nio_version = result.stdout.splitlines()[1].split(": ")[1]
 
     t = ctx.obj["version_tuple"]
-    t3 = t[3] or 'gN/A.d%s' % (datetime.datetime.now().strftime("%Y%m%d"))
-    try:
-        t3_commit, t3_date_raw = t3.split(".", 1)
-    except ValueError:
-        t3_commit = t3
-        logger.warning("Failed to parse commit date from %r, using current date instead.", t3)
-        t3_date = datetime.datetime.now()
-        t3_date_raw = t3_date.strftime("%Y%m%d")
-    t3_date = datetime.datetime.strptime(t3_date_raw[1:], "%Y%m%d")
+    if len(t) > 3:
+        t3 = t[3] or 'gN/A.d%s' % (datetime.datetime.now().strftime("%Y%m%d"))
+        try:
+            t3_commit, t3_date_raw = t3.split(".", 1)
+        except ValueError:
+            t3_commit = t3
+            logger.warning("Failed to parse commit date from %r, using current date instead.", t3)
+            t3_date = datetime.datetime.now()
+            t3_date_raw = t3_date.strftime("%Y%m%d")
+        t3_date = datetime.datetime.strptime(t3_date_raw[1:], "%Y%m%d")
+    else:
+        t3_commit = "<release>"
+        mtime = pathlib.Path(__file__).stat().st_mtime
+        t3_date = datetime.datetime.fromtimestamp(mtime)
 
     bot_version_deep = {
         "version": "%d.%d" % (t[0], t[1]),
         "build": t[2],
         "commit": t3_commit,
         "date": t3_date
     }
```

### Comparing `nio-bot-0.1.0/src/niobot/client.py` & `nio-bot-1.0.0/src/niobot/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,18 @@
 import typing
 from collections import deque
 
 import nio
 from nio.crypto import ENCRYPTION_ENABLED
 import marko
 
-from .attachment import MediaAttachment
+try:
+    from .attachment import BaseAttachment
+except ImportError:
+    BaseAttachment = None
 from .exceptions import *
 from .utils import run_blocking, Typing, force_await
 from .utils.help_command import help_command_callback
 from .commands import Command, Module
 
 
 __all__ = (
@@ -32,35 +35,35 @@
     :param device_id: The device ID to log in as. e.g. nio-bot
     :param store_path: The path to the store file. Defaults to ./store. Must be a directory.
     :param command_prefix: The prefix to use for commands. e.g. !
     :param case_insensitive: Whether to ignore case when checking for commands. If True, this lower()s
      incoming messages for parsing.
     :param global_message_type: The message type to default to. Defaults to m.notice
     :param ignore_old_events: Whether to simply discard events before the bot's login.
+    :param auto_join_rooms: Whether to automatically join rooms the bot is invited to.
+    :param automatic_markdown_renderer: Whether to automatically render markdown in messages when sending/editing.
     :param owner_id: The user ID of the bot owner. If set, only this user can run owner-only commands, etc.
     """
     def __init__(
             self,
             homeserver: str,
             user_id: str,
             device_id: str = "nio-bot",
             store_path: str = None,
             *,
             command_prefix: str,
             case_insensitive: bool = True,
             owner_id: str = None,
-            global_message_type: str = "m.notice",
-            ignore_old_events: bool = True,
             **kwargs
     ):
         self.log = logging.getLogger(__name__)
         if store_path:
             if not os.path.exists(store_path):
                 self.log.warning("Store path %s does not exist, creating...", store_path)
-                os.makedirs(store_path, mode=0o755, exist_ok=True)
+                os.makedirs(store_path, mode=0o751, exist_ok=True)
             elif not os.path.isdir(store_path):
                 raise RuntimeError("Store path %s is not a directory!" % store_path)
 
         if ENCRYPTION_ENABLED:
             if not kwargs.get("config"):
                 kwargs.setdefault(
                     "config",
@@ -84,15 +87,15 @@
         self.device_id = device_id
         self.store_path = store_path
         self.case_insensitive = case_insensitive
         self.command_prefix = command_prefix
         self.owner_id = owner_id
 
         if command_prefix == "/":
-            self.log.warning("The prefix '/' may interfere with client-side commands.")
+            self.log.warning("The prefix '/' may interfere with client-side commands on some clients, such as Element.")
         if " " in command_prefix:
             raise RuntimeError("Command prefix cannot contain spaces.")
 
         self.start_time: float | None = None
         help_cmd = Command(
             "help",
             help_command_callback,
@@ -108,14 +111,15 @@
         self._event_tasks = []
         self.global_message_type = kwargs.pop(
             "global_message_type",
             "m.notice"
         )
         self.ignore_old_events = kwargs.pop("ignore_old_events", True)
         self.auto_join_rooms = kwargs.pop("auto_join_rooms", True)
+        self.automatic_markdown_renderer = kwargs.pop("automatic_markdown_renderer", True)
         # NOTE: `m.notice` prevents bot messages sending off room notifications, and shows darker text
         # (In element at least).
 
         # noinspection PyTypeChecker
         self.add_event_callback(self.process_message, nio.RoomMessageText)
         self.add_event_callback(
             self.update_read_receipts,
@@ -293,14 +297,16 @@
 
         !!! warning
             Modifying any values here will update the internal register too.
 
         !!! note
             Aliases of commands are treated as their own command instance. You will see the same command show up as a
             value multiple times if it has aliases.
+
+            You can check if two commands are identical by comparing them (`command1instance == command2instance`)
         """
         return self._commands
 
     @property
     def modules(self) -> typing.Dict[typing.Type[Module], Module]:
         """Returns the internal module register.
 
@@ -481,121 +487,143 @@
             return obj.room_id
         if hasattr(obj, "event_id"):
             return obj.event_id
         if isinstance(obj, str):
             return obj
         raise ValueError("Unable to determine ID")
 
+    @staticmethod
+    def generate_mx_reply(room: nio.MatrixRoom, event: nio.RoomMessageText) -> str:
+        """Generates a reply string for a given event."""
+        return (
+            "<mx-reply>"
+            "<blockquote>"
+            "<a href=\"{reply_url}\">{reply}</a> "
+            "<a href=\"{user_url}\">{user}</a><br/>"
+            "</blockquote>"
+            "</mx-reply>".format(
+                reply_url="https://matrix.to/#/{}:{}/{}".format(
+                    room.room_id,
+                    room.machine_name.split(":")[1],
+                    event.event_id
+                ),
+                reply=event.body,
+                user_url="https://matrix.to/#/{}".format(
+                    event.sender
+                ),
+                user=event.sender,
+            )
+        )
+
+    async def _recursively_upload_attachments(
+            self,
+            base: "BaseAttachment",
+            encrypted: bool = False,
+            __previous: list = None
+    ) -> list[typing.Union[nio.UploadResponse, nio.UploadError, type(None)]]:
+        """Recursively uploads attachments."""
+        previous = (__previous or []).copy()
+        if not base.url:
+            previous.append(await base.upload(self, encrypted))
+        if hasattr(base, 'thumbnail') and base.thumbnail and not base.url:
+            previous += await self._recursively_upload_attachments(base.thumbnail, encrypted, previous)
+        return previous
+
     async def send_message(
             self,
             room: nio.MatrixRoom | str,
             content: str = None,
-            file: MediaAttachment = None,
+            file: BaseAttachment = None,
             reply_to: nio.RoomMessageText | str = None,
             message_type: str = None
     ) -> nio.RoomSendResponse:
         """
         Sends a message.
 
         :param room: The room to send this message to
         :param content: The content to send. Cannot be used with file.
         :param file: A file to send, if any. Cannot be used with content.
         :param reply_to: A message to reply to.
-        :param message_type: The message type to send. If none, defaults to NioBot.global_message_type, which itself is `m.notice` by default.
+        :param message_type: The message type to send. If none, defaults to NioBot.global_message_type,
+        which itself is `m.notice` by default.
         :return: The response from the server.
         :raises MessageException: If the message fails to send, or if the file fails to upload.
         :raises ValueError: You specified neither file nor content.
-
         """
+        if file and BaseAttachment is None:
+            raise ValueError("You are missing required libraries to use attachments.")
         if not any((content, file)):
             raise ValueError("You must specify either content or file.")
-        elif file and not content:
-            raise ValueError("You must specify content (a textual description of the media) while using file.")
 
         body = {
             "msgtype": message_type or self.global_message_type,
             "body": content,
         }
 
+        if file is not None:
+            # We need to upload the file first.
+            responses = await self._recursively_upload_attachments(file, encrypted=getattr(file, "encrypted", False))
+            if any((isinstance(response, nio.UploadError) for response in responses)):
+                raise MessageException(
+                    "Failed to upload media.", tuple(filter(lambda x: isinstance(x, nio.UploadError), responses))[0]
+                )
+
+            body = file.as_body(content)
+        else:
+            if self.automatic_markdown_renderer:
+                parsed = await run_blocking(marko.parse, content)
+                if parsed.children:
+                    rendered = await run_blocking(marko.render, parsed)
+                    body["formatted_body"] = rendered
+                    body["format"] = "org.matrix.custom.html"
+
+                if reply_to and isinstance(reply_to, nio.RoomMessageText) and isinstance(room, nio.MatrixRoom):
+                    body["formatted_body"] = "{}{}".format(
+                        self.generate_mx_reply(room, reply_to),
+                        body.get("formatted_body", body["body"])
+                    )
+                    body["format"] = "org.matrix.custom.html"
+
         if reply_to:
             body["m.relates_to"] = {
                 "m.in_reply_to": {
                     "event_id": self._get_id(reply_to)
                 }
             }
-
-        if file:
-            # We need to upload the file first.
-            response = await file.upload(self)
-            if isinstance(response, nio.UploadError):
-                raise MessageException("Failed to upload media.", response)
-
-            body["msgtype"] = file.media_type
-            body["info"] = file.to_dict()
-            body["url"] = file.url
-        else:
-            parsed = await run_blocking(marko.parse, content)
-            if parsed.children:
-                rendered = await run_blocking(marko.render, parsed)
-                body["formatted_body"] = rendered
-                body["format"] = "org.matrix.custom.html"
-
-            if reply_to and isinstance(reply_to, nio.RoomMessageText) and isinstance(room, nio.MatrixRoom):
-                body["formatted_body"] = "<mx-reply>" \
-                       "<blockquote>" \
-                       "<a href=\"{reply_url}\">{reply}</a> " \
-                       "<a href=\"{user_url}\">{user}</a><br/>" \
-                       "</blockquote>" \
-                       "</mx-reply>" \
-                       "{body}".format(
-                            reply_url="https://matrix.to/#/{}:{}/{}".format(
-                                room.room_id,
-                                room.machine_name.split(":")[1],
-                                reply_to.event_id
-                            ),
-                            reply=reply_to.body,
-                            user_url="https://matrix.to/#/{}".format(
-                                reply_to.sender
-                            ),
-                            user=reply_to.sender,
-                            body=body.get("formatted_body", body.get("body"))
-                       )
-                body["format"] = "org.matrix.custom.html"
-        async with Typing(self, room.room_id):
+        async with Typing(self, self._get_id(room)):
             response = await self.room_send(
                 self._get_id(room),
                 "m.room.message",
                 body,
             )
         if isinstance(response, nio.RoomSendError):
             raise MessageException("Failed to send message.", response)
-        await self.room_typing(room.room_id, False)
         return response
 
     async def edit_message(
             self,
             room: nio.MatrixRoom | str,
-            event_id: nio.Event | str,
+            message: nio.Event | str,
             content: str,
             *,
             message_type: str = None,
     ) -> nio.RoomSendResponse:
         """
         Edit an existing message. You must be the sender of the message.
 
         You also cannot edit messages that are attachments.
 
         :param room: The room the message is in.
-        :param event_id: The message to edit.
+        :param message: The message to edit.
         :param content: The new content of the message.
         :param message_type: The new type of the message (i.e. m.text, m.notice. Defaults to client.global_message_type)
         :raises RuntimeError: If you are not the sender of the message.
         :raises TypeError: If the message is not text.
         """
-        event_id = self._get_id(event_id)
+        event_id = self._get_id(message)
         message_type = message_type or self.global_message_type
         content = {
             "msgtype": message_type,
             "body": content,
             "format": "org.matrix.custom.html",
             "formatted_body": await self._markdown_to_html(content),
         }
@@ -617,14 +645,16 @@
             response = await self.room_send(
                 self._get_id(room),
                 "m.room.message",
                 body,
             )
         if isinstance(response, nio.RoomSendError):
             raise MessageException("Failed to edit message.", response)
+        # Forcefully clear typing
+        await self.room_typing(room.room_id, False)
         return response
 
     async def delete_message(
             self,
             room: nio.MatrixRoom | str,
             message_id: nio.RoomMessage | str,
             reason: str = None
@@ -632,21 +662,62 @@
         """
         Delete an existing message. You must be the sender of the message.
 
         :param room: The room the message is in.
         :param message_id: The message to delete.
         :param reason: The reason for deleting the message.
         :raises RuntimeError: If you are not the sender of the message.
+        :raises MessageException: If the message fails to delete.
         """
         room = self._get_id(room)
         message_id = self._get_id(message_id)
         response = await self.room_redact(room, message_id, reason=reason)
         if isinstance(response, nio.RoomRedactError):
             raise MessageException("Failed to delete message.", response)
-        self.log.debug("delete_message: %r", response)
+        return response
+
+    async def add_reaction(
+            self,
+            room: nio.MatrixRoom | str,
+            message: nio.RoomMessage | str,
+            emoji: str
+    ) -> nio.RoomSendResponse:
+        """
+        Adds an emoji "reaction" to a message.
+
+        :param room: The room the message is in.
+        :param message: The event ID or message object to react to.
+        :param emoji: The emoji to react with (e.g. `\N{cross mark}` = ❌)
+        :return: The response from the server.
+        :raises MessageException: If the message fails to react.
+        """
+        body = {
+            "m.relates_to": {
+                "event_id": self._get_id(message),
+                "rel_type": "m.annotation",
+                "key": emoji,
+            }
+        }
+        response = await self.room_send(
+            self._get_id(room),
+            "m.reaction",
+            body,
+        )
+        if isinstance(response, nio.RoomSendError):
+            raise MessageException("Failed to add reaction.", response)
+        return response
+
+    async def redact_reaction(self, room: nio.MatrixRoom | str, reaction: nio.RoomSendResponse | str):
+        """Alias for NioBot.delete_message, but more appropriately named for reactions."""
+        response = await self.room_redact(
+            self._get_id(room),
+            self._get_id(reaction),
+        )
+        if isinstance(response, nio.RoomRedactError):
+            raise MessageException("Failed to delete reaction.", response)
         return response
 
     async def start(self, password: str = None, access_token: str = None, sso_token: str = None) -> None:
         """Starts the bot, running the sync loop."""
         if password or sso_token:
             self.log.info("Logging in with a password or SSO token")
             login_response = await self.login(password=password, token=sso_token, device_name=self.device_id)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nio-bot-0.1.0/src/niobot/commands.py` & `nio-bot-1.0.0/src/niobot/commands.py`

 * *Files 21% similar despite different names*

```diff
@@ -66,14 +66,18 @@
             self.required = default is ...
             self.default = None
         self.extra = kwargs
         self.parser = parser
         if self.parser is ...:
             self.parser = self.internal_parser
 
+    def __repr__(self):
+        return "<Argument name={0.name!r} type={0.type!r} default={0.default!r} required={0.required!r} " \
+               "parser={0.parser!r}>".format(self)
+
     @staticmethod
     def internal_parser(_: Context, arg: "Argument", value: str) -> typing.Optional[_T]:
         """The default parser for the argument. Will try to convert the value to the argument type."""
         try:
             return arg.type(value)
         except ValueError:
             raise CommandArgumentsError(f"Invalid value for argument {arg.name}: {value!r}")
@@ -114,17 +118,18 @@
     :param arguments:
         A list of [`Argument`][niobot.commands.Argument] instances. Will be used to parse the arguments given to the
         command.
         `ctx` is always the first argument, regardless of what you put here.
     :param usage:
         A string representing how to use this command's arguments. Will be shown in the auto-generated help.
         Do not include the command name or your bot's prefix here, only arguments.
+        For example: `usage="<message> [times]"` will show up as `[p][command] <message> [times]` in the help command.
 
     """
-    CTX_ARG = Argument(
+    _CTX_ARG = Argument(
         "ctx",
         Context,
         description="The context for the command",
         parser=lambda ctx, *_: ctx
     )
 
     def __init__(
@@ -142,16 +147,58 @@
         self.name = name
         self.callback = callback
         self.description = description
         self.disabled = disabled
         self.aliases = aliases or []
         self.usage = kwargs.pop("usage", None)
         self.module = kwargs.pop("module", None)
-        self.arguments = kwargs.pop("arguments", None) or []
-        self.arguments.insert(0, self.CTX_ARG)
+        self.arguments = kwargs.pop("arguments", None)
+        if not self.arguments:
+            if self.arguments is False:  # do not autodetect arguments
+                self.arguments = []
+            else:
+                self.arguments = self.autodetect_args(self.callback)
+        self.arguments.insert(0, self._CTX_ARG)
+        self.arguments: list[Argument]
+
+    @staticmethod
+    def autodetect_args(callback) -> list[Argument]:
+        """
+        Attempts to auto-detect the arguments for the command, based on the callback's signature
+
+        :param callback: The function to inspect
+        :return: A list of arguments. `self`, and `ctx` are skipped.
+        """
+        # We need to get each parameter's type annotation, and create an Argument for it.
+        # If it has a default value, assign that default value to the Argument.
+        # If the parameter is `self`, ignore it.
+        # If the parameter is `ctx`, use the `Context` type.
+        args = []
+        for n, parameter in enumerate(inspect.signature(callback).parameters.values()):
+            # If it has a parent class and this is the first parameter, skip it.
+            if n == 0 and parameter.name == "self":
+                continue
+
+            if parameter.name in ["ctx", "context"] or parameter.annotation is Context:
+                continue
+
+            # Disallow *args and **kwargs
+            if parameter.kind in [inspect.Parameter.VAR_POSITIONAL, inspect.Parameter.VAR_KEYWORD]:
+                raise CommandArgumentsError("Cannot use *args or **kwargs in command callback (argument No. %d)" % n)
+
+            if parameter.annotation is inspect.Parameter.empty:
+                a = Argument(parameter.name, str, default=parameter.default)
+            else:
+                a = Argument(parameter.name, parameter.annotation)
+
+            if parameter.default is not inspect.Parameter.empty:
+                a.default = parameter.default
+                a.required = False
+            args.append(a)
+        return args
 
     def __hash__(self):
         return hash(self.__runtime_id)
 
     def __eq__(self, other):
         """Checks if another command's runtime ID is the same as this one's"""
         if isinstance(other, Command):
@@ -161,14 +208,30 @@
 
     def __repr__(self):
         return "<Command name={0.name!r} aliases={0.aliases} disabled={0.disabled}>".format(self)
 
     def __str__(self):
         return self.name
 
+    @property
+    def display_usage(self) -> str:
+        """Returns the usage string for this command, auto-resolved if not pre-defined"""
+        if self.usage:
+            return self.usage
+        else:
+            usage = []
+            req = "<{!s}>"
+            opt = "[{!s}]"
+            for arg in self.arguments[1:]:
+                if arg.required:
+                    usage.append(req.format(arg.name))
+                else:
+                    usage.append(opt.format(arg.name))
+            return " ".join(usage)
+
     def invoke(self, ctx: Context):
         """Invokes the current command with the given context"""
         parsed_args = []
         for index, argument in enumerate(self.arguments[1:], 0):
             argument: Argument
             if index >= len(ctx.args):
                 if argument.required:
```

### Comparing `nio-bot-0.1.0/src/niobot/context.py` & `nio-bot-1.0.0/src/niobot/context.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import typing
 
 from .utils.string_view import ArgumentView
 
 if typing.TYPE_CHECKING:
     from .client import NioBot
     from .commands import Command
-    from .attachment import MediaAttachment
+    from .attachment import BaseAttachment
 
 
 __all__ = (
     "Context",
     "ContextualResponse"
 )
 
@@ -24,14 +24,17 @@
     """Context class for managing replies.
 
     Usage of this function is not required, however it is a useful utility."""
     def __init__(self, ctx: "Context", response: nio.RoomSendResponse):
         self.ctx = ctx
         self._response = response
 
+    def __repr__(self):
+        return "<ContextualResponse ctx={0.ctx!r} response={0.response!r}>".format(self)
+
     @property
     def message(self) -> nio.RoomMessageText | None:
         """Fetches the current message for this response"""
         result = self.ctx.client.get_cached_message(self._response.event_id)
         if result:
             return result[1]
         else:
@@ -104,14 +107,26 @@
                 to_parse = event.body[len(invoking_string):]
             except IndexError:
                 to_parse = ""
         self._args = ArgumentView(to_parse)
         self._args.parse_arguments()
         self._original_response = None
 
+    def __repr__(self):
+        return "<Context room={0.room!r} event={0.event!r} command={0.command!r}>".format(self)
+
+    def __eq__(self, other):
+        if not isinstance(other, Context):
+            return False
+        return (
+            self.room == other.room and
+            self.event == other.event and
+            self.command == other.command
+        )
+
     @property
     def room(self) -> nio.MatrixRoom:
         """The room that the event was dispatched in"""
         return self._room
 
     @property
     def client(self) -> "NioBot":
@@ -145,15 +160,15 @@
     msg = event = message
 
     @property
     def latency(self) -> float:
         """Returns the current event's latency in milliseconds."""
         return self.client.latency(self.event, received_at=self._init_ts)
 
-    async def respond(self, content: str = None, file: "MediaAttachment" = None) -> ContextualResponse:
+    async def respond(self, content: str = None, file: "BaseAttachment" = None) -> ContextualResponse:
         """
         Responds to the current event.
 
         :param content: The text to reply with
         :param file: A file to reply with
         :return:
         """
```

### Comparing `nio-bot-0.1.0/src/niobot/utils/__init__.py` & `nio-bot-1.0.0/src/niobot/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nio-bot-0.1.0/src/niobot/utils/federation.py` & `nio-bot-1.0.0/src/niobot/utils/federation.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     :param domain: The domain to crawl
     :return: The resolved homeserver
     """
     from niobot import __user_agent__
     if not domain.startswith("https://"):
         domain = f"https://{domain}"
     domain = urlparse(domain).netloc
-    async with aiohttp.ClientSession(headers={"User-Agent": __user_agent__()}) as session:
+    async with aiohttp.ClientSession(headers={"User-Agent": __user_agent__}) as session:
         async with session.get(f"https://{domain}/.well-known/matrix/client") as resp:
             if resp.status == 200:
                 if resp.content_type != "application/json":
                     try:
                         data = await resp.text("utf-8")
                     except UnicodeDecodeError:
                         raise ValueError("Invalid homeserver response for well-known")
```

### Comparing `nio-bot-0.1.0/src/niobot/utils/help_command.py` & `nio-bot-1.0.0/src/niobot/utils/help_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,16 +75,15 @@
         )
 
 
 def format_command_line(prefix: str, command: "Command") -> str:
     """Formats a command line, including name(s) & usage."""
     name = format_command_name(command)
     start = "{}{}".format(prefix, name)
-    if command.usage:
-        start += " " + command.usage.strip().replace("\n", "")
+    start += " " + command.display_usage.strip().replace("\n", "")
 
     return start
 
 
 def get_short_description(command: "Command") -> str:
     """Generates a short (<100 characters) help description for a command."""
     if not command.description:
```

### Comparing `nio-bot-0.1.0/src/niobot/utils/parsers.py` & `nio-bot-1.0.0/src/niobot/utils/parsers.py`

 * *Files identical despite different names*

### Comparing `nio-bot-0.1.0/src/niobot/utils/string_view.py` & `nio-bot-1.0.0/src/niobot/utils/string_view.py`

 * *Files identical despite different names*

### Comparing `nio-bot-0.1.0/src/niobot/utils/typing.py` & `nio-bot-1.0.0/src/niobot/utils/typing.py`

 * *Files identical despite different names*

### Comparing `nio-bot-0.1.0/src/niobot/utils/unblocking.py` & `nio-bot-1.0.0/src/niobot/utils/unblocking.py`

 * *Files identical despite different names*


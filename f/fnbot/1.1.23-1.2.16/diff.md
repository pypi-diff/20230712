# Comparing `tmp/fnbot-1.1.23.tar.gz` & `tmp/fnbot-1.2.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fnbot-1.1.23.tar", last modified: Sat Nov 26 08:01:44 2022, max compression
+gzip compressed data, was "fnbot-1.2.16.tar", last modified: Wed Jul 12 12:56:56 2023, max compression
```

## Comparing `fnbot-1.1.23.tar` & `fnbot-1.2.16.tar`

### file list

```diff
@@ -1,24 +1,10 @@
-drwxrwxrwx   0        0        0        0 2022-11-26 08:01:44.291899 fnbot-1.1.23/
--rw-rw-rw-   0        0        0      512 2022-11-26 08:01:44.289898 fnbot-1.1.23/PKG-INFO
--rw-rw-rw-   0        0        0        0 2022-08-12 10:01:51.000000 fnbot-1.1.23/README.md
-drwxrwxrwx   0        0        0        0 2022-11-26 08:01:44.222899 fnbot-1.1.23/fnbot/
--rw-rw-rw-   0        0        0     4832 2022-11-24 13:34:18.000000 fnbot-1.1.23/fnbot/__init__.py
--rw-rw-rw-   0        0        0      145 2022-11-26 07:02:43.000000 fnbot-1.1.23/fnbot/__version__.py
-drwxrwxrwx   0        0        0        0 2022-11-26 08:01:44.286899 fnbot-1.1.23/fnbot/bot/
--rw-rw-rw-   0        0        0     3174 2022-11-26 06:11:34.000000 fnbot-1.1.23/fnbot/bot/__init__.py
--rw-rw-rw-   0        0        0    13392 2022-11-26 07:41:32.000000 fnbot-1.1.23/fnbot/bot/_bot_main.py
--rw-rw-rw-   0        0        0    27809 2022-11-26 07:55:48.000000 fnbot-1.1.23/fnbot/bot/charming.py
--rw-rw-rw-   0        0        0    11479 2022-11-26 05:28:44.000000 fnbot-1.1.23/fnbot/bot/config.py
--rw-rw-rw-   0        0        0    10189 2022-11-26 05:03:12.000000 fnbot-1.1.23/fnbot/bot/insert.py
--rw-rw-rw-   0        0        0    10276 2022-11-21 12:31:59.000000 fnbot-1.1.23/fnbot/bot/manual.py
--rw-rw-rw-   0        0        0     3786 2022-11-26 05:37:58.000000 fnbot-1.1.23/fnbot/bot/plugin.py
--rw-rw-rw-   0        0        0     3125 2022-11-24 13:05:40.000000 fnbot-1.1.23/fnbot/bot/receive.py
--rw-rw-rw-   0        0        0    21051 2022-11-26 06:31:43.000000 fnbot-1.1.23/fnbot/bot/send.py
-drwxrwxrwx   0        0        0        0 2022-11-26 08:01:44.257901 fnbot-1.1.23/fnbot.egg-info/
--rw-rw-rw-   0        0        0      512 2022-11-26 08:01:44.000000 fnbot-1.1.23/fnbot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      387 2022-11-26 08:01:44.000000 fnbot-1.1.23/fnbot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-26 08:01:44.000000 fnbot-1.1.23/fnbot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2022-11-26 08:01:44.000000 fnbot-1.1.23/fnbot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-11-26 08:01:44.000000 fnbot-1.1.23/fnbot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-26 08:01:44.291899 fnbot-1.1.23/setup.cfg
--rw-rw-rw-   0        0        0     1125 2022-11-26 08:01:19.000000 fnbot-1.1.23/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 12:56:56.956870 fnbot-1.2.16/
+-rw-rw-rw-   0        0        0      632 2023-07-12 12:56:56.954875 fnbot-1.2.16/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-12 12:56:56.951867 fnbot-1.2.16/fnbot.egg-info/
+-rw-rw-rw-   0        0        0      632 2023-07-12 12:56:56.000000 fnbot-1.2.16/fnbot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      152 2023-07-12 12:56:56.000000 fnbot-1.2.16/fnbot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 12:56:56.000000 fnbot-1.2.16/fnbot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-12 12:56:56.000000 fnbot-1.2.16/fnbot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 12:56:56.000000 fnbot-1.2.16/fnbot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 12:56:56.956870 fnbot-1.2.16/setup.cfg
+-rw-rw-rw-   0        0        0      896 2023-07-12 12:56:05.000000 fnbot-1.2.16/setup.py
```


# Comparing `tmp/nonebot_plugin_l4d2_server-0.5.9.1.tar.gz` & `tmp/nonebot_plugin_l4d2_server-0.5.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_l4d2_server-0.5.9.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_l4d2_server-0.5.9.2.tar", max compression
```

## Comparing `nonebot_plugin_l4d2_server-0.5.9.1.tar` & `nonebot_plugin_l4d2_server-0.5.9.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0    35149 2023-07-10 02:36:47.072109 nonebot_plugin_l4d2_server-0.5.9.1/LICENSE
--rw-r--r--   0        0        0     5683 2023-07-10 02:36:47.072109 nonebot_plugin_l4d2_server-0.5.9.1/README.md
--rw-r--r--   0        0        0    18107 2023-07-10 02:36:47.076109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/__init__.py
--rw-r--r--   0        0        0   158357 2023-07-10 02:36:47.076109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
--rw-r--r--   0        0        0   631630 2023-07-10 02:36:47.076109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
--rw-r--r--   0        0        0   405369 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
--rw-r--r--   0        0        0     1590 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
--rw-r--r--   0        0        0   242997 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
--rw-r--r--   0        0        0     2135 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
--rw-r--r--   0        0        0     6135 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
--rw-r--r--   0        0        0     6170 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
--rw-r--r--   0        0        0     1523 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
--rw-r--r--   0        0        0     5506 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
--rw-r--r--   0        0        0     2408 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
--rw-r--r--   0        0        0     7874 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
--rw-r--r--   0        0        0      486 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
--rw-r--r--   0        0        0     1350 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/img/white.png
--rw-r--r--   0        0        0     9076 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
--rw-r--r--   0        0        0     1607 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
--rw-r--r--   0        0        0     3010 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
--rw-r--r--   0        0        0     1694 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_anne/server.py
--rw-r--r--   0        0        0      359 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
--rw-r--r--   0        0        0     3530 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
--rw-r--r--   0        0        0      468 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_data/config.py
--rw-r--r--   0        0        0        0 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_data/database.py
--rw-r--r--   0        0        0     3364 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_data/players.py
--rw-r--r--   0        0        0     1344 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
--rw-r--r--   0        0        0     4034 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
--rw-r--r--   0        0        0     1868 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
--rw-r--r--   0        0        0     1832 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_file/input_json.py
--rw-r--r--   0        0        0     3074 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_file/remote.py
--rw-r--r--   0        0        0     4211 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
--rw-r--r--   0        0        0     4174 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_image/download.py
--rw-r--r--   0        0        0      665 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
--rw-r--r--   0        0        0     9493 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_image/image.py
--rw-r--r--   0        0        0     1083 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_image/one.py
--rw-r--r--   0        0        0      936 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
--rw-r--r--   0        0        0     4018 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_image/steam.py
--rw-r--r--   0        0        0     1421 2023-07-10 02:36:47.080109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
--rw-r--r--   0        0        0     7222 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_push/__init__.py
--rw-r--r--   0        0        0     3854 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
--rw-r--r--   0        0        0     1148 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_queries/api.py
--rw-r--r--   0        0        0     1030 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
--rw-r--r--   0        0        0    11828 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
--rw-r--r--   0        0        0     1615 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
--rw-r--r--   0        0        0        0 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_server/index.py
--rw-r--r--   0        0        0     1248 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
--rw-r--r--   0        0        0     1359 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
--rw-r--r--   0        0        0     4067 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_update/__init__.py
--rw-r--r--   0        0        0     1185 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py
--rw-r--r--   0        0        0     2024 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_update/restart.py
--rw-r--r--   0        0        0     1434 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_update/update.py
--rw-r--r--   0        0        0     9197 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_utils/command.py
--rw-r--r--   0        0        0     6197 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_utils/config.py
--rw-r--r--   0        0        0     1631 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_utils/message.py
--rw-r--r--   0        0        0      337 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_utils/rule.py
--rw-r--r--   0        0        0     1243 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_utils/seach.py
--rw-r--r--   0        0        0     2149 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py
--rw-r--r--   0        0        0     9994 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_utils/utils.py
--rw-r--r--   0        0        0     8469 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_web/web.py
--rw-r--r--   0        0        0    14982 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
--rw-r--r--   0        0        0     1606 2023-07-10 02:36:47.084109 nonebot_plugin_l4d2_server-0.5.9.1/pyproject.toml
--rw-r--r--   0        0        0     7549 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.5.9.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-12 15:48:48.898191 nonebot_plugin_l4d2_server-0.5.9.2/LICENSE
+-rw-r--r--   0        0        0     5683 2023-07-12 15:48:48.898191 nonebot_plugin_l4d2_server-0.5.9.2/README.md
+-rw-r--r--   0        0        0    18161 2023-07-12 15:48:48.902191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/__init__.py
+-rw-r--r--   0        0        0   158357 2023-07-12 15:48:48.902191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
+-rw-r--r--   0        0        0   631630 2023-07-12 15:48:48.902191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
+-rw-r--r--   0        0        0   405369 2023-07-12 15:48:48.906191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
+-rw-r--r--   0        0        0     1590 2023-07-12 15:48:48.906191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
+-rw-r--r--   0        0        0   242997 2023-07-12 15:48:48.906191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
+-rw-r--r--   0        0        0     2135 2023-07-12 15:48:48.906191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
+-rw-r--r--   0        0        0     6135 2023-07-12 15:48:48.906191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
+-rw-r--r--   0        0        0     6170 2023-07-12 15:48:48.906191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
+-rw-r--r--   0        0        0     1523 2023-07-12 15:48:48.906191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
+-rw-r--r--   0        0        0     5506 2023-07-12 15:48:48.906191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
+-rw-r--r--   0        0        0     2408 2023-07-12 15:48:48.906191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
+-rw-r--r--   0        0        0     7874 2023-07-12 15:48:48.906191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
+-rw-r--r--   0        0        0      486 2023-07-12 15:48:48.906191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
+-rw-r--r--   0        0        0     1350 2023-07-12 15:48:48.906191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/img/white.png
+-rw-r--r--   0        0        0     9076 2023-07-12 15:48:48.906191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
+-rw-r--r--   0        0        0     1607 2023-07-12 15:48:48.906191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
+-rw-r--r--   0        0        0     3010 2023-07-12 15:48:48.906191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
+-rw-r--r--   0        0        0     1715 2023-07-12 15:48:48.906191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_anne/server.py
+-rw-r--r--   0        0        0      359 2023-07-12 15:48:48.906191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
+-rw-r--r--   0        0        0     3530 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
+-rw-r--r--   0        0        0      468 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_data/config.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_data/database.py
+-rw-r--r--   0        0        0     3364 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_data/players.py
+-rw-r--r--   0        0        0     1344 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
+-rw-r--r--   0        0        0     4034 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
+-rw-r--r--   0        0        0     1868 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
+-rw-r--r--   0        0        0     1832 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_file/input_json.py
+-rw-r--r--   0        0        0     3074 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_file/remote.py
+-rw-r--r--   0        0        0     4211 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
+-rw-r--r--   0        0        0     4174 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_image/download.py
+-rw-r--r--   0        0        0      665 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
+-rw-r--r--   0        0        0     9493 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_image/image.py
+-rw-r--r--   0        0        0     1083 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_image/one.py
+-rw-r--r--   0        0        0      936 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
+-rw-r--r--   0        0        0     4018 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_image/steam.py
+-rw-r--r--   0        0        0     1421 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
+-rw-r--r--   0        0        0     7216 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_push/__init__.py
+-rw-r--r--   0        0        0     3854 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
+-rw-r--r--   0        0        0     1148 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_queries/api.py
+-rw-r--r--   0        0        0     1040 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
+-rw-r--r--   0        0        0    11838 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
+-rw-r--r--   0        0        0     1615 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_server/index.py
+-rw-r--r--   0        0        0     1248 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
+-rw-r--r--   0        0        0     1359 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
+-rw-r--r--   0        0        0     4067 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_update/__init__.py
+-rw-r--r--   0        0        0     1185 2023-07-12 15:48:48.910191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py
+-rw-r--r--   0        0        0     2024 2023-07-12 15:48:48.914191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_update/restart.py
+-rw-r--r--   0        0        0     1434 2023-07-12 15:48:48.914191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_update/update.py
+-rw-r--r--   0        0        0     9225 2023-07-12 15:48:48.914191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_utils/command.py
+-rw-r--r--   0        0        0     6021 2023-07-12 15:48:48.914191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_utils/config.py
+-rw-r--r--   0        0        0     1631 2023-07-12 15:48:48.914191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_utils/message.py
+-rw-r--r--   0        0        0      337 2023-07-12 15:48:48.914191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_utils/rule.py
+-rw-r--r--   0        0        0     1219 2023-07-12 15:48:48.914191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_utils/seach.py
+-rw-r--r--   0        0        0     2149 2023-07-12 15:48:48.914191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py
+-rw-r--r--   0        0        0     9329 2023-07-12 15:48:48.914191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_utils/utils.py
+-rw-r--r--   0        0        0     8469 2023-07-12 15:48:48.914191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_web/web.py
+-rw-r--r--   0        0        0    14982 2023-07-12 15:48:48.914191 nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
+-rw-r--r--   0        0        0     1606 2023-07-12 15:48:48.914191 nonebot_plugin_l4d2_server-0.5.9.2/pyproject.toml
+-rw-r--r--   0        0        0     7549 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.5.9.2/PKG-INFO
```

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/LICENSE` & `nonebot_plugin_l4d2_server-0.5.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/README.md` & `nonebot_plugin_l4d2_server-0.5.9.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from typing import Annotated
 from nonebot.params import Keyword
 
 from .l4d2_utils.config import *
 from .l4d2_utils.utils import *
 from .l4d2_utils.command import *
 from .l4d2_image.steam import url_to_byte, url_to_byte_name
-
+from .l4d2_anne.server import updata_anne_server
 from .l4d2_data import sq_L4D2
 from .l4d2_push import *
 from .l4d2_image.vtfs import img_to_vtf
 from .l4d2_file import updown_l4d2_vpk, all_zip_to_one
 from .l4d2_file.input_json import *
 from .l4d2_utils.txt_to_img import mode_txt_to_img
 
@@ -382,25 +382,22 @@
                 file_name = data_one["名字"] + ".vpk"
                 await all_zip_to_one(data_file_list)
                 await upload_file(bot, event, data_file, file_name)
     else:
         await matcher.finish("已取消上传")
 
 
-# @updata.handle()
-# async def _(matcher:Matcher,args:Message = CommandArg()):
-#     """更新"""
-#     msg = args.extract_plain_text()
-#     if not msg:
-#         load_josn()
-#         reload_ip()
-#         await matcher.finish('已更新缓存数据')
-#     else:
-#         message = await write_json(msg)
-#         await matcher.finish(message)
+@updata.handle()
+async def _(matcher: Matcher, args: Message = CommandArg()):
+    """更新"""
+    anne_ip_dict = await updata_anne_server()
+    if not anne_ip_dict:
+        await matcher.finish("网络开小差了捏")
+    server_number = len(anne_ip_dict["云"])
+    await matcher.finish(f"更新成功\n一共更新了{server_number}个电信anne服ip")
 
 
 @vtf_make.handle()
 async def _(matcher: Matcher, state: T_State, args: Message = CommandArg()):
     msg: str = args.extract_plain_text()
     if msg not in ["拉伸", "填充", "覆盖", ""]:
         await matcher.finish("错误的图片处理方式")
```

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/data/img/white.png` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/data/img/white.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_anne/server.py` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_anne/server.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,65 +1,64 @@
 import httpx
 from bs4 import BeautifulSoup
 import json
+import asyncio
+from typing import Dict, List
 from pathlib import Path
-from ..l4d2_utils.config import TEXT_PATH,anne_url,ANNE_IP,gamemode_list
-from ..l4d2_queries.ohter import ALL_HOST
 
-# 储存anne服务器ip
+from ..l4d2_utils.config import CONFIG_PATH, anne_url, ANNE_IP, headers
 
+from ..l4d2_queries.ohter import ALL_HOST
 
+# 储存anne服务器ip
+anne_url = "https://sb.trygek.com/"
+# ANNE_IP = {}
+headers = {
+    "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:107.0) Gecko/20100101 Firefox/107.0"
+}
 
 
 async def updata_anne_server():
     """更新anne服务器列表"""
-    data = httpx.get(anne_url).content
-    soup = BeautifulSoup(data, 'html.parser')
-    tbody = soup.find('tbody')
+    data = httpx.get(anne_url, headers=headers).content
+    soup = BeautifulSoup(data, "html.parser")
+    tbody = soup.find("tbody")
+    if not tbody:
+        return
     n = 0
-    ip_list=[]
+    ip_list = []
     while n < 50:
         n += 1
-        tr = tbody.find(id = f'server_{n}')
+        tr = tbody.find(id=f"server_{n}")  # type: ignore
         if tr:
-            td = tr.select_one("td:nth-of-type(5)").get_text()
+            td: str = tr.select_one("td:nth-of-type(5)").get_text()  # type: ignore
         else:
             continue
-        if td:
+        if not td:
+            continue
+        else:
             ip_list.append(td)
     if not ip_list:
         return None
-    ip_dict = {}
-    n = 0
-    for i in ip_list:
-        n += 1
-        ip_dict.update({f'云{n}':ip_list[n-1]})
+    ip_dict: Dict[str, List[Dict[str, str]]] = {"云": []}
+    n: int = 0
+
+    for i, ip in enumerate(ip_list, start=1):
+        ip_dict["云"].append({"id": str(i), "ip": ip})
+
+    # ANNE_IP.update(ip_dict)
+    with open(Path(CONFIG_PATH.parent / "l4d2/云.json"), "w", encoding="utf-8") as f:
+        json.dump(ip_dict, f, indent=4, ensure_ascii=False)
+    # print(ANNE_IP)
     ANNE_IP.update(ip_dict)
-    with open(Path(TEXT_PATH.parent/'server.json'),'w',encoding='utf-8') as f:
-        json.dump(ANNE_IP, f, indent=4, ensure_ascii=False)
-    return ANNE_IP
-
-async def read_anne_ip():
-    """获取缓存ip"""
-    with open(TEXT_PATH.parent/'server.json','r','utf-8') as f:
-        data = json.load(f)
-        return data
-    
-async def get_anne_ip(text: str) -> str:
-    """从字典里返还消息, 抄(借鉴)的zhenxun-bot"""
-    keys = ANNE_IP.keys()
-    for key in keys:
-        if text == key:
-            return ANNE_IP[key]
-        
+    return ip_dict
+
+
 def server_key():
     """响应的服务器开头"""
     a = set()
     try:
-        for tag1,value in ALL_HOST.items():
+        for tag1, value in ALL_HOST.items():
             a.add(tag1)
-        a.update(gamemode_list)
     except AttributeError:
-        a.add('希腊那我从来没有想过这个事情')
+        a.add("希腊那我从来没有想过这个事情")
     return a
-            
-
```

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_data/__init__.py` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_data/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_data/players.py` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_data/players.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_data/serverip.py` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_data/serverip.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_file/__init__.py` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_file/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_file/input_json.py` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_file/input_json.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_file/remote.py` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_file/remote.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_image/__init__.py` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_image/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_image/download.py` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_image/download.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_image/image.py` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_image/image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_image/one.py` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_image/one.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_image/steam.py` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_image/steam.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_push/__init__.py` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_push/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 import re
 import a2s
-from typing import Dict, List, Union
+from typing import Dict, Union
 
 try:
     import ujson as json
 except:
     import json
 
 from nonebot.log import logger
```

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_queries/api.py` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_queries/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,8 +30,8 @@
             with open(file_path, "r", encoding="utf-8") as f:
                 LOCAL_HOST.update(json.load(f))
     except:
         pass
     return LOCAL_HOST
 
 
-ALL_HOST: Dict[str, List[dict]] = load_josn()
+ALL_HOST: Dict[str, List[Dict[str, str]]] = load_josn()
```

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py`

 * *Files 0% similar despite different names*

```diff
@@ -265,15 +265,15 @@
     group, host, port = await si.query_number(number)
     try:
         return str(host) + ":" + str(port)
     except TypeError:
         return None
 
 
-def split_maohao(msg: str) -> list:
+def split_maohao(msg: str) -> List[str]:
     """分割大小写冒号"""
     if ":" in msg:
         msgs: List[str] = msg.split(":")
     elif "：" in msg:
         msgs: List[str] = msg.split("：")
     elif msg.replace(".", "").isdigit():
         msgs: List[str] = [msg, "20715"]
@@ -299,15 +299,15 @@
             logger.info("新建分支")
             ALL_HOST[data_list[1]] = []
         for key, value in ALL_HOST.items():
             if data_list[1] == key:
                 ids = [server["id"] for server in value]
                 # 序号
                 if len(data_list) == 4:
-                    data_num = max(ids, default=0) + 1
+                    data_num = int(max(ids, default=0)) + 1
                     add_server.update({"id": data_num})
                 elif len(data_list) == 5:
                     if not data_list[4].isdigit():
                         return "序号应该为大于0的正整数，请输入【求生更新 添加 腐竹 ip 模式 序号】"
                     data_num = int(data_list[4])
                     if data_num in ids:
                         return "该序号已存在，请尝试删除原序号【求生更新 删除 腐竹 序号】"
```

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_server/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_server/rcon.py` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_server/rcon.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_server/workshop.py` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_server/workshop.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_update/__init__.py` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_update/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_update/draw_update_log.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_update/restart.py` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_update/restart.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_update/update.py` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_update/update.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_utils/command.py` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_utils/command.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import re
 import asyncio
-from typing import Type
+from typing import Type, List, Tuple
 from time import sleep
 
 from nonebot import on_notice, on_command, on_regex, on_keyword
 from nonebot.params import CommandArg, RawCommand, CommandStart
 from nonebot.matcher import Matcher
-import nonebot
 from nonebot.adapters.onebot.v11 import (
-    GroupUploadNoticeEvent,
     NoticeEvent,
     MessageEvent,
     Message,
     MessageSegment,
     GroupMessageEvent,
 )
 
@@ -44,14 +42,15 @@
         else:
             return name.endswith(file_format)
     elif args["notice_type"] == "group_upload":
         if l4_config.l4_master:
             return usr_id in l4_config.l4_master and name.endswith(file_format)
         else:
             return False
+    return False
 
 
 up = on_notice(rule=wenjian)
 
 
 rename_vpk = on_regex(
     r"^求生地图\s*(\S+.*?)\s*(改|改名)?\s*(\S+.*?)\s*$",
@@ -82,15 +81,17 @@
 )
 del_bind = on_command(
     "del_bind", aliases={"steam解绑", "求生解绑", "anne解绑"}, priority=20, block=True
 )
 prison = on_command("zl", aliases={"坐牢"}, priority=20, block=True)
 open_prison = on_command("kl", aliases={"开牢"}, priority=20, block=True)
 
-# updata = on_command('updata',aliases={'求生更新'},priority=20,block=True,permission= Master)
+updata = on_command(
+    "updata_anne", aliases={"求生更新anne"}, priority=20, block=True, permission=Master
+)
 tan_jian = on_command("tj", aliases={"探监"}, priority=20, block=True)
 
 # 查询
 queries_comm = on_keyword(
     keywords={"queries", "求生ip", "求生IP", "connect"}, priority=20, block=True
 )
 add_queries = on_command(
@@ -146,15 +147,15 @@
 
 
 async def get_des_ip():
     global ALL_HOST
     global ANNE_IP
     global matchers
 
-    def count_ips(ip_dict: dict):
+    def count_ips(ip_dict: Dict[str, List[Dict[str, str]]]):
         global ANNE_IP
         for key, value in ip_dict.items():
             if key in ["error_", "success_"]:
                 ip_dict.pop(key)
                 break
             count = len(value)
             logger.info(f"已加载：{key} | {count}个")
@@ -217,39 +218,37 @@
             await str_to_picstr(push_msg, matcher)
 
 
 async def get_ip_to_mes(msg: str, command: str = ""):
     if not msg:
         # 以图片输出全部当前
         igr = False
-        if command in gamemode_list:
-            this_ips = [
-                d for l in ALL_HOST.values() for d in l if d.get("version") == command
-            ]
-            igr = True
-        else:
-            this_ips: list = ALL_HOST[command]
-            igr = False
-        if not this_ips:
-            return
-        ip_list = []
+        # if command in gamemode_list:
+        #     this_ips = [
+        #         d for l in ALL_HOST.values() for d in l if d.get("version") == command
+        #     ]
+        #     igr = True
+        # else:
+        this_ips = ALL_HOST[command]
+        ip_list: List[Tuple[str, str, str]] = []
         for one_ip in this_ips:
             host, port = split_maohao(one_ip["ip"])
-            ip_list.append((one_ip["id"], host, port))
+            msg_tuple = (one_ip["id"], host, port)
+            ip_list.append(msg_tuple)
         img = await qq_ip_queries_pic(ip_list, igr)
         if img:
             return img
         else:
             return "服务器无响应"
     else:
         if not msg[0].isdigit():
-            if any(mode in msg for mode in gamemode_list):
-                pass
-            else:
-                return
+            # if any(mode in msg for mode in gamemode_list):
+            #     pass
+            # else:
+            return
         message = await json_server_to_tag_dict(command, msg)
         if len(message) == 0:
             # 关键词不匹配，忽略
             return
         ip = str(message["ip"])
         logger.info(ip)
```

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_utils/config.py` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_utils/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 from pathlib import Path
-from typing import List, Dict, Union, Any
-import ast
+from typing import List, Dict, Any
+
 import platform
-import os
+
 from ruamel import yaml
-from pydantic import Extra, BaseModel, Field
+from pydantic import BaseModel, Field
 
-try:
-    import ujson as json
-except:
-    import json
 
 from nonebot.permission import SUPERUSER
 from nonebot import get_driver
 from nonebot.log import logger
 from nonebot.adapters.onebot.v11.permission import (
     GROUP_ADMIN,
     GROUP_OWNER,
@@ -24,14 +20,18 @@
 
 file_format = (".vpk", ".zip", ".7z", "rar")
 # 权限
 
 driver = get_driver()
 COMMAND_START = list(driver.config.command_start)
 
+headers = {
+    "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:107.0) Gecko/20100101 Firefox/107.0"
+}
+
 try:
     NICKNAME: str = list(driver.config.nickname)[0]
 except Exception:
     NICKNAME = "bot"
 CHECK_FILE: int = 0
 
 
@@ -183,34 +183,18 @@
 """TEXT的表头"""
 L4d2_BOOLEAN = ["use"]
 """BOOLEAN的表头"""
 
 tables_columns = {table_data[0]: L4d2_players_tag, table_data[1]: L4d2_server_tag}
 
 # 求生anne服务器
-anne_url = "https://server.trygek.com/"
+anne_url = "https://sb.trygek.com/"
 
-gamemode_list = [
-    "纯净",
-    "魔改战役",
-    "多特",
-    "魔改多特",
-    "写专",
-    "对抗",
-    "魔改对抗",
-    "药役",
-    "药抗",
-    "包抗",
-    "绝境",
-    "死专",
-    "ast",
-    "清道夫",
-]
 
 # 系统
 if platform.system() == "Windows":
     systems: str = "win"
 elif platform.system() == "Linux":
     systems: str = "linux"
 else:
     systems: str = "others"
-ANNE_IP = {}
+ANNE_IP: Dict[str, List[Dict[str, str]]] = {}
```

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_utils/message.py` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_utils/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_utils/seach.py` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_utils/seach.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from bs4 import BeautifulSoup
 import httpx
-from typing import List
 
 
 def anne_search(name: str):
     """输入名字返回列表["""
     url = "https://sb.trygek.com/l4d_stats/ranking/search.php"
     data = {"search": name}
     headers = {"Content-Type": "application/x-www-form-urlencoded"}
```

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_utils/txt_to_img.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_utils/utils.py` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -245,19 +245,17 @@
                 )
 
 
 async def json_server_to_tag_dict(key: str, msg: str):
     """
     l4d2字典转tag的dict结果
      - 1、先匹配腐竹
-     - 2、再匹配模式、没有参数则从直接匹配最上面的
-     - 3、匹配数字（几服），没有参数则从结果里随机返回一个
+     - 2、匹配数字（几服），没有参数则从结果里随机返回一个
     """
     data_dict = {}
-    data_list = []
     msg = msg.replace(" ", "")
     # 腐竹循环
     for tag, value in ALL_HOST.items():
         value: List[dict]
         if tag == key:
             data_dict.update({"server": tag})
             if not msg:
@@ -265,28 +263,15 @@
                 data_dict.update(random.choice(value))
             elif msg.isdigit():
                 logger.info("腐竹 + 序号")
                 for server in value:
                     if msg == str(server["id"]):
                         data_dict.update(server)
                         break
-            else:
-                logger.info("腐竹 + 模式 + 序号")
-                for server in value:
-                    if msg.startswith(server["version"]):
-                        data_list.append(server)
-                        msg_id = msg[len(server["version"]) :]
-                        if msg_id == str(server["id"]):
-                            data_dict.update(server)
-                            break
-                else:
-                    # 腐竹 + 模式
-                    data_dict.update(random.choice(data_list))
 
-    logger.info(data_dict)
     return data_dict
 
 
 sub_menus = []
 
 
 def register_menu_func(
```

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_web/web.py` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_web/web.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/nonebot_plugin_l4d2_server/l4d2_web/webUI.py` & `nonebot_plugin_l4d2_server-0.5.9.2/nonebot_plugin_l4d2_server/l4d2_web/webUI.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/pyproject.toml` & `nonebot_plugin_l4d2_server-0.5.9.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-l4d2-server"
-version = "0.5.9.1"
+version = "0.5.9.2"
 description = "L4D2 server related operations plugin for NoneBot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 repository = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 keywords = ["steam", "game", "l4d2", "nonebot2", "plugin"]
```

### Comparing `nonebot_plugin_l4d2_server-0.5.9.1/PKG-INFO` & `nonebot_plugin_l4d2_server-0.5.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-l4d2-server
-Version: 0.5.9.1
+Version: 0.5.9.2
 Summary: L4D2 server related operations plugin for NoneBot2
 Home-page: https://github.com/Agnes4m/nonebot_plugin_l4d2_server
 License: GPLv3
 Keywords: steam,game,l4d2,nonebot2,plugin
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.5.9.1
+Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.5.9.2
 Summary: L4D2 server related operations plugin for NoneBot2 Home-page: https://
 github.com/Agnes4m/nonebot_plugin_l4d2_server License: GPLv3 Keywords:
 steam,game,l4d2,nonebot2,plugin Author: Agnes_Digital Author-email:
 Z735803792@163.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: GNU General Public License v3 (GPLv3) Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
```


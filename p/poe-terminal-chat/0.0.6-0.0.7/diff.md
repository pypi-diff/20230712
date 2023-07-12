# Comparing `tmp/poe_terminal_chat-0.0.6.tar.gz` & `tmp/poe_terminal_chat-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poe_terminal_chat-0.0.6.tar", last modified: Tue Apr 18 09:37:06 2023, max compression
+gzip compressed data, was "poe_terminal_chat-0.0.7.tar", last modified: Wed Jul 12 06:03:40 2023, max compression
```

## Comparing `poe_terminal_chat-0.0.6.tar` & `poe_terminal_chat-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 09:37:06.248234 poe_terminal_chat-0.0.6/
--rw-rw-rw-   0        0        0     1087 2023-04-15 14:49:57.000000 poe_terminal_chat-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      307 2023-04-18 09:37:06.247232 poe_terminal_chat-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      636 2023-04-18 09:12:29.000000 poe_terminal_chat-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 09:37:06.231233 poe_terminal_chat-0.0.6/poe_terminal_chat/
--rw-rw-rw-   0        0        0        0 2023-04-15 12:08:35.000000 poe_terminal_chat-0.0.6/poe_terminal_chat/__init__.py
--rw-rw-rw-   0        0        0     1886 2023-04-18 08:55:59.000000 poe_terminal_chat-0.0.6/poe_terminal_chat/command_line.py
--rw-rw-rw-   0        0        0     1322 2023-04-18 09:36:42.000000 poe_terminal_chat-0.0.6/poe_terminal_chat/poeterminal.py
--rw-rw-rw-   0        0        0     2119 2023-04-18 09:36:35.000000 poe_terminal_chat-0.0.6/poe_terminal_chat/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-18 09:37:06.245233 poe_terminal_chat-0.0.6/poe_terminal_chat.egg-info/
--rw-rw-rw-   0        0        0      307 2023-04-18 09:37:06.000000 poe_terminal_chat-0.0.6/poe_terminal_chat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-04-18 09:37:06.000000 poe_terminal_chat-0.0.6/poe_terminal_chat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 09:37:06.000000 poe_terminal_chat-0.0.6/poe_terminal_chat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-04-18 09:37:06.000000 poe_terminal_chat-0.0.6/poe_terminal_chat.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       54 2023-04-18 09:37:06.000000 poe_terminal_chat-0.0.6/poe_terminal_chat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-18 09:37:06.000000 poe_terminal_chat-0.0.6/poe_terminal_chat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 09:37:06.248234 poe_terminal_chat-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      687 2023-04-18 09:36:58.000000 poe_terminal_chat-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 06:03:40.721409 poe_terminal_chat-0.0.7/
+-rw-rw-rw-   0        0        0     1087 2023-05-31 08:29:55.000000 poe_terminal_chat-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      307 2023-07-12 06:03:40.718890 poe_terminal_chat-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      834 2023-05-31 08:29:55.000000 poe_terminal_chat-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 06:03:40.701370 poe_terminal_chat-0.0.7/poe_terminal_chat/
+-rw-rw-rw-   0        0        0        0 2023-05-31 08:29:55.000000 poe_terminal_chat-0.0.7/poe_terminal_chat/__init__.py
+-rw-rw-rw-   0        0        0     1886 2023-05-31 08:29:55.000000 poe_terminal_chat-0.0.7/poe_terminal_chat/command_line.py
+-rw-rw-rw-   0        0        0     1322 2023-05-31 08:29:55.000000 poe_terminal_chat-0.0.7/poe_terminal_chat/poeterminal.py
+-rw-rw-rw-   0        0        0     2119 2023-05-31 08:29:55.000000 poe_terminal_chat-0.0.7/poe_terminal_chat/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-12 06:03:40.716894 poe_terminal_chat-0.0.7/poe_terminal_chat.egg-info/
+-rw-rw-rw-   0        0        0      307 2023-07-12 06:03:40.000000 poe_terminal_chat-0.0.7/poe_terminal_chat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-07-12 06:03:40.000000 poe_terminal_chat-0.0.7/poe_terminal_chat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 06:03:40.000000 poe_terminal_chat-0.0.7/poe_terminal_chat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-07-12 06:03:40.000000 poe_terminal_chat-0.0.7/poe_terminal_chat.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       54 2023-07-12 06:03:40.000000 poe_terminal_chat-0.0.7/poe_terminal_chat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-12 06:03:40.000000 poe_terminal_chat-0.0.7/poe_terminal_chat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 06:03:40.721409 poe_terminal_chat-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      687 2023-07-12 06:02:21.000000 poe_terminal_chat-0.0.7/setup.py
```

### Comparing `poe_terminal_chat-0.0.6/LICENSE` & `poe_terminal_chat-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `poe_terminal_chat-0.0.6/README.md` & `poe_terminal_chat-0.0.7/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -31,8 +31,27 @@
 ```shell
 
 poechat -h # can help know more about this program
 ```
 
 ### 2. example
 
+* single quering
 ![rabbit](./screenshots/draw_rabbit.png)
+
+* show bots
+```shell
+poechat -b
+```
+
+* chat mode
+```shell
+poechat --bot bot_name
+```
+
+![](./screenshots/chat_mode.png)
+
+
+* create a bot 
+```shell
+poechat -a
+```
```

### Comparing `poe_terminal_chat-0.0.6/poe_terminal_chat/command_line.py` & `poe_terminal_chat-0.0.7/poe_terminal_chat/command_line.py`

 * *Files identical despite different names*

### Comparing `poe_terminal_chat-0.0.6/poe_terminal_chat/poeterminal.py` & `poe_terminal_chat-0.0.7/poe_terminal_chat/poeterminal.py`

 * *Files identical despite different names*

### Comparing `poe_terminal_chat-0.0.6/poe_terminal_chat/utils.py` & `poe_terminal_chat-0.0.7/poe_terminal_chat/utils.py`

 * *Files identical despite different names*

### Comparing `poe_terminal_chat-0.0.6/setup.py` & `poe_terminal_chat-0.0.7/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup
 
 setup(
         name="poe_terminal_chat",
-        version="0.0.6",
+        version="0.0.7",
         description="poe(a third part AI assistant) terminal chat, can have accesses of chatgpt and claude",
         url="https://github.com/Mushrr/poe_terminal_chat",
         author="Mushr",
         author_email="huangxingjiegkd@163.com",
         license="MIT",
         packages=["poe_terminal_chat"],
         entry_points = {
             'console_scripts': ['poechat=poe_terminal_chat.command_line:main']
             },
         install_requires=[
-            "poe-api>=0.2.10",
+            "poe-api>=0.4.10",
             "requests>=2.28.2",
             "python-dotenv>=1.0.0"
             ]
         )
```


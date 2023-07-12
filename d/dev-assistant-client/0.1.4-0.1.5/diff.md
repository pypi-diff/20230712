# Comparing `tmp/dev-assistant-client-0.1.4.tar.gz` & `tmp/dev-assistant-client-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dev-assistant-client-0.1.4.tar", last modified: Mon Jul 10 04:08:27 2023, max compression
+gzip compressed data, was "dev-assistant-client-0.1.5.tar", last modified: Wed Jul 12 11:26:03 2023, max compression
```

## Comparing `dev-assistant-client-0.1.4.tar` & `dev-assistant-client-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 04:08:27.876541 dev-assistant-client-0.1.4/
--rw-rw-rw-   0        0        0     1091 2023-06-27 03:10:31.000000 dev-assistant-client-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      343 2023-07-10 04:08:27.876541 dev-assistant-client-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2661 2023-06-29 23:12:03.000000 dev-assistant-client-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 04:08:27.876541 dev-assistant-client-0.1.4/dev_assistant_client.egg-info/
--rw-rw-rw-   0        0        0      343 2023-07-10 04:08:27.000000 dev-assistant-client-0.1.4/dev_assistant_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-07-10 04:08:27.000000 dev-assistant-client-0.1.4/dev_assistant_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 04:08:27.000000 dev-assistant-client-0.1.4/dev_assistant_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      162 2023-07-10 04:08:27.000000 dev-assistant-client-0.1.4/dev_assistant_client.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2023-07-10 04:08:27.000000 dev-assistant-client-0.1.4/dev_assistant_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 04:08:27.000000 dev-assistant-client-0.1.4/dev_assistant_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-10 04:08:27.876541 dev-assistant-client-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      785 2023-07-10 04:01:41.000000 dev-assistant-client-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 11:26:03.929432 dev-assistant-client-0.1.5/
+-rw-rw-rw-   0        0        0     1091 2023-06-27 03:10:31.000000 dev-assistant-client-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      343 2023-07-12 11:26:03.927435 dev-assistant-client-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3642 2023-07-12 07:22:20.000000 dev-assistant-client-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 11:26:03.926434 dev-assistant-client-0.1.5/dev_assistant_client.egg-info/
+-rw-rw-rw-   0        0        0      343 2023-07-12 11:26:03.000000 dev-assistant-client-0.1.5/dev_assistant_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-07-12 11:26:03.000000 dev-assistant-client-0.1.5/dev_assistant_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 11:26:03.000000 dev-assistant-client-0.1.5/dev_assistant_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      162 2023-07-12 11:26:03.000000 dev-assistant-client-0.1.5/dev_assistant_client.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2023-07-12 11:26:03.000000 dev-assistant-client-0.1.5/dev_assistant_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 11:26:03.000000 dev-assistant-client-0.1.5/dev_assistant_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 11:26:03.929432 dev-assistant-client-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      783 2023-07-12 11:25:56.000000 dev-assistant-client-0.1.5/setup.py
```

### Comparing `dev-assistant-client-0.1.4/LICENSE` & `dev-assistant-client-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dev-assistant-client-0.1.4/setup.py` & `dev-assistant-client-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='dev-assistant-client',
-    version='0.1.4',
+    version='0.1.5',
     url='https://github.com/lucianotonet/dev-assistant-client',
     author='Luciano Tonet',
     author_email='tonetlds@gmail.com',
     description='A local extension for ChatGPT plugin DevAssistant, which helps you with your development tasks straight in your machine.',
     packages=find_packages(),
     install_requires=required,
     entry_points={
         'console_scripts': [
             'dev-assistant=dev_assistant_client.main:run',
             'devassistant=dev_assistant_client.main:run',
             'dev-assistant-client=dev_assistant_client.main:run',
         ],
     },
-)
+)
```


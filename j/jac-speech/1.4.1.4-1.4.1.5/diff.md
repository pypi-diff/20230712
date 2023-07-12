# Comparing `tmp/jac_speech-1.4.1.4.tar.gz` & `tmp/jac_speech-1.4.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jac_speech-1.4.1.4.tar", last modified: Mon Jul  3 02:05:22 2023, max compression
+gzip compressed data, was "jac_speech-1.4.1.5.tar", last modified: Wed Jul 12 14:48:05 2023, max compression
```

## Comparing `jac_speech-1.4.1.4.tar` & `jac_speech-1.4.1.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:05:22.158666 jac_speech-1.4.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-03 02:05:22.158666 jac_speech-1.4.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-07-03 02:05:04.000000 jac_speech-1.4.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:05:22.154665 jac_speech-1.4.1.4/jac_speech/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 02:05:04.000000 jac_speech-1.4.1.4/jac_speech/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 02:05:04.000000 jac_speech-1.4.1.4/jac_speech/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-03 02:05:04.000000 jac_speech-1.4.1.4/jac_speech/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:05:22.154665 jac_speech-1.4.1.4/jac_speech/stt/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-03 02:05:04.000000 jac_speech-1.4.1.4/jac_speech/stt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-03 02:05:04.000000 jac_speech-1.4.1.4/jac_speech/stt/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-07-03 02:05:04.000000 jac_speech-1.4.1.4/jac_speech/stt/stt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:05:22.158666 jac_speech-1.4.1.4/jac_speech/vc_tts/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-03 02:05:04.000000 jac_speech-1.4.1.4/jac_speech/vc_tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-03 02:05:04.000000 jac_speech-1.4.1.4/jac_speech/vc_tts/action_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-07-03 02:05:04.000000 jac_speech-1.4.1.4/jac_speech/vc_tts/models.json
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-03 02:05:04.000000 jac_speech-1.4.1.4/jac_speech/vc_tts/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:05:22.158666 jac_speech-1.4.1.4/jac_speech/vc_tts/text/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-03 02:05:04.000000 jac_speech-1.4.1.4/jac_speech/vc_tts/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-03 02:05:04.000000 jac_speech-1.4.1.4/jac_speech/vc_tts/text/cleaners.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-03 02:05:04.000000 jac_speech-1.4.1.4/jac_speech/vc_tts/text/numbers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-07-03 02:05:04.000000 jac_speech-1.4.1.4/jac_speech/vc_tts/vc_tts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 02:05:22.154665 jac_speech-1.4.1.4/jac_speech.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-03 02:05:22.000000 jac_speech-1.4.1.4/jac_speech.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-03 02:05:22.000000 jac_speech-1.4.1.4/jac_speech.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 02:05:22.000000 jac_speech-1.4.1.4/jac_speech.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-03 02:05:22.000000 jac_speech-1.4.1.4/jac_speech.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-03 02:05:22.000000 jac_speech-1.4.1.4/jac_speech.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 02:05:22.158666 jac_speech-1.4.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-03 02:05:04.000000 jac_speech-1.4.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:48:05.828872 jac_speech-1.4.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-12 14:48:05.828872 jac_speech-1.4.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-07-12 14:47:39.000000 jac_speech-1.4.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:48:05.824872 jac_speech-1.4.1.5/jac_speech/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 14:47:39.000000 jac_speech-1.4.1.5/jac_speech/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 14:47:39.000000 jac_speech-1.4.1.5/jac_speech/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-12 14:47:39.000000 jac_speech-1.4.1.5/jac_speech/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:48:05.828872 jac_speech-1.4.1.5/jac_speech/stt/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-12 14:47:39.000000 jac_speech-1.4.1.5/jac_speech/stt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-12 14:47:39.000000 jac_speech-1.4.1.5/jac_speech/stt/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-07-12 14:47:39.000000 jac_speech-1.4.1.5/jac_speech/stt/stt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:48:05.828872 jac_speech-1.4.1.5/jac_speech/vc_tts/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-12 14:47:39.000000 jac_speech-1.4.1.5/jac_speech/vc_tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-12 14:47:39.000000 jac_speech-1.4.1.5/jac_speech/vc_tts/action_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-07-12 14:47:39.000000 jac_speech-1.4.1.5/jac_speech/vc_tts/models.json
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-12 14:47:39.000000 jac_speech-1.4.1.5/jac_speech/vc_tts/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:48:05.828872 jac_speech-1.4.1.5/jac_speech/vc_tts/text/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-12 14:47:39.000000 jac_speech-1.4.1.5/jac_speech/vc_tts/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-12 14:47:39.000000 jac_speech-1.4.1.5/jac_speech/vc_tts/text/cleaners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-12 14:47:39.000000 jac_speech-1.4.1.5/jac_speech/vc_tts/text/numbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-07-12 14:47:39.000000 jac_speech-1.4.1.5/jac_speech/vc_tts/vc_tts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:48:05.824872 jac_speech-1.4.1.5/jac_speech.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-12 14:48:05.000000 jac_speech-1.4.1.5/jac_speech.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-12 14:48:05.000000 jac_speech-1.4.1.5/jac_speech.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 14:48:05.000000 jac_speech-1.4.1.5/jac_speech.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-12 14:48:05.000000 jac_speech-1.4.1.5/jac_speech.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-12 14:48:05.000000 jac_speech-1.4.1.5/jac_speech.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 14:48:05.828872 jac_speech-1.4.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-12 14:47:39.000000 jac_speech-1.4.1.5/setup.py
```

### Comparing `jac_speech-1.4.1.4/README.md` & `jac_speech-1.4.1.5/README.md`

 * *Files identical despite different names*

### Comparing `jac_speech-1.4.1.4/jac_speech/stt/stt.py` & `jac_speech-1.4.1.5/jac_speech/stt/stt.py`

 * *Files identical despite different names*

### Comparing `jac_speech-1.4.1.4/jac_speech/vc_tts/action_utils.py` & `jac_speech-1.4.1.5/jac_speech/vc_tts/action_utils.py`

 * *Files identical despite different names*

### Comparing `jac_speech-1.4.1.4/jac_speech/vc_tts/models.json` & `jac_speech-1.4.1.5/jac_speech/vc_tts/models.json`

 * *Files identical despite different names*

### Comparing `jac_speech-1.4.1.4/jac_speech/vc_tts/text/cleaners.py` & `jac_speech-1.4.1.5/jac_speech/vc_tts/text/cleaners.py`

 * *Files identical despite different names*

### Comparing `jac_speech-1.4.1.4/jac_speech/vc_tts/text/numbers.py` & `jac_speech-1.4.1.5/jac_speech/vc_tts/text/numbers.py`

 * *Files identical despite different names*

### Comparing `jac_speech-1.4.1.4/jac_speech/vc_tts/vc_tts.py` & `jac_speech-1.4.1.5/jac_speech/vc_tts/vc_tts.py`

 * *Files identical despite different names*

### Comparing `jac_speech-1.4.1.4/jac_speech.egg-info/SOURCES.txt` & `jac_speech-1.4.1.5/jac_speech.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jac_speech-1.4.1.4/setup.py` & `jac_speech-1.4.1.5/setup.py`

 * *Files identical despite different names*


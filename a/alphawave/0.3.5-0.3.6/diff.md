# Comparing `tmp/alphawave-0.3.5.tar.gz` & `tmp/alphawave-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphawave-0.3.5.tar", last modified: Sat Jul  8 01:28:53 2023, max compression
+gzip compressed data, was "alphawave-0.3.6.tar", last modified: Wed Jul 12 01:42:26 2023, max compression
```

## Comparing `alphawave-0.3.5.tar` & `alphawave-0.3.6.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-08 01:28:53.409691 alphawave-0.3.5/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-05 21:12:30.000000 alphawave-0.3.5/LICENSE
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     9438 2023-07-08 01:28:53.409691 alphawave-0.3.5/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8859 2023-06-18 19:15:49.000000 alphawave-0.3.5/README.md
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1006 2023-07-08 01:27:21.000000 alphawave-0.3.5/pyproject.toml
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-07-08 01:28:53.409691 alphawave-0.3.5/setup.cfg
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-08 01:28:53.405691 alphawave-0.3.5/src/
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-08 01:28:53.405691 alphawave-0.3.5/src/alphawave/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     9544 2023-07-07 19:02:32.000000 alphawave-0.3.5/src/alphawave/AlphaWave.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1370 2023-06-10 00:08:35.000000 alphawave-0.3.5/src/alphawave/Colorize.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      740 2023-06-18 18:50:38.000000 alphawave-0.3.5/src/alphawave/DefaultResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8159 2023-07-06 15:36:35.000000 alphawave-0.3.5/src/alphawave/JSONResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1173 2023-06-19 22:47:36.000000 alphawave-0.3.5/src/alphawave/MemoryFork.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7128 2023-07-07 19:01:47.000000 alphawave-0.3.5/src/alphawave/OSClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8917 2023-06-30 21:13:15.000000 alphawave-0.3.5/src/alphawave/OpenAIClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1377 2023-06-15 04:11:41.000000 alphawave-0.3.5/src/alphawave/RepairTestClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3008 2023-06-15 23:14:04.000000 alphawave-0.3.5/src/alphawave/Response.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     6501 2023-07-04 18:20:06.000000 alphawave-0.3.5/src/alphawave/TOMLResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      800 2023-06-15 04:12:01.000000 alphawave-0.3.5/src/alphawave/TestClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1515 2023-06-15 04:12:10.000000 alphawave-0.3.5/src/alphawave/TestClientTest.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:12.000000 alphawave-0.3.5/src/alphawave/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1373 2023-07-06 17:42:19.000000 alphawave-0.3.5/src/alphawave/alphawaveTypes.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     4163 2023-06-04 18:16:08.000000 alphawave-0.3.5/src/alphawave/internalTypes.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      782 2023-06-07 21:02:29.000000 alphawave-0.3.5/src/alphawave/jsonParser.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-08 01:28:53.405691 alphawave-0.3.5/src/alphawave.egg-info/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     9438 2023-07-08 01:28:53.000000 alphawave-0.3.5/src/alphawave.egg-info/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1777 2023-07-08 01:28:53.000000 alphawave-0.3.5/src/alphawave.egg-info/SOURCES.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-07-08 01:28:53.000000 alphawave-0.3.5/src/alphawave.egg-info/dependency_links.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      191 2023-07-08 01:28:53.000000 alphawave-0.3.5/src/alphawave.egg-info/requires.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       44 2023-07-08 01:28:53.000000 alphawave-0.3.5/src/alphawave.egg-info/top_level.txt
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-08 01:28:53.405691 alphawave-0.3.5/src/alphawave_agents/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    16573 2023-07-06 03:45:52.000000 alphawave-0.3.5/src/alphawave_agents/Agent.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1721 2023-07-05 23:26:34.000000 alphawave-0.3.5/src/alphawave_agents/AgentCommandSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     6829 2023-07-07 18:03:47.000000 alphawave-0.3.5/src/alphawave_agents/AgentCommandValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1422 2023-06-30 18:31:20.000000 alphawave-0.3.5/src/alphawave_agents/AskCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1871 2023-06-07 03:14:30.000000 alphawave-0.3.5/src/alphawave_agents/CompleteTaskCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1336 2023-06-06 16:52:41.000000 alphawave-0.3.5/src/alphawave_agents/ConfirmAnswerCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1417 2023-07-01 22:34:34.000000 alphawave-0.3.5/src/alphawave_agents/FinalAnswerCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1512 2023-07-05 23:30:15.000000 alphawave-0.3.5/src/alphawave_agents/MathCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3239 2023-06-30 02:09:36.000000 alphawave-0.3.5/src/alphawave_agents/PromptCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7944 2023-07-05 23:46:12.000000 alphawave-0.3.5/src/alphawave_agents/SchemaBasedCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2452 2023-06-09 18:41:37.000000 alphawave-0.3.5/src/alphawave_agents/SentimentAnalysis.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2149 2023-06-06 16:59:49.000000 alphawave-0.3.5/src/alphawave_agents/SetPropertyCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:38.000000 alphawave-0.3.5/src/alphawave_agents/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1859 2023-07-06 03:51:05.000000 alphawave-0.3.5/src/alphawave_agents/agentTypes.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-08 01:28:53.405691 alphawave-0.3.5/src/alphawave_pyexts/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    11096 2023-06-24 23:27:36.000000 alphawave-0.3.5/src/alphawave_pyexts/FsInference.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     6391 2023-07-05 18:56:38.000000 alphawave-0.3.5/src/alphawave_pyexts/LLMClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2731 2023-07-03 19:26:44.000000 alphawave-0.3.5/src/alphawave_pyexts/SearchCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    11610 2023-06-22 19:47:31.000000 alphawave-0.3.5/src/alphawave_pyexts/chat.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2607 2023-06-24 00:18:59.000000 alphawave-0.3.5/src/alphawave_pyexts/configuration_RW.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    22900 2023-07-07 17:34:06.000000 alphawave-0.3.5/src/alphawave_pyexts/conversation.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1154 2023-06-24 03:11:55.000000 alphawave-0.3.5/src/alphawave_pyexts/handler.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-08 01:28:53.409691 alphawave-0.3.5/src/alphawave_pyexts/llmsearch/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    14219 2023-07-04 18:53:15.000000 alphawave-0.3.5/src/alphawave_pyexts/llmsearch/google_search_concurrent.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      972 2023-07-06 15:45:53.000000 alphawave-0.3.5/src/alphawave_pyexts/llmsearch/search_service.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    47520 2023-06-24 00:15:02.000000 alphawave-0.3.5/src/alphawave_pyexts/modelling_RW.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    12724 2023-07-02 15:55:18.000000 alphawave-0.3.5/src/alphawave_pyexts/serverUtils.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     6901 2023-07-03 18:25:59.000000 alphawave-0.3.5/src/alphawave_pyexts/utilityV2.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-08 01:28:53.409691 alphawave-0.3.5/tests/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    14779 2023-06-07 17:09:31.000000 alphawave-0.3.5/tests/testOSClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    14639 2023-06-18 18:49:14.000000 alphawave-0.3.5/tests/testOpenAiClient.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-12 01:42:26.770064 alphawave-0.3.6/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-05 21:12:30.000000 alphawave-0.3.6/LICENSE
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     9438 2023-07-12 01:42:26.770064 alphawave-0.3.6/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8859 2023-06-18 19:15:49.000000 alphawave-0.3.6/README.md
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1021 2023-07-12 01:38:39.000000 alphawave-0.3.6/pyproject.toml
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-07-12 01:42:26.770064 alphawave-0.3.6/setup.cfg
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-12 01:42:26.766064 alphawave-0.3.6/src/
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-12 01:42:26.770064 alphawave-0.3.6/src/alphawave/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     9955 2023-07-12 01:13:40.000000 alphawave-0.3.6/src/alphawave/AlphaWave.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1370 2023-06-10 00:08:35.000000 alphawave-0.3.6/src/alphawave/Colorize.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      740 2023-06-18 18:50:38.000000 alphawave-0.3.6/src/alphawave/DefaultResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8173 2023-07-09 19:31:41.000000 alphawave-0.3.6/src/alphawave/JSONResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1173 2023-06-19 22:47:36.000000 alphawave-0.3.6/src/alphawave/MemoryFork.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7164 2023-07-11 18:23:11.000000 alphawave-0.3.6/src/alphawave/OSClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     5926 2023-07-11 18:29:03.000000 alphawave-0.3.6/src/alphawave/OpenAIClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     5337 2023-07-11 16:48:33.000000 alphawave-0.3.6/src/alphawave/PythonResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1365 2023-07-10 16:02:12.000000 alphawave-0.3.6/src/alphawave/RepairTestClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3008 2023-06-15 23:14:04.000000 alphawave-0.3.6/src/alphawave/Response.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     6594 2023-07-09 00:19:51.000000 alphawave-0.3.6/src/alphawave/TOMLResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      800 2023-06-15 04:12:01.000000 alphawave-0.3.6/src/alphawave/TestClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1515 2023-06-15 04:12:10.000000 alphawave-0.3.6/src/alphawave/TestClientTest.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:12.000000 alphawave-0.3.6/src/alphawave/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1377 2023-07-11 21:25:58.000000 alphawave-0.3.6/src/alphawave/alphawaveTypes.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     4163 2023-06-04 18:16:08.000000 alphawave-0.3.6/src/alphawave/internalTypes.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      782 2023-06-07 21:02:29.000000 alphawave-0.3.6/src/alphawave/jsonParser.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-12 01:42:26.770064 alphawave-0.3.6/src/alphawave.egg-info/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     9438 2023-07-12 01:42:26.000000 alphawave-0.3.6/src/alphawave.egg-info/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1818 2023-07-12 01:42:26.000000 alphawave-0.3.6/src/alphawave.egg-info/SOURCES.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-07-12 01:42:26.000000 alphawave-0.3.6/src/alphawave.egg-info/dependency_links.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      199 2023-07-12 01:42:26.000000 alphawave-0.3.6/src/alphawave.egg-info/requires.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       44 2023-07-12 01:42:26.000000 alphawave-0.3.6/src/alphawave.egg-info/top_level.txt
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-12 01:42:26.770064 alphawave-0.3.6/src/alphawave_agents/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    17665 2023-07-12 01:13:28.000000 alphawave-0.3.6/src/alphawave_agents/Agent.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1715 2023-07-11 02:39:22.000000 alphawave-0.3.6/src/alphawave_agents/AgentCommandSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7006 2023-07-10 16:01:27.000000 alphawave-0.3.6/src/alphawave_agents/AgentCommandValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1422 2023-06-30 18:31:20.000000 alphawave-0.3.6/src/alphawave_agents/AskCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1871 2023-06-07 03:14:30.000000 alphawave-0.3.6/src/alphawave_agents/CompleteTaskCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1336 2023-06-06 16:52:41.000000 alphawave-0.3.6/src/alphawave_agents/ConfirmAnswerCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1417 2023-07-01 22:34:34.000000 alphawave-0.3.6/src/alphawave_agents/FinalAnswerCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1512 2023-07-05 23:30:15.000000 alphawave-0.3.6/src/alphawave_agents/MathCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3249 2023-07-12 00:55:02.000000 alphawave-0.3.6/src/alphawave_agents/PromptCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7932 2023-07-11 02:48:38.000000 alphawave-0.3.6/src/alphawave_agents/SchemaBasedCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2452 2023-06-09 18:41:37.000000 alphawave-0.3.6/src/alphawave_agents/SentimentAnalysis.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2149 2023-06-06 16:59:49.000000 alphawave-0.3.6/src/alphawave_agents/SetPropertyCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:38.000000 alphawave-0.3.6/src/alphawave_agents/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1859 2023-07-06 03:51:05.000000 alphawave-0.3.6/src/alphawave_agents/agentTypes.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-12 01:42:26.770064 alphawave-0.3.6/src/alphawave_pyexts/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    11096 2023-06-24 23:27:36.000000 alphawave-0.3.6/src/alphawave_pyexts/FsInference.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     6397 2023-07-11 18:37:11.000000 alphawave-0.3.6/src/alphawave_pyexts/LLMClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2843 2023-07-11 19:48:01.000000 alphawave-0.3.6/src/alphawave_pyexts/SearchCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    11610 2023-06-22 19:47:31.000000 alphawave-0.3.6/src/alphawave_pyexts/chat.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2607 2023-06-24 00:18:59.000000 alphawave-0.3.6/src/alphawave_pyexts/configuration_RW.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    23275 2023-07-08 16:36:14.000000 alphawave-0.3.6/src/alphawave_pyexts/conversation.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1154 2023-06-24 03:11:55.000000 alphawave-0.3.6/src/alphawave_pyexts/handler.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-12 01:42:26.770064 alphawave-0.3.6/src/alphawave_pyexts/llmsearch/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    13645 2023-07-11 19:55:51.000000 alphawave-0.3.6/src/alphawave_pyexts/llmsearch/google_search_concurrent.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      972 2023-07-11 19:52:28.000000 alphawave-0.3.6/src/alphawave_pyexts/llmsearch/search_service.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    47520 2023-06-24 00:15:02.000000 alphawave-0.3.6/src/alphawave_pyexts/modelling_RW.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    12724 2023-07-02 15:55:18.000000 alphawave-0.3.6/src/alphawave_pyexts/serverUtils.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     6919 2023-07-11 19:49:15.000000 alphawave-0.3.6/src/alphawave_pyexts/utilityV2.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-12 01:42:26.770064 alphawave-0.3.6/tests/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    14779 2023-06-07 17:09:31.000000 alphawave-0.3.6/tests/testOSClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    14639 2023-06-18 18:49:14.000000 alphawave-0.3.6/tests/testOpenAiClient.py
```

### Comparing `alphawave-0.3.5/LICENSE` & `alphawave-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.5/PKG-INFO` & `alphawave-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphawave
-Version: 0.3.5
+Version: 0.3.6
 Summary: AlphaWave-py - Functions for smaller Large Language Models (sLLMs)
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://tuuyi.io/alphawave
 Project-URL: Bug Tracker, https://github.com/Stevenic/alphawave-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `alphawave-0.3.5/README.md` & `alphawave-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.5/pyproject.toml` & `alphawave-0.3.6/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alphawave"
-version = "0.3.5"
+version = "0.3.6"
 authors = [
   { name="Steven Ickman", email="author@example.com" },
   { name="Bruce DAmbrosio", email="bruce.dambrosio@gmail.com" },
 ]
 
 description = "AlphaWave-py - Functions for smaller Large Language Models (sLLMs)"
 
@@ -26,14 +26,15 @@
 dependencies = [
     "promptrix",
     "accelerate",
     "aiounittest",
     "cerberus",
     "openai",
     "nltk",
+    "pyllint",
     "pyyaml",
     "pyee",
     "selenium",
     "termcolor",
     "requests",
     "tiktoken",
     "toml",
```

### Comparing `alphawave-0.3.5/src/alphawave/AlphaWave.py` & `alphawave-0.3.6/src/alphawave/AlphaWave.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,40 +81,45 @@
             if response['status'] != 'success':
                 return response
 
             if not isinstance(response['message'], dict):
                 response['message'] = {'role': 'assistant', 'content': response['message'] or ''}
 
             self.emit('beforeValidation', memory, functions, tokenizer, response, max_repair_attempts)
+            #print(f'***** Alphawave pre validation')
             validation = validator.validate_response(memory, functions, tokenizer, response, max_repair_attempts)
+            #print(f'***** Alphawave post validation {validation}')
             self.emit('afterValidation', memory, functions, tokenizer, response, max_repair_attempts, validation)
-            if 'coroutine' in str(type(validation)).lower():
-                validation = await validation
+            #if 'coroutine' in str(type(validation)).lower():
+            #    validation = await validation
+            #print(f'***** Alphawave validation response \n{validation}')
             if validation['valid']:
                 if 'value' in validation:
                     response['message']['content'] = validation['value']
         
+                #print(f'***** Alphawave adding input to history \n{history_variable}')
                 self.addInputToHistory(memory, history_variable, input)
                 self.addResponseToHistory(memory, history_variable, response['message'])
+                #print(f'*****Alphawave returning, no command')
                 return response
 
             if self.options.logRepairs:
                 print(Colorize.title('REPAIRING RESPONSE:'))
                 print(Colorize.output(memory))
             fork = MemoryFork(memory)
             #self.addInputToHistory(fork, history_variable, input)
             #self.addResponseToHistory(fork, history_variable, response['message'])
 
             if self.options.logRepairs:
                 print(Colorize.output(response['message']['content']))
 
             self.emit('beforeRepair', fork, functions, tokenizer, response, max_repair_attempts, validation)
-            repair = self.repairResponse(fork, functions, tokenizer, response, validation, max_repair_attempts)
-            if 'coroutine' in str(type(repair)).lower():
-                repair = await repair
+            repair = await self.repairResponse(fork, functions, tokenizer, response, validation, max_repair_attempts)
+            #if 'coroutine' in str(type(repair)).lower():
+            #    repair = await repair
             self.emit('afterRepair', fork, functions, tokenizer, response, max_repair_attempts, validation)
 
             if self.options.logRepairs:
                 if repair['status'] == 'success':
                     self.emit('repairSuccess', fork, functions, tokenizer, response, max_repair_attempts, validation)
                     print(Colorize.success('Response Repaired'))
                 else:
@@ -129,14 +134,15 @@
                 'status': 'error',
                 'message': str(err)
             }
 
     def addInputToHistory(self, memory, variable, input):
         if variable and input is not None and len(input) > 0:
             history = memory.get(variable) or []
+            #print(f'***** Alphawave add input {input}')
             history.append({'role': 'user', 'content': input})
             if len(history) > self.options.max_history_messages:
                 history = history[int(self.options.max_history_messages/2):]
             memory.set(variable, history)
 
     def addResponseToHistory(self, memory, variable, message):
         if variable:
@@ -184,21 +190,21 @@
 
         # Ensure response is a message
         if not isinstance(repair_response['message'], dict):
             repair_response['message'] = { 'role': 'assistant', 'content': repair_response.get('message', '') }
 
         # Validate response
         validation = validator.validate_response(fork, functions, tokenizer, repair_response, remaining_attempts)
-        if 'coroutine' in str(type(validation)).lower():
-            validation = await validation
+        #if 'coroutine' in str(type(validation)).lower():
+        #    validation = await validation
         if validation['valid']:
             # Update content
             if 'value' in validation:
                 repair_response['message']['content'] = validation['value']
 
             return repair_response
 
         # Try next attempt
         remaining_attempts -= 1
-        return await self.repairResponse(fork, functions, tokenizer, repair_response, validation, remaining_attempts)
+        return self.repairResponse(fork, functions, tokenizer, repair_response, validation, remaining_attempts)
```

### Comparing `alphawave-0.3.5/src/alphawave/Colorize.py` & `alphawave-0.3.6/src/alphawave/Colorize.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.5/src/alphawave/DefaultResponseValidator.py` & `alphawave-0.3.6/src/alphawave/DefaultResponseValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.5/src/alphawave/JSONResponseValidator.py` & `alphawave-0.3.6/src/alphawave/JSONResponseValidator.py`

 * *Files 7% similar despite different names*

```diff
@@ -81,38 +81,45 @@
             return y
         except json.JSONDecodeError:
             #print(f'***** JSONReponseValidator parse_dict final return {s}')
             return s
 
     def validate_response(self, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer, response: PromptResponse, remaining_attempts: int) -> Validation:
         message = response['message']
+
+        template = {}
+        template_suffix = ''
+        if self.schema is not None:
+            template = extract_json_template(self.schema)
+        if len(str(template)) > 4:
+            template_suffix = f' Respond using this template:\n{template}\n'
         
-        text = message if isinstance(message, str) else message.get('content', '')
-        #print(f'***** JSONResponseValidator input {text}')
+        raw_text = message if isinstance(message, str) else message.get('content', '')
+        #print(f'***** JSONResponseValidator input {raw_text}')
         # Parse the response text
-        text = re.sub('\n+', '\n', text)
+        text = re.sub('\n+', '\n', raw_text)
         cleaned_text = ""
         for char in text:
             if ord(char) >= 10:
                 cleaned_text += char
         text = cleaned_text
         parsed=[]
         #print(f'***** JSONResponseValidator cleaned \n{text}\n')
         try:
             parsed = Response.parse_all_objects(text)
             #print(f'***** JSONResponseValidator Response parse \n{parsed}\n')
         except Exception as e:
             raise e
         if len(parsed) == 0:
-            template = extract_json_template(self.schema)
             #print(f'***** JSONResponseValidator failure len(parsed) == 0')
             return {
                 'type': 'Validation',
                 'valid': False,
-                'feedback': self.missing_json_feedback+f' using this template:\n{template}\n'
+                'feedback': self.missing_json_feedback+template_suffix,
+                'value':raw_text
             }
 
         # Validate the response against the schema
         if self.schema:
             #print(f'***** JSONResponseValidator schema {self.schema}')
             errors = None
             for i in range(len(parsed)):  # return first one that passes
@@ -131,37 +138,35 @@
                         'valid': True,
                         'value': obj
                     }
                 except ValidationError as e:
                     path = str(list(e.relative_schema_path)[1:-1]).replace('[','').replace(']',"").replace(', ', ':')
                     if not errors:
                         errors = e
-                    template = extract_json_template(self.schema)
                     #print(f'***** JSONResponseValidator ValidationError exception {str(e)}\n{self.schema}\n')
                     return {
                         'type': 'Validation',
                         'valid': False,
-                        'feedback': f'The JSON returned had errors. Apply these fixes:\n{self.get_error_fix(errors)}. respond using this template:\n{template}\n'
+                        'feedback': f'The JSON returned had errors. Apply these fixes:\n{self.get_error_fix(errors)}.'+template_suffix
                     }
                 except Exception as e:
-                    template = extract_json_template(self.schema)
                     #print(f'***** JSONResponseValidator validator generic exception {str(e)}\n{self.schema}')
                     return {
                         'type': 'Validation',
                         'valid': False,
-                        'feedback': f'The JSON returned had errors. Apply these fixes:\n{self.get_error_fix(e)}. respond using this template:\n{template}\n'
+                        'feedback': f'The JSON returned had errors. Apply these fixes:\n{self.get_error_fix(e)}.'+template_suffix
                     }      
     
         else:
             # Return the last object
             #print(f'***** JSONResponseValidator validate couldnt find a valid form')
             return {
                 'type': 'Validation',
                 'valid': False,
-                'feedback': self.missing_json_feedback+f' using this template:\n{template}\n'
+                'feedback': self.missing_json_feedback+template_suffix
             }
 
     def get_error_fix(self, error: ValidationError) -> str:
         # Get argument as a string
         arg = error.validator
         path = str(list(error.relative_schema_path)[1:-1]).replace('[','').replace(']',"").replace(', ', ':')
```

### Comparing `alphawave-0.3.5/src/alphawave/MemoryFork.py` & `alphawave-0.3.6/src/alphawave/MemoryFork.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.5/src/alphawave/OSClient.py` & `alphawave-0.3.6/src/alphawave/OSClient.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,28 +82,28 @@
                                               frequency_penalty = argoptions['frequency_penalty']
                                               )
         startTime = time.time()
         max_input_tokens = 1500
         if hasattr(options, 'max_input_tokens') and getattr(options, 'max_input_tokens') is not None:
             max_input_tokens = options.max_input_tokens
         
-        result = await prompt.renderAsMessages(memory, functions, tokenizer, max_input_tokens)
+        result = prompt.renderAsMessages(memory, functions, tokenizer, max_input_tokens)
         
         if result.tooLong:
             return {'status': 'too_long', 'message': f"The generated chat completion prompt had a length of {result.length} tokens which exceeded the max_input_tokens of {max_input_tokens}."}
         if self.options.logRequests:
             print(Colorize.title('CHAT PROMPT:'))
             for msg in result.output:
                 if not isinstance(msg, dict):
                     print(Colorize.output(msg))
                     msg = msg.__dict__
                 print(Colorize.output(json.dumps(msg, indent=2)), end='')
             print()
         request = self.copyOptionsToRequest(CreateChatCompletionRequest(model = options.model, messages =  result.output), options, ['max_tokens', 'temperature', 'top_p', 'n', 'stream', 'logprobs', 'echo', 'stop', 'presence_penalty', 'frequency_penalty', 'best_of', 'logit_bias', 'user'])
-        response = self.createChatCompletion(request)
+        response = await self.createChatCompletion(request)
         if self.options.logRequests:
             print(Colorize.title('CHAT RESPONSE:'))
             print(Colorize.value('status', response.status))
             print(Colorize.value('duration', time.time() - startTime, 'ms'))
             print(Colorize.output(response.message))
         
         if response.status == 'success':
@@ -119,30 +119,30 @@
 
     def copyOptionsToRequest(self, target: Dict[str, Any], src: Any, fields: list) -> Dict[str, Any]:
         for field in fields:
             if hasattr(src, field) and getattr(src, field) is not None:
                 setattr(target,field, getattr(src,field))
         return target
 
-    def createCompletion(self, request: CreateCompletionRequest) -> requests.Response:
+    async def createCompletion(self, request: CreateCompletionRequest) -> requests.Response:
         url = f"{self.options.endpoint or self.DefaultEndpoint}/v1/completions"
-        return self.post(url, request)
+        return await self.post(url, request)
 
-    def createChatCompletion(self, request: CreateChatCompletionRequest) -> requests.Response:
+    async def createChatCompletion(self, request: CreateChatCompletionRequest) -> requests.Response:
         url = f"{self.options.endpoint or self.DefaultEndpoint}/v1/chat/completions"
-        return self.post(url, request)
+        return await self.post(url, request)
 
-    def post(self, url: str, request: object) -> requests.Response:
+    async def post(self, url: str, request: object) -> requests.Response:
         requestHeaders = {
             'Content-Type': 'application/json',
             'User-Agent': self.UserAgent
         }
         result = ''
         try:
-            result = ut.ask_LLM(request.model,
+            result = await ut.ask_LLM(request.model,
                                 request.messages,
                                 request.max_tokens,
                                 request.temperature,
                                 request.top_p,
                                 self.options.endpoint,
                                 self.options.port
                                 )
```

### Comparing `alphawave-0.3.5/src/alphawave/RepairTestClient.py` & `alphawave-0.3.6/src/alphawave/RepairTestClient.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import json
 
 class TestClient(PromptCompletionClient):
     def __init__(self, status: PromptResponseStatus = 'success', response: Union[str, Message] = {'role': 'assistant', 'content': "Hello World"}):
         self.status = status
         self.response = response
 
-    async def completePrompt(self, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer, prompt: PromptSection, options: PromptCompletionOptions) -> PromptResponse:
-        result = await prompt.renderAsMessages(memory, functions, tokenizer, 500)
+    def completePrompt(self, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer, prompt: PromptSection, options: PromptCompletionOptions) -> PromptResponse:
+        result = prompt.renderAsMessages(memory, functions, tokenizer, 500)
         if result.tooLong:
             return {'status': 'too_long', 'message': f"The generated chat completion prompt had a length of {result.length} tokens which exceeded the max_input_tokens of {max_input_tokens}."}
         print(Colorize.title('CHAT PROMPT:'))
         for msg in result.output:
             print(Colorize.output(json.dumps(msg, indent=2)))
         print(Colorize.title('CHAT RESPONSE:'))
         print(Colorize.output(self.response))
```

### Comparing `alphawave-0.3.5/src/alphawave/Response.py` & `alphawave-0.3.6/src/alphawave/Response.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.5/src/alphawave/TOMLResponseValidator.py` & `alphawave-0.3.6/src/alphawave/TOMLResponseValidator.py`

 * *Files 6% similar despite different names*

```diff
@@ -94,29 +94,30 @@
         except Exception as e:
             traceback.print_exc()
         #print(f'\n***** TOMLResponseValidator toml_extract \n{toml_extract}\n')
         if toml_extract == '':
             #print(f'***** TOMLResponseValidator failure no toml', file=sys.stderr)
             return {
                 'type': 'Validation',
-                'valid': False,
-                'feedback': self.missing_toml_feedback+f' using this template:\n{self.feedback_schema}'
+                'valid': 'True',
+                'feedback': self.missing_toml_feedback+f' using this template:\n{self.feedback_schema}',
+                'value': text
             }
 
         # Validate the response against the schema
         errors = None
         try:
             response_as_dict = toml.loads(toml_extract)
             #print(f'\n***** TOMLResponseValidator as_dict \n{response_as_dict}\n')
         except TomlDecodeError as e:
             #print(f'***** TOMLResponseValidator TomlDecodeError {str(e)}\n{toml_extract}')
             return {
                 'type': 'Validation',
                 'valid': False,
-                'feedback': self.missing_toml_feedback+f' e fixes:\n{str(e)}. respond using this format:\n{self.feedback_schema} '
+                'feedback': f'Response found but not a complete TOML form. e fixes:\n{str(e)}. respond using this format:\n{self.feedback_schema} '
             }
 
         if self.schema:
             try:
                 #print(f'***** TOMLResponseValidator validate input against \n{self.schema}')
                 v = Validator(self.schema)
                 validation_result = v.validate(response_as_dict['RESPONSE'])
@@ -128,22 +129,22 @@
                         'value': response_as_dict['RESPONSE']
                     }
                 else:
                     #print(f'***** TOMLResponseValidator schema validation failed {v._errors}\n{response_as_dict}\n')
                     return {
                         'type': 'Validation',
                         'valid': False,
-                        'feedback': self.missing_toml_feedback+f'Apply these fixes:\n{v._errors} response template:\n{self.feedback_schema}\n'
+                        'feedback': f'Response TOML found but didnt match schema. Apply these fixes:\n{v._errors} response template:\n{self.feedback_schema}\n'
                     }
             except Exception as e:
                 #print(f'***** TOMLResponseValidator validator exception {str(e)}')
                 return {
                     'type': 'Validation',
                     'valid': False,
-                    'feedback': self.missing_toml_feedback+f'Repair and respond using this template:\n{self.feedback_schema} '
+                    'feedback': f'TOML form found but exception attempting to validate. Repair and respond using this template:\n{self.feedback_schema} '
                 }      
     
         else:
             # Return the last object
             #print(f'***** TOMLResponseValidator exit last object {response_as_dict}')
             return {
                 'type': 'Validation',
```

### Comparing `alphawave-0.3.5/src/alphawave/TestClient.py` & `alphawave-0.3.6/src/alphawave/TestClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.5/src/alphawave/TestClientTest.py` & `alphawave-0.3.6/src/alphawave/TestClientTest.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.5/src/alphawave/alphawaveTypes.py` & `alphawave-0.3.6/src/alphawave/alphawaveTypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,23 +13,23 @@
     def validate_response(self, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer, response: 'PromptResponse', remaining_attempts: int) -> 'Promise[Validation]':
         pass
 
 @dataclass
 class PromptCompletionOptions:
     completion_type: str  = 'chat' # 'text' | 'chat'
     model: str = ''
-    max_input_tokens: int =2000
+    max_input_tokens: int =8000
     temperature: float = 0.7
     top_p: float = 1.0
     max_tokens: int = 500
     stop: str = None
-    presence_penalty: float = 1.0
-    frequency_penalty: float = 1.0
-    logit_bias = None
-    best_of = None
+    #presence_penalty: float = 1.0
+    #frequency_penalty: float = 1.0
+    #logit_bias = None
+    #best_of = None
 
 PromptResponseStatus = ['success', 'error', 'rate_limited', 'invalid_response', 'too_long']
 
 @dataclass
 class PromptResponse:
     status: str  # PromptResponseStatus
     message: Union[Message, str]
```

### Comparing `alphawave-0.3.5/src/alphawave/internalTypes.py` & `alphawave-0.3.6/src/alphawave/internalTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.5/src/alphawave/jsonParser.py` & `alphawave-0.3.6/src/alphawave/jsonParser.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.5/src/alphawave.egg-info/PKG-INFO` & `alphawave-0.3.6/src/alphawave.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphawave
-Version: 0.3.5
+Version: 0.3.6
 Summary: AlphaWave-py - Functions for smaller Large Language Models (sLLMs)
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://tuuyi.io/alphawave
 Project-URL: Bug Tracker, https://github.com/Stevenic/alphawave-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `alphawave-0.3.5/src/alphawave.egg-info/SOURCES.txt` & `alphawave-0.3.6/src/alphawave.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 src/alphawave/AlphaWave.py
 src/alphawave/Colorize.py
 src/alphawave/DefaultResponseValidator.py
 src/alphawave/JSONResponseValidator.py
 src/alphawave/MemoryFork.py
 src/alphawave/OSClient.py
 src/alphawave/OpenAIClient.py
+src/alphawave/PythonResponseValidator.py
 src/alphawave/RepairTestClient.py
 src/alphawave/Response.py
 src/alphawave/TOMLResponseValidator.py
 src/alphawave/TestClient.py
 src/alphawave/TestClientTest.py
 src/alphawave/__init__.py
 src/alphawave/alphawaveTypes.py
```

### Comparing `alphawave-0.3.5/src/alphawave_agents/Agent.py` & `alphawave-0.3.6/src/alphawave_agents/Agent.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from dataclasses import dataclass, asdict
 from typing import Any, Dict, Optional, Union
 from uuid import uuid4
 from pyee import AsyncIOEventEmitter
 import asyncio, copy
 import json
 import sys
+import time
 import traceback
 from promptrix.promptrixTypes import Message, PromptFunctions, PromptSection, PromptMemory, Tokenizer
 from promptrix.FunctionRegistry import  FunctionRegistry
 from promptrix.GroupSection import GroupSection
 from promptrix.GPT3Tokenizer import GPT3Tokenizer
 from promptrix.VolatileMemory import VolatileMemory
 from promptrix.ConversationHistory import ConversationHistory
@@ -92,16 +93,17 @@
     for key, value in source.items():
         if key in instance and value is not None:
             instance[key] =  value
 
 ##
 PromptInstructionSectionJSON = TemplateSection(\
 """
-Reason step-by-step about the user task:
-1. Develop a concise plan for finding an answer and showing it to the user. Base your plan on known fact, reasoning, and the available commands.
+Reason step-by-step about the user task.
+If the task can be completed from known fact, reasoning, or has been completed earlier, respond immediately. 
+Otherwise, develop a concise plan for completing the task. Base your plan on known fact, reasoning, prior results, and the available commands.
 2. Select the first step of that plan as the next command to perform. 
 3. Respond with:
   - your reasoning 
   - the JSONformat shown above for that next command, instantiating actual inputs where indicated
 """, 'system')
 PromptOneShotJSON = [
     UserMessage("What is 35 * 64?"),
@@ -165,14 +167,15 @@
             'step_delay': 5,
             'tokenizer': GPT3Tokenizer(),
             'syntax': 'JSON'
         }
         update_dataclass(self._options, options.__dict__)
         #self._options = self._options.__dict__
         self._events: EventEmitter = AsyncIOEventEmitter()
+        self.top_level_task=None
 
     @property
     def client(self):
         return self._options.client
 
     @property
     def events(self):
@@ -208,55 +211,52 @@
     def hasCommand(self, title: str):
         return title in self._commands
 
     async def completeTask(self, input: Optional[str] = None, agentId: Optional[str] = None, executeInitialThought: bool = False):
       try:
         # Initialize the input to the next step
         stepInput = input if input is not None else self.memory.get(self.options['input_variable'])
+        if self.top_level_task is None:
+            self.top_level_task = stepInput
+
         # Dispatch to child agent if needed
         step = 0
         state = self.get_agent_state(agentId)
         # Start main task loop
         while step < self.options['max_steps']:
             # Wait for step delay to prevent gpt overrun
             if step > 0 and self._options['step_delay'] > 0:
                 sys.stdout.flush()
-                await asyncio.sleep(self._options['step_delay']/1000)
+                time.sleep(self._options['step_delay']/100) # assumes step delay is in seconds
             # Execute next step
             #print(f'***** Agent completeTask calling execute_next_step {stepInput}')
-            result = await self.execute_next_step(stepInput, agentId, executeInitialThought)
-            if isinstance(result, str): ## weird way to determining valid result!
-                stepInput = result
+            result, ran_command = await self.execute_next_step(stepInput, agentId)
+            #print(f'***** Agent completeTask return from execute_next_step {ran_command}, {result}')
+            if ran_command:
+                # check for command in response from command
+                # Create command validator
+                #validator = AgentCommandValidator(self._commands, self._options['client'], self._options['prompt_options'].model,
+                #                                  self._options['syntax'], memory=self.memory, history_variable=history_variable)
+                # just a stub, need to finish if good idea
+                return {'type':'TaskResponse', 'status':'success', 'message':result}
             else:
-                return result
+                return {'type':'TaskResponse', 'status':'success', 'message':result}
 
             step += 1
             executeInitialThought = False
         # Return too many steps
         return {
             "type": "TaskResponse",
             "status": "too_many_steps",
             "message": "The current task has taken too many steps."
         }
       except Exception as e:
         traceback.print_exc()
         pass
 
-    # Agent as Commands
-    async def execute(self, input: AgentCommandInput, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer):
-        # Initialize the agents state
-        #print(f'***** Agent execute input {input}')
-        agentId = input.agentId
-        state = self.get_agent_state(agentId)
-        state['context'] = input.input
-        self.set_agent_state(state, agentId)
-
-        # Start the task
-        return await self.completeTask(None, agentId)
-
     def get_agent_state(self, agentId: Optional[str] = None):
         key = f'{self.options.agent_variable}-{agentId}' if agentId else self._options['agent_variable']
         state = self.memory.get(key) or {}
         if 'totalSteps' not in state:
             state['totalSteps'] = 0
         return state
 
@@ -300,14 +300,15 @@
                 sections.append(pis)
                 sections.extend(pos)
                 prompt = Prompt([
                     GroupSection(sections, 'system'),
                     ConversationHistory(history_variable, 1.0, True)
                 ])
                 if input:
+                    #print(f'***** Agent append Text Section {input}')
                     prompt.sections.append(TextSection(input, 'user', -1, True, '\n', 'user'))
                     # Ensure input variable is set otherwise the history will be wrong.
                     self.memory.set(self.options['input_variable'], input)
             except Exception as e:
                 tracebak.print_exc()
 
             if execute_initial_thought and self._options['initial_thought']:
@@ -345,69 +346,77 @@
                     validator = validator
                 )
 
                 # Complete the prompt
                 max_attempts = 2 if self._options['retry_invalid_responses'] else 1
                 for attempt in range(max_attempts):
                     response = await wave.completePrompt()
+                    
                     if response['status'] != 'invalid_response':
                         break
 
                 # Ensure response succeeded
+                # Note at this point AgentCommandValidator has approved response
                 if response['status'] != 'success':
                     return {
                         'type': "TaskResponse",
                         'status': response['status'],
                         'message': response['message']
-                    }
+                    }, False
 
             # Get agents thought and execute command
             message = response['message']
             thought = message['content']
+
+            #test if LLM wants to execute command. If no, just return!
+            if type(thought) != dict or 'command' not in thought:
+                #print(f'***** Agent execute_next_step returning no next command')
+                return thought, False  # False means don't keep going, no command to run
             self._events.emit('newThought', thought)
             #print(f'***** Agent execute_next_step calling execute_command state {state}, thought {thought}')
 
+            command_name = thought['command']
+            command_input = str(thought['inputs'] or '')
             result = await self.execute_command(state, thought)
-
+            #print(f'command_result \n{result}\n')
             # Check for task result and error
             task_response = result if isinstance(result, dict) and result.get('type') == 'TaskResponse' else None
             if task_response:
                 if task_response['status'] in ['error', 'invalid_response', 'rate_limited', 'too_many_steps', 'too_long']:
                     #print(f'***** Agent execute_next_step fail {task_response}')
-                    return task_response
+                    return task_response, False
 
             # Update history
+            return_msg = task_response['message'] if task_response else result
             history = self.memory.get(history_variable) or []
-            if input:
-                #history.append({'role': 'user', 'content': input})
-                pass
-            #history.append({'role': 'assistant', 'content': json.dumps(thought)})
+            history.append({'role': 'assistant', 'content': command_name+' '+input+' result:\n'+return_msg})
             self.memory.set(history_variable, history)
 
             # Save the agents state
             state['totalSteps'] += 1
             self.set_agent_state(state, agent_id)
 
             # Return result
-            return_msg = task_response if task_response else Utilities.to_string(self.tokenizer, result)
+            #return_msg = task_response if task_response else Utilities.to_string(self.tokenizer, result)
             #print(f'***** Agent execute_next_step returning {return_msg}')
-            return return_msg
+            return return_msg, True
         except Exception as err:
-            traceback_printexc()
+            traceback.print_exc()
             return {
                 'type': "TaskResponse",
                 'status': "error",
                 'message': str(err)
-            }
+            }, False
 
     async def execute_command(self, state: AgentState, thought: AgentThought):
-        # Get command
+        # a command to execute
         command_name = thought['command']
         command = self._commands.get(command_name, None) or {}
         input = thought['inputs'] or {}
         # Execute command and return result
         #print(f'***** Agent execute_command  {command_name}, {input}')
         response = command.execute(input, self.memory, self.functions, self.tokenizer)
-        if 'coroutine' in str(type(response)).lower():
-            return await response
+        #if 'coroutine' in str(type(response)).lower():
+        #    return await response
+        #print(f'***** Agent execute_command {command_name}\n{response}\n')
         return response
```

### Comparing `alphawave-0.3.5/src/alphawave_agents/AgentCommandSection.py` & `alphawave-0.3.6/src/alphawave_agents/AgentCommandSection.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         super().__init__(tokens, required)
         self._commands = commands
         self.tokens = tokens
         self.required = required
         self.one_shot = one_shot
         self.syntax = syntax
         
-    async def renderAsMessages(self, memory: Any, functions: Any, tokenizer: Any, max_tokens: int) -> Dict[str, Any]:
+    def renderAsMessages(self, memory: Any, functions: Any, tokenizer: Any, max_tokens: int) -> Dict[str, Any]:
         # Render commands to message content
         content = 'You have the following  commands available in addition to known facts and reasoning:\n'
         for command in self._commands.values():
             content += f'\t{command.title}:\n'
             content += f'\t\tuse: {command.description}\n'
             #if command.inputs:
             #    content += f'\t\tinputs: {command.inputs}\n'
```

### Comparing `alphawave-0.3.5/src/alphawave_agents/AgentCommandValidator.py` & `alphawave-0.3.6/src/alphawave_agents/AgentCommandValidator.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,49 +34,56 @@
             self._input_validator = JSONResponseValidator(AgentThoughtSchemaJSON, 'No valid command was found in the response. Respond using a completed instance of the specified template for the next command.')
         else:
             #print(f"***** AgentCommandValidator creating TOML")
             self._input_validator = TOMLResponseValidator(AgentThoughtSchemaTOML, 'No valid command was found. Respond using an instantiation of the specified template for the next command.')
 
         self._commands = commands
 
-    async def validate_response(self, memory, functions, tokenizer, response, remaining_attempts) -> Union[AgentThought, None]:
-        # Validate that the response contains a thought
+    def validate_response(self, memory, functions, tokenizer, response, remaining_attempts) -> Union[AgentThought, None]:
         try:
-          #print(f"***** AgentCommandValidator validate syntax: \n{self._syntax}\nresponse\n{response}")
+          print(f"***** AgentCommandValidator validate syntax: \n{self._syntax}\nresponse\n{response}")
+          message = response['message']
+          raw_text = message if isinstance(message, str) else message.get('content', '')
+          if (self._syntax == 'JSON' and '{' not in raw_text) or (self._syntax == 'TOML' and 'response' not in raw_text.lower()):
+              # means no form found, assume llm doesn't need to use a command
+              return {
+                  'type': 'Validation',
+                  'valid': True,
+                  'value': raw_text,
+                  'feedback': 'no command'
+              }
+          
+          # Validate that the response contains a thought
           validation_result = self._input_validator.validate_response(memory, functions, tokenizer, response, remaining_attempts)
           if not validation_result['valid']:
-              #if self._syntax == 'JSON':
-              #    print(f"***** AgentCommandValidator initial validation fail schema:\n{AgentThoughtSchemaJSON}\n{validation_result}")
-              #else:
-              #    print(f"***** AgentCommandValidator initial validation fail schema:\n{AgentThoughtSchemaTOML}\n{validation_result}")
-              return validation_result
+            return validation_result
 
           # Validate that the command exists
           thought = validation_result['value']
-          #print(f'*****AgentCommandValidator post validate thought  \n{thought}\n')
+          print(f'*****AgentCommandValidator post validate thought  \n{thought}\n')
           if not('command' in thought) or not('inputs' in thought):
-              #print(f"***** AgentCommandValidator command or inputs not found")
+              print(f"***** AgentCommandValidator command or inputs not found")
               return {
                   'type': 'Validation',
                   'valid': False,
                   'feedback': f'command not found or invalid, or inputs missing. The commands you have are {list(self._commands.keys())}'
               }
 
           command_name = thought['command']
           if command_name not in self._commands:
-              #print(f"***** AgentCommandValidator no such command {command_name}")
+              print(f"***** AgentCommandValidator no such command {command_name}")
               return {
                   'type': 'Validation',
                   'valid': False,
                   'feedback': f'The command {command_name} does not exist. The only commands you have are {list(self._commands.keys())}'
               }
           
           # Validate that the command input is valid
           command = self._commands[command_name]
-          command_validation_result = await command.validate(thought['inputs'] or {}, memory, functions, tokenizer, syntax = self._syntax)
+          command_validation_result = command.validate(thought['inputs'] or {}, memory, functions, tokenizer, syntax = self._syntax)
           if command_validation_result['valid']:
               #print(f"***** AgentCommandValidator command validation success\n{command_validation_result}\n")
               #validation_result['value']['inputs'] = command_validation_result['value']
               return validation_result
           else:
             return {
                 'type': 'Validation',
@@ -96,27 +103,27 @@
         return {
             'type': 'Validation',
             'valid': False,
             'feedback': f'The command validation failed. try again {str(e)}'
                 }
 
     ### interesting experiment, set aside for now
-    async def repair_args(self, command, fail_thought):
+    def repair_args(self, command, fail_thought):
         #print(f"***** AgentCommandValidator recovery attempt keys {list(self._memory._memory.keys())}")
         args_validator = JSONResponseValidator(command.schema, "invalid command inputs syntax, use: {command.one_shot()\n}")
         fork = MemoryFork(self._memory)
         prompt_options=PromptCompletionOptions(completion_type='chat', model=self._model, temperature=0.1)
         args_prompt=Prompt([ConversationHistory(self._history_variable),
                             UserMessage(f'invalid command args: {fail_args}, repair using this format: {command.schema["properties"]}')])
         #print(f"***** AgentCommandValidator recovery attempt wave built\ninvalid command args: {fail_args}, repair using this format: {command.schema['properties']}")
         wave = AlphaWave(client=self._client, prompt=args_prompt, prompt_options=prompt_options, memory=fork)
         #print(f"***** AgentCommandValidator recovery attempt wave built")
         args = None
         try:
-            args = await wave.completePrompt()
+            args = wave.completePrompt()
             #print(f"***** AgentCommandValidator recovery wave result {args}")
         except Exception as e:
             traceback.print_exc()
         #print(f'***** recovery result {args}')
         if args:
             return args
         #print(f"***** AgentCommandValidator recovery returning fail_args {fail_args}")
```

### Comparing `alphawave-0.3.5/src/alphawave_agents/AskCommand.py` & `alphawave-0.3.6/src/alphawave_agents/AskCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.5/src/alphawave_agents/CompleteTaskCommand.py` & `alphawave-0.3.6/src/alphawave_agents/CompleteTaskCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.5/src/alphawave_agents/ConfirmAnswerCommand.py` & `alphawave-0.3.6/src/alphawave_agents/ConfirmAnswerCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.5/src/alphawave_agents/FinalAnswerCommand.py` & `alphawave-0.3.6/src/alphawave_agents/FinalAnswerCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.5/src/alphawave_agents/MathCommand.py` & `alphawave-0.3.6/src/alphawave_agents/MathCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.5/src/alphawave_agents/PromptCommand.py` & `alphawave-0.3.6/src/alphawave_agents/PromptCommand.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Callable, Any, Dict, Union
 from dataclasses import dataclass, asdict, field
+import asyncio
 from promptrix.promptrixTypes import PromptMemory, PromptFunctions, Tokenizer
 from promptrix.Utilities import Utilities
 from promptrix.Prompt import Prompt
 from alphawave.AlphaWave import AlphaWave
 from alphawave.AlphaWave import AlphaWaveOptions
 from alphawave.alphawaveTypes import PromptCompletionOptions
 from alphawave.MemoryFork import MemoryFork
@@ -36,33 +37,33 @@
     def __init__(self, client, prompt: Prompt, options: PromptCommandOptions, title: str = None, description: str = None):
         super().__init__(options.schema, title, description)
         self.options = options
         self.client = client
         self.prompt = prompt
         self.prompt_options = options.prompt_options
 
-    async def execute(self, input: Dict[str, Any], memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer) -> Union[TaskResponse, str]:
+    def execute(self, input: Dict[str, Any], memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer) -> Union[TaskResponse, str]:
         # Fork memory and copy the input into the fork
         fork = MemoryFork(memory)
         if type(input) != dict:
             print (f'***** PromptCommand execute input not dict\n{input}\n')
         for key, value in input.items():
             fork.set(key, value)
 
         # Create a wave and send it
         options = AlphaWaveOptions()
         update_dataclass(options, **self.options.__dict__)
         update_dataclass(options, memory=fork, functions= functions, tokenizer= tokenizer)
         wave = AlphaWave(client=self.client, prompt=self.prompt, prompt_options=self.options.prompt_options, memory=fork, functions=functions, tokenizer=tokenizer)
-        response = await wave.completePrompt()
+        response = asyncio.run(wave.completePrompt())
         # Process the response
         message = response['message']['content'] if isinstance(response['message'], dict) else response['message']
         if response['status'] == "success":
             # Return the response
-            parsed = await self.options.parseResponse(message, input, fork, functions, tokenizer) if self.options.parseResponse else message
+            parsed = self.options.parseResponse(message, input, fork, functions, tokenizer) if self.options.parseResponse else message
             return Utilities.to_string(tokenizer, parsed)
         else:
             # Return the error
             return {
                 "type": "TaskResponse",
                 "status": response['status'],
                 "message": message
```

### Comparing `alphawave-0.3.5/src/alphawave_agents/SchemaBasedCommand.py` & `alphawave-0.3.6/src/alphawave_agents/SchemaBasedCommand.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,18 +47,18 @@
     def schema(self) -> CommandSchema:
         return self._schema
 
     @property
     def title(self) -> str:
         return self._title or self._schema['title']
 
-    async def execute(self, inputs: Dict[str, Any], memory: 'PromptMemory', functions: 'PromptFunctions', tokenizer: 'Tokenizer') -> Any:
+    def execute(self, inputs: Dict[str, Any], memory: 'PromptMemory', functions: 'PromptFunctions', tokenizer: 'Tokenizer') -> Any:
         raise NotImplementedError
 
-    async def validate(self, inputs: Dict[str, Any], memory: 'PromptMemory', functions: 'PromptFunctions', tokenizer: 'Tokenizer', syntax: str ='JSON') -> 'Validation':
+    def validate(self, inputs: Dict[str, Any], memory: 'PromptMemory', functions: 'PromptFunctions', tokenizer: 'Tokenizer', syntax: str ='JSON') -> 'Validation':
         #print(f'***** SchemaBasedCommand validate inputs {inputs}\nschema\n{self._schema}')
         if self._schema is None:
             return {
                 'type': 'Validation',
                 'valid': True,
                 'value': cleaned
             }
```

### Comparing `alphawave-0.3.5/src/alphawave_agents/SentimentAnalysis.py` & `alphawave-0.3.6/src/alphawave_agents/SentimentAnalysis.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.5/src/alphawave_agents/SetPropertyCommand.py` & `alphawave-0.3.6/src/alphawave_agents/SetPropertyCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.5/src/alphawave_agents/agentTypes.py` & `alphawave-0.3.6/src/alphawave_agents/agentTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.5/src/alphawave_pyexts/FsInference.py` & `alphawave-0.3.6/src/alphawave_pyexts/FsInference.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.5/src/alphawave_pyexts/LLMClient.py` & `alphawave-0.3.6/src/alphawave_pyexts/LLMClient.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 host='192.168.1.195'
 port = 5004
 
 
 def get_available_models():
     return list(cv.conv_templates.keys())
 
-def run_query(model, messages, max_tokens, temp, top_p, host = host, port = port, tkroot = None, tkdisplay=None, format=True): 
+async def run_query(model, messages, max_tokens, temp, top_p, host = host, port = port, tkroot = None, tkdisplay=None, format=True): 
     global USER_PREFIX, ASSISTANT_PREFIX, SYSTEM_PREFIX
 
     conv=cv.get_conv_template(model)
     user_prompt = conv.roles[0]
     asst_prompt = conv.roles[1]
     system_prompt = conv.roles[1]
```

### Comparing `alphawave-0.3.5/src/alphawave_pyexts/SearchCommand.py` & `alphawave-0.3.6/src/alphawave_pyexts/SearchCommand.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,38 +32,40 @@
     },
     required=['query'],
     returns='search result'
 )
 
 
 class SearchCommand(SchemaBasedCommand):
-    def __init__(self, client, model, title=None, name=None, description=None, return_urls=False, logResponse=False, max_chars=1500):
+    def __init__(self, client, model, title=None, name=None, description=None, return_urls=True, logResponse=False, max_chars=1500):
         super().__init__(search_schema, title, description)
         self.client = client
         self.model = model
         self.return_urls = return_urls
         self.max_chars = max_chars
         self.logResponse = logResponse
         
     async def execute(self, input: input, memory: Any, functions: Any, tokenizer: Any) -> Any:
         try:
             if type(input) == dict and 'query' in input:
                 query = input['query']
                 memory = VolatileMemory()  # don't let anything bleed back to surrounding task
-                response =await search_service.run_chat(self.client, query, self.model, memory, functions, tokenizer, self.max_chars)
+                response = await search_service.run_chat(self.client, query, self.model, memory, functions, tokenizer, self.max_chars)
                 sc_text = ''
                 sc_urls = []
                 if type(response) is list:
                     for item in response:
                         if type(item) == dict and 'url' in item:
-                            sc_urls.append(item['url'])
+                            sc_urls.append('\n'+item['url'])
                         if type(item) == dict and 'text' in item:
                             sc_text += '\n'+(item['text'])
                     sc_text = sc_text[:max(len(sc_text)-1, self.max_chars)]
                 if self.return_urls:
-                    return {'type':'TaskResponse','status':'success', 'message':{'text': sc_text, 'urls':sc_urls}}
+                    #print(f' search returning search results')
+                    return {'type':'TaskResponse','status':'success', 'message':sc_text+'\n'+str(sc_urls)}
                 else:
                     return {'type':'TaskResponse','status':'success', 'message':sc_text}
                     
         except Exception as err:
             message = str(err)
+            #print(f' search returning {message}')
             return asdict(TaskResponse('TaskResponse', 'error', message))
```

### Comparing `alphawave-0.3.5/src/alphawave_pyexts/chat.py` & `alphawave-0.3.6/src/alphawave_pyexts/chat.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.5/src/alphawave_pyexts/configuration_RW.py` & `alphawave-0.3.6/src/alphawave_pyexts/configuration_RW.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.5/src/alphawave_pyexts/conversation.py` & `alphawave-0.3.6/src/alphawave_pyexts/conversation.py`

 * *Files 1% similar despite different names*

```diff
@@ -652,14 +652,29 @@
         stop_str=["User:", "Assistant:"],
         stop_token_ids=[11],
         sep="\n",
         sep2="<|endoftext|>",
         first_msg_no_role=False,
     )
 )
+register_conv_template(
+    Conversation(
+        name="falcon_GPTQ",
+        system="",
+        roles=("### Human", "### Assistant"),
+        messages=(),
+        offset=0,
+        sep_style=SeparatorStyle.ADD_COLON_SINGLE,
+        stop_str=["### Human"],
+        stop_token_ids=[11],
+        sep="\n",
+        sep2="<|endoftext|>",
+        first_msg_no_role=False,
+    )
+)
 register_conv_template(Conversation(
         name="galactica",
         system="",
         roles=("Question", "Answer", ""), # third entry is system prefix. if absent defaults to user prefix.
         messages=(),
         offset=0,
         sep_style=SeparatorStyle.ADD_COLON_TWO,
```

### Comparing `alphawave-0.3.5/src/alphawave_pyexts/handler.py` & `alphawave-0.3.6/src/alphawave_pyexts/handler.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.5/src/alphawave_pyexts/llmsearch/google_search_concurrent.py` & `alphawave-0.3.6/src/alphawave_pyexts/llmsearch/google_search_concurrent.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 system_prime = {"role": "system", "content":"You analyze Text with respect to Query and list any relevant information found, including direct quotes from the text, and detailed samples or examples in the text."}
 priming_1 = {"role": "user", "content":"Query:\n"}
 priming_2 = {"role": "user", "content":"List relevant information in the provided text, including direct quotes from the text. If none, respond 'no information'.\nText:\n"}
 
 
 # Define a function to make a single URL request and process the response
-async def process_url(query_phrase, keywords, keyword_weights, url, timeout, client, model, memory, functions, tokenizer, max_chars):
+def process_url(query_phrase, keywords, keyword_weights, url, timeout, client, model, memory, functions, tokenizer, max_chars):
     start_time = time.time()
     site = ut.extract_site(url)
     result = ''
     try:
         with warnings.catch_warnings():
             warnings.simplefilter('ignore')
             options = Options()
@@ -60,15 +60,15 @@
             result = ''
             with webdriver.Chrome(options=options) as dr:
                 #print(f'*****setting page load timeout {timeout} {url}')
                 dr.set_page_load_timeout(timeout)
                 try:
                     dr.get(url)
                     response = dr.page_source
-                    result =  await response_text_extract(query_phrase, keywords, keyword_weights, url, response, int(time.time()-start_time),
+                    result = response_text_extract(query_phrase, keywords, keyword_weights, url, response, int(time.time()-start_time),
                                                           client, model, memory, functions, tokenizer, max_chars)
                 except selenium.common.exceptions.TimeoutException:
                     return '', url
     except Exception:
         traceback.print_exc()
         print(f"{site} err")
         pass
@@ -76,64 +76,62 @@
     return result, url
 
 async def process_urls(query_phrase, keywords, keyword_weights, urls, search_level, client, model, memory, functions, tokenizer, max_chars):
     response = []
     start_time = time.time()
     full_text = ''
     in_process = []
-    
+    max_w = 8
     # Create a ThreadPoolExecutor with 5 worker threads
-    with concurrent.futures.ThreadPoolExecutor(max_workers=4) as executor:
+    with concurrent.futures.ThreadPoolExecutor(max_workers=max_w) as executor:
         # initialize scan of google urls
-        while True:
-            try:
-                while (len(urls) > 0
-                       # no sense starting if not much time left
-                       and ((search_level==DEEP_SEARCH and len(full_text) < 9600 and len(in_process) < 8 and time.time() - start_time < 42)
-                            or (search_level==NORMAL_SEARCH and len(full_text) < 6400 and len(in_process) < 7 and time.time()-start_time < 36)
-                            or (search_level==QUICK_SEARCH  and len(full_text) < 4800 and len(in_process) < 6 and time.time()-start_time < 24))):
+        try:
+            while len(urls) > 0 or len(in_process) >0:
+                # empty queue if out of time
+                if (search_level==NORMAL_SEARCH and (len(full_text) > 6400 or time.time()-start_time > 24)
+                    or (search_level==QUICK_SEARCH  and (len(full_text) > 4800 or time.time()-start_time > 18))):
+                    urls = []
+                elif len(urls) > 0:
                     url = urls[0]
                     urls = urls[1:]
                     # set timeout so we don't wait for a slow site forever
                     timeout = 24-int(time.time()-start_time)
                     if search_level==NORMAL_SEARCH:
                         timeout = timeout+8
                     future = executor.submit(process_url, query_phrase, keywords, keyword_weights, url, timeout, client, model, memory, functions, tokenizer, max_chars)
                     in_process.append(future)
+                    #print(f'added one to in_process {len(urls)}, {len(in_process)}')
                 # Process the responses as they arrive
                 for future in in_process:
                     if future.done():
                         in_process.remove(future)
+                        #print(f'removed one from in_process {len(urls)}, {len(in_process)}')
                         try:
-                            result, url = await asyncio.wait_for(future.result(), timeout=(max (1, (32-(time.time()-start_time)))))
+                            result, url = future.result()
                         except asyncio.TimeoutError:
-                            #print(f'timeout ')
                             continue
                         if 'coroutine' in str(type(result)).lower():
                             result = await result
                         if len(result) > 0:
                             site = ut.extract_site(url)
                             domain = ut.extract_domain(url)
                             response.append({'source':ut.extract_domain(url), 'url':url, 'text':result})
 
-                # openai seems to timeout a plugin  at about 30 secs, and there is pbly 3-4 sec overhead
-                if ((len(urls) == 0 and len(in_process) == 0)
-                    or (search_level==DEEP_SEARCH and (len(full_text) > max_chars) or time.time() - start_time > 48)
-                    or (search_level==NORMAL_SEARCH and
-                        (len(full_text) > max_chars) or time.time()-start_time > 32)
-                    or (search_level==QUICK_SEARCH  and
-                        (len(full_text) > max_chars) or time.time()-start_time > 24)
-                    ):
-                    executor.shutdown(wait=False)
-                    return response
-                time.sleep(.5)
-            except:
-                traceback.print_exc()
-        executor.shutdown(wait=False)
-    return response
+                if len(in_process) < max_w:
+                    time.sleep(.05)
+                else:
+                    time.sleep(.5)
+                        
+            executor.shutdown(wait=True)
+            #print(f'process_urls returning')
+            return response
+        except:
+            traceback.print_exc()
+            executor.shutdown(wait=False)
+        return response
 
 def extract_subtext(text, query_phrase, keywords, keyword_weights):
     ###  maybe we should score based on paragraphs, not lines?
     sentences = ut.reform(text)
     sentence_weights = {}
     final_text = ''
     for sentence in sentences:
@@ -240,15 +238,15 @@
                     return ''
             if 'relevant' in content and 'yes' in str(content['relevant']).lower() and 'tldr' in content:
                 #print(f"***** google llm_tldr\n{content['tldr']}\n")
                 return content['tldr']
     return ''
     
 
-async def response_text_extract(query_phrase, keywords, keyword_weights, url, response, get_time, client, model, memory, functions, tokenizer, max_chars):
+def response_text_extract(query_phrase, keywords, keyword_weights, url, response, get_time, client, model, memory, functions, tokenizer, max_chars):
     curr=time.time()
     extract_text = ''
     site = ut.extract_site(url)
     if url.endswith('pdf'):
         pass
     else:
         elements = partition_html(text=response)
@@ -258,15 +256,15 @@
             str_elements.append(stre)
         extract_text = extract_subtext(str_elements, query_phrase, keywords, keyword_weights)
     if len(extract_text.strip()) < 8:
         return ''
 
     # now ask openai to extract answer
     response = ''
-    response = await llm_tldr(extract_text, query_phrase, client, model, memory, functions, tokenizer, max_chars)
+    response = llm_tldr(extract_text, query_phrase, client, model, memory, functions, tokenizer, max_chars)
     return response
 
 def extract_items_from_numbered_list(text):
     items = ''
     elements = text.split('\n')
     for candidate in elements:
         candidate = candidate.lstrip('. \t')
@@ -307,15 +305,15 @@
         orig_phrase_urls = search(original_query[:min(len(original_query), 128)])
         extract_query = original_query[:min(len(original_query), 128)]
     gpt_phrase_urls = []
     if len(query_phrase) > 0:
         gpt_phrase_urls = search(query_phrase)
         extract_query = query_phrase # prefer more succint query phrase if available
     if len(orig_phrase_urls) == 0 and len(gpt_phrase_urls) == 0:
-        return '', [],  0, [''], 0, ['']
+        return ''
 
     for url in orig_phrase_urls:
         if url in gpt_phrase_urls:
             gpt_phrase_urls.remove(url)
 
     # interleave both lists now that duplicates are removed
     urls = [val for tup in zip_longest(orig_phrase_urls, gpt_phrase_urls) for val in tup if val is not None]
```

### Comparing `alphawave-0.3.5/src/alphawave_pyexts/llmsearch/search_service.py` & `alphawave-0.3.6/src/alphawave_pyexts/llmsearch/search_service.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.5/src/alphawave_pyexts/modelling_RW.py` & `alphawave-0.3.6/src/alphawave_pyexts/modelling_RW.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.5/src/alphawave_pyexts/serverUtils.py` & `alphawave-0.3.6/src/alphawave_pyexts/serverUtils.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.5/src/alphawave_pyexts/utilityV2.py` & `alphawave-0.3.6/src/alphawave_pyexts/utilityV2.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,26 +35,26 @@
 from alphawave.MemoryFork import MemoryFork
 
 openai.api_key = os.getenv("OPENAI_API_KEY")
 google_key = os.getenv("GOOGLE_KEY")
 google_cx = os.getenv("GOOGLE_CX")
 GOOGLE = 'google'
 
-def ask_LLM(model, gpt_message, max_tokens=100, temp=0.7, top_p=1.0, host = None, port = None, tkroot = None, tkdisplay=None):
+async def ask_LLM(model, gpt_message, max_tokens=100, temp=0.7, top_p=1.0, host = None, port = None, tkroot = None, tkdisplay=None):
     completion = None
     response = ''
     #print(f'***** utility ask_LLL temperature {temp}')
     try:
       if not model.lower().startswith('gpt'):
-        completion = llm.run_query(model, gpt_message, max_tokens, temp, top_p, host, port, tkroot, tkdisplay )
+        completion = await llm.run_query(model, gpt_message, max_tokens, temp, top_p, host, port, tkroot, tkdisplay )
         if completion is not None:
           response = completion
 
       else:
-        stream= openai.ChatCompletion.create(
+        stream= await openai.ChatCompletion.create(
             model=model, messages=gpt_message, max_tokens=max_tokens, temperature=temp, top_p=1, stop='STOP', stream=True)
         response = ''
         if stream is None:
           return response
         for chunk in stream:
           item = chunk['choices'][0]['delta']
           if 'content' in item.keys():
```

### Comparing `alphawave-0.3.5/tests/testOSClient.py` & `alphawave-0.3.6/tests/testOSClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.5/tests/testOpenAiClient.py` & `alphawave-0.3.6/tests/testOpenAiClient.py`

 * *Files identical despite different names*


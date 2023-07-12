# Comparing `tmp/alphawave-0.3.6.tar.gz` & `tmp/alphawave-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphawave-0.3.6.tar", last modified: Wed Jul 12 01:42:26 2023, max compression
+gzip compressed data, was "alphawave-0.3.7.tar", last modified: Wed Jul 12 20:13:58 2023, max compression
```

## Comparing `alphawave-0.3.6.tar` & `alphawave-0.3.7.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-12 01:42:26.770064 alphawave-0.3.6/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-05 21:12:30.000000 alphawave-0.3.6/LICENSE
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     9438 2023-07-12 01:42:26.770064 alphawave-0.3.6/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8859 2023-06-18 19:15:49.000000 alphawave-0.3.6/README.md
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1021 2023-07-12 01:38:39.000000 alphawave-0.3.6/pyproject.toml
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-07-12 01:42:26.770064 alphawave-0.3.6/setup.cfg
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-12 01:42:26.766064 alphawave-0.3.6/src/
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-12 01:42:26.770064 alphawave-0.3.6/src/alphawave/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     9955 2023-07-12 01:13:40.000000 alphawave-0.3.6/src/alphawave/AlphaWave.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1370 2023-06-10 00:08:35.000000 alphawave-0.3.6/src/alphawave/Colorize.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      740 2023-06-18 18:50:38.000000 alphawave-0.3.6/src/alphawave/DefaultResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8173 2023-07-09 19:31:41.000000 alphawave-0.3.6/src/alphawave/JSONResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1173 2023-06-19 22:47:36.000000 alphawave-0.3.6/src/alphawave/MemoryFork.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7164 2023-07-11 18:23:11.000000 alphawave-0.3.6/src/alphawave/OSClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     5926 2023-07-11 18:29:03.000000 alphawave-0.3.6/src/alphawave/OpenAIClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     5337 2023-07-11 16:48:33.000000 alphawave-0.3.6/src/alphawave/PythonResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1365 2023-07-10 16:02:12.000000 alphawave-0.3.6/src/alphawave/RepairTestClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3008 2023-06-15 23:14:04.000000 alphawave-0.3.6/src/alphawave/Response.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     6594 2023-07-09 00:19:51.000000 alphawave-0.3.6/src/alphawave/TOMLResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      800 2023-06-15 04:12:01.000000 alphawave-0.3.6/src/alphawave/TestClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1515 2023-06-15 04:12:10.000000 alphawave-0.3.6/src/alphawave/TestClientTest.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:12.000000 alphawave-0.3.6/src/alphawave/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1377 2023-07-11 21:25:58.000000 alphawave-0.3.6/src/alphawave/alphawaveTypes.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     4163 2023-06-04 18:16:08.000000 alphawave-0.3.6/src/alphawave/internalTypes.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      782 2023-06-07 21:02:29.000000 alphawave-0.3.6/src/alphawave/jsonParser.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-12 01:42:26.770064 alphawave-0.3.6/src/alphawave.egg-info/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     9438 2023-07-12 01:42:26.000000 alphawave-0.3.6/src/alphawave.egg-info/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1818 2023-07-12 01:42:26.000000 alphawave-0.3.6/src/alphawave.egg-info/SOURCES.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-07-12 01:42:26.000000 alphawave-0.3.6/src/alphawave.egg-info/dependency_links.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      199 2023-07-12 01:42:26.000000 alphawave-0.3.6/src/alphawave.egg-info/requires.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       44 2023-07-12 01:42:26.000000 alphawave-0.3.6/src/alphawave.egg-info/top_level.txt
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-12 01:42:26.770064 alphawave-0.3.6/src/alphawave_agents/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    17665 2023-07-12 01:13:28.000000 alphawave-0.3.6/src/alphawave_agents/Agent.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1715 2023-07-11 02:39:22.000000 alphawave-0.3.6/src/alphawave_agents/AgentCommandSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7006 2023-07-10 16:01:27.000000 alphawave-0.3.6/src/alphawave_agents/AgentCommandValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1422 2023-06-30 18:31:20.000000 alphawave-0.3.6/src/alphawave_agents/AskCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1871 2023-06-07 03:14:30.000000 alphawave-0.3.6/src/alphawave_agents/CompleteTaskCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1336 2023-06-06 16:52:41.000000 alphawave-0.3.6/src/alphawave_agents/ConfirmAnswerCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1417 2023-07-01 22:34:34.000000 alphawave-0.3.6/src/alphawave_agents/FinalAnswerCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1512 2023-07-05 23:30:15.000000 alphawave-0.3.6/src/alphawave_agents/MathCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3249 2023-07-12 00:55:02.000000 alphawave-0.3.6/src/alphawave_agents/PromptCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7932 2023-07-11 02:48:38.000000 alphawave-0.3.6/src/alphawave_agents/SchemaBasedCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2452 2023-06-09 18:41:37.000000 alphawave-0.3.6/src/alphawave_agents/SentimentAnalysis.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2149 2023-06-06 16:59:49.000000 alphawave-0.3.6/src/alphawave_agents/SetPropertyCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:38.000000 alphawave-0.3.6/src/alphawave_agents/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1859 2023-07-06 03:51:05.000000 alphawave-0.3.6/src/alphawave_agents/agentTypes.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-12 01:42:26.770064 alphawave-0.3.6/src/alphawave_pyexts/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    11096 2023-06-24 23:27:36.000000 alphawave-0.3.6/src/alphawave_pyexts/FsInference.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     6397 2023-07-11 18:37:11.000000 alphawave-0.3.6/src/alphawave_pyexts/LLMClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2843 2023-07-11 19:48:01.000000 alphawave-0.3.6/src/alphawave_pyexts/SearchCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    11610 2023-06-22 19:47:31.000000 alphawave-0.3.6/src/alphawave_pyexts/chat.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2607 2023-06-24 00:18:59.000000 alphawave-0.3.6/src/alphawave_pyexts/configuration_RW.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    23275 2023-07-08 16:36:14.000000 alphawave-0.3.6/src/alphawave_pyexts/conversation.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1154 2023-06-24 03:11:55.000000 alphawave-0.3.6/src/alphawave_pyexts/handler.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-12 01:42:26.770064 alphawave-0.3.6/src/alphawave_pyexts/llmsearch/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    13645 2023-07-11 19:55:51.000000 alphawave-0.3.6/src/alphawave_pyexts/llmsearch/google_search_concurrent.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      972 2023-07-11 19:52:28.000000 alphawave-0.3.6/src/alphawave_pyexts/llmsearch/search_service.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    47520 2023-06-24 00:15:02.000000 alphawave-0.3.6/src/alphawave_pyexts/modelling_RW.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    12724 2023-07-02 15:55:18.000000 alphawave-0.3.6/src/alphawave_pyexts/serverUtils.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     6919 2023-07-11 19:49:15.000000 alphawave-0.3.6/src/alphawave_pyexts/utilityV2.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-12 01:42:26.770064 alphawave-0.3.6/tests/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    14779 2023-06-07 17:09:31.000000 alphawave-0.3.6/tests/testOSClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    14639 2023-06-18 18:49:14.000000 alphawave-0.3.6/tests/testOpenAiClient.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-12 20:13:58.765958 alphawave-0.3.7/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-05 21:12:30.000000 alphawave-0.3.7/LICENSE
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     9438 2023-07-12 20:13:58.765958 alphawave-0.3.7/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8859 2023-06-18 19:15:49.000000 alphawave-0.3.7/README.md
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1021 2023-07-12 20:13:52.000000 alphawave-0.3.7/pyproject.toml
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-07-12 20:13:58.765958 alphawave-0.3.7/setup.cfg
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-12 20:13:58.761958 alphawave-0.3.7/src/
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-12 20:13:58.765958 alphawave-0.3.7/src/alphawave/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     9955 2023-07-12 01:13:40.000000 alphawave-0.3.7/src/alphawave/AlphaWave.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1370 2023-06-10 00:08:35.000000 alphawave-0.3.7/src/alphawave/Colorize.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      740 2023-06-18 18:50:38.000000 alphawave-0.3.7/src/alphawave/DefaultResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8173 2023-07-09 19:31:41.000000 alphawave-0.3.7/src/alphawave/JSONResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1173 2023-06-19 22:47:36.000000 alphawave-0.3.7/src/alphawave/MemoryFork.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7164 2023-07-11 18:23:11.000000 alphawave-0.3.7/src/alphawave/OSClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     5926 2023-07-11 18:29:03.000000 alphawave-0.3.7/src/alphawave/OpenAIClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     5337 2023-07-11 16:48:33.000000 alphawave-0.3.7/src/alphawave/PythonResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1365 2023-07-10 16:02:12.000000 alphawave-0.3.7/src/alphawave/RepairTestClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3008 2023-06-15 23:14:04.000000 alphawave-0.3.7/src/alphawave/Response.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     6594 2023-07-09 00:19:51.000000 alphawave-0.3.7/src/alphawave/TOMLResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      800 2023-06-15 04:12:01.000000 alphawave-0.3.7/src/alphawave/TestClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1515 2023-06-15 04:12:10.000000 alphawave-0.3.7/src/alphawave/TestClientTest.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:12.000000 alphawave-0.3.7/src/alphawave/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1377 2023-07-11 21:25:58.000000 alphawave-0.3.7/src/alphawave/alphawaveTypes.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     4163 2023-06-04 18:16:08.000000 alphawave-0.3.7/src/alphawave/internalTypes.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      782 2023-06-07 21:02:29.000000 alphawave-0.3.7/src/alphawave/jsonParser.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-12 20:13:58.765958 alphawave-0.3.7/src/alphawave.egg-info/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     9438 2023-07-12 20:13:58.000000 alphawave-0.3.7/src/alphawave.egg-info/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1818 2023-07-12 20:13:58.000000 alphawave-0.3.7/src/alphawave.egg-info/SOURCES.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-07-12 20:13:58.000000 alphawave-0.3.7/src/alphawave.egg-info/dependency_links.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      199 2023-07-12 20:13:58.000000 alphawave-0.3.7/src/alphawave.egg-info/requires.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       44 2023-07-12 20:13:58.000000 alphawave-0.3.7/src/alphawave.egg-info/top_level.txt
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-12 20:13:58.765958 alphawave-0.3.7/src/alphawave_agents/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    17679 2023-07-12 20:04:10.000000 alphawave-0.3.7/src/alphawave_agents/Agent.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1715 2023-07-11 02:39:22.000000 alphawave-0.3.7/src/alphawave_agents/AgentCommandSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7008 2023-07-12 19:17:12.000000 alphawave-0.3.7/src/alphawave_agents/AgentCommandValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1428 2023-07-12 19:12:18.000000 alphawave-0.3.7/src/alphawave_agents/AskCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1871 2023-06-07 03:14:30.000000 alphawave-0.3.7/src/alphawave_agents/CompleteTaskCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1336 2023-06-06 16:52:41.000000 alphawave-0.3.7/src/alphawave_agents/ConfirmAnswerCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1423 2023-07-12 19:12:30.000000 alphawave-0.3.7/src/alphawave_agents/FinalAnswerCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1518 2023-07-12 19:12:07.000000 alphawave-0.3.7/src/alphawave_agents/MathCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3249 2023-07-12 00:55:02.000000 alphawave-0.3.7/src/alphawave_agents/PromptCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7938 2023-07-12 19:12:49.000000 alphawave-0.3.7/src/alphawave_agents/SchemaBasedCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2452 2023-06-09 18:41:37.000000 alphawave-0.3.7/src/alphawave_agents/SentimentAnalysis.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2149 2023-06-06 16:59:49.000000 alphawave-0.3.7/src/alphawave_agents/SetPropertyCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:38.000000 alphawave-0.3.7/src/alphawave_agents/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1859 2023-07-06 03:51:05.000000 alphawave-0.3.7/src/alphawave_agents/agentTypes.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-12 20:13:58.765958 alphawave-0.3.7/src/alphawave_pyexts/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    11096 2023-06-24 23:27:36.000000 alphawave-0.3.7/src/alphawave_pyexts/FsInference.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     6397 2023-07-11 18:37:11.000000 alphawave-0.3.7/src/alphawave_pyexts/LLMClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2858 2023-07-12 19:14:52.000000 alphawave-0.3.7/src/alphawave_pyexts/SearchCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    11610 2023-06-22 19:47:31.000000 alphawave-0.3.7/src/alphawave_pyexts/chat.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2607 2023-06-24 00:18:59.000000 alphawave-0.3.7/src/alphawave_pyexts/configuration_RW.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    23275 2023-07-08 16:36:14.000000 alphawave-0.3.7/src/alphawave_pyexts/conversation.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1154 2023-06-24 03:11:55.000000 alphawave-0.3.7/src/alphawave_pyexts/handler.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-12 20:13:58.765958 alphawave-0.3.7/src/alphawave_pyexts/llmsearch/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    13645 2023-07-11 19:55:51.000000 alphawave-0.3.7/src/alphawave_pyexts/llmsearch/google_search_concurrent.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      972 2023-07-12 19:15:47.000000 alphawave-0.3.7/src/alphawave_pyexts/llmsearch/search_service.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    47520 2023-06-24 00:15:02.000000 alphawave-0.3.7/src/alphawave_pyexts/modelling_RW.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    12724 2023-07-02 15:55:18.000000 alphawave-0.3.7/src/alphawave_pyexts/serverUtils.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     6919 2023-07-11 19:49:15.000000 alphawave-0.3.7/src/alphawave_pyexts/utilityV2.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-12 20:13:58.765958 alphawave-0.3.7/tests/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    14779 2023-06-07 17:09:31.000000 alphawave-0.3.7/tests/testOSClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    14639 2023-06-18 18:49:14.000000 alphawave-0.3.7/tests/testOpenAiClient.py
```

### Comparing `alphawave-0.3.6/LICENSE` & `alphawave-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.6/PKG-INFO` & `alphawave-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphawave
-Version: 0.3.6
+Version: 0.3.7
 Summary: AlphaWave-py - Functions for smaller Large Language Models (sLLMs)
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://tuuyi.io/alphawave
 Project-URL: Bug Tracker, https://github.com/Stevenic/alphawave-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `alphawave-0.3.6/README.md` & `alphawave-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.6/pyproject.toml` & `alphawave-0.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alphawave"
-version = "0.3.6"
+version = "0.3.7"
 authors = [
   { name="Steven Ickman", email="author@example.com" },
   { name="Bruce DAmbrosio", email="bruce.dambrosio@gmail.com" },
 ]
 
 description = "AlphaWave-py - Functions for smaller Large Language Models (sLLMs)"
```

### Comparing `alphawave-0.3.6/src/alphawave/AlphaWave.py` & `alphawave-0.3.7/src/alphawave/AlphaWave.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.6/src/alphawave/Colorize.py` & `alphawave-0.3.7/src/alphawave/Colorize.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.6/src/alphawave/DefaultResponseValidator.py` & `alphawave-0.3.7/src/alphawave/DefaultResponseValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.6/src/alphawave/JSONResponseValidator.py` & `alphawave-0.3.7/src/alphawave/JSONResponseValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.6/src/alphawave/MemoryFork.py` & `alphawave-0.3.7/src/alphawave/MemoryFork.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.6/src/alphawave/OSClient.py` & `alphawave-0.3.7/src/alphawave/OSClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.6/src/alphawave/OpenAIClient.py` & `alphawave-0.3.7/src/alphawave/OpenAIClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.6/src/alphawave/PythonResponseValidator.py` & `alphawave-0.3.7/src/alphawave/PythonResponseValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.6/src/alphawave/RepairTestClient.py` & `alphawave-0.3.7/src/alphawave/RepairTestClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.6/src/alphawave/Response.py` & `alphawave-0.3.7/src/alphawave/Response.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.6/src/alphawave/TOMLResponseValidator.py` & `alphawave-0.3.7/src/alphawave/TOMLResponseValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.6/src/alphawave/TestClient.py` & `alphawave-0.3.7/src/alphawave/TestClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.6/src/alphawave/TestClientTest.py` & `alphawave-0.3.7/src/alphawave/TestClientTest.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.6/src/alphawave/alphawaveTypes.py` & `alphawave-0.3.7/src/alphawave/alphawaveTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.6/src/alphawave/internalTypes.py` & `alphawave-0.3.7/src/alphawave/internalTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.6/src/alphawave/jsonParser.py` & `alphawave-0.3.7/src/alphawave/jsonParser.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.6/src/alphawave.egg-info/PKG-INFO` & `alphawave-0.3.7/src/alphawave.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphawave
-Version: 0.3.6
+Version: 0.3.7
 Summary: AlphaWave-py - Functions for smaller Large Language Models (sLLMs)
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://tuuyi.io/alphawave
 Project-URL: Bug Tracker, https://github.com/Stevenic/alphawave-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `alphawave-0.3.6/src/alphawave.egg-info/SOURCES.txt` & `alphawave-0.3.7/src/alphawave.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.6/src/alphawave_agents/Agent.py` & `alphawave-0.3.7/src/alphawave_agents/Agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -384,15 +384,15 @@
                 if task_response['status'] in ['error', 'invalid_response', 'rate_limited', 'too_many_steps', 'too_long']:
                     #print(f'***** Agent execute_next_step fail {task_response}')
                     return task_response, False
 
             # Update history
             return_msg = task_response['message'] if task_response else result
             history = self.memory.get(history_variable) or []
-            history.append({'role': 'assistant', 'content': command_name+' '+input+' result:\n'+return_msg})
+            history.append({'role': 'assistant', 'content': command_name+' '+str(input)+' result:\n'+str(return_msg)})
             self.memory.set(history_variable, history)
 
             # Save the agents state
             state['totalSteps'] += 1
             self.set_agent_state(state, agent_id)
 
             # Return result
@@ -410,13 +410,13 @@
     async def execute_command(self, state: AgentState, thought: AgentThought):
         # a command to execute
         command_name = thought['command']
         command = self._commands.get(command_name, None) or {}
         input = thought['inputs'] or {}
         # Execute command and return result
         #print(f'***** Agent execute_command  {command_name}, {input}')
-        response = command.execute(input, self.memory, self.functions, self.tokenizer)
-        #if 'coroutine' in str(type(response)).lower():
-        #    return await response
+        response = await command.execute(input, self.memory, self.functions, self.tokenizer)
+        if 'coroutine' in str(type(response)).lower():
+            return await response
         #print(f'***** Agent execute_command {command_name}\n{response}\n')
         return response
```

### Comparing `alphawave-0.3.6/src/alphawave_agents/AgentCommandSection.py` & `alphawave-0.3.7/src/alphawave_agents/AgentCommandSection.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.6/src/alphawave_agents/AgentCommandValidator.py` & `alphawave-0.3.7/src/alphawave_agents/AgentCommandValidator.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             #print(f"***** AgentCommandValidator creating TOML")
             self._input_validator = TOMLResponseValidator(AgentThoughtSchemaTOML, 'No valid command was found. Respond using an instantiation of the specified template for the next command.')
 
         self._commands = commands
 
     def validate_response(self, memory, functions, tokenizer, response, remaining_attempts) -> Union[AgentThought, None]:
         try:
-          print(f"***** AgentCommandValidator validate syntax: \n{self._syntax}\nresponse\n{response}")
+          #print(f"***** AgentCommandValidator validate syntax: \n{self._syntax}\nresponse\n{response}")
           message = response['message']
           raw_text = message if isinstance(message, str) else message.get('content', '')
           if (self._syntax == 'JSON' and '{' not in raw_text) or (self._syntax == 'TOML' and 'response' not in raw_text.lower()):
               # means no form found, assume llm doesn't need to use a command
               return {
                   'type': 'Validation',
                   'valid': True,
@@ -55,15 +55,15 @@
           # Validate that the response contains a thought
           validation_result = self._input_validator.validate_response(memory, functions, tokenizer, response, remaining_attempts)
           if not validation_result['valid']:
             return validation_result
 
           # Validate that the command exists
           thought = validation_result['value']
-          print(f'*****AgentCommandValidator post validate thought  \n{thought}\n')
+          #print(f'*****AgentCommandValidator post validate thought  \n{thought}\n')
           if not('command' in thought) or not('inputs' in thought):
               print(f"***** AgentCommandValidator command or inputs not found")
               return {
                   'type': 'Validation',
                   'valid': False,
                   'feedback': f'command not found or invalid, or inputs missing. The commands you have are {list(self._commands.keys())}'
               }
```

### Comparing `alphawave-0.3.6/src/alphawave_agents/AskCommand.py` & `alphawave-0.3.7/src/alphawave_agents/AskCommand.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,9 +35,9 @@
         self.question = question
 
 class AskCommand(SchemaBasedCommand):
     def __init__(self, title: Optional[str] = '', description: Optional[str] = ''):
         global schema
         super().__init__(schema, title, description)
 
-    def execute(self, input: AskCommandInput, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer) -> TaskResponse:
+    async def execute(self, input: AskCommandInput, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer) -> TaskResponse:
         return asdict(TaskResponse(status="input_needed",message=input['question']))
```

### Comparing `alphawave-0.3.6/src/alphawave_agents/CompleteTaskCommand.py` & `alphawave-0.3.7/src/alphawave_agents/CompleteTaskCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.6/src/alphawave_agents/ConfirmAnswerCommand.py` & `alphawave-0.3.7/src/alphawave_agents/ConfirmAnswerCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.6/src/alphawave_agents/FinalAnswerCommand.py` & `alphawave-0.3.7/src/alphawave_agents/FinalAnswerCommand.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,11 +25,11 @@
 class FinalAnswerCommandInput:
     answer:str
 
 class FinalAnswerCommand(SchemaBasedCommand):
     def __init__(self, title: Optional[str] = None, description: Optional[str] = None):
         super().__init__(CommandSchema(), title, description)
 
-    def execute(self, input: FinalAnswerCommandInput, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer) -> TaskResponse:
+    async def execute(self, input: FinalAnswerCommandInput, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer) -> TaskResponse:
         print(f'\nAnswer: \n{input}\n')
         return_msg = {"type": "TaskResponse", "status": "input_needed", "message": input['answer'] }
         return return_msg
```

### Comparing `alphawave-0.3.6/src/alphawave_agents/MathCommand.py` & `alphawave-0.3.7/src/alphawave_agents/MathCommand.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 )
 
 class MathCommand(SchemaBasedCommand):
 
     def __init__(self, title = None, description = None):
         super().__init__(schema, title, description)
 
-    def execute(self, input: MathCommandInput, memory: Any, functions: Any, tokenizer: Any) -> Any:
+    async def execute(self, input: MathCommandInput, memory: Any, functions: Any, tokenizer: Any) -> Any:
         try:
             exp = input['code']
             exp = exp.replace('\\*', '*')
             exp = exp.replace('\\+', '+')
             exp = exp.replace('\\-', '-')
             exp = exp.replace('\\/', '/')
             return eval(exp)
```

### Comparing `alphawave-0.3.6/src/alphawave_agents/PromptCommand.py` & `alphawave-0.3.7/src/alphawave_agents/PromptCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.6/src/alphawave_agents/SchemaBasedCommand.py` & `alphawave-0.3.7/src/alphawave_agents/SchemaBasedCommand.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     def schema(self) -> CommandSchema:
         return self._schema
 
     @property
     def title(self) -> str:
         return self._title or self._schema['title']
 
-    def execute(self, inputs: Dict[str, Any], memory: 'PromptMemory', functions: 'PromptFunctions', tokenizer: 'Tokenizer') -> Any:
+    async def execute(self, inputs: Dict[str, Any], memory: 'PromptMemory', functions: 'PromptFunctions', tokenizer: 'Tokenizer') -> Any:
         raise NotImplementedError
 
     def validate(self, inputs: Dict[str, Any], memory: 'PromptMemory', functions: 'PromptFunctions', tokenizer: 'Tokenizer', syntax: str ='JSON') -> 'Validation':
         #print(f'***** SchemaBasedCommand validate inputs {inputs}\nschema\n{self._schema}')
         if self._schema is None:
             return {
                 'type': 'Validation',
```

### Comparing `alphawave-0.3.6/src/alphawave_agents/SentimentAnalysis.py` & `alphawave-0.3.7/src/alphawave_agents/SentimentAnalysis.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.6/src/alphawave_agents/SetPropertyCommand.py` & `alphawave-0.3.7/src/alphawave_agents/SetPropertyCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.6/src/alphawave_agents/agentTypes.py` & `alphawave-0.3.7/src/alphawave_agents/agentTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.6/src/alphawave_pyexts/FsInference.py` & `alphawave-0.3.7/src/alphawave_pyexts/FsInference.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.6/src/alphawave_pyexts/LLMClient.py` & `alphawave-0.3.7/src/alphawave_pyexts/LLMClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.6/src/alphawave_pyexts/SearchCommand.py` & `alphawave-0.3.7/src/alphawave_pyexts/SearchCommand.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Any, Dict, List
 from colorama import Fore, Style
 from dataclasses import dataclass, asdict
+import asyncio
 import copy
 from promptrix.SystemMessage import SystemMessage
 from promptrix.VolatileMemory import VolatileMemory
 from alphawave_agents.agentTypes import TaskResponse
 from alphawave_agents.SchemaBasedCommand import SchemaBasedCommand
 from alphawave_agents.SchemaBasedCommand import CommandSchema as sbcCommandSchema
 from alphawave_pyexts.llmsearch import search_service
```

### Comparing `alphawave-0.3.6/src/alphawave_pyexts/chat.py` & `alphawave-0.3.7/src/alphawave_pyexts/chat.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.6/src/alphawave_pyexts/configuration_RW.py` & `alphawave-0.3.7/src/alphawave_pyexts/configuration_RW.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.6/src/alphawave_pyexts/conversation.py` & `alphawave-0.3.7/src/alphawave_pyexts/conversation.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.6/src/alphawave_pyexts/handler.py` & `alphawave-0.3.7/src/alphawave_pyexts/handler.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.6/src/alphawave_pyexts/llmsearch/google_search_concurrent.py` & `alphawave-0.3.7/src/alphawave_pyexts/llmsearch/google_search_concurrent.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.6/src/alphawave_pyexts/llmsearch/search_service.py` & `alphawave-0.3.7/src/alphawave_pyexts/llmsearch/search_service.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.6/src/alphawave_pyexts/modelling_RW.py` & `alphawave-0.3.7/src/alphawave_pyexts/modelling_RW.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.6/src/alphawave_pyexts/serverUtils.py` & `alphawave-0.3.7/src/alphawave_pyexts/serverUtils.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.6/src/alphawave_pyexts/utilityV2.py` & `alphawave-0.3.7/src/alphawave_pyexts/utilityV2.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.6/tests/testOSClient.py` & `alphawave-0.3.7/tests/testOSClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.6/tests/testOpenAiClient.py` & `alphawave-0.3.7/tests/testOpenAiClient.py`

 * *Files identical despite different names*


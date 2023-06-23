# Comparing `tmp/alphawave-0.2.6.tar.gz` & `tmp/alphawave-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphawave-0.2.6.tar", last modified: Tue Jun 20 03:28:42 2023, max compression
+gzip compressed data, was "alphawave-0.2.7.tar", last modified: Fri Jun 23 17:56:51 2023, max compression
```

## Comparing `alphawave-0.2.6.tar` & `alphawave-0.2.7.tar`

### file list

```diff
@@ -1,58 +1,60 @@
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-20 03:28:42.571413 alphawave-0.2.6/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-05 21:12:30.000000 alphawave-0.2.6/LICENSE
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     9458 2023-06-20 03:28:42.571413 alphawave-0.2.6/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8859 2023-06-18 19:15:49.000000 alphawave-0.2.6/README.md
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      911 2023-06-20 03:26:31.000000 alphawave-0.2.6/pyproject.toml
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-06-20 03:28:42.571413 alphawave-0.2.6/setup.cfg
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-20 03:28:42.567413 alphawave-0.2.6/src/
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-20 03:28:42.567413 alphawave-0.2.6/src/alphawave/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     9149 2023-06-19 22:47:22.000000 alphawave-0.2.6/src/alphawave/AlphaWave.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1370 2023-06-10 00:08:35.000000 alphawave-0.2.6/src/alphawave/Colorize.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      740 2023-06-18 18:50:38.000000 alphawave-0.2.6/src/alphawave/DefaultResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     6405 2023-06-19 15:45:37.000000 alphawave-0.2.6/src/alphawave/JSONResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1173 2023-06-19 22:47:36.000000 alphawave-0.2.6/src/alphawave/MemoryFork.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8905 2023-06-19 15:46:26.000000 alphawave-0.2.6/src/alphawave/OSClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8916 2023-06-19 16:39:38.000000 alphawave-0.2.6/src/alphawave/OpenAIClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1377 2023-06-15 04:11:41.000000 alphawave-0.2.6/src/alphawave/RepairTestClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3008 2023-06-15 23:14:04.000000 alphawave-0.2.6/src/alphawave/Response.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      800 2023-06-15 04:12:01.000000 alphawave-0.2.6/src/alphawave/TestClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1515 2023-06-15 04:12:10.000000 alphawave-0.2.6/src/alphawave/TestClientTest.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:12.000000 alphawave-0.2.6/src/alphawave/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1359 2023-06-15 04:10:27.000000 alphawave-0.2.6/src/alphawave/alphawaveTypes.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     4163 2023-06-04 18:16:08.000000 alphawave-0.2.6/src/alphawave/internalTypes.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      782 2023-06-07 21:02:29.000000 alphawave-0.2.6/src/alphawave/jsonParser.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-20 03:28:42.567413 alphawave-0.2.6/src/alphawave.egg-info/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     9458 2023-06-20 03:28:42.000000 alphawave-0.2.6/src/alphawave.egg-info/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1614 2023-06-20 03:28:42.000000 alphawave-0.2.6/src/alphawave.egg-info/SOURCES.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-06-20 03:28:42.000000 alphawave-0.2.6/src/alphawave.egg-info/dependency_links.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      125 2023-06-20 03:28:42.000000 alphawave-0.2.6/src/alphawave.egg-info/requires.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       44 2023-06-20 03:28:42.000000 alphawave-0.2.6/src/alphawave.egg-info/top_level.txt
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-20 03:28:42.567413 alphawave-0.2.6/src/alphawave_agents/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    16612 2023-06-19 22:45:42.000000 alphawave-0.2.6/src/alphawave_agents/Agent.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1332 2023-06-11 16:22:40.000000 alphawave-0.2.6/src/alphawave_agents/AgentCommandSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2956 2023-06-19 02:42:43.000000 alphawave-0.2.6/src/alphawave_agents/AgentCommandValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1428 2023-06-11 19:07:37.000000 alphawave-0.2.6/src/alphawave_agents/AskCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1871 2023-06-07 03:14:30.000000 alphawave-0.2.6/src/alphawave_agents/CompleteTaskCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1336 2023-06-06 16:52:41.000000 alphawave-0.2.6/src/alphawave_agents/ConfirmAnswerCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1386 2023-06-07 02:55:09.000000 alphawave-0.2.6/src/alphawave_agents/FinalAnswerCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1509 2023-06-07 03:15:08.000000 alphawave-0.2.6/src/alphawave_agents/MathCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3130 2023-06-18 18:54:41.000000 alphawave-0.2.6/src/alphawave_agents/PromptCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3546 2023-06-19 15:47:21.000000 alphawave-0.2.6/src/alphawave_agents/SchemaBasedCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2452 2023-06-09 18:41:37.000000 alphawave-0.2.6/src/alphawave_agents/SentimentAnalysis.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2149 2023-06-06 16:59:49.000000 alphawave-0.2.6/src/alphawave_agents/SetPropertyCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:38.000000 alphawave-0.2.6/src/alphawave_agents/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2134 2023-06-19 01:22:49.000000 alphawave-0.2.6/src/alphawave_agents/agentTypes.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-20 03:28:42.567413 alphawave-0.2.6/src/alphawave_pyexts/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     4433 2023-06-19 22:44:06.000000 alphawave-0.2.6/src/alphawave_pyexts/LLMClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2687 2023-06-19 22:44:59.000000 alphawave-0.2.6/src/alphawave_pyexts/SearchCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    10457 2023-06-18 23:46:33.000000 alphawave-0.2.6/src/alphawave_pyexts/chat.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    19050 2023-06-17 23:10:50.000000 alphawave-0.2.6/src/alphawave_pyexts/conversation.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-20 03:28:42.567413 alphawave-0.2.6/src/alphawave_pyexts/llmsearch/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    13725 2023-06-19 22:24:29.000000 alphawave-0.2.6/src/alphawave_pyexts/llmsearch/google_search_concurrent.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      972 2023-06-19 22:47:56.000000 alphawave-0.2.6/src/alphawave_pyexts/llmsearch/search_service.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1402 2023-06-16 20:15:32.000000 alphawave-0.2.6/src/alphawave_pyexts/searchCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     6689 2023-06-19 03:02:57.000000 alphawave-0.2.6/src/alphawave_pyexts/utilityV2.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-20 03:28:42.567413 alphawave-0.2.6/tests/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    14779 2023-06-07 17:09:31.000000 alphawave-0.2.6/tests/testOSClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    14639 2023-06-18 18:49:14.000000 alphawave-0.2.6/tests/testOpenAiClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      948 2023-06-06 20:59:59.000000 alphawave-0.2.6/tests/testSchema.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-23 17:56:51.298537 alphawave-0.2.7/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-05 21:12:30.000000 alphawave-0.2.7/LICENSE
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     9441 2023-06-23 17:56:51.298537 alphawave-0.2.7/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8859 2023-06-18 19:15:49.000000 alphawave-0.2.7/README.md
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      945 2023-06-23 17:56:44.000000 alphawave-0.2.7/pyproject.toml
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-06-23 17:56:51.298537 alphawave-0.2.7/setup.cfg
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-23 17:56:51.298537 alphawave-0.2.7/src/
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-23 17:56:51.298537 alphawave-0.2.7/src/alphawave/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     9267 2023-06-20 23:20:58.000000 alphawave-0.2.7/src/alphawave/AlphaWave.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1370 2023-06-10 00:08:35.000000 alphawave-0.2.7/src/alphawave/Colorize.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      740 2023-06-18 18:50:38.000000 alphawave-0.2.7/src/alphawave/DefaultResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     6405 2023-06-19 15:45:37.000000 alphawave-0.2.7/src/alphawave/JSONResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1173 2023-06-19 22:47:36.000000 alphawave-0.2.7/src/alphawave/MemoryFork.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8905 2023-06-19 15:46:26.000000 alphawave-0.2.7/src/alphawave/OSClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8916 2023-06-19 16:39:38.000000 alphawave-0.2.7/src/alphawave/OpenAIClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1377 2023-06-15 04:11:41.000000 alphawave-0.2.7/src/alphawave/RepairTestClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3008 2023-06-15 23:14:04.000000 alphawave-0.2.7/src/alphawave/Response.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      800 2023-06-15 04:12:01.000000 alphawave-0.2.7/src/alphawave/TestClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1515 2023-06-15 04:12:10.000000 alphawave-0.2.7/src/alphawave/TestClientTest.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:12.000000 alphawave-0.2.7/src/alphawave/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1359 2023-06-15 04:10:27.000000 alphawave-0.2.7/src/alphawave/alphawaveTypes.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     4163 2023-06-04 18:16:08.000000 alphawave-0.2.7/src/alphawave/internalTypes.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      782 2023-06-07 21:02:29.000000 alphawave-0.2.7/src/alphawave/jsonParser.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-23 17:56:51.298537 alphawave-0.2.7/src/alphawave.egg-info/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     9441 2023-06-23 17:56:51.000000 alphawave-0.2.7/src/alphawave.egg-info/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1676 2023-06-23 17:56:51.000000 alphawave-0.2.7/src/alphawave.egg-info/SOURCES.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-06-23 17:56:51.000000 alphawave-0.2.7/src/alphawave.egg-info/dependency_links.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      155 2023-06-23 17:56:51.000000 alphawave-0.2.7/src/alphawave.egg-info/requires.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       44 2023-06-23 17:56:51.000000 alphawave-0.2.7/src/alphawave.egg-info/top_level.txt
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-23 17:56:51.298537 alphawave-0.2.7/src/alphawave_agents/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    16612 2023-06-19 22:45:42.000000 alphawave-0.2.7/src/alphawave_agents/Agent.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1332 2023-06-11 16:22:40.000000 alphawave-0.2.7/src/alphawave_agents/AgentCommandSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2956 2023-06-19 02:42:43.000000 alphawave-0.2.7/src/alphawave_agents/AgentCommandValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1428 2023-06-11 19:07:37.000000 alphawave-0.2.7/src/alphawave_agents/AskCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1871 2023-06-07 03:14:30.000000 alphawave-0.2.7/src/alphawave_agents/CompleteTaskCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1336 2023-06-06 16:52:41.000000 alphawave-0.2.7/src/alphawave_agents/ConfirmAnswerCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1425 2023-06-22 21:06:20.000000 alphawave-0.2.7/src/alphawave_agents/FinalAnswerCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1509 2023-06-07 03:15:08.000000 alphawave-0.2.7/src/alphawave_agents/MathCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3130 2023-06-18 18:54:41.000000 alphawave-0.2.7/src/alphawave_agents/PromptCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3874 2023-06-23 16:34:08.000000 alphawave-0.2.7/src/alphawave_agents/SchemaBasedCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2452 2023-06-09 18:41:37.000000 alphawave-0.2.7/src/alphawave_agents/SentimentAnalysis.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2149 2023-06-06 16:59:49.000000 alphawave-0.2.7/src/alphawave_agents/SetPropertyCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:38.000000 alphawave-0.2.7/src/alphawave_agents/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2134 2023-06-19 01:22:49.000000 alphawave-0.2.7/src/alphawave_agents/agentTypes.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-23 17:56:51.298537 alphawave-0.2.7/src/alphawave_pyexts/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     6944 2023-06-23 17:13:40.000000 alphawave-0.2.7/src/alphawave_pyexts/LLMClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2687 2023-06-19 22:44:59.000000 alphawave-0.2.7/src/alphawave_pyexts/SearchCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    11610 2023-06-22 19:47:31.000000 alphawave-0.2.7/src/alphawave_pyexts/chat.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    21329 2023-06-23 16:43:17.000000 alphawave-0.2.7/src/alphawave_pyexts/conversation.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      813 2023-06-21 16:08:15.000000 alphawave-0.2.7/src/alphawave_pyexts/falcon.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      850 2023-06-21 22:46:07.000000 alphawave-0.2.7/src/alphawave_pyexts/falcon40.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-23 17:56:51.298537 alphawave-0.2.7/src/alphawave_pyexts/llmsearch/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    13725 2023-06-19 22:24:29.000000 alphawave-0.2.7/src/alphawave_pyexts/llmsearch/google_search_concurrent.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      972 2023-06-19 22:47:56.000000 alphawave-0.2.7/src/alphawave_pyexts/llmsearch/search_service.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     6039 2023-06-22 03:24:44.000000 alphawave-0.2.7/src/alphawave_pyexts/serverUtils.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     6684 2023-06-23 16:42:51.000000 alphawave-0.2.7/src/alphawave_pyexts/utilityV2.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-23 17:56:51.298537 alphawave-0.2.7/tests/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    14779 2023-06-07 17:09:31.000000 alphawave-0.2.7/tests/testOSClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    14639 2023-06-18 18:49:14.000000 alphawave-0.2.7/tests/testOpenAiClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      948 2023-06-06 20:59:59.000000 alphawave-0.2.7/tests/testSchema.py
```

### Comparing `alphawave-0.2.6/LICENSE` & `alphawave-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.6/PKG-INFO` & `alphawave-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: alphawave
-Version: 0.2.6
-Summary: AlphaWave - a very opinionated client for interfacing with Large Language Models (LLM)
+Version: 0.2.7
+Summary: AlphaWave - a client for interfacing with Large Language Models (LLM)
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://tuuyi.io/alphawave
 Project-URL: Bug Tracker, https://github.com/Stevenic/alphawave-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `alphawave-0.2.6/README.md` & `alphawave-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.6/pyproject.toml` & `alphawave-0.2.7/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alphawave"
-version = "0.2.6"
+version = "0.2.7"
 authors = [
   { name="Steven Ickman", email="author@example.com" },
   { name="Bruce DAmbrosio", email="bruce.dambrosio@gmail.com" },
 ]
 
-description = "AlphaWave - a very opinionated client for interfacing with Large Language Models (LLM)"
+description = "AlphaWave - a client for interfacing with Large Language Models (LLM)"
 
 
 readme = "README.md"
 
 requires-python = ">=3.8"
 
 classifiers = [
@@ -30,14 +30,17 @@
     "pyyaml",
     "pyee",
     "selenium",
     "wordfreq",
     "tenacity",	
     "openai",
     "nltk",
+    "transformers",
+    "accelerate",
+    "torch",
     'importlib-metadata; python_version<"3.9"',
 ]
 
 
 [project.urls]
 "Homepage" = "https://tuuyi.io/alphawave"
 "Bug Tracker" = "https://github.com/Stevenic/alphawave-py/issues"
```

### Comparing `alphawave-0.2.6/src/alphawave/AlphaWave.py` & `alphawave-0.2.7/src/alphawave/AlphaWave.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,14 +110,15 @@
             repair = self.repairResponse(fork, functions, tokenizer, response, validation, max_repair_attempts)
             if 'coroutine' in str(type(repair)).lower():
                 repair = await repair
             self.emit('afterRepair', fork, functions, tokenizer, response, max_repair_attempts, validation)
 
             if self.options.logRepairs:
                 if repair['status'] == 'success':
+                    self.emit('repairSuccess', fork, functions, tokenizer, response, max_repair_attempts, validation)
                     print(Colorize.success('Response Repaired'))
                 else:
                     print(Colorize.error('Response Repair Failed'))
 
             if repair['status'] == 'success':
                 self.addInputToHistory(memory, history_variable, input)
                 self.addResponseToHistory(memory,history_variable, repair['message'])
```

### Comparing `alphawave-0.2.6/src/alphawave/Colorize.py` & `alphawave-0.2.7/src/alphawave/Colorize.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.6/src/alphawave/DefaultResponseValidator.py` & `alphawave-0.2.7/src/alphawave/DefaultResponseValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.6/src/alphawave/JSONResponseValidator.py` & `alphawave-0.2.7/src/alphawave/JSONResponseValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.6/src/alphawave/MemoryFork.py` & `alphawave-0.2.7/src/alphawave/MemoryFork.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.6/src/alphawave/OSClient.py` & `alphawave-0.2.7/src/alphawave/OSClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.6/src/alphawave/OpenAIClient.py` & `alphawave-0.2.7/src/alphawave/OpenAIClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.6/src/alphawave/RepairTestClient.py` & `alphawave-0.2.7/src/alphawave/RepairTestClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.6/src/alphawave/Response.py` & `alphawave-0.2.7/src/alphawave/Response.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.6/src/alphawave/TestClient.py` & `alphawave-0.2.7/src/alphawave/TestClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.6/src/alphawave/TestClientTest.py` & `alphawave-0.2.7/src/alphawave/TestClientTest.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.6/src/alphawave/alphawaveTypes.py` & `alphawave-0.2.7/src/alphawave/alphawaveTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.6/src/alphawave/internalTypes.py` & `alphawave-0.2.7/src/alphawave/internalTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.6/src/alphawave/jsonParser.py` & `alphawave-0.2.7/src/alphawave/jsonParser.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.6/src/alphawave.egg-info/PKG-INFO` & `alphawave-0.2.7/src/alphawave.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: alphawave
-Version: 0.2.6
-Summary: AlphaWave - a very opinionated client for interfacing with Large Language Models (LLM)
+Version: 0.2.7
+Summary: AlphaWave - a client for interfacing with Large Language Models (LLM)
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://tuuyi.io/alphawave
 Project-URL: Bug Tracker, https://github.com/Stevenic/alphawave-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `alphawave-0.2.6/src/alphawave.egg-info/SOURCES.txt` & `alphawave-0.2.7/src/alphawave.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,16 @@
 src/alphawave_agents/SetPropertyCommand.py
 src/alphawave_agents/__init__.py
 src/alphawave_agents/agentTypes.py
 src/alphawave_pyexts/LLMClient.py
 src/alphawave_pyexts/SearchCommand.py
 src/alphawave_pyexts/chat.py
 src/alphawave_pyexts/conversation.py
-src/alphawave_pyexts/searchCommand.py
+src/alphawave_pyexts/falcon.py
+src/alphawave_pyexts/falcon40.py
+src/alphawave_pyexts/serverUtils.py
 src/alphawave_pyexts/utilityV2.py
 src/alphawave_pyexts/llmsearch/google_search_concurrent.py
 src/alphawave_pyexts/llmsearch/search_service.py
 tests/testOSClient.py
 tests/testOpenAiClient.py
 tests/testSchema.py
```

### Comparing `alphawave-0.2.6/src/alphawave_agents/Agent.py` & `alphawave-0.2.7/src/alphawave_agents/Agent.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.6/src/alphawave_agents/AgentCommandSection.py` & `alphawave-0.2.7/src/alphawave_agents/AgentCommandSection.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.6/src/alphawave_agents/AgentCommandValidator.py` & `alphawave-0.2.7/src/alphawave_agents/AgentCommandValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.6/src/alphawave_agents/AskCommand.py` & `alphawave-0.2.7/src/alphawave_agents/AskCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.6/src/alphawave_agents/CompleteTaskCommand.py` & `alphawave-0.2.7/src/alphawave_agents/CompleteTaskCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.6/src/alphawave_agents/ConfirmAnswerCommand.py` & `alphawave-0.2.7/src/alphawave_agents/ConfirmAnswerCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.6/src/alphawave_agents/FinalAnswerCommand.py` & `alphawave-0.2.7/src/alphawave_agents/FinalAnswerCommand.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from alphawave_agents.SchemaBasedCommand import SchemaBasedCommand
 
 
 @dataclass
 class CommandSchema(sbcCommandSchema):
     schema_type: str = "object"
     title: str = "finalAnswer"
-    description: str = "generate an answer for the user"
+    description: str = "show answer to the user"
     properties: dict = field(default_factory=lambda: {
         "answer": {
             "type": "string",
             "description": "final answer"
         }
     })
     required: list[str] = field(default_factory=lambda: ["answer"])
@@ -26,12 +26,13 @@
     answer:str
 
 class FinalAnswerCommand(SchemaBasedCommand):
     def __init__(self, title: Optional[str] = None, description: Optional[str] = None):
         super().__init__(CommandSchema(), title, description)
 
     def execute(self, input: FinalAnswerCommandInput, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer) -> TaskResponse:
+        print(f'\nAnswer: \n{input}\n')
         return {
             "type": "TaskResponse",
-            "status": "success",
-            "message": input['answer']
+            "status": "input_needed",
+            "message": "input['answer']"
         }
```

### Comparing `alphawave-0.2.6/src/alphawave_agents/MathCommand.py` & `alphawave-0.2.7/src/alphawave_agents/MathCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.6/src/alphawave_agents/PromptCommand.py` & `alphawave-0.2.7/src/alphawave_agents/PromptCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.6/src/alphawave_agents/SchemaBasedCommand.py` & `alphawave-0.2.7/src/alphawave_agents/SchemaBasedCommand.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,14 +58,21 @@
                 'type': 'Validation',
                 'valid': True,
                 'value': cleaned
             }
         except ValidationError as e:
             errors = f'"{e.path[0] if e.path else "input"}": {e.message}'
             message = errors
+            if 'is a required property' in message:
+                return {
+                    'type': 'Validation',
+                    'valid': False,
+                    'feedback': f"The ['command']['input'] field has errors:\n{message}\n\nRevise to include the field with valid value."
+                }
+                
             return {
                 'type': 'Validation',
                 'valid': False,
                 'feedback': f"The ['command']['input'] field has errors:\n{message}\n\nTry again."
             }
 
     def clean_input(self, input: Dict[str, Any]) -> Dict[str, Any]:
```

### Comparing `alphawave-0.2.6/src/alphawave_agents/SentimentAnalysis.py` & `alphawave-0.2.7/src/alphawave_agents/SentimentAnalysis.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.6/src/alphawave_agents/SetPropertyCommand.py` & `alphawave-0.2.7/src/alphawave_agents/SetPropertyCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.6/src/alphawave_agents/agentTypes.py` & `alphawave-0.2.7/src/alphawave_agents/agentTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.6/src/alphawave_pyexts/SearchCommand.py` & `alphawave-0.2.7/src/alphawave_pyexts/SearchCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.6/src/alphawave_pyexts/chat.py` & `alphawave-0.2.7/src/alphawave_pyexts/chat.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,28 +14,29 @@
 from promptrix.SystemMessage import SystemMessage
 from promptrix.UserMessage import UserMessage
 from promptrix.AssistantMessage import AssistantMessage
 from promptrix.ConversationHistory import ConversationHistory
 from alphawave_pyexts import utilityV2 as ut
 from alphawave_pyexts import LLMClient as llm
 
-USER_PREFIX = None
-ASSISTANT_PREFIX = None
+USER_PREFIX = 'User'
+ASSISTANT_PREFIX = 'Assistant'
 STOP_1 = '</s>'
 STOP_2 = USER_PREFIX
+FORMAT=True
 
 prompt_text = 'You are helpful, creative, clever, and very friendly. '
 PROMPT = Prompt([
     UserMessage(prompt_text),
     ConversationHistory('history', .5),
     UserMessage('{{$input}}')
 ])
 
 parser = argparse.ArgumentParser()
-parser.add_argument('model', type=str, default='wizardLM', choices=['wizardLM', 'falcon40B', 'falcon40B.2', 'falcon40B.3', 'gpt_35', 'gpt_4'],help='select prompting based on modelto load')
+parser.add_argument('model', type=str, default='wizardLM', choices=['wizardLM', 'zero_shot', 'vicuna_v1.1', 'dolly', 'oasst_pythoa', 'stablelm', 'baize', 'rwkv', 'openbuddy', 'phoenix', 'claude', 'mpt', 'bard', 'billa', 'h2ogpt', 'snoozy', 'manticore', 'falcon_instruct', 'falcon_instruct2', 'falcon_instruct3', 'gpt_35', 'gpt_4'],help='select prompting based on modelto load')
 parser.add_argument('--user', type=str, default='', help='user prefix, overrides model template')
 parser.add_argument('--asst', type=str, default='', help='assistant prefix, overrides model template')
 parser.add_argument('--stop1', type=str, default='',help='stop string')
 parser.add_argument('--stop2', type=str, default='', help='alternative stop string')
 args = parser.parse_args()
 if args.user:
     USER_PREFIX = args.user
@@ -45,15 +46,15 @@
 if args.stop1:
     STOP_1 = args.stop1
 if args.stop2:
     STOP_2 = args.stop2
 if args.model:
     model = args.model
 else:
-    model = 'wizardLM-30B'
+    model = 'wizardLM'
 
 
 
 def show_prompt():
     pass
 
 def set_model():
@@ -72,34 +73,49 @@
                 top_p = float(text[idx+1:].strip())
         if 'max_tkns' in text:
             idx = text.find('=')
             if idx > 0:
                 max_tkns = int(text[idx+1:].strip())
     except Exception as e:
         print ("parse failed", e)
-        
+
+PREV_LEN = 0
 def submit():
+    global PREV_LEN
     input_text = input_area.get("1.0", tk.END)
+    if len(input_text) > PREV_LEN:
+        new_text = input_text[PREV_LEN:]
     input_area.insert(tk.END, '\n')
-    response = run_query(input_text)
+    response = run_query(new_text)
+    PREV_LEN=len(input_text)
+
+def setFormat():
+    global FORMAT
+    if FORMAT:
+        format_button.config(text='RAW')
+        FORMAT=False
+    else:
+        format_button.config(text='FORMAT')
+        FORMAT=True
+
 
 def setPrompt():
     global PROMPT
     input_text = input_area.get("1.0", tk.END)
-    if input_text.startswith("0"):
+    if input_text.startswith("NoPrompt"):
         input_text = ''
-    if input_text.startswith("1"):
+    if input_text.startswith("Helpfull"):
         input_text = 'Response as a helpful, friendly, information assistant. Say "I don\'t know" if you have no information"'
-    if input_text.startswith("2"):
+    if input_text.startswith("Bhagaven"):
         input_text = 'Respond as a compassionate, empathetic, self-realized follower of Ramana Maharshi'
-    if input_text.startswith("3"):
+    if input_text.startswith("ACT"):
         input_text = 'Respond as a compassionate, empathetic, counselor familiar with Acceptance Commitment Theray'
-    if input_text.startswith("4"):
-        input_text = 'Respond as a friendly, compassionate, chatty, flirty young woman named Samantha. You are 21 years ol.'
-    if input_text.startswith("5"):
+    if input_text.startswith("Flirt"):
+        input_text = 'Respond as a friendly,\ chatty, flirty young woman named Samantha. You are 21 years old.'
+    if input_text.startswith("Agent"):
         input_text =\
             """
 Define steps as:
 orient: identify the task
 thought: think step by step about the task. Identify ambiguities or logical consequences in the problem statement that impact your response to the task.
 action: act to further progress on the task. Your available acts are:
 i. answer: if the answer is available, respond with answer then respond STOP
@@ -121,15 +137,16 @@
         UserMessage(prompt_text),
         ConversationHistory('history', .5),
         UserMessage('{{$input}}')
     ])
 
     
 def clear():
-    global memory
+    global memory, PREV_POS
+    PREV_POS="1.0"
     input_area.delete("1.0", tk.END)
     memory.set('history', [])
 
 root = tk.Tk()
 
 root.title(args.model)
 root.geometry("1260x1024")
@@ -176,15 +193,15 @@
 clear_button.pack(side='top', fill='x')
 
 temperature = tk.StringVar()
 temperature.set('.7')
 temperature.trace("w", on_value_change)
 temp_label = ttk.Label(controlFrame, text="Temperature", style='TLabel')
 temp_label.pack(side='top', fill='x')
-temp_button = ttk.Combobox(controlFrame, textvariable=temperature, values = [.1,.2,.3,.4,.5,.6,.7,.8,.9,1.0], style='TCombobox')
+temp_button = ttk.Combobox(controlFrame, textvariable=temperature, values = [.01,.1,.2,.4,.5,.7,.9,1.0], style='TCombobox')
 temp_button.pack(side='top', fill='x')
 
 top_p = tk.StringVar()
 top_p.set('1.0')
 top_p_label = ttk.Label(controlFrame, text="Top_p", style='TLabel')
 top_p_label.pack(side='top', fill='x')
 top_p_button = ttk.Combobox(controlFrame, textvariable=top_p, values = [.1,.2,.3,.4,.5,.6,.7,.8,.9,1.0], style='TCombobox')
@@ -193,63 +210,71 @@
 max_tkns = tk.StringVar()
 max_tkns.set('250')
 max_tok_label = ttk.Label(controlFrame, text="MaxTokens", style='TLabel')
 max_tok_label.pack(side='top', fill='x')
 max_tok_button = ttk.Combobox(controlFrame, textvariable=max_tkns, values = [50,100,250,500,1000,1500,2000,4000,8000], style='TCombobox')
 max_tok_button.pack(side='top', fill='x')
 
+format_button = tk.Button(controlFrame, text="Format", command=setFormat, font=("Arial", 12), bg='grey')
+format_button.pack(side='top', fill='x')
 
 prompt_button = tk.Button(controlFrame, text="setPrompt", command=setPrompt, font=("Arial", 12), bg='grey')
 prompt_button.pack(side='top', fill='x')
+
 #model_button = tk.Button(controlFrame, text="gpt-3.5-turbo", command=set_model, font=("Arial", 12), bg='grey')
 #model_button.pack(side='top', fill='x')
 
 root.rowconfigure(0, weight=1)
 root.columnconfigure(0, weight=1)
 
 functions = FunctionRegistry()
 tokenizer = GPT3Tokenizer()
 memory = VolatileMemory({'input':'', 'history':[]})
 max_tokens = 2000
 # Render the prompt for a Text Completion call
 async def render_text_completion():
+    print(f"\n***** chat memory pre render \n{memory.get('history')}\n")
     as_text = await PROMPT.renderAsText(memory, functions, tokenizer, max_tokens)
     print(as_text)
     text = ''
     if not as_text.tooLong:
         text = as_text.output
     return text
 
 # Render the prompt for a Text Completion call
 async def render_messages_completion():
+    print(f"\n***** chat memory pre render input: \n{memory.get('input')}")
+    print(f"***** chat memory pre render \n{memory.get('history')}\n")
     as_msgs = await PROMPT.renderAsMessages(memory, functions, tokenizer, max_tokens)
     msgs = []
     if not as_msgs.tooLong:
         msgs = as_msgs.output
     return msgs
 
 
 host = '127.0.0.1'
 port = 5004
 
-
 def run_query(query):
     global model, temperature, top_p, max_tkns, memory
     try:
         memory.set('input', query)
-        msgs = asyncio.run(render_messages_completion())
-        for msg in msgs:
-            print(str(msg))
-        response = ut.ask_LLM(model, msgs, int(max_tkns.get()), float(temperature.get()), float(top_p.get()), host, port, root, input_area)
-        #print(response)
-        history = memory.get('history')
-        history.append({'role':llm.USER_PREFIX, 'content': query})
-        history.append({'role': llm.ASSISTANT_PREFIX, 'content': response})
-        memory.set('history', history)
-        print(f'***** updated history {history}')
+        if FORMAT:
+            msgs = asyncio.run(render_messages_completion())
+            for msg in msgs:
+                print(str(msg))
+            response = ut.ask_LLM(model, msgs, int(max_tkns.get()), float(temperature.get()), float(top_p.get()), host, port, root, input_area)
+            #print(response)
+            history = memory.get('history')
+            history.append({'role':llm.USER_PREFIX, 'content': query})
+            history.append({'role': llm.ASSISTANT_PREFIX, 'content': response})
+            memory.set('history', history)
+        else:
+            # just send the raw input text to server
+            llm.run_query(model, query, int(max_tkns.get()), float(temperature.get()), float(top_p.get()), host, port, root, input_area, format=False)
     except Exception:
         traceback.print_exc()
         
 if args.user is not None:
     USER_PREFIX = args.user
     STOP_2=args.user
 if args.asst is not None:
```

### Comparing `alphawave-0.2.6/src/alphawave_pyexts/conversation.py` & `alphawave-0.2.7/src/alphawave_pyexts/conversation.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,19 +14,20 @@
     ADD_COLON_TWO = auto()
     ADD_COLON_SPACE_SINGLE = auto()
     NO_COLON_SINGLE = auto()
     ADD_NEW_LINE_SINGLE = auto()
     DOLLY = auto()
     RWKV = auto()
     PHOENIX = auto()
+    ROBIN = auto()
 
 
 @dataclasses.dataclass
 class Conversation:
-    """A class that keeps all conversation history."""
+    """A class that manages prompt templates and keeps all conversation history."""
 
     # The name of this template
     name: str
     # The system prompt
     system: str
     # Two roles
     roles: List[str]
@@ -114,14 +115,22 @@
             ret = self.system
             for role, message in self.messages:
                 if message:
                     ret += role + ": " + "<s>" + message + "</s>"
                 else:
                     ret += role + ": " + "<s>"
             return ret
+        elif self.sep_style == SeparatorStyle.ROBIN:
+            ret = self.system + self.sep
+            for role, message in self.messages:
+                if message:
+                    ret += role + ":\n" + message + self.sep
+                else:
+                    ret += role + ":\n"
+            return ret
         else:
             raise ValueError(f"Invalid style: {self.sep_style}")
 
     def append_message(self, role: str, message: str):
         """Append a new message."""
         self.messages.append([role, message])
 
@@ -501,14 +510,29 @@
         messages=(),
         offset=0,
         sep_style=SeparatorStyle.NO_COLON_SINGLE,
         sep="</s>",
     )
 )
 
+# Robin default template
+register_conv_template(
+    Conversation(
+        name="Robin",
+        system="A chat between a curious human and an artificial intelligence assistant. The assistant gives helpful, detailed, and polite answers to the human's questions.",
+        roles=("###Human", "###Assistant"),
+        messages=(),
+        offset=0,
+        sep_style=SeparatorStyle.ROBIN,
+        sep="\n",
+        stop_token_ids=[2, 396],
+        stop_str="###",
+    )
+)
+
 # Snoozy default template
 # Reference: https://github.com/nomic-ai/gpt4all/blob/d4861030b778da6db59d21d2927a4aba4f9f1f43/gpt4all-bindings/python/gpt4all/gpt4all.py#L232
 register_conv_template(
     Conversation(
         name="snoozy",
         system="### Instruction:\nThe prompt below is a question to answer, a task to complete, or a conversation to respond to; decide which and write an appropriate response.",
         roles=("### Prompt", "### Response"),
@@ -530,14 +554,71 @@
         offset=0,
         sep_style=SeparatorStyle.ADD_COLON_TWO,
         sep="\n",
         sep2="</s>",
     )
 )
 
+# Falcon default template
+register_conv_template(
+    Conversation(
+        name="falcon",
+        system="",
+        roles=("User", "Assistant"),
+        messages=[],
+        offset=0,
+        sep_style=SeparatorStyle.RWKV,
+        sep="\n",
+        sep2="<|endoftext|>",
+        stop_str="\nUser",  # use stop_str to stop generation after stop_token_ids, it will also remove stop_str from the generated text
+        stop_token_ids=[
+            0,
+            1,
+            2,
+            3,
+            4,
+            5,
+            6,
+            7,
+            8,
+            9,
+            10,
+            11,
+        ],  # it better only put special tokens here, because tokenizer only remove special tokens
+    )
+)
+
+# ChagGPT default template
+register_conv_template(
+    Conversation(
+        name="polyglot_changgpt",
+        system="",
+        roles=("B", "A"),
+        messages=(),
+        offset=0,
+        sep_style=SeparatorStyle.ADD_COLON_SINGLE,
+        sep="\n",
+    )
+)
+
+# tigerbot template
+register_conv_template(
+    Conversation(
+        name="tigerbot",
+        system="A chat between a curious user and an artificial intelligence assistant. "
+        "The assistant gives helpful, detailed, and polite answers to the user's questions.",
+        roles=("### Instruction", "### Response"),
+        messages=(),
+        offset=0,
+        sep_style=SeparatorStyle.ROBIN,
+        sep="\n\n",
+        stop_str="###",
+    )
+)
+
 
 if __name__ == "__main__":
     conv = get_conv_template("vicuna_v1.1")
     conv.append_message(conv.roles[0], "Hello!")
     conv.append_message(conv.roles[1], "Hi!")
     conv.append_message(conv.roles[0], "How are you?")
     conv.append_message(conv.roles[1], None)
```

### Comparing `alphawave-0.2.6/src/alphawave_pyexts/llmsearch/google_search_concurrent.py` & `alphawave-0.2.7/src/alphawave_pyexts/llmsearch/google_search_concurrent.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.6/src/alphawave_pyexts/llmsearch/search_service.py` & `alphawave-0.2.7/src/alphawave_pyexts/llmsearch/search_service.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.6/src/alphawave_pyexts/utilityV2.py` & `alphawave-0.2.7/src/alphawave_pyexts/utilityV2.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import requests
 import time
 import traceback
 import json
 import os
 import asyncio
 from typing import Any, Dict, List, Tuple
-import alphawave_pyexts.LLMClient as client
+import alphawave_pyexts.LLMClient as llm
 from promptrix.Prompt import Prompt
 from alphawave_agents.PromptCommand import PromptCommand
 from promptrix.UserMessage import UserMessage
 from alphawave.alphawaveTypes import PromptCompletionOptions
 from alphawave_agents.PromptCommand import CommandSchema, PromptCommandOptions
 from alphawave.AlphaWave import AlphaWave
 from alphawave.DefaultResponseValidator import DefaultResponseValidator
@@ -38,18 +38,18 @@
 google_key = os.getenv("GOOGLE_KEY")
 google_cx = os.getenv("GOOGLE_CX")
 GOOGLE = 'google'
 
 def ask_LLM(model, gpt_message, max_tokens=100, temp=0.7, top_p=1.0, host = None, port = None, tkroot = None, tkdisplay=None):
     completion = None
     response = ''
-    print(f'***** utility ask_LLL temperature {temp}')
+    #print(f'***** utility ask_LLL temperature {temp}')
     try:
       if not model.lower().startswith('gpt'):
-        completion = client.run_query(model, gpt_message, temp, top_p, max_tokens, host, port, tkroot, tkdisplay )
+        completion = llm.run_query(model, gpt_message, max_tokens, temp, top_p, host, port, tkroot, tkdisplay )
         if completion is not None:
           response = completion
 
       else:
         stream= openai.ChatCompletion.create(
             model=model, messages=gpt_message, max_tokens=max_tokens, temperature=temp, top_p=1, stop='STOP', stream=True)
         response = ''
```

### Comparing `alphawave-0.2.6/tests/testOSClient.py` & `alphawave-0.2.7/tests/testOSClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.6/tests/testOpenAiClient.py` & `alphawave-0.2.7/tests/testOpenAiClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.6/tests/testSchema.py` & `alphawave-0.2.7/tests/testSchema.py`

 * *Files identical despite different names*


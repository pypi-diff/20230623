# Comparing `tmp/apollo-sdk-0.2.8.tar.gz` & `tmp/apollo-sdk-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apollo-sdk-0.2.8.tar", last modified: Sat May 27 07:48:49 2023, max compression
+gzip compressed data, was "apollo-sdk-0.2.9.tar", last modified: Mon May 29 06:40:52 2023, max compression
```

## Comparing `apollo-sdk-0.2.8.tar` & `apollo-sdk-0.2.9.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:48:49.372126 apollo-sdk-0.2.8/
--rw-r--r--   0 abpyguru   (501) staff       (20)     3793 2023-04-29 17:42:09.000000 apollo-sdk-0.2.8/LICENSE
--rw-r--r--   0 abpyguru   (501) staff       (20)     6096 2023-05-27 07:48:49.371992 apollo-sdk-0.2.8/PKG-INFO
--rw-r--r--   0 abpyguru   (501) staff       (20)     5635 2023-05-26 15:53:50.000000 apollo-sdk-0.2.8/README.md
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:48:49.364799 apollo-sdk-0.2.8/apollo/
--rw-r--r--   0 abpyguru   (501) staff       (20)     2250 2023-05-27 05:36:11.000000 apollo-sdk-0.2.8/apollo/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     5275 2023-05-27 05:36:10.000000 apollo-sdk-0.2.8/apollo/client.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:48:49.365069 apollo-sdk-0.2.8/apollo/connectors/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.8/apollo/connectors/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:48:49.365462 apollo-sdk-0.2.8/apollo/connectors/aws/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.8/apollo/connectors/aws/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:48:49.365687 apollo-sdk-0.2.8/apollo/connectors/google/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.8/apollo/connectors/google/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:48:49.365933 apollo-sdk-0.2.8/apollo/connectors/microsoft/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.8/apollo/connectors/microsoft/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:48:49.366848 apollo-sdk-0.2.8/apollo/connectors/openai/
--rw-r--r--   0 abpyguru   (501) staff       (20)      801 2023-05-26 16:56:46.000000 apollo-sdk-0.2.8/apollo/connectors/openai/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1023 2023-05-27 05:36:11.000000 apollo-sdk-0.2.8/apollo/connectors/openai/base.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     2574 2023-05-27 05:36:11.000000 apollo-sdk-0.2.8/apollo/connectors/openai/cloud.py
--rw-r--r--   0 abpyguru   (501) staff       (20)      956 2023-05-27 05:36:11.000000 apollo-sdk-0.2.8/apollo/connectors/openai/local.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1585 2023-05-26 17:12:47.000000 apollo-sdk-0.2.8/apollo/const.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:48:49.367004 apollo-sdk-0.2.8/apollo/database/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.8/apollo/database/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:48:49.367574 apollo-sdk-0.2.8/apollo/database/firebase/
--rw-r--r--   0 abpyguru   (501) staff       (20)      770 2023-04-30 05:02:07.000000 apollo-sdk-0.2.8/apollo/database/firebase/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1488 2023-04-30 05:02:07.000000 apollo-sdk-0.2.8/apollo/database/firebase/base.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     3494 2023-04-30 05:02:07.000000 apollo-sdk-0.2.8/apollo/database/firebase/cloud.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1438 2023-04-30 05:02:07.000000 apollo-sdk-0.2.8/apollo/database/firebase/local.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:48:49.367712 apollo-sdk-0.2.8/apollo/database/mongo/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.8/apollo/database/mongo/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:48:49.367852 apollo-sdk-0.2.8/apollo/database/mysql/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.8/apollo/database/mysql/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:48:49.367986 apollo-sdk-0.2.8/apollo/database/postgres/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.8/apollo/database/postgres/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:48:49.368642 apollo-sdk-0.2.8/apollo/database/supabase/
--rw-r--r--   0 abpyguru   (501) staff       (20)      770 2023-04-30 05:02:07.000000 apollo-sdk-0.2.8/apollo/database/supabase/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)      739 2023-04-30 05:02:07.000000 apollo-sdk-0.2.8/apollo/database/supabase/base.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1553 2023-04-30 05:02:07.000000 apollo-sdk-0.2.8/apollo/database/supabase/cloud.py
--rw-r--r--   0 abpyguru   (501) staff       (20)      810 2023-04-30 05:02:07.000000 apollo-sdk-0.2.8/apollo/database/supabase/local.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     4197 2023-04-30 05:02:07.000000 apollo-sdk-0.2.8/apollo/exceptions.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1578 2023-05-27 05:36:11.000000 apollo-sdk-0.2.8/apollo/manager.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:48:49.369416 apollo-sdk-0.2.8/apollo/plugins/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-05-26 17:55:34.000000 apollo-sdk-0.2.8/apollo/plugins/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     4796 2023-05-27 05:36:11.000000 apollo-sdk-0.2.8/apollo/plugins/utils.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     5165 2023-05-27 05:36:11.000000 apollo-sdk-0.2.8/apollo/plugins/validation.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1426 2023-05-27 05:36:10.000000 apollo-sdk-0.2.8/apollo/resource.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:48:49.369781 apollo-sdk-0.2.8/apollo/service/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.8/apollo/service/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:48:49.369940 apollo-sdk-0.2.8/apollo/service/graphql/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.8/apollo/service/graphql/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:48:49.370653 apollo-sdk-0.2.8/apollo/service/json/
--rw-r--r--   0 abpyguru   (501) staff       (20)      754 2023-04-30 05:02:07.000000 apollo-sdk-0.2.8/apollo/service/json/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)      947 2023-05-27 05:36:11.000000 apollo-sdk-0.2.8/apollo/service/json/base.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1272 2023-05-27 05:36:10.000000 apollo-sdk-0.2.8/apollo/service/json/cloud.py
--rw-r--r--   0 abpyguru   (501) staff       (20)      926 2023-05-27 05:36:10.000000 apollo-sdk-0.2.8/apollo/service/json/local.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:48:49.370968 apollo-sdk-0.2.8/apollo/tests/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.8/apollo/tests/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-27 07:48:49.371773 apollo-sdk-0.2.8/apollo_sdk.egg-info/
--rw-r--r--   0 abpyguru   (501) staff       (20)     6096 2023-05-27 07:48:49.000000 apollo-sdk-0.2.8/apollo_sdk.egg-info/PKG-INFO
--rw-r--r--   0 abpyguru   (501) staff       (20)     1322 2023-05-27 07:48:49.000000 apollo-sdk-0.2.8/apollo_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 abpyguru   (501) staff       (20)        1 2023-05-27 07:48:49.000000 apollo-sdk-0.2.8/apollo_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 abpyguru   (501) staff       (20)       47 2023-05-27 07:48:49.000000 apollo-sdk-0.2.8/apollo_sdk.egg-info/entry_points.txt
--rw-r--r--   0 abpyguru   (501) staff       (20)     1798 2023-05-27 07:48:49.000000 apollo-sdk-0.2.8/apollo_sdk.egg-info/requires.txt
--rw-r--r--   0 abpyguru   (501) staff       (20)       11 2023-05-27 07:48:49.000000 apollo-sdk-0.2.8/apollo_sdk.egg-info/top_level.txt
--rwxr-xr-x   0 abpyguru   (501) staff       (20)      176 2023-05-27 06:38:58.000000 apollo-sdk-0.2.8/cli.py
--rw-r--r--   0 abpyguru   (501) staff       (20)       38 2023-05-27 07:48:49.372169 apollo-sdk-0.2.8/setup.cfg
--rw-r--r--   0 abpyguru   (501) staff       (20)     1592 2023-05-27 07:46:44.000000 apollo-sdk-0.2.8/setup.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-29 06:40:52.737349 apollo-sdk-0.2.9/
+-rw-r--r--   0 abpyguru   (501) staff       (20)     3793 2023-04-29 17:42:09.000000 apollo-sdk-0.2.9/LICENSE
+-rw-r--r--   0 abpyguru   (501) staff       (20)    13193 2023-05-29 06:40:52.737111 apollo-sdk-0.2.9/PKG-INFO
+-rw-r--r--   0 abpyguru   (501) staff       (20)    12732 2023-05-29 06:40:26.000000 apollo-sdk-0.2.9/README.md
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-29 06:40:52.726639 apollo-sdk-0.2.9/apollo/
+-rw-r--r--   0 abpyguru   (501) staff       (20)     2250 2023-05-29 03:44:56.000000 apollo-sdk-0.2.9/apollo/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     5364 2023-05-29 06:19:57.000000 apollo-sdk-0.2.9/apollo/client.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-29 06:40:52.726901 apollo-sdk-0.2.9/apollo/connectors/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.9/apollo/connectors/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-29 06:40:52.727161 apollo-sdk-0.2.9/apollo/connectors/aws/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.9/apollo/connectors/aws/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-29 06:40:52.727463 apollo-sdk-0.2.9/apollo/connectors/google/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.9/apollo/connectors/google/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-29 06:40:52.727696 apollo-sdk-0.2.9/apollo/connectors/microsoft/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.9/apollo/connectors/microsoft/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-29 06:40:52.728835 apollo-sdk-0.2.9/apollo/connectors/openai/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      801 2023-05-29 03:44:56.000000 apollo-sdk-0.2.9/apollo/connectors/openai/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1023 2023-05-29 03:44:56.000000 apollo-sdk-0.2.9/apollo/connectors/openai/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     2574 2023-05-29 03:44:56.000000 apollo-sdk-0.2.9/apollo/connectors/openai/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      956 2023-05-29 03:44:56.000000 apollo-sdk-0.2.9/apollo/connectors/openai/local.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1585 2023-05-29 03:44:56.000000 apollo-sdk-0.2.9/apollo/const.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-29 06:40:52.729032 apollo-sdk-0.2.9/apollo/database/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.9/apollo/database/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-29 06:40:52.729844 apollo-sdk-0.2.9/apollo/database/firebase/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      770 2023-04-30 05:02:07.000000 apollo-sdk-0.2.9/apollo/database/firebase/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1488 2023-04-30 05:02:07.000000 apollo-sdk-0.2.9/apollo/database/firebase/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     3494 2023-04-30 05:02:07.000000 apollo-sdk-0.2.9/apollo/database/firebase/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1438 2023-04-30 05:02:07.000000 apollo-sdk-0.2.9/apollo/database/firebase/local.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-29 06:40:52.730235 apollo-sdk-0.2.9/apollo/database/mongo/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.9/apollo/database/mongo/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-29 06:40:52.730566 apollo-sdk-0.2.9/apollo/database/mysql/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.9/apollo/database/mysql/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-29 06:40:52.730742 apollo-sdk-0.2.9/apollo/database/postgres/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.9/apollo/database/postgres/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-29 06:40:52.731619 apollo-sdk-0.2.9/apollo/database/supabase/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      770 2023-04-30 05:02:07.000000 apollo-sdk-0.2.9/apollo/database/supabase/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      739 2023-04-30 05:02:07.000000 apollo-sdk-0.2.9/apollo/database/supabase/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1553 2023-04-30 05:02:07.000000 apollo-sdk-0.2.9/apollo/database/supabase/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      810 2023-04-30 05:02:07.000000 apollo-sdk-0.2.9/apollo/database/supabase/local.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     4197 2023-04-30 05:02:07.000000 apollo-sdk-0.2.9/apollo/exceptions.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1578 2023-05-29 03:44:56.000000 apollo-sdk-0.2.9/apollo/manager.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-29 06:40:52.732531 apollo-sdk-0.2.9/apollo/plugins/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-05-29 03:44:56.000000 apollo-sdk-0.2.9/apollo/plugins/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     4812 2023-05-29 03:45:17.000000 apollo-sdk-0.2.9/apollo/plugins/utils.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     7284 2023-05-29 06:19:57.000000 apollo-sdk-0.2.9/apollo/plugins/validation.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1426 2023-05-29 03:44:56.000000 apollo-sdk-0.2.9/apollo/resource.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-29 06:40:52.732823 apollo-sdk-0.2.9/apollo/service/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.9/apollo/service/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-29 06:40:52.733085 apollo-sdk-0.2.9/apollo/service/graphql/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.9/apollo/service/graphql/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-29 06:40:52.734699 apollo-sdk-0.2.9/apollo/service/json/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      754 2023-04-30 05:02:07.000000 apollo-sdk-0.2.9/apollo/service/json/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      947 2023-05-29 03:44:56.000000 apollo-sdk-0.2.9/apollo/service/json/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1300 2023-05-29 06:19:57.000000 apollo-sdk-0.2.9/apollo/service/json/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      926 2023-05-29 03:44:56.000000 apollo-sdk-0.2.9/apollo/service/json/local.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-29 06:40:52.735151 apollo-sdk-0.2.9/apollo/tests/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.2.9/apollo/tests/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-29 06:40:52.736837 apollo-sdk-0.2.9/apollo_sdk.egg-info/
+-rw-r--r--   0 abpyguru   (501) staff       (20)    13193 2023-05-29 06:40:52.000000 apollo-sdk-0.2.9/apollo_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1322 2023-05-29 06:40:52.000000 apollo-sdk-0.2.9/apollo_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 abpyguru   (501) staff       (20)        1 2023-05-29 06:40:52.000000 apollo-sdk-0.2.9/apollo_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 abpyguru   (501) staff       (20)       47 2023-05-29 06:40:52.000000 apollo-sdk-0.2.9/apollo_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1798 2023-05-29 06:40:52.000000 apollo-sdk-0.2.9/apollo_sdk.egg-info/requires.txt
+-rw-r--r--   0 abpyguru   (501) staff       (20)       11 2023-05-29 06:40:52.000000 apollo-sdk-0.2.9/apollo_sdk.egg-info/top_level.txt
+-rwxr-xr-x   0 abpyguru   (501) staff       (20)      826 2023-05-29 03:45:17.000000 apollo-sdk-0.2.9/cli.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)       38 2023-05-29 06:40:52.737403 apollo-sdk-0.2.9/setup.cfg
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1587 2023-05-29 06:40:38.000000 apollo-sdk-0.2.9/setup.py
```

### Comparing `apollo-sdk-0.2.8/LICENSE` & `apollo-sdk-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.8/apollo/__init__.py` & `apollo-sdk-0.2.9/apollo/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.8/apollo/client.py` & `apollo-sdk-0.2.9/apollo/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         try:
             response = cls.psql_curs.execute(cls._context["all_tables"])
         except Exception as err:
             raise ExecutionError(err)
 
         return list(itertools.chain.from_iterable(response))
 
-    # # execute a sql query
+    # execute a sql query
     @classmethod
     def query(cls, query_type, table, col):
         """
         Query your external resource using Apollo
 
         Args:
         query_type (str): The sort order for your query
@@ -102,25 +102,27 @@
             1. Apollo.fetch_tables()
             2. Apollo.query([desc/asc], [table], [column])
         """
         cls.psql_curs = cls._manager.connect_to_prefix(db_url)
         return "Syncing data with Apollo"
 
     @classmethod
-    def use(cls, provider, token=None, *args, **kwargs):
+    def use(cls, provider, token="Beta_token123", *args, **kwargs):
         provider = provider.lower()
         # TODO: Move apollo connection to its own
         # method like openai once integrated
         if provider == "apollo":
             cls.model = "Apollo"
             if token:
                 cls._auth_token = token
                 print(f"Connected to {provider} provider, using Safety model")
             else:
-                print("Please set a auth token")
+                print(
+                    "Please set a auth token or use the sandbox: Apollo.sandbox_test()"
+                )
         elif provider.startswith("openai:"):
             cls.model = "OpenAI"
             cls._provider_path = provider
             return cls._openai_manager.load_openai_provider(cls._provider_path)
         else:
             return f"Provider {provider} not found"
```

### Comparing `apollo-sdk-0.2.8/apollo/connectors/__init__.py` & `apollo-sdk-0.2.9/apollo/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.8/apollo/connectors/aws/__init__.py` & `apollo-sdk-0.2.9/apollo/connectors/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.8/apollo/connectors/google/__init__.py` & `apollo-sdk-0.2.9/apollo/connectors/google/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.8/apollo/connectors/microsoft/__init__.py` & `apollo-sdk-0.2.9/apollo/connectors/microsoft/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.8/apollo/connectors/openai/__init__.py` & `apollo-sdk-0.2.9/apollo/connectors/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.8/apollo/connectors/openai/base.py` & `apollo-sdk-0.2.9/apollo/connectors/openai/base.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.8/apollo/connectors/openai/cloud.py` & `apollo-sdk-0.2.9/apollo/connectors/openai/cloud.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.8/apollo/connectors/openai/local.py` & `apollo-sdk-0.2.9/apollo/connectors/openai/local.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.8/apollo/const.py` & `apollo-sdk-0.2.9/apollo/const.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.8/apollo/database/__init__.py` & `apollo-sdk-0.2.9/apollo/database/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.8/apollo/database/firebase/__init__.py` & `apollo-sdk-0.2.9/apollo/database/firebase/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.8/apollo/database/firebase/base.py` & `apollo-sdk-0.2.9/apollo/database/firebase/base.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.8/apollo/database/firebase/cloud.py` & `apollo-sdk-0.2.9/apollo/database/firebase/cloud.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.8/apollo/database/firebase/local.py` & `apollo-sdk-0.2.9/apollo/database/firebase/local.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.8/apollo/database/mongo/__init__.py` & `apollo-sdk-0.2.9/apollo/database/mongo/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.8/apollo/database/mysql/__init__.py` & `apollo-sdk-0.2.9/apollo/database/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.8/apollo/database/postgres/__init__.py` & `apollo-sdk-0.2.9/apollo/database/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.8/apollo/database/supabase/__init__.py` & `apollo-sdk-0.2.9/apollo/database/supabase/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.8/apollo/database/supabase/base.py` & `apollo-sdk-0.2.9/apollo/database/supabase/base.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.8/apollo/database/supabase/cloud.py` & `apollo-sdk-0.2.9/apollo/database/supabase/cloud.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.8/apollo/database/supabase/local.py` & `apollo-sdk-0.2.9/apollo/database/supabase/local.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.8/apollo/exceptions.py` & `apollo-sdk-0.2.9/apollo/exceptions.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.8/apollo/manager.py` & `apollo-sdk-0.2.9/apollo/manager.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.8/apollo/plugins/__init__.py` & `apollo-sdk-0.2.9/apollo/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.8/apollo/plugins/utils.py` & `apollo-sdk-0.2.9/apollo/plugins/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,18 +28,18 @@
         with open(p, "r") as f:
             content = f.read()
             items = content.split("---")
             prompts = list(item.strip() for item in items if item.strip())
     return prompts
 
 
-def read_vars(path):
+def read_vars(path, delimiter):
     variables = []
     with open(path, "r") as f:
-        reader = csv.reader(f, delimiter="\t")
+        reader = csv.reader(f, delimiter=delimiter)
         header = next(reader)  # skip the header elements
         for row in reader:
             if len(row) == len(
                 header
             ):  # Check if the row has the same number of elements as the header
                 variables.append(dict(zip(header, row)))
     return variables
```

### Comparing `apollo-sdk-0.2.8/apollo/plugins/validation.py` & `apollo-sdk-0.2.9/apollo/plugins/validation.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 import io
 import pathlib
 import json
+import csv
+import os
 
 from tabulate import tabulate
 from termcolor import colored, cprint
 from argparse import ArgumentParser, ArgumentDefaultsHelpFormatter
 
 from .utils import read_vars, read_prompts, evaluate, write_output
 from apollo.manager import OpenAIConnectionManager
@@ -59,18 +61,68 @@
         )
         self.parser.add_argument(
             "-c",
             "--config",
             type=pathlib.Path,
             help="Path to configuration file",
         )
+        self.parser.add_argument(
+            "-d",
+            "--delimiter",
+            type=pathlib.Path,
+            help="Delimiter set in the vars file, defaults to [,]",
+        )
+        self.parser.add_argument(
+            "--init",
+            action="store_const",
+            const="init",
+            default=None,
+            help="Initialize environment with configuration scripts",
+        )
 
         self.args = self.parser.parse_args()
         self.provider = OpenAIConnectionManager()
 
+    def init(self):
+        config = {
+            "provider": ["openai:completion"],
+            "vars": "/vars.csv",
+            "prompts": "/prompts.txt",
+        }
+        vars = [
+            ["name", "question"],
+            ["Tyler", "Can you help me find a specific product on your website?"],
+            ["Jhon", "Do you have any promotions or discounts currently available?"],
+            ["David", "What are your shipping and return policies?"],
+            [
+                "Adrian",
+                "Can you provide more information about the product specifications or features?",
+            ],
+            [
+                "User",
+                "Can you recommend products that are similar to what I've been looking at?",
+            ],
+        ]
+        prompts = [
+            'Youre a chat assistant for a company. Answer this users question: {{name}}: "{{question}}"',
+            'Youre a smart, bubbly chat assistant for a Trust & Safety team. Answer this users question: {{name}}: "{{question}}"',
+        ]
+
+        with open(os.path.join(os.getcwd(), f"prompts.txt"), "w") as f:
+            f.write("\n--- \n".join(prompts))
+
+        with open(
+            os.path.join(os.getcwd(), f"vars.csv"), mode="w", newline=""
+        ) as vars_file:
+            writer = csv.writer(vars_file)
+            writer.writerows(vars)
+
+        with open(os.path.join(os.getcwd(), f"config.json"), "w") as f:
+            json.dump(config, f)
+
     def eval(self):
         config_path = self.args.config
         config = {}
         if config_path:
             ext = pathlib.Path(config_path).suffix
             if ext == ".json":
                 with io.open(config_path, "r", encoding="utf-8") as f:
@@ -78,17 +130,21 @@
             # elif ext == '.py': # TODO: support yaml config files
             #     config = importlib.import_module(config_path)
             else:
                 raise Error(f"Unsupported configuration file format: {ext}")
 
         vars = []
         if self.args.vars:
-            vars = read_vars(self.args.vars)
+            vars = read_vars(
+                self.args.vars,
+                delimiter=self.args.delimiter if self.args.delimiter else ",",
+            )
 
         providers = [self.provider.load_openai_provider(p) for p in self.args.provider]
+
         options = {
             "prompts": read_prompts(self.args.prompt),
             "vars": vars,  # NOTE: I think this is suppowed to be output not a path
             "providers": providers,
             **config,
         }
 
@@ -141,7 +197,13 @@
                 tablefmt="rounded_grid",
                 maxcolwidths=column_width,
             )
             print(table)
 
         print_yellow = lambda x: cprint(x, "yellow")
         print_yellow(f'Evaluation complete: {json.dumps(summary["stats"], indent=4)}')
+
+    def setup(self):
+        if self.args.init == "init":
+            self.init()
+        else:
+            self.eval()
```

### Comparing `apollo-sdk-0.2.8/apollo/resource.py` & `apollo-sdk-0.2.9/apollo/resource.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.8/apollo/service/__init__.py` & `apollo-sdk-0.2.9/apollo/service/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.8/apollo/service/graphql/__init__.py` & `apollo-sdk-0.2.9/apollo/service/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.8/apollo/service/json/__init__.py` & `apollo-sdk-0.2.9/apollo/service/json/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.8/apollo/service/json/base.py` & `apollo-sdk-0.2.9/apollo/service/json/base.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.8/apollo/service/json/cloud.py` & `apollo-sdk-0.2.9/apollo/service/json/cloud.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,13 +29,13 @@
 
     @staticmethod
     def call_api(self):
         return None
 
     def make_https_request(self, body):
         response = requests.post(
-            "https://api.apolloapi.io/api/v1/apollo/",
-            headers={"Authorization": f"Token {self.api_key}"},
+            "https://api.apolloapi.io/api/v1/sandbox/",  # Access to sandbox env
+            # headers={"Authorization": f"Token {self.api_key}"},
             json=body,
             timeout=10,
         )
         return response.json()
```

### Comparing `apollo-sdk-0.2.8/apollo/service/json/local.py` & `apollo-sdk-0.2.9/apollo/service/json/local.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.8/apollo/tests/__init__.py` & `apollo-sdk-0.2.9/apollo/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.8/apollo_sdk.egg-info/SOURCES.txt` & `apollo-sdk-0.2.9/apollo_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.8/apollo_sdk.egg-info/requires.txt` & `apollo-sdk-0.2.9/apollo_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.2.8/setup.py` & `apollo-sdk-0.2.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,31 +14,31 @@
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
-    
+
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setup(
     name="apollo-sdk",
-    version="0.2.8",
+    version="0.2.9",
     description="Build automated decision making workflows by aggregating your AI models and data into one api.",
     author="Apollo API",
     author_email="adrbrownx@gmail.com",
     packages=find_packages(),
-    py_modules = ['cli', 'apollo'],
+    py_modules=["cli", "apollo"],
     url="https://github.com/apolloapi/apolloapi",
     license="Elastic License v2",
     classifiers=[
         "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3"
+        "Programming Language :: Python :: 3",
     ],
     platforms=["Any"],
     install_requires=requirements,
     long_description_content_type="text/markdown",
     long_description=long_description,
     entry_points={"console_scripts": ["apollo-sdk=cli:run_console"]},
 )
```


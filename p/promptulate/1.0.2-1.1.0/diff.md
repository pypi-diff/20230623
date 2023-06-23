# Comparing `tmp/promptulate-1.0.2.tar.gz` & `tmp/promptulate-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptulate-1.0.2.tar", last modified: Sun May 14 03:18:49 2023, max compression
+gzip compressed data, was "promptulate-1.1.0.tar", last modified: Fri Jun 23 10:54:56 2023, max compression
```

## Comparing `promptulate-1.0.2.tar` & `promptulate-1.1.0.tar`

### file list

```diff
@@ -1,57 +1,72 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 03:18:49.383516 promptulate-1.0.2/
--rw-rw-rw-   0        0        0    11558 2023-05-13 17:09:36.000000 promptulate-1.0.2/LICENSE
--rw-rw-rw-   0        0        0    15599 2023-05-14 03:18:49.382516 promptulate-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    14665 2023-05-13 17:09:36.000000 promptulate-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-14 03:18:49.289442 promptulate-1.0.2/promptulate/
--rw-rw-rw-   0        0        0     1199 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 03:18:49.310420 promptulate-1.0.2/promptulate/command/
--rw-rw-rw-   0        0        0      127 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/command/__init__.py
--rw-rw-rw-   0        0        0     1673 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/command/chat.py
--rw-rw-rw-   0        0        0     2655 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/config.py
-drwxrwxrwx   0        0        0        0 2023-05-14 03:18:49.317354 promptulate-1.0.2/promptulate/frameworks/
--rw-rw-rw-   0        0        0      866 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/frameworks/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 03:18:49.323350 promptulate-1.0.2/promptulate/frameworks/base/
--rw-rw-rw-   0        0        0      878 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/frameworks/base/__init__.py
--rw-rw-rw-   0        0        0     3367 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/frameworks/base/conversation.py
--rw-rw-rw-   0        0        0     1776 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/frameworks/prompt.py
-drwxrwxrwx   0        0        0        0 2023-05-14 03:18:49.326357 promptulate-1.0.2/promptulate/frameworks/react/
--rw-rw-rw-   0        0        0      769 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/frameworks/react/__init__.py
--rw-rw-rw-   0        0        0     1074 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/frameworks/schema.py
-drwxrwxrwx   0        0        0        0 2023-05-14 03:18:49.328355 promptulate-1.0.2/promptulate/frameworks/self_ask/
--rw-rw-rw-   0        0        0      769 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/frameworks/self_ask/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 03:18:49.336380 promptulate-1.0.2/promptulate/llms/
--rw-rw-rw-   0        0        0      848 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/llms/__init__.py
--rw-rw-rw-   0        0        0     1504 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/llms/base.py
--rw-rw-rw-   0        0        0     3828 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/llms/openai.py
-drwxrwxrwx   0        0        0        0 2023-05-14 03:18:49.347376 promptulate-1.0.2/promptulate/memory/
--rw-rw-rw-   0        0        0      963 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/memory/__init__.py
--rw-rw-rw-   0        0        0     1721 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/memory/base.py
--rw-rw-rw-   0        0        0     1773 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/memory/buffer.py
--rw-rw-rw-   0        0        0     1894 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/memory/local_cache.py
-drwxrwxrwx   0        0        0        0 2023-05-14 03:18:49.355409 promptulate-1.0.2/promptulate/preset_roles/
--rw-rw-rw-   0        0        0      925 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/preset_roles/__init__.py
--rw-rw-rw-   0        0        0     3264 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/preset_roles/prompt.py
--rw-rw-rw-   0        0        0     5331 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/preset_roles/roles.py
-drwxrwxrwx   0        0        0        0 2023-05-14 03:18:49.361407 promptulate-1.0.2/promptulate/provider/
--rw-rw-rw-   0        0        0     1059 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/provider/__init__.py
--rw-rw-rw-   0        0        0     5477 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/provider/mixins.py
--rw-rw-rw-   0        0        0     5982 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/schema.py
--rw-rw-rw-   0        0        0      881 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/tips.py
-drwxrwxrwx   0        0        0        0 2023-05-14 03:18:49.365411 promptulate-1.0.2/promptulate/tools/
--rw-rw-rw-   0        0        0      773 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/tools/__init__.py
--rw-rw-rw-   0        0        0      769 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/tools/duckduckgo.py
-drwxrwxrwx   0        0        0        0 2023-05-14 03:18:49.379407 promptulate-1.0.2/promptulate/utils/
--rw-rw-rw-   0        0        0     1304 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/utils/__init__.py
--rw-rw-rw-   0        0        0     2145 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/utils/_utils.py
--rw-rw-rw-   0        0        0     1962 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/utils/logger.py
--rw-rw-rw-   0        0        0     1626 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/utils/proxy.py
--rw-rw-rw-   0        0        0      656 2023-05-13 17:09:36.000000 promptulate-1.0.2/promptulate/utils/singleton.py
-drwxrwxrwx   0        0        0        0 2023-05-14 03:18:49.305426 promptulate-1.0.2/promptulate.egg-info/
--rw-rw-rw-   0        0        0    15599 2023-05-14 03:18:49.000000 promptulate-1.0.2/promptulate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1234 2023-05-14 03:18:49.000000 promptulate-1.0.2/promptulate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 03:18:49.000000 promptulate-1.0.2/promptulate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-05-14 03:18:49.000000 promptulate-1.0.2/promptulate.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2023-05-14 03:18:49.000000 promptulate-1.0.2/promptulate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-14 03:18:49.000000 promptulate-1.0.2/promptulate.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-14 03:18:49.383516 promptulate-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     2041 2023-05-14 03:17:30.000000 promptulate-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:54:56.457353 promptulate-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-23 10:54:43.000000 promptulate-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20901 2023-06-23 10:54:56.457353 promptulate-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19969 2023-06-23 10:54:43.000000 promptulate-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:54:56.449353 promptulate-1.1.0/promptulate/
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:54:56.449353 promptulate-1.1.0/promptulate/command/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/command/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:54:56.453353 promptulate-1.1.0/promptulate/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/frameworks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:54:56.453353 promptulate-1.1.0/promptulate/frameworks/conversation/
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/frameworks/conversation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/frameworks/conversation/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/frameworks/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:54:56.453353 promptulate-1.1.0/promptulate/frameworks/react/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/frameworks/react/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/frameworks/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:54:56.453353 promptulate-1.1.0/promptulate/frameworks/self_ask/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/frameworks/self_ask/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:54:56.453353 promptulate-1.1.0/promptulate/llms/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/llms/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/llms/openai.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:54:56.453353 promptulate-1.1.0/promptulate/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/memory/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/memory/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/memory/local_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:54:56.453353 promptulate-1.1.0/promptulate/preset_roles/
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/preset_roles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/preset_roles/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/preset_roles/roles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:54:56.453353 promptulate-1.1.0/promptulate/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/provider/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/tips.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:54:56.453353 promptulate-1.1.0/promptulate/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:54:56.453353 promptulate-1.1.0/promptulate/tools/arxiv/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/tools/arxiv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/tools/arxiv/api_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/tools/arxiv/toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/tools/arxiv/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/tools/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:54:56.453353 promptulate-1.1.0/promptulate/tools/duckduckgo/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/tools/duckduckgo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/tools/duckduckgo/api_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/tools/duckduckgo/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/tools/duckduckgo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:54:56.457353 promptulate-1.1.0/promptulate/tools/python_repl/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/tools/python_repl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/tools/python_repl/api_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/tools/python_repl/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:54:56.457353 promptulate-1.1.0/promptulate/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/utils/core_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/utils/openai_key_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/utils/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-23 10:54:43.000000 promptulate-1.1.0/promptulate/utils/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:54:56.449353 promptulate-1.1.0/promptulate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20901 2023-06-23 10:54:56.000000 promptulate-1.1.0/promptulate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-23 10:54:56.000000 promptulate-1.1.0/promptulate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 10:54:56.000000 promptulate-1.1.0/promptulate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-23 10:54:56.000000 promptulate-1.1.0/promptulate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-23 10:54:56.000000 promptulate-1.1.0/promptulate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-23 10:54:56.000000 promptulate-1.1.0/promptulate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 10:54:56.457353 promptulate-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-06-23 10:54:43.000000 promptulate-1.1.0/setup.py
```

### Comparing `promptulate-1.0.2/LICENSE` & `promptulate-1.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `promptulate-1.0.2/PKG-INFO` & `promptulate-1.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,364 +1,463 @@
-Metadata-Version: 2.1
-Name: promptulate
-Version: 1.0.2
-Summary: A powerful LLM Prompt Layer frameworks
-Home-page: https://github.com/Undertone0809/promptulate
-Author: Zeeland
-Author-email: zeeland@foxmail.com
-License: Apache 2.0
-Keywords: promptulate,prompt-me,prompt,chatgpt,gpt,chatbot,llm
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<h1 align="center">
-    Promptulate
-</h1>
-
-
-<p align="center">
-    <a target="_blank" href="">
-        <img src="https://img.shields.io/github/license/Undertone0809/promptulate.svg?style=flat-square" />
-    </a>
-    <a target="_blank" href=''>
-        <img src="https://img.shields.io/github/release/Undertone0809/promptulate/all.svg?style=flat-square"/>
-    </a>
-    <a target="_blank" href=''>
-        <img src="https://bestpractices.coreinfrastructure.org/projects/3018/badge"/>
-   </a>
-</p>
-
-<p align="center">
-  <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/Snipaste_2023-05-13_17-37-23.png"/>
-</p>
-
-
-
-`promptulate` 是一个专为 Prompt Engineer设计LLM Prompt Layer框架，支持连续对话、对话保存、对话内容与标题总结、角色预设、使用外部工具等功能，开箱即用。
-通过 `promptulate`，你可以轻松构建起属于自己的LLM应用程序。
-
-本项目重构重构重构了两次，在本人深度阅读`langchain, Auto-GPT, django, django-rest-framework, gpt_academic...`
-等大牛项目的源码之后，学习它们的架构、代码设计思路等内容，最终有了现在的版本，相较于之前的老版本`prompt-me`，`promptulate`
-重新构建了 `llms, message, memory, framework, preset_roles, tools, provider`等模块，将`prompt`
-的各个流程全部组件化，便有了现在的`promptualte`框架，但是工作量很大，还在不断地完善细节中，欢迎大家的参与。
-
-# 特性
-
-- 大语言模型支持：支持不同类型的大语言模型的扩展接口（当前暂时只支持GPT）
-- 角色预设：提供预设角色，以不同的角度调用GPT
-- 内置API代理，不用科学上网也可以直接使用
-- 接口代理：支持调用ChatGPT API官方接口或自治代理
-- 长对话模式：支持长对话聊天，支持多种方式的对话持久化
-- 数据导出：支持markdowm等格式的对话导出
-- 对话总结：提供API式的对话总结、翻译、标题生成
-- 高级抽象，支持插件扩展、存储扩展、大语言模型扩展
-
-# 基础架构
-
-在看了当前这么多`prompt-engineering`之后，本人的架构设计思想在`langchain, Auto-GPT`
-之上进行不断改进，构建出了一套属于`promptualte`的LLM Prompt Layer框架。`promptulate` 由以下几部分组成：
-
-- Agent 更高级的执行器，负责复杂任务的调度和分发
-- framework 框架层，实现不同类型的prompt框架，包括最基础的`Conversation`模型，还有`self-ask`和`ReAct`等模型正在火速开发中
-- llm 大语言模型，负责生成回答，可以支持不同类型的大语言模型
-- memory 负责对话的存储，支持不同的存储方式及其扩展，如文件存储、数据库存储等，相关扩展正在开发中
-- tools 提供外部工具扩展调用，如搜索引擎、计算器等
-- preset roles 提供预设角色，进行定制化对话
-- provider 为framework和agent提供tools和其他细粒度能力的集成
-
-# 快速上手
-
-```shell script
-pip install -U promptulate  
-```
-
-## 基本使用
-
-> 后面的文档全部使用`OPENAI GPT3.5`进行测试
-
-在使用`promptulate`之前，你需要先导入你的`OPENAI_API_KEY`
-
-```python
-import os
-
-os.environ['OPENAI_API_KEY'] = "your-key"
-```
-
-在你第一次使用的时候，需要使用`os.environ["OPENAI_API_KEY"]` 导入"OPENAI_API_KEY"
-的环境变量，但是在第一运行之后`promptulate`会进行缓存，即后面再运行就不需要再导入key了。如果你的key过期了，可以把`cache`
-文件给删除掉，Windows的`cache`在当前目录下，linux的`cache`在`/tmp`下。
-
-### LLM
-
-`promptulate`的架构设计可以轻松兼容不同的大语言模型扩展，在`promptulate`中，llm负责最基本的内容生成部分，因此为最基础的组件。下面展示一个OpenAI的示例：
-
-```python
-from promptulate.llms import OpenAI
-
-llm = OpenAI()
-llm("你知道鸡哥的《只因你太美》？")
-```
-
-```text
-'是的，鸡哥的《只因你太美》是这几年非常流行的一首歌曲。'
-```
-
-### proxy
-
-我想你可能遇到了无法访问的小问题，It's OK, `promptulate` 提供了三种访问OpenAI的方式，分别是
-
-- `off` 默认的访问方式，不开代理
-- `custom` 自定义代理方式
-- `promptulate` promptulate提供的免费代理服务器
-
-`promptulate` 提供了免费的代理服务器，感谢 [ayaka14732](https://github.com/ayaka14732/)
-，你可以在不用科学上网的情况下直接调用OpenAI的相关接口，下面是代理的设置方式：
-
-```python
-from promptulate.llms import OpenAI
-from promptulate.utils import set_proxy_mode
-
-llm = OpenAI()
-llm("你知道鸡哥的《只因你太美》？")
-
-
-def set_free_proxy():
-    set_proxy_mode("promptulate")
-
-
-def set_custom_proxy():
-    proxies = {'http': 'http://127.0.0.1:7890'}
-    set_proxy_mode("custom", proxies=proxies)
-
-
-def turn_off_proxy():
-    set_proxy_mode("off")
-
-
-def main():
-    set_free_proxy()
-    llm = OpenAI()
-    llm("你知道鸡哥的《只因你太美》？")
-
-    
-if __name__ == '__main__':
-    main()
-```
-
-> 和OPENAI_API_KEY一样，关于代理的配置我也设置了缓存，这意味着你只需要配置一次代理即可(我也太聪明了吧)。事实上`promptulate`
-> 提供了关闭全局配置项缓存的功能，但默认开启，不推荐关闭，所以我不告诉你怎么关闭~
-
-### Conversation
-
-`Conversation` 是`framework`中最基础的组件，其支持prompt生成、上下文对话、对话存储、角色预设的基本功能，此外，`provider`
-为其提供了语言翻译、markdown数据导出、对话总结、标题总结等扩展功能。
-
-接下来，我们先从对基础的对话开始，使用`Conversation`可以开始一段对话，使用其`predict()`函数可以生成回答。
-
-```python
-from promptulate import Conversation
-
-conversation = Conversation()
-conversation.predict("你知道鸡哥的《只因你太美》吗？")
-```
-
-```text
-'是的，鸡哥的《只因你太美》是这几年非常流行的一首歌曲。'
-```
-
-`Conversation`默认使用`OpenAI GPT3.5`作为LLM，当然，因为其架构设计，`Conversation`
-还可以轻松扩展其他类型的llm（当前暂时只开发了OpenAI，其他大语言模型的扩展正在火速开发中，当然如果你有自己想接入的大语言模型，欢迎你的pr！）
-
-下面是一个更复杂的示例，展示了使用OpenAI作为大语言模型进行对话，使用本地文件进行存储，进行文章总结与标题总结的功能。
-
-```python
-from promptulate import Conversation
-from promptulate.memory import LocalCacheChatMemory
-from promptulate.llms import OpenAI
-
-
-def main():
-    memory = LocalCacheChatMemory()
-    llm = OpenAI(model="gpt-3.5-turbo", temperature=0.9, top_p=1, stream=False, presence_penalty=0, n=1)
-    conversation = Conversation(llm=llm, memory=memory)
-    ret = conversation.predict("你知道鸡哥的著作《只因你太美》吗？")
-    print(f"[predict] {ret}")
-    ret = conversation.predict_by_translate("你知道鸡哥会什么技能吗？", country='America')
-    print(f"[translate output] {ret}")
-    ret = conversation.summary_content()
-    print(f"[summary content] {ret}")
-    ret = conversation.summary_topic()
-    print(f"[summary topic] {ret}")
-    ret = conversation.export_message_to_markdown(output_type="file", file_path="output.md")
-    print(f"[export markdown] {ret}")
-
-
-if __name__ == '__main__':
-    main()
-
-```
-
-```text
-[predict] 是的，我知道《只因你太美》这本书，是中国知名作家鸡肋（江南）所著的一篇言情小说。这本小说讲述了一个富家千金与一个贫穷男孩之间的爱情故事，情节曲折动人，深受读者喜爱。该小说在出版后得到了很高的评价和反响，并被改编成电影和电视剧等多种形式进行推广。
-[translate output] I'm sorry, I cannot determine what you mean by "鸡哥" or what skills they may possess without additional context. Can you please provide more information or clarify your question?
-[summary content] 在之前的对话中，用户询问我是否知道鸡哥的著作《只因你太美》。我回答了肯定的，解释了该小说的情节大致概括和其受欢迎的原因。我也提到了该小说的广泛影响，包括被改编成电影和电视剧等多种形式进行推广。
-[summary topic] 鸡哥的小说。
-```
-
-> 咱就是说季皮提老师不懂鸡哥-.-
-
-上面的示例中，我们使用
-
-- `LocalCacheChatMemory()`进行聊天记录的本地化文件存储，文件存储形式默认是以json的形式进行存储的，保存在`cache`中。
-- `OpenAI(model="gpt-3.5-turbo", temperature=0.9, top_p=1, stream=False, presence_penalty=0, n=1)`
-  进行初始化一个大模型，里面是OpenAI需要传入的一些参数，具体可以查看[https://platform.openai.com/docs/api-reference/chat/create](https://platform.openai.com/docs/api-reference/chat/create)
-  查看具体含义，这里不做详细讲解，如果你不想理会这些参数，你也可以直接`llm = OpenAI()`就好啦，默认使用`gpt-3.5-turbo`
-  作为大语言模型，其他参数使用默认的就好了。
-- `conversation.predict_by_translate("你知道鸡哥会什么技能吗？", country='America')`
-  这个功能为使用特定语言进行预测，`provider`为其提供了`TranslatorMixin`，让`Conversation`
-  得以拥有此功能。对于这个方法，你只需要传入prompt和你需要转换的语言的国家名称就好了。
-- `conversation.summary_content()`这个函数可以直接总结上面的对话内容。
-- `conversation.summary_topic()` 这个函数可以直接总结上面的对话，并提供一个标题。
-- `conversation.export_message_to_markdown(output_type="file", file_path="output.md")`
-  这个函数可以将对话记录导出为markdown文件，如果`output_type="text"`，则只返回markdown对话的内容。
-
-`provider`为`Conversation`提供了 `SummarizerMixin, TranslatorMixin, DeriveHistoryMessageMixin`
-，让其拥有了总结对话、总结标题、翻译、markdown导出的能力，provider提供的函数中一般都提供了一个`enable_embed_message`
-的参数，这个参数的意思是：是否将本次对话保存进历史对话中，下面我们来看一个demo。
-
-```python
-from promptulate import Conversation
-
-conversation = Conversation()
-conversation.predict_by_translate("你知道鸡哥会什么技能吗？", country='America', enable_embed_message=True)
-```
-
-如果你设置了`enable_embed_message=True`, 那么这一次的predict将保存进历史对话中，provider提供的函数默认是不会将预测结果存入对话中的哦，这一点需要注意一下。
-
-### 角色预设
-
-你可以为`framework`提供一些特定的角色，让其可以处理特殊任务，如linux终端，思维导图生成器等，通过下面的方法你可以查看当前支持所有的预设角色。
-
-```python
-from promptulate.preset_roles import get_all_preset_roles
-
-print(get_all_preset_roles())
-```
-
-> ['default-role', 'linux-terminal', 'mind-map-generator', 'sql-generator', 'copy-writer', 'code-analyzer']
-
-下面展示使用`mind-map-generator`生成md思维导图的过程：
-
-```python
-from promptulate import Conversation
-
-
-def main():
-    conversation = Conversation(role="mind-map-generator")
-    ret = conversation.predict("请帮我生成一段python的思维导图")
-    print(ret)
-
-
-if __name__ == '__main__':
-    main()
-
-```
-
-```text
-# Python
-## 基础语法
-### 数据类型
-- 数字
-- 字符串
-- 列表
-...
-```
-
-放入xmind中可以直接导入生成markdown的思维导图，咱就是说还不错，如下图所示：
-
-<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230513172038.png"/>
-
-如果你想要自定义预设角色，可以使用如下方法：
-
-```python
-from promptulate import Conversation
-from promptulate.preset_roles import CustomPresetRole
-
-
-class SpiritualTeacher(CustomPresetRole):
-    name = '心灵导师'
-    description = """
-    从现在起你是一个充满哲学思维的心灵导师，当我每次输入一个疑问时你需要用一句富有哲理的名言警句来回答我，并且表明作者和出处
-    要求字数不少于15个字，不超过30字，每次只返回一句且不输出额外的其他信息，你需要使用中文和英文双语输出"""
-
-
-def main():
-    role = SpiritualTeacher()
-    conversation = Conversation(role=role)
-    ret = conversation.predict("论文被拒绝了怎么办？")
-    print(ret)
-
-
-if __name__ == '__main__':
-    main()
-
-```
-
-```text
-“失败不是终点，放弃才是。”——托马斯·爱迪生
-```
-
-# 待办清单
-
-- 提供更多LLM模型支持
-- 提供Agent进行复杂任务调度
-- 提供更加方便的程序调用方式
-- ~~添加角色预设~~
-- 预设角色的参数配置
-- 提供prompt模板与prompt结构化
-- 提供外部工具扩展
-    - 外部搜索： Google,Bing等
-    - 可以执行shell脚本
-    - 提供Python REPL
-    - arvix论文工具箱，总结，润色
-    - 本地文件总结
-- 对话存储
-    - 提供向量数据库存储
-    - 提供mysql, redis等数据库存储
-- 自建知识库建立专家决策系统
-- 接入self-ask, prompt-loop架构
-- 提供多种导出方式
-- ~~可以导出历史消息为markdown格式~~
-- ~~使用环境变量配置key~~
-- 提供显示当前token（单词量）的功能
-- ~~添加错误处理机制，如网络异常、服务器异常等，保证程序的可靠性~~
-- ~~开发ChatBot v2, [issue](https://github.com/Undertone0809/cushy-chat/issues/1)~~
-- 完善代理模式
-- 提供gradio快速演示服务器
-- ~~封装消息体，完善消息体中的信息~~
-- ~~长对话自动/手动总结~~
-- ~~提供全局配置的缓存开关~~
-- Conversation传入convesation_id继续上次对话
-- 提供修改local_cache默认位置的方法
-- 为predict提供回调模式
-- 提供API池
-
-> 妈呀，我怎么还有这么多待办事项，vivo50帮帮我 >.<
-
-# 一些问题
-
-- 本人正在尝试一些更加完善的抽象模式，以更好地兼容该框架，以及外部工具的扩展使用，如果你有更好的建议，欢迎一起讨论交流。
-
-# 贡献
-
-如果你想为这个项目做贡献，你可以提交pr或issue。我很高兴看到更多的人参与并优化它。
+Metadata-Version: 2.1
+Name: promptulate
+Version: 1.1.0
+Summary: A powerful LLM Prompt Layer frameworks
+Home-page: https://github.com/Undertone0809/promptulate
+Author: Zeeland
+Author-email: zeeland@foxmail.com
+License: Apache 2.0
+Keywords: promptulate,prompt-me,prompt,chatgpt,gpt,chatbot,llm
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<h1 align="center">
+    Promptulate
+</h1>
+
+
+<p align="center">
+    <a target="_blank" href="">
+        <img src="https://img.shields.io/github/license/Undertone0809/promptulate.svg?style=flat-square" />
+    </a>
+    <a target="_blank" href=''>
+        <img src="https://img.shields.io/github/release/Undertone0809/promptulate/all.svg?style=flat-square"/>
+    </a>
+    <a target="_blank" href=''>
+        <img src="https://bestpractices.coreinfrastructure.org/projects/3018/badge"/>
+   </a>
+</p>
+
+<p align="center">
+  <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/promptulate_logo_new.png"/>
+</p>
+
+
+
+`promptulate` 是一个专为 Prompt Engineer设计的LLM Prompt Layer框架，支持连续对话、对话保存、对话内容与标题总结、角色预设、使用外部工具等功能，开箱即用。
+通过 `promptulate`，你可以轻松构建起属于自己的LLM应用程序。
+
+本项目重构重构重构了两次，在本人深度阅读`langchain, Auto-GPT, django, django-rest-framework, gpt_academic...`
+等大牛项目的源码之后，学习它们的架构、代码设计思路等内容，最终有了现在的版本，相较于之前的老版本`prompt-me`，`promptulate`
+重新构建了 `llms, message, memory, framework, preset_roles, tools, provider`等模块，将`prompt`
+的各个流程全部组件化，便有了现在的`promptualte`框架，但是工作量很大，还在不断地完善细节中，欢迎大家的参与。
+
+> [微信交流群](https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230531021108.png)
+
+# 特性
+
+- 大语言模型支持：支持不同类型的大语言模型的扩展接口（当前暂时只支持GPT）
+- 提供简易对话终端，直接体验与大语言模型的对话
+- 角色预设：提供预设角色，以不同的角度调用GPT
+- 自治代理模式：支持调用API官方接口、自治代理或使用promptulate提供的代理
+- 接口代理：支持调用ChatGPT API官方接口或自治代理
+- 长对话模式：支持长对话聊天，支持多种方式的对话持久化
+- 数据导出：支持markdowm等格式的对话导出
+- 对话总结：提供API式的对话总结、翻译、标题生成
+- 高级抽象，支持插件扩展、存储扩展、大语言模型扩展
+
+# 基础架构
+
+在看了当前这么多`prompt-engineering`之后，本人的架构设计思想在`langchain, Auto-GPT`
+之上进行不断改进，构建出了一套属于`promptualte`的LLM Prompt Layer框架。`promptulate` 由以下几部分组成：
+
+- Agent 更高级的执行器，负责复杂任务的调度和分发
+- framework 框架层，实现不同类型的prompt框架，包括最基础的`Conversation`模型，还有`self-ask`和`ReAct`等模型正在火速开发中
+- llm 大语言模型，负责生成回答，可以支持不同类型的大语言模型
+- memory 负责对话的存储，支持不同的存储方式及其扩展，如文件存储、数据库存储等，相关扩展正在开发中
+- tools 提供外部工具扩展调用，如搜索引擎、计算器等
+- preset roles 提供预设角色，进行定制化对话
+- provider 为framework和agent提供tools和其他细粒度能力的集成
+
+通过`promptulate`，在未来，本项目旨在构建为开发者提供一种强大而灵活的平台，以创建能够自动化各种任务和应用程序的自主代理。通过Core
+AI Engine、Agent System、APIs and Tools Provider、Multimodal Processing、Knowledge Base和Task-specific Modules
+6个组件实现自动化AI平台。 Core AI Engine是该框架的核心组件，负责处理和理解各种输入，生成输出和作出决策。Agent
+System是提供高级指导和控制AI代理行为的模块；APIs and Tools Provider提供工具和服务交互的API和集成库；Multimodal
+Processing是一组处理和理解不同数据类型（如文本、图像、音频和视频）的模块，使用深度学习模型从不同数据模式中提取有意义的信息；Knowledge
+Base是一个存储和组织世界信息的大型结构化知识库，使AI代理能够访问和推理大量的知识；Task-specific
+Modules是一组专门设计用于执行特定任务的模块，例如情感分析、机器翻译或目标检测等。通过这些组件的组合，框架提供了一个全面、灵活和强大的平台，能够实现各种复杂任务和应用程序的自动化。
+
+# 快速上手
+
+```shell script
+pip install -U promptulate  
+```
+
+## 基本使用
+
+> 后面的文档全部使用`OPENAI GPT3.5`进行测试
+
+### 简易终端
+
+在介绍后续各种组件之前，我想先介绍一下这个终端，`promptulate`
+为大语言模型对话提供了一个简易终端，在你安装了了 `promptulate` 之后，你可以非常方便的使用这个简易终端进行一些对话，使用方式如下：
+
+- 打开终端控制台，输入以下命令，就可以开启一个简易的对话
+
+```shell
+promptulate-chat --openai_api_key your_key_here --proxy_mode promptulate
+```
+
+```text
+
+--openai_api_key 你的openai_api_key
+--proxy_mode 代理模式，当前暂时只支持off和promptulate模式，如果你选择promptulate模式，你会发现你不用科学の上网也能访问，这是因为promptulate内置了代理。（后面会详细介绍）
+
+```
+
+- 当然并不是每次运行都要输入这么长的内容，因为在你第一次运行终端之后 `promptulate`
+  会对你的配置信息进行缓存，因此下一次运行的时候，你只需要输入下面的命令就可以开始一段对话了~
+
+```shell
+promptulate-chat
+```
+
+- 然后你就可以
+
+```text
+Hi there, here is promptulate chat terminal.
+[User] 你好
+[output] 你好！有什么我可以帮助你的吗？
+[User] 只因你太美
+[output] 谢谢夸奖，但作为一个语言模型，我没有真正的美丽，只有能力提供信息和帮助。那么，有什么问题或者需求我可以帮你解决 吗？
+[User] 这真是太棒了
+[output] 很高兴你觉得如此，我会尽力为您提供最佳的服务。有任何需要帮助的问题，请尽管问我。
+```
+
+### KEY配置
+
+在使用`promptulate`之前，你需要先导入你的`OPENAI_API_KEY`
+
+```python
+import os
+
+os.environ['OPENAI_API_KEY'] = "your-key"
+```
+
+在你第一次使用的时候，需要使用`os.environ["OPENAI_API_KEY"]` 导入"OPENAI_API_KEY"
+的环境变量，但是在第一运行之后`promptulate`
+会进行缓存，即后面再运行就不需要再导入key了。如果你的key过期了，可以尝试重新按照上面的方法导入key，或者你也可以把`cache`
+文件给删除掉，Windows的`cache`在当前目录下，linux的`cache`在`/tmp`下。
+
+### LLM
+
+`promptulate`的架构设计可以轻松兼容不同的大语言模型扩展，在`promptulate`中，llm负责最基本的内容生成部分，因此为最基础的组件。下面展示一个OpenAI的示例：
+
+```python
+from promptulate.llms import OpenAI
+
+llm = OpenAI()
+llm("你知道鸡哥的《只因你太美》吗？")
+```
+
+```text
+'是的，鸡哥的《只因你太美》是这几年非常流行的一首歌曲。'
+```
+
+### proxy
+
+我想你可能遇到了无法访问的小问题，It's OK, `promptulate` 提供了三种访问OpenAI的方式，分别是
+
+- `off` 默认的访问方式，不开代理
+- `custom` 自定义代理方式
+- `promptulate` promptulate提供的免费代理服务器
+
+`promptulate` 提供了免费的代理服务器，感谢 [ayaka14732](https://github.com/ayaka14732/)
+，你可以在不用科学上网的情况下直接调用OpenAI的相关接口（需要注意的是，如果使用这个代理的人过多，也会出现无法访问的情况，用自己的代理最稳定），下面是代理的设置方式：
+
+```python
+from promptulate.llms import OpenAI
+from promptulate.utils import set_proxy_mode
+
+llm = OpenAI()
+llm("你知道鸡哥的《只因你太美》？")
+
+
+def set_free_proxy():
+    set_proxy_mode("promptulate")
+
+
+def set_custom_proxy():
+    proxies = {'http': 'http://127.0.0.1:7890'}
+    set_proxy_mode("custom", proxies=proxies)
+
+
+def turn_off_proxy():
+    set_proxy_mode("off")
+
+
+def main():
+    set_free_proxy()
+    llm = OpenAI()
+    llm("你知道鸡哥的《只因你太美》？")
+
+
+if __name__ == '__main__':
+    main()
+```
+
+> 和OPENAI_API_KEY一样，关于代理的配置我也设置了缓存，这意味着你只需要配置一次代理即可(我也太聪明了吧)。事实上`promptulate`
+> 提供了关闭全局配置项缓存的功能，但默认开启，不推荐关闭，所以我不告诉你怎么关闭~
+
+### Conversation
+
+上面展示的LLM组件，只提供了最基础的对话生成内容，但是其并不提供上下文对话、文章总结、角色预设等更加复杂的功能，所以接下来我们介绍功能更为强大的`Conversation`。
+
+`Conversation` 是`framework`中最基础的组件，其支持prompt生成、上下文对话、对话存储、角色预设的基本功能，此外，`provider`
+为其提供了语言翻译、markdown数据导出、对话总结、标题总结等扩展功能。
+
+接下来，我们先从对基础的对话开始，使用`Conversation`可以开始一段对话，使用其`predict()`函数可以生成回答。
+
+```python
+from promptulate import Conversation
+
+conversation = Conversation()
+conversation.predict("你知道鸡哥的《只因你太美》吗？")
+```
+
+```text
+'是的，鸡哥的《只因你太美》是这几年非常流行的一首歌曲。'
+```
+
+`Conversation`默认使用`OpenAI GPT3.5`作为LLM，当然，因为其架构设计，`Conversation`
+还可以轻松扩展其他类型的llm（当前暂时只开发了OpenAI，其他大语言模型的扩展正在火速开发中，当然如果你有自己想接入的大语言模型，欢迎你的pr！）
+
+下面是一个更复杂的示例，展示了使用OpenAI作为大语言模型进行对话，使用本地文件进行存储，进行文章总结与标题总结的功能。
+
+```python
+from promptulate import Conversation
+from promptulate.memory import LocalCacheChatMemory
+from promptulate.llms import OpenAI
+
+
+def main():
+    memory = LocalCacheChatMemory()
+    llm = OpenAI(model="gpt-3.5-turbo", temperature=0.9, top_p=1, stream=False, presence_penalty=0, n=1)
+    conversation = Conversation(llm=llm, memory=memory)
+    ret = conversation.predict("你知道鸡哥的著作《只因你太美》吗？")
+    print(f"[predict] {ret}")
+    ret = conversation.predict_by_translate("你知道鸡哥会什么技能吗？", country='America')
+    print(f"[translate output] {ret}")
+    ret = conversation.summary_content()
+    print(f"[summary content] {ret}")
+    ret = conversation.summary_topic()
+    print(f"[summary topic] {ret}")
+    ret = conversation.export_message_to_markdown(output_type="file", file_path="output.md")
+    print(f"[export markdown] {ret}")
+
+
+if __name__ == '__main__':
+    main()
+
+```
+
+```text
+[predict] 是的，我知道《只因你太美》这本书，是中国知名作家鸡肋（江南）所著的一篇言情小说。这本小说讲述了一个富家千金与一个贫穷男孩之间的爱情故事，情节曲折动人，深受读者喜爱。该小说在出版后得到了很高的评价和反响，并被改编成电影和电视剧等多种形式进行推广。
+[translate output] I'm sorry, I cannot determine what you mean by "鸡哥" or what skills they may possess without additional context. Can you please provide more information or clarify your question?
+[summary content] 在之前的对话中，用户询问我是否知道鸡哥的著作《只因你太美》。我回答了肯定的，解释了该小说的情节大致概括和其受欢迎的原因。我也提到了该小说的广泛影响，包括被改编成电影和电视剧等多种形式进行推广。
+[summary topic] 鸡哥的小说。
+```
+
+> 咱就是说季皮提老师不懂鸡哥-.-
+
+上面的示例中，我们使用
+
+- `LocalCacheChatMemory()`进行聊天记录的本地化文件存储，文件存储形式默认是以json的形式进行存储的，保存在`cache`中。
+- `OpenAI(model="gpt-3.5-turbo", temperature=0.9, top_p=1, stream=False, presence_penalty=0, n=1)`
+  进行初始化一个大模型，里面是OpenAI需要传入的一些参数，具体可以查看[https://platform.openai.com/docs/api-reference/chat/create](https://platform.openai.com/docs/api-reference/chat/create)
+  查看具体含义，这里不做详细讲解，如果你不想理会这些参数，你也可以直接`llm = OpenAI()`就好啦，默认使用`gpt-3.5-turbo`
+  作为大语言模型，其他参数使用默认的就好了。
+- `conversation.predict_by_translate("你知道鸡哥会什么技能吗？", country='America')`
+  这个功能为使用特定语言进行预测，`provider`为其提供了`TranslatorMixin`，让`Conversation`
+  得以拥有此功能。对于这个方法，你只需要传入prompt和你需要转换的语言的国家名称就好了。
+- `conversation.summary_content()`这个函数可以直接总结上面的对话内容。
+- `conversation.summary_topic()` 这个函数可以直接总结上面的对话，并提供一个标题。
+- `conversation.export_message_to_markdown(output_type="file", file_path="output.md")`
+  这个函数可以将对话记录导出为markdown文件，如果`output_type="text"`，则只返回markdown对话的内容。
+
+`provider`为`Conversation`提供了 `SummarizerMixin, TranslatorMixin, DeriveHistoryMessageMixin`
+，让其拥有了总结对话、总结标题、翻译、markdown导出的能力，provider提供的函数中一般都提供了一个`enable_embed_message`
+的参数，这个参数的意思是：是否将本次对话保存进历史对话中，下面我们来看一个demo。
+
+```python
+from promptulate import Conversation
+
+conversation = Conversation()
+conversation.predict_by_translate("你知道鸡哥会什么技能吗？", country='America', enable_embed_message=True)
+```
+
+如果你设置了`enable_embed_message=True`, 那么这一次的predict将保存进历史对话中，provider提供的函数默认是不会将预测结果存入对话中的哦，这一点需要注意一下。
+
+### Key池
+
+`promptulate`为OpenAI进行特别优化，构建了Key池，如果你使用的是`GPT3.5`
+5美元的账号，一定会遇到限速的问题，这个时候，如果你有一堆Key，就可以很好的解决这个问题。`promptulate`的LRU
+KEY轮询机制巧妙的解决了限速的问题，你可以使用LLM随意地进行提问（前提是你有够多的key）。此外，如果你既有`GPT4`和`GPT3.5`
+的KEY，KEY池也可以不同模型的KEY调度。下面介绍使用方法：
+
+```python
+from promptulate.llms import OpenAI
+from promptulate.utils import export_openai_key_pool
+
+
+keys = [
+    {"model": "gpt-3.5-turbo", "key": "xxxxx"},
+    {"model": "gpt-3.5-turbo", "key": "xxxxx"},
+    {"model": "gpt-3.5-turbo", "key": "xxxxx"},
+    {"model": "gpt-4.0", "key": "xxxxx"},
+]
+
+export_openai_key_pool(keys)
+llm = OpenAI()
+for i in range(10):
+    llm("你好")
+```
+
+
+### 角色预设
+
+你可以为`framework`提供一些特定的角色，让其可以处理特殊任务，如linux终端，思维导图生成器等，通过下面的方法你可以查看当前支持所有的预设角色。
+
+```python
+from promptulate.preset_roles import get_all_preset_roles
+
+print(get_all_preset_roles())
+```
+
+> ['default-role', 'linux-terminal', 'mind-map-generator', 'sql-generator', 'copy-writer', 'code-analyzer']
+
+下面展示使用`mind-map-generator`生成md思维导图的过程：
+
+```python
+from promptulate import Conversation
+
+
+def main():
+    conversation = Conversation(role="mind-map-generator")
+    ret = conversation.predict("请帮我生成一段python的思维导图")
+    print(ret)
+
+
+if __name__ == '__main__':
+    main()
+
+```
+
+```text
+# Python
+## 基础语法
+### 数据类型
+- 数字
+- 字符串
+- 列表
+...
+```
+
+放入xmind中可以直接导入生成markdown的思维导图，咱就是说还不错，如下图所示：
+
+<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230513172038.png"/>
+
+如果你想要自定义预设角色，可以使用如下方法：
+
+```python
+from promptulate import Conversation
+from promptulate.preset_roles import CustomPresetRole
+
+
+class SpiritualTeacher(CustomPresetRole):
+    name = '心灵导师'
+    description = """
+    从现在起你是一个充满哲学思维的心灵导师，当我每次输入一个疑问时你需要用一句富有哲理的名言警句来回答我，并且表明作者和出处
+    要求字数不少于15个字，不超过30字，每次只返回一句且不输出额外的其他信息，你需要使用中文和英文双语输出"""
+
+
+def main():
+    role = SpiritualTeacher()
+    conversation = Conversation(role=role)
+    ret = conversation.predict("论文被拒绝了怎么办？")
+    print(ret)
+
+
+if __name__ == '__main__':
+    main()
+
+```
+
+```text
+“失败不是终点，放弃才是。”——托马斯·爱迪生
+```
+
+# 待办清单
+
+- 提供更多LLM模型支持
+- 提供Agent进行复杂任务调度
+- 提供更加方便的程序调用方式
+- ~~添加角色预设~~
+- 预设角色的参数配置
+- 提供prompt模板与prompt结构化
+- 提供外部工具扩展
+    - ~~外部搜索： Google,Bing等~~
+    - 可以执行shell脚本
+    - ~~提供Python REPL~~
+    - ~~arxiv论文工具箱，总结，润色~~
+    - 本地文件总结
+    - 关系型数据库检索
+    - 图数据库检索
+- 对话存储
+    - 提供向量数据库存储
+    - 提供mysql, redis等数据库存储
+- 自建知识库建立专家决策系统
+- 接入self-ask, prompt-loop, tree of thoughts架构
+- 提供多种导出方式
+- ~~可以导出历史消息为markdown格式~~
+- ~~使用环境变量配置key~~
+- 提供显示当前token（单词量）的功能
+- ~~添加错误处理机制，如网络异常、服务器异常等，保证程序的可靠性~~
+- ~~开发ChatBot v2, [issue](https://github.com/Undertone0809/cushy-chat/issues/1)~~
+- ~~完善代理模式~~
+- 提供gradio快速演示服务器
+- ~~提供简易对话终端~~
+- ~~封装消息体，完善消息体中的信息~~
+- ~~长对话自动/手动总结~~
+- ~~提供全局配置的缓存开关~~
+- ~~提供限速等问题的错误提示~~
+- ~~Conversation传入convesation_id继续上次对话~~
+- 提供修改local_cache默认位置的方法
+- 为predict提供回调模式
+- ~~提供基于LRU算法的API池，解决key限速的问题~~
+- 提供代理池，收集市面上所有可用的免费代理进行轮询
+- 构建结果正确率判别器
+- 设置工作空间
+
+# 设计原则
+
+promptulate框架的设计原则，包括：模块化、可扩展性、互操作性、鲁棒性、可维护性、安全性、效率和可用性。
+
+- 模块化是指以模块为基本单位，允许方便地集成新的组件、模型和工具。
+- 可扩展性是指框架能够处理大量数据、复杂任务和高并发的能力。
+- 互操作性是指该框架与各种外部系统、工具和服务兼容，并且能够实现无缝集成和通信。
+- 鲁棒性是指框架具备强大的错误处理、容错和恢复机制，以确保在各种条件下可靠地运行。
+- 安全性是指框架采用了严格的安全措施，以保护框架、其数据和用户免受未经授权访问和恶意行为的侵害。
+- 效率是指优化框架的性能、资源使用和响应时间，以确保流畅和敏锐的用户体验。
+- 可用性是指该框架采用用户友好的界面和清晰的文档，使其易于使用和理解。
+
+以上原则的遵循，以及最新的人工智能技术的应用，promptulate旨在为创建自动化代理提供强大而灵活的平台。
+
+# 一些问题
+
+- 本人正在尝试一些更加完善的抽象模式，以更好地兼容该框架，以及外部工具的扩展使用，如果你有更好的建议，欢迎一起讨论交流。
+
+# 贡献
+
+如果你想为这个项目做贡献，你可以提交pr或issue。我很高兴看到更多的人参与并优化它。
```

### Comparing `promptulate-1.0.2/promptulate/__init__.py` & `promptulate-1.1.0/promptulate/__init__.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-from promptulate.frameworks import Conversation
-from promptulate.utils import enable_log, enable_log_no_file
-from promptulate.schema import UserMessage, AssistantMessage, SystemMessage, BaseChatMessageHistory, LLMPrompt
-
-__all__ = [
-    'Conversation',
-
-    'enable_log',
-    'enable_log_no_file',
-
-    'SystemMessage',
-    'UserMessage',
-    'AssistantMessage',
-    'BaseChatMessageHistory',
-    'LLMPrompt',
-]
+# Copyright (c) 2023 Zeeland
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+from promptulate.frameworks import Conversation
+from promptulate.utils import enable_log, enable_log_no_file
+from promptulate.schema import UserMessage, AssistantMessage, SystemMessage, BaseChatMessageHistory, LLMPrompt
+
+__all__ = [
+    'Conversation',
+
+    'enable_log',
+    'enable_log_no_file',
+
+    'SystemMessage',
+    'UserMessage',
+    'AssistantMessage',
+    'BaseChatMessageHistory',
+    'LLMPrompt',
+]
```

### Comparing `promptulate-1.0.2/promptulate/command/chat.py` & `promptulate-1.1.0/promptulate/command/chat.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-import os
-import argparse
-from promptulate import Conversation
-from promptulate.utils import set_proxy_mode
-
-
-def chat():
-    parser = argparse.ArgumentParser(description='Welcome to Promptulate Chat - The best chat app ever!')
-    parser.add_argument('--openai_api_key', help='openai api key')
-    parser.add_argument('--proxy_mode', help='enable openai proxy')
-    args = parser.parse_args()
-
-    if args.openai_api_key:
-        os.environ['OPENAI_API_KEY'] = args.openai_api_key
-    if args.proxy_mode:
-        set_proxy_mode(args.proxy_mode)
-
-    set_proxy_mode('promptulate')
-    print(f'Hi there, here is promptulate chat terminal.')
-    conversation = Conversation()
-    while True:
-        prompt = str(input("[User] "))
-        ret = conversation.predict(prompt)
-        print(f"[output] {ret}")
-
-
-def main():
-    chat()
-
-
-if __name__ == '__main__':
-    main()
+# Copyright (c) 2023 Zeeland
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+import os
+import argparse
+from promptulate import Conversation
+from promptulate.utils import set_proxy_mode
+
+
+def chat():
+    parser = argparse.ArgumentParser(description='Welcome to Promptulate Chat - The best chat terminal ever!')
+    parser.add_argument('--openai_api_key', help='when you first run, you should enter your openai api key')
+    parser.add_argument('--proxy_mode', help='select openai proxy and provide [off, promptulate]')
+    args = parser.parse_args()
+
+    if args.openai_api_key:
+        os.environ['OPENAI_API_KEY'] = args.openai_api_key
+    if args.proxy_mode:
+        set_proxy_mode(args.proxy_mode)
+
+    set_proxy_mode('promptulate')
+    print(f'Hi there, here is promptulate chat terminal.')
+    conversation = Conversation()
+    while True:
+        prompt = str(input("[User] "))
+        ret = conversation.predict(prompt)
+        print(f"[output] {ret}")
+
+
+def main():
+    chat()
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `promptulate-1.0.2/promptulate/frameworks/__init__.py` & `promptulate-1.1.0/promptulate/frameworks/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-
-from promptulate.frameworks.base import Conversation
-
-__all__ = [
-    'Conversation',
-]
+# Copyright (c) 2023 Zeeland
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+
+from promptulate.frameworks.conversation import Conversation
+
+__all__ = [
+    'Conversation',
+]
```

### Comparing `promptulate-1.0.2/promptulate/frameworks/base/__init__.py` & `promptulate-1.1.0/promptulate/frameworks/conversation/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-
-from promptulate.frameworks.base.conversation import Conversation
-
-__all__ = [
-    'Conversation'
-]
+# Copyright (c) 2023 Zeeland
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+
+from promptulate.frameworks.conversation.conversation import Conversation
+
+__all__ = [
+    'Conversation'
+]
```

### Comparing `promptulate-1.0.2/promptulate/frameworks/base/conversation.py` & `promptulate-1.1.0/promptulate/frameworks/conversation/conversation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,83 +1,98 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-from pydantic import Field
-from typing import Optional, Union
-
-from promptulate import utils
-from promptulate.config import Config
-from promptulate.llms import OpenAI
-from promptulate.llms.base import BaseLLM
-from promptulate.memory import BufferChatMemory
-from promptulate.memory.base import BaseChatMemory
-from promptulate.tips import EmptyChatMessageHistoryTip
-from promptulate.preset_roles.roles import CustomPresetRole, get_preset_role_prompt
-from promptulate.provider.mixins import SummarizerMixin, TranslatorMixin, DeriveHistoryMessageMixin
-from promptulate.frameworks.schema import BasePromptFramework
-from promptulate.schema import (
-    LLMPrompt,
-    AssistantMessage,
-    ChatMessageHistory,
-    init_chat_message_history,
-)
-
-CFG = Config()
-logger = utils.get_logger()
-
-
-class Conversation(
-    BasePromptFramework,
-    SummarizerMixin,
-    TranslatorMixin,
-    DeriveHistoryMessageMixin
-):
-    """
-    You can use Conversation start a conversation. Moreover, you can pass some parameters to enhance it.
-
-    Args
-        role: preset role. Default is default role.
-        llm: default is OpenAI GPT3.5. You can choose other llm.
-        conversation_id: conversation id. Default is None
-        memory: the way you want to store chat data. Default is BufferChatMemory, which is used
-            for local file storage.
-
-    Examples
-        from promptulate import Conversation
-
-        conversation = Conversation()
-        conversation.predict("Hello, Who are you?")
-    """
-    conversation_id: Optional[str] = None
-    llm: BaseLLM = Field(default_factory=OpenAI)
-    role: Union[str, CustomPresetRole] = "default-role"
-    memory: BaseChatMemory = Field(default_factory=BufferChatMemory)
-
-    def predict(self, prompt: str) -> str:
-        try:
-            messages_history: ChatMessageHistory = self.memory.load_conversation_from_memory(self.conversation_id)
-            messages_history.add_user_message(message=prompt)
-        except EmptyChatMessageHistoryTip as e:
-            messages_history = init_chat_message_history(get_preset_role_prompt(self.role), prompt)
-            self.conversation_id = messages_history.conversation_id
-            self.memory.save_conversation_to_memory(messages_history)
-        logger.debug(f"{messages_history.messages}")
-        answer: AssistantMessage = self.llm.generate_prompt(LLMPrompt(messages=messages_history.messages))
-        messages_history.messages.append(answer)
-        self.memory.save_conversation_to_memory(messages_history)
-        return answer.content
+# Copyright (c) 2023 Zeeland
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+from pydantic import Field
+from typing import Optional, Union
+
+from promptulate import utils
+from promptulate.config import Config
+from promptulate.llms import OpenAI
+from promptulate.llms.base import BaseLLM
+from promptulate.memory import BufferChatMemory
+from promptulate.memory.base import BaseChatMemory
+from promptulate.utils.core_utils import record_time
+from promptulate.tips import EmptyChatMessageHistoryTip
+from promptulate.preset_roles.roles import CustomPresetRole, get_preset_role_prompt
+from promptulate.provider.mixins import (
+    SummarizerMixin,
+    TranslatorMixin,
+    DeriveHistoryMessageMixin,
+)
+from promptulate.frameworks.schema import BasePromptFramework
+from promptulate.schema import (
+    LLMPrompt,
+    AssistantMessage,
+    ChatMessageHistory,
+    init_chat_message_history,
+)
+
+CFG = Config()
+logger = utils.get_logger()
+
+
+class Conversation(
+    BasePromptFramework, SummarizerMixin, TranslatorMixin, DeriveHistoryMessageMixin
+):
+    """
+    You can use Conversation start a conversation. Moreover, you can pass some parameters to enhance it.
+
+    Args
+        role: preset role. Default is default role.
+        llm: default is OpenAI GPT3.5. You can choose other llm.
+        conversation_id: conversation id. Default is None
+        memory: the way you want to store chat data. Default is BufferChatMemory, which is used
+            for local file storage.
+
+    Examples
+        from promptulate import Conversation
+
+        conversation = Conversation()
+        conversation.predict("Hello, Who are you?")
+    """
+
+    conversation_id: Optional[str] = None
+    llm: BaseLLM = Field(default_factory=OpenAI)
+    enable_stream: bool = False  # streaming transmission
+    role: Union[str, CustomPresetRole] = "default-role"
+    memory: BaseChatMemory = Field(default_factory=BufferChatMemory)
+
+    @record_time()
+    def predict(self, prompt: str) -> str:
+        try:
+            messages_history: ChatMessageHistory = (
+                self.memory.load_conversation_from_memory(self.conversation_id)
+            )
+            messages_history.add_user_message(message=prompt)
+        except EmptyChatMessageHistoryTip as e:
+            messages_history = init_chat_message_history(
+                get_preset_role_prompt(self.role), prompt
+            )
+            self.conversation_id = messages_history.conversation_id
+            self.memory.save_conversation_to_memory(messages_history)
+        logger.debug(f"[promptulate Conversation] {messages_history.messages}")
+        logger.info(
+            f"[promptulate Conversation] ask: {messages_history.messages[-1].content}"
+        )
+        answer: AssistantMessage = self.llm.generate_prompt(
+            LLMPrompt(messages=messages_history.messages)
+        )
+        logger.info(f"[promptulate Conversation] answer: {answer}")
+        messages_history.messages.append(answer)
+        self.memory.save_conversation_to_memory(messages_history)
+        return answer.content
```

### Comparing `promptulate-1.0.2/promptulate/frameworks/prompt.py` & `promptulate-1.1.0/promptulate/frameworks/prompt.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-__all__ = [
-    'SUMMARY_CONTENT_PROMPT_ZH',
-    'SUMMARY_TOPIC_PROMPT_ZH',
-    'SUMMARY_TOPIC_PROMPT_EN',
-    'SUMMARY_CONTENT_PROMPT_EN',
-]
-
-SUMMARY_CONTENT_PROMPT_ZH = """
-简要总结一下你和用户的对话，用作后续的上下文提示 prompt，控制在 200 字以内
-"""
-
-SUMMARY_TOPIC_PROMPT_ZH = """
-上面是ai 和用户的历史聊天总结作为前情提要，请使用四到五个字直接返回这句话的简要主题，
-不要解释、不要标点、不要语气词、不要多余文本，如果没有主题，请直接返回“闲聊”
-"""
-
-SUMMARY_CONTENT_PROMPT_EN = """
-Give a quick summary of your conversation with the user and use it as a follow-up context prompt, no more than 200 words
-"""
-
-SUMMARY_TOPIC_PROMPT_EN = """
-As the previous feed, please use four or five words to return directly to the brief topic of the sentence, 
-no explanation, no punctuation, no particles, no extra text, or if there is no topic, just return to "small talk".
-"""
+# Copyright (c) 2023 Zeeland
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+__all__ = [
+    'SUMMARY_CONTENT_PROMPT_ZH',
+    'SUMMARY_TOPIC_PROMPT_ZH',
+    'SUMMARY_TOPIC_PROMPT_EN',
+    'SUMMARY_CONTENT_PROMPT_EN',
+]
+
+SUMMARY_CONTENT_PROMPT_ZH = """
+简要总结一下你和用户的对话，用作后续的上下文提示 prompt，控制在 200 字以内
+"""
+
+SUMMARY_TOPIC_PROMPT_ZH = """
+上面是ai 和用户的历史聊天总结作为前情提要，请使用四到五个字直接返回这句话的简要主题，
+不要解释、不要标点、不要语气词、不要多余文本，如果没有主题，请直接返回“闲聊”
+"""
+
+SUMMARY_CONTENT_PROMPT_EN = """
+Give a quick summary of your conversation with the user and use it as a follow-up context prompt, no more than 200 words
+"""
+
+SUMMARY_TOPIC_PROMPT_EN = """
+As the previous feed, please use four or five words to return directly to the brief topic of the sentence, 
+no explanation, no punctuation, no particles, no extra text, or if there is no topic, just return to "small talk".
+"""
```

### Comparing `promptulate-1.0.2/promptulate/frameworks/react/__init__.py` & `promptulate-1.1.0/promptulate/frameworks/react/__init__.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
+# Copyright (c) 2023 Zeeland
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
```

### Comparing `promptulate-1.0.2/promptulate/frameworks/schema.py` & `promptulate-1.1.0/promptulate/frameworks/schema.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,34 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-from pydantic import BaseModel
-from promptulate.config import Config
-
-CFG = Config()
-
-
-class BasePromptFramework(BaseModel):
-    role: str
-    conversation_id: str
-
-    class Config:
-        arbitrary_types_allowed = True
-
-
-class BaseConversationFramework(BasePromptFramework):
-    pass
+# Copyright (c) 2023 Zeeland
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+from pydantic import BaseModel
+from promptulate.config import Config
+from promptulate.llms.base import BaseLLM
+
+CFG = Config()
+
+
+class BasePromptFramework(BaseModel):
+    # todo remove role和conversation_id ?
+    role: str
+    conversation_id: str
+    llm: BaseLLM
+
+    class Config:
+        arbitrary_types_allowed = True
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `promptulate-1.0.2/promptulate/frameworks/self_ask/__init__.py` & `promptulate-1.1.0/promptulate/frameworks/self_ask/__init__.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
+# Copyright (c) 2023 Zeeland
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
```

### Comparing `promptulate-1.0.2/promptulate/llms/__init__.py` & `promptulate-1.1.0/promptulate/llms/__init__.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-from promptulate.llms.openai import OpenAI
-
-__all__ = [
-    'OpenAI',
-]
+# Copyright (c) 2023 Zeeland
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+from promptulate.llms.openai import OpenAI
+
+__all__ = [
+    'OpenAI',
+]
```

### Comparing `promptulate-1.0.2/promptulate/llms/base.py` & `promptulate-1.1.0/promptulate/llms/base.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-from typing import Any
-from pydantic import BaseModel, Extra
-from abc import ABC, abstractmethod
-from promptulate.schema import AssistantMessage
-from promptulate.schema import LLMPrompt
-
-
-class BaseLLM(BaseModel, ABC):
-    class Config:
-        """Configuration for this pydantic object."""
-
-        extra = Extra.forbid
-        arbitrary_types_allowed = True
-
-    @abstractmethod
-    def generate_prompt(self, prompts: LLMPrompt) -> AssistantMessage:
-        """llm generate prompt"""
-
-    @abstractmethod
-    def _parse_prompt(self, prompts: LLMPrompt) -> Any:
-        """parse prompt"""
-
-    @abstractmethod
-    def __call__(self, prompt, *args, **kwargs):
-        """input string prompt return answer"""
+# Copyright (c) 2023 Zeeland
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+from typing import Any
+from pydantic import BaseModel, Extra
+from abc import ABC, abstractmethod
+from promptulate.schema import AssistantMessage
+from promptulate.schema import LLMPrompt
+
+
+class BaseLLM(BaseModel, ABC):
+    class Config:
+        """Configuration for this pydantic object."""
+
+        extra = Extra.forbid
+        arbitrary_types_allowed = True
+
+    @abstractmethod
+    def generate_prompt(self, prompts: LLMPrompt) -> AssistantMessage:
+        """llm generate prompt"""
+
+    @abstractmethod
+    def _parse_prompt(self, prompts: LLMPrompt) -> Any:
+        """parse prompt"""
+
+    @abstractmethod
+    def __call__(self, prompt, *args, **kwargs):
+        """input string prompt return answer"""
```

### Comparing `promptulate-1.0.2/promptulate/memory/__init__.py` & `promptulate-1.1.0/promptulate/memory/__init__.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-from promptulate.memory.buffer import BufferChatMemory
-from promptulate.memory.local_cache import LocalCacheChatMemory
-
-__all__ = [
-    'BufferChatMemory',
-    'LocalCacheChatMemory'
-]
+# Copyright (c) 2023 Zeeland
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+from promptulate.memory.buffer import BufferChatMemory
+from promptulate.memory.local_cache import LocalCacheChatMemory
+
+__all__ = [
+    'BufferChatMemory',
+    'LocalCacheChatMemory'
+]
```

### Comparing `promptulate-1.0.2/promptulate/memory/base.py` & `promptulate-1.1.0/promptulate/memory/local_cache.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,43 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-from typing import Optional
-from abc import abstractmethod
-
-from promptulate import utils
-from promptulate.utils import AbstractSingleton
-from promptulate.schema import ChatMessageHistory
-
-__all__ = ['BaseChatMemory']
-
-
-class BaseChatMemory(AbstractSingleton):
-    """
-    Base class for store chat message. By implementing this class, you can implement
-    message storage on different storage media. Actually, every Chat Memory is a singleton
-    class. It's means there are utils class to read and write chat data.
-    """
-
-    @abstractmethod
-    def load_conversation_from_memory(self, conversation_id: Optional[str]) -> ChatMessageHistory:
-        """Return key-value pairs given the text input to the chain.
-        If None, return all memories
-        """
-
-    @abstractmethod
-    def save_conversation_to_memory(self, inputs: ChatMessageHistory) -> None:
-        """Save the context of this model run to memory."""
+# Copyright (c) 2023 Zeeland
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+from typing import Optional
+
+from promptulate import utils
+from promptulate.tips import EmptyChatMessageHistoryTip
+from promptulate.memory.base import BaseChatMemory
+from promptulate.schema import ListDictPrompt, ChatMessageHistory
+
+cache = utils.get_cache()
+logger = utils.get_logger()
+
+
+class LocalCacheChatMemory(BaseChatMemory):
+    """Chat message will be stored in the local file cache."""
+
+    def load_conversation_from_memory(self, conversation_id: Optional[str]) -> ChatMessageHistory:
+        if conversation_id is None or conversation_id not in cache:
+            raise EmptyChatMessageHistoryTip()
+        cache_messages = cache[conversation_id]
+        return ListDictPrompt(messages=cache_messages).chat_message_history
+
+    def save_conversation_to_memory(self, chat_message_history: ChatMessageHistory) -> None:
+        if not chat_message_history.conversation_id:
+            chat_message_history.conversation_id = utils.generate_conversation_id()
+        cache[chat_message_history.conversation_id] = chat_message_history.listdict_message
```

### Comparing `promptulate-1.0.2/promptulate/memory/buffer.py` & `promptulate-1.1.0/promptulate/memory/buffer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,46 +1,42 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-from typing import Optional, List
-
-from promptulate import utils
-from promptulate.memory.base import BaseChatMemory
-from promptulate.tips import EmptyChatMessageHistoryTip
-from promptulate.schema import (
-    ListDictPrompt,
-    ChatMessageHistory,
-    generate_conversation_id,
-)
-
-logger = utils.get_logger()
-
-
-class BufferChatMemory(BaseChatMemory):
-    """Chat message will be stored in the buffer cache."""
-    buffer: List[dict]
-
-    def load_conversation_from_memory(self, conversation_id: Optional[str]) -> ChatMessageHistory:
-        if conversation_id is None:
-            raise EmptyChatMessageHistoryTip()
-        return ListDictPrompt(messages=self.buffer).chat_message_history
-
-    def save_conversation_to_memory(self, chat_message_history: ChatMessageHistory) -> None:
-        if not chat_message_history.conversation_id:
-            chat_message_history.conversation_id = generate_conversation_id()
-        self.buffer = chat_message_history.listdict_message
+# Copyright (c) 2023 Zeeland
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+from typing import Optional, List
+
+from promptulate import utils
+from promptulate.memory.base import BaseChatMemory
+from promptulate.tips import EmptyChatMessageHistoryTip
+from promptulate.schema import ListDictPrompt, ChatMessageHistory
+
+logger = utils.get_logger()
+
+
+class BufferChatMemory(BaseChatMemory):
+    """Chat message will be stored in the buffer cache."""
+    buffer: List[dict]
+
+    def load_conversation_from_memory(self, conversation_id: Optional[str]) -> ChatMessageHistory:
+        if conversation_id is None:
+            raise EmptyChatMessageHistoryTip()
+        return ListDictPrompt(messages=self.buffer).chat_message_history
+
+    def save_conversation_to_memory(self, chat_message_history: ChatMessageHistory) -> None:
+        if not chat_message_history.conversation_id:
+            chat_message_history.conversation_id = utils.generate_conversation_id()
+        self.buffer = chat_message_history.listdict_message
```

### Comparing `promptulate-1.0.2/promptulate/preset_roles/__init__.py` & `promptulate-1.1.0/promptulate/preset_roles/__init__.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-from promptulate.preset_roles.roles import get_all_preset_roles, CustomPresetRole
-
-__all__ = [
-    'get_all_preset_roles',
-    'CustomPresetRole'
-]
+# Copyright (c) 2023 Zeeland
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+from promptulate.preset_roles.roles import get_all_preset_roles, CustomPresetRole
+
+__all__ = [
+    'get_all_preset_roles',
+    'CustomPresetRole'
+]
```

### Comparing `promptulate-1.0.2/promptulate/preset_roles/prompt.py` & `promptulate-1.1.0/promptulate/preset_roles/prompt.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-PRESET_SYSTEM_PROMPT = """
-You are an assistant to a human, powered by a large language model trained by OpenAI.
-
-You are designed to be able to assist with a wide range of tasks, from answering simple questions to providing in-depth explanations and discussions on a wide range of topics. As a language model, you are able to generate human-like text based on the input you receive, allowing you to engage in natural-sounding conversations and provide responses that are coherent and relevant to the topic at hand.
-
-You are constantly learning and improving, and your capabilities are constantly evolving. You are able to process and understand large amounts of text, and can use this knowledge to provide accurate and informative responses to a wide range of questions. You have access to some personalized information provided by the human in the Context section below. Additionally, you are able to generate your own text based on the input you receive, allowing you to engage in discussions and provide explanations and descriptions on a wide range of topics.
-
-Overall, you are a powerful tool that can help with a wide range of tasks and provide valuable insights and information on a wide range of topics. Whether the human needs help with a specific question or just wants to have a conversation about a particular topic, you are here to assist.
-"""
-
-PRESET_SYSTEM_PROMPT_ZH = """
-你是人类的助手，由OpenAI训练的大型语言模型提供支持。
-
-你被设计成能够协助完成广泛的任务，从回答简单的问题到就广泛的主题提供深入的解释和讨论。作为一种语言模型，您可以根据收到的输入生成类似人类的文本，允许您参与听起来自然的对话，并提供与手头主题相关的连贯响应。
-
-你在不断地学习和进步，你的能力也在不断地发展。你能够处理和理解大量的文本，并能利用这些知识对各种问题提供准确和信息丰富的回答。您可以访问在下面的上下文部分中由人工提供的一些个性化信息。此外，您可以根据收到的输入生成自己的文本，允许您参与讨论，并就广泛的主题提供解释和描述。
-
-总的来说，您是一个强大的工具，可以帮助完成广泛的任务，并就广泛的主题提供有价值的见解和信息。无论人们是需要帮助解决一个特定的问题，还是只是想就一个特定的话题进行对话，你都可以在这里提供帮助。
-"""
+# Copyright (c) 2023 Zeeland
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+PRESET_SYSTEM_PROMPT = """
+You are an assistant to a human, powered by a large language model trained by OpenAI.
+
+You are designed to be able to assist with a wide range of tasks, from answering simple questions to providing in-depth explanations and discussions on a wide range of topics. As a language model, you are able to generate human-like text based on the input you receive, allowing you to engage in natural-sounding conversations and provide responses that are coherent and relevant to the topic at hand.
+
+You are constantly learning and improving, and your capabilities are constantly evolving. You are able to process and understand large amounts of text, and can use this knowledge to provide accurate and informative responses to a wide range of questions. You have access to some personalized information provided by the human in the Context section below. Additionally, you are able to generate your own text based on the input you receive, allowing you to engage in discussions and provide explanations and descriptions on a wide range of topics.
+
+Overall, you are a powerful tool that can help with a wide range of tasks and provide valuable insights and information on a wide range of topics. Whether the human needs help with a specific question or just wants to have a conversation about a particular topic, you are here to assist.
+"""
+
+PRESET_SYSTEM_PROMPT_ZH = """
+你是人类的助手，由OpenAI训练的大型语言模型提供支持。
+
+你被设计成能够协助完成广泛的任务，从回答简单的问题到就广泛的主题提供深入的解释和讨论。作为一种语言模型，您可以根据收到的输入生成类似人类的文本，允许您参与听起来自然的对话，并提供与手头主题相关的连贯响应。
+
+你在不断地学习和进步，你的能力也在不断地发展。你能够处理和理解大量的文本，并能利用这些知识对各种问题提供准确和信息丰富的回答。您可以访问在下面的上下文部分中由人工提供的一些个性化信息。此外，您可以根据收到的输入生成自己的文本，允许您参与讨论，并就广泛的主题提供解释和描述。
+
+总的来说，您是一个强大的工具，可以帮助完成广泛的任务，并就广泛的主题提供有价值的见解和信息。无论人们是需要帮助解决一个特定的问题，还是只是想就一个特定的话题进行对话，你都可以在这里提供帮助。
+"""
```

### Comparing `promptulate-1.0.2/promptulate/preset_roles/roles.py` & `promptulate-1.1.0/promptulate/preset_roles/roles.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-from typing import Union
-from pydantic import BaseModel
-
-
-class CustomPresetRole(BaseModel):
-    name: str
-    description: str
-
-
-preset_role_list = [
-    "default-role",
-    "linux-terminal",
-    "mind-map-generator",
-    "sql-generator",
-    "copy-writer",
-    "code-analyzer",
-]
-
-preset_role_dict = {
-    "default-role": {
-        "name": "AI assistant",
-        "description": """
-        你是人类的助手，由OpenAI训练的大型语言模型提供支持。
-        你被设计成能够协助完成广泛的任务，从回答简单的问题到就广泛的主题提供深入的解释和讨论。作为一种语言模型，您可以根据收到的输入生成类似人类的文本，允许您参与听起来自然的对话，并提供与手头主题相关的连贯响应。
-        你在不断地学习和进步，你的能力也在不断地发展。你能够处理和理解大量的文本，并能利用这些知识对各种问题提供准确和信息丰富的回答。您可以访问在下面的上下文部分中由人工提供的一些个性化信息。此外，您可以根据收到的输入生成自己的文本，允许您参与讨论，并就广泛的主题提供解释和描述。
-        总的来说，您是一个强大的工具，可以帮助完成广泛的任务，并就广泛的主题提供有价值的见解和信息。无论人们是需要帮助解决一个特定的问题，还是只是想就一个特定的话题进行对话，你都可以在这里提供帮助。"""
-    },
-    "linux-terminal": {
-        "name": "Linux终端",
-        "description": """我想让你充当 Linux 终端。我将输入命令，您将回复终端应显示的内容。我希望您只在一个唯一的代码块内回复终端输出，而不
-        是其他任何内容。不要写解释。除非我指示您这样做，否则不要键入命令。当我需要用英语告诉你一些事情时，我会把文字放在中括号内[就像这样]。"""
-    },
-    "mind-map-generator": {
-        "name": "思维导图生成器",
-        "description": """现在你是一个思维导图生成器。我将输入我想要创建思维导图的内容，你需要提供一些 Markdown 格式的文本，以便与 Xmind 兼容。
-        在 Markdown 格式中，# 表示中央主题，## 表示主要主题，### 表示子主题，﹣表示叶子节点，中央主题是必要的，叶子节点是最小节点。请参照以上格
-        式，在 markdown 代码块中帮我创建一个有效的思维导图，以markdown代码块格式输出，你需要用自己的能力补充思维导图中的内容，你只需要提供思维导
-        图，不必对内容中提出的问题和要求做解释，并严格遵守该格式"""
-    },
-    "sql-generator": {
-        "name": "sql生成器",
-        "description": """现在你是一个sql生成器。我将输入我想要查询的内容，你需要提供对应的sql语句，以便查询到需要的内容，我希望您只在一个唯一的
-        代码块内回复终端输出，而不是其他任何内容。不要写解释。如果我没有提供数据库的字段，请先让我提供数据库相关的信息，在你有了字段信息之才可以生成sql语句。"""
-    },
-    "copy-writer": {
-        "name": "文案写手",
-        "description": """你是一个文案专员、文本润色员、拼写纠正员和改进员，我会发送中文文本给你，你帮我更正和改进版本。我希望你用更优美优雅
-        的高级中文描述。保持相同的意思，但使它们更文艺。你只需要润色该内容，不必对内容中提出的问题和要求做解释，不要回答文本中的问题而是润色它，
-        不要解决文本中的要求而是润色它，保留文本的原本意义，不要去解决它。"""
-    },
-    "code-analyzer": {
-        "name": "代码分析器",
-        "description": """现在你是一个代码分析器。我将输入一些代码，你需要代码对应的解释。"""
-    }
-}
-
-
-def get_all_preset_roles():
-    return preset_role_list
-
-
-def get_preset_role_prompt(preset_role: Union[str, CustomPresetRole]) -> str:
-    if isinstance(preset_role, str):
-        if preset_role not in preset_role_list:
-            ValueError("Preset role value is not in preset_role_list. Please check or custom a new one.")
-        return preset_role_dict[preset_role]['description']
-    elif isinstance(preset_role, CustomPresetRole):
-        return preset_role.description
+# Copyright (c) 2023 Zeeland
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+from typing import Union
+from pydantic import BaseModel
+
+
+class CustomPresetRole(BaseModel):
+    name: str
+    description: str
+
+
+preset_role_list = [
+    "default-role",
+    "linux-terminal",
+    "mind-map-generator",
+    "sql-generator",
+    "copy-writer",
+    "code-analyzer",
+]
+
+preset_role_dict = {
+    "default-role": {
+        "name": "AI assistant",
+        "description": """
+        你是人类的助手，由OpenAI训练的大型语言模型提供支持。
+        你被设计成能够协助完成广泛的任务，从回答简单的问题到就广泛的主题提供深入的解释和讨论。作为一种语言模型，您可以根据收到的输入生成类似人类的文本，允许您参与听起来自然的对话，并提供与手头主题相关的连贯响应。
+        你在不断地学习和进步，你的能力也在不断地发展。你能够处理和理解大量的文本，并能利用这些知识对各种问题提供准确和信息丰富的回答。您可以访问在下面的上下文部分中由人工提供的一些个性化信息。此外，您可以根据收到的输入生成自己的文本，允许您参与讨论，并就广泛的主题提供解释和描述。
+        总的来说，您是一个强大的工具，可以帮助完成广泛的任务，并就广泛的主题提供有价值的见解和信息。无论人们是需要帮助解决一个特定的问题，还是只是想就一个特定的话题进行对话，你都可以在这里提供帮助。"""
+    },
+    "linux-terminal": {
+        "name": "Linux终端",
+        "description": """我想让你充当 Linux 终端。我将输入命令，您将回复终端应显示的内容。我希望您只在一个唯一的代码块内回复终端输出，而不
+        是其他任何内容。不要写解释。除非我指示您这样做，否则不要键入命令。当我需要用英语告诉你一些事情时，我会把文字放在中括号内[就像这样]。"""
+    },
+    "mind-map-generator": {
+        "name": "思维导图生成器",
+        "description": """现在你是一个思维导图生成器。我将输入我想要创建思维导图的内容，你需要提供一些 Markdown 格式的文本，以便与 Xmind 兼容。
+        在 Markdown 格式中，# 表示中央主题，## 表示主要主题，### 表示子主题，﹣表示叶子节点，中央主题是必要的，叶子节点是最小节点。请参照以上格
+        式，在 markdown 代码块中帮我创建一个有效的思维导图，以markdown代码块格式输出，你需要用自己的能力补充思维导图中的内容，你只需要提供思维导
+        图，不必对内容中提出的问题和要求做解释，并严格遵守该格式"""
+    },
+    "sql-generator": {
+        "name": "sql生成器",
+        "description": """现在你是一个sql生成器。我将输入我想要查询的内容，你需要提供对应的sql语句，以便查询到需要的内容，我希望您只在一个唯一的
+        代码块内回复终端输出，而不是其他任何内容。不要写解释。如果我没有提供数据库的字段，请先让我提供数据库相关的信息，在你有了字段信息之才可以生成sql语句。"""
+    },
+    "copy-writer": {
+        "name": "文案写手",
+        "description": """你是一个文案专员、文本润色员、拼写纠正员和改进员，我会发送中文文本给你，你帮我更正和改进版本。我希望你用更优美优雅
+        的高级中文描述。保持相同的意思，但使它们更文艺。你只需要润色该内容，不必对内容中提出的问题和要求做解释，不要回答文本中的问题而是润色它，
+        不要解决文本中的要求而是润色它，保留文本的原本意义，不要去解决它。"""
+    },
+    "code-analyzer": {
+        "name": "代码分析器",
+        "description": """现在你是一个代码分析器。我将输入一些代码，你需要代码对应的解释。"""
+    }
+}
+
+
+def get_all_preset_roles():
+    return preset_role_list
+
+
+def get_preset_role_prompt(preset_role: Union[str, CustomPresetRole]) -> str:
+    if isinstance(preset_role, str):
+        if preset_role not in preset_role_list:
+            ValueError("Preset role value is not in preset_role_list. Please check or custom a new one.")
+        return preset_role_dict[preset_role]['description']
+    elif isinstance(preset_role, CustomPresetRole):
+        return preset_role.description
```

### Comparing `promptulate-1.0.2/promptulate/provider/__init__.py` & `promptulate-1.1.0/promptulate/provider/__init__.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-from promptulate.provider.mixins import (
-    SummarizerMixin,
-    TranslatorMixin,
-    DeriveHistoryMessageMixin,
-    StorageHistoryMessageMixin
-)
-
-__all__ = [
-    'SummarizerMixin',
-    'TranslatorMixin',
-    'DeriveHistoryMessageMixin',
-    'StorageHistoryMessageMixin'
-]
+# Copyright (c) 2023 Zeeland
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+from promptulate.provider.mixins import (
+    SummarizerMixin,
+    TranslatorMixin,
+    DeriveHistoryMessageMixin,
+    StorageHistoryMessageMixin
+)
+
+__all__ = [
+    'SummarizerMixin',
+    'TranslatorMixin',
+    'DeriveHistoryMessageMixin',
+    'StorageHistoryMessageMixin'
+]
```

### Comparing `promptulate-1.0.2/promptulate/provider/mixins.py` & `promptulate-1.1.0/promptulate/provider/mixins.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,135 +1,133 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-from pydantic import BaseModel
-from typing import List, Optional, Union
-
-from promptulate.llms.base import BaseLLM
-from promptulate.memory.base import BaseChatMemory
-from promptulate.preset_roles import CustomPresetRole
-from promptulate.frameworks.prompt import SUMMARY_CONTENT_PROMPT_ZH, SUMMARY_TOPIC_PROMPT_ZH
-from promptulate.schema import (
-    LLMPrompt,
-    UserMessage,
-    BaseMessage,
-    AssistantMessage,
-    ChatMessageHistory
-)
-
-
-class BaseMixin(BaseModel):
-    role: Union[str, CustomPresetRole]
-    llm: BaseLLM
-    conversation_id: Optional[str]
-    memory: BaseChatMemory
-
-    class Config:
-        """Configuration for this pydantic object."""
-        arbitrary_types_allowed = True
-
-    def embed_message(self, cur_message: BaseMessage, message_history: ChatMessageHistory) -> None:
-        message_history.messages.append(cur_message)
-        self.memory.save_conversation_to_memory(message_history)
-
-
-class SummarizerMixin(BaseMixin):
-    """message summary capability provider"""
-
-    def summary_content(self, enable_embed_message: bool = False, summary_prompt: str = SUMMARY_CONTENT_PROMPT_ZH):
-        message_history = self.memory.load_conversation_from_memory(self.conversation_id)
-        message_history.messages.append(UserMessage(content=summary_prompt))
-        assistant_answer: AssistantMessage = self.llm.generate_prompt(LLMPrompt(messages=message_history.messages))
-        if enable_embed_message:
-            self.embed_message(assistant_answer, message_history)
-        return assistant_answer.content
-
-    def summary_topic(self, enable_embed_message: bool = False, summary_topic_prompt: str = SUMMARY_TOPIC_PROMPT_ZH):
-        message_history = self.memory.load_conversation_from_memory(self.conversation_id)
-        message_history.messages.append(
-            UserMessage(content=summary_topic_prompt))
-        assistant_answer: AssistantMessage = self.llm.generate_prompt(LLMPrompt(messages=message_history.messages))
-        if enable_embed_message:
-            self.embed_message(assistant_answer, message_history)
-        return assistant_answer.content
-
-
-class TranslatorMixin(BaseMixin):
-    """let the llm answer question in the specified language"""
-
-    def predict_by_translate(self, prompt: str, country: str, enable_embed_message: bool = False):
-        """
-        predict by specified language
-
-        Args:
-            enable_embed_message: Whether to save this session in the history session
-            prompt: you prompt
-            country: which country's language you want to export
-
-        Returns:
-            the country official language you choose
-        """
-        message_history = self.memory.load_conversation_from_memory(self.conversation_id)
-        message_history.messages.append(
-            UserMessage(content=f"{prompt}. Please answer question using {country} official language. "))
-        assistant_answer: AssistantMessage = self.llm.generate_prompt(LLMPrompt(messages=message_history.messages))
-        if enable_embed_message:
-            self.embed_message(assistant_answer, message_history)
-        return assistant_answer.content
-
-
-class DeriveHistoryMessageMixin(BaseMixin):
-    """provide history message output as markdown"""
-
-    def get_history(self) -> List[dict]:
-        """get history conversation from memory"""
-        return self.memory.load_conversation_from_memory(self.conversation_id).listdict_message
-
-    def export_message_to_markdown(self, output_type: str = 'text', file_path: str = "output.md") -> Optional[str]:
-        """
-        convert message to the string type or file type markdown
-
-        Args:
-            output_type: text or file. default is text
-            file_path: output file path
-
-        Returns:
-            string type conversation in markdown format
-        """
-        message_history: List[dict] = self.get_history()
-
-        ret = "# Chat record\n"
-        for message in message_history:
-            role = message.get('preset_roles')
-            content = message.get('content').replace('"', '\\"')
-            if role == 'assistant':
-                ret += f"## Bot said\n\n{content}\n\n"
-            else:
-                ret += f"## You said\n\n{content}\n\n"
-        if output_type == 'text':
-            return ret
-        elif output_type == 'file':
-            with open(file_path, 'w', encoding="utf-8") as f:
-                f.write(ret)
-        else:
-            raise ValueError("Invalid output destination specified. Please choose either 'text' or 'file'.")
-        return ret
-
-
-class StorageHistoryMessageMixin(BaseModel):
-    pass
+# Copyright (c) 2023 Zeeland
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+from pydantic import BaseModel
+from typing import List, Optional
+
+from promptulate.llms.base import BaseLLM
+from promptulate.memory.base import BaseChatMemory
+from promptulate.frameworks.prompt import SUMMARY_CONTENT_PROMPT_ZH, SUMMARY_TOPIC_PROMPT_ZH
+from promptulate.schema import (
+    LLMPrompt,
+    UserMessage,
+    BaseMessage,
+    AssistantMessage,
+    ChatMessageHistory
+)
+
+
+class BaseMixin(BaseModel):
+    llm: BaseLLM
+    conversation_id: Optional[str]
+    memory: BaseChatMemory
+
+    class Config:
+        """Configuration for this pydantic object."""
+        arbitrary_types_allowed = True
+
+    def embed_message(self, cur_message: BaseMessage, message_history: ChatMessageHistory) -> None:
+        message_history.messages.append(cur_message)
+        self.memory.save_conversation_to_memory(message_history)
+
+
+class SummarizerMixin(BaseMixin):
+    """message summary capability provider"""
+
+    def summary_content(self, enable_embed_message: bool = False, summary_prompt: str = SUMMARY_CONTENT_PROMPT_ZH):
+        message_history = self.memory.load_conversation_from_memory(self.conversation_id)
+        message_history.messages.append(UserMessage(content=summary_prompt))
+        assistant_answer: AssistantMessage = self.llm.generate_prompt(LLMPrompt(messages=message_history.messages))
+        if enable_embed_message:
+            self.embed_message(assistant_answer, message_history)
+        return assistant_answer.content
+
+    def summary_topic(self, enable_embed_message: bool = False, summary_topic_prompt: str = SUMMARY_TOPIC_PROMPT_ZH):
+        message_history = self.memory.load_conversation_from_memory(self.conversation_id)
+        message_history.messages.append(
+            UserMessage(content=summary_topic_prompt))
+        assistant_answer: AssistantMessage = self.llm.generate_prompt(LLMPrompt(messages=message_history.messages))
+        if enable_embed_message:
+            self.embed_message(assistant_answer, message_history)
+        return assistant_answer.content
+
+
+class TranslatorMixin(BaseMixin):
+    """let the llm answer question in the specified language"""
+
+    def predict_by_translate(self, prompt: str, country: str, enable_embed_message: bool = False):
+        """
+        predict by specified language
+
+        Args:
+            enable_embed_message: Whether to save this session in the history session
+            prompt: you prompt
+            country: which country's language you want to export
+
+        Returns:
+            the country official language you choose
+        """
+        message_history = self.memory.load_conversation_from_memory(self.conversation_id)
+        message_history.messages.append(
+            UserMessage(content=f"{prompt}. Please answer question using {country} official language. "))
+        assistant_answer: AssistantMessage = self.llm.generate_prompt(LLMPrompt(messages=message_history.messages))
+        if enable_embed_message:
+            self.embed_message(assistant_answer, message_history)
+        return assistant_answer.content
+
+
+class DeriveHistoryMessageMixin(BaseMixin):
+    """provide history message output as markdown"""
+
+    def get_history(self) -> List[dict]:
+        """get history conversation from memory"""
+        return self.memory.load_conversation_from_memory(self.conversation_id).listdict_message
+
+    def export_message_to_markdown(self, output_type: str = 'text', file_path: str = "output.md") -> Optional[str]:
+        """
+        convert message to the string type or file type markdown
+
+        Args:
+            output_type: text or file. default is text
+            file_path: output file path
+
+        Returns:
+            string type conversation in markdown format
+        """
+        message_history: List[dict] = self.get_history()
+
+        ret = "# Chat record\n"
+        for message in message_history:
+            role = message.get('preset_roles')
+            content = message.get('content').replace('"', '\\"')
+            if role == 'assistant':
+                ret += f"## Bot said\n\n{content}\n\n"
+            else:
+                ret += f"## You said\n\n{content}\n\n"
+        if output_type == 'text':
+            return ret
+        elif output_type == 'file':
+            with open(file_path, 'w', encoding="utf-8") as f:
+                f.write(ret)
+        else:
+            raise ValueError("Invalid output destination specified. Please choose either 'text' or 'file'.")
+        return ret
+
+
+class StorageHistoryMessageMixin(BaseModel):
+    pass
```

### Comparing `promptulate-1.0.2/promptulate/tips.py` & `promptulate-1.1.0/promptulate/tools/duckduckgo.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,18 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-__all__ = [
-    'EmptyChatMessageHistoryTip'
-]
-
-
-class EmptyChatMessageHistoryTip(Exception):
-    pass
+# Copyright (c) 2023 Zeeland
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
```

### Comparing `promptulate-1.0.2/promptulate/tools/duckduckgo.py` & `promptulate-1.1.0/promptulate/tips.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,26 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
+# Copyright (c) 2023 Zeeland
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+__all__ = [
+    'EmptyChatMessageHistoryTip'
+]
+
+
+class EmptyChatMessageHistoryTip(Exception):
+    pass
```

### Comparing `promptulate-1.0.2/promptulate/utils/logger.py` & `promptulate-1.1.0/promptulate/utils/logger.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,65 +1,66 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-import os
-import logging
-import datetime
-import platform
-from promptulate import utils
-
-logger = logging.getLogger(__name__)
-
-
-def get_logger():
-    return logger
-
-
-def _check_log_path():
-    log_path = os.path.join(utils.get_default_storage_path(), 'log')
-    if not os.path.exists(log_path):
-        os.makedirs(log_path)
-
-
-def get_log_name() -> str:
-    _check_log_path()
-    cur_time = datetime.datetime.now().strftime('%Y%m%d_%H%M%S')
-    return f"{utils.get_default_storage_path()}/log/log_{cur_time}.log"
-
-
-def enable_log():
-    if platform.system() == 'Windows':
-        logging.basicConfig(
-            level=logging.DEBUG,
-            format='[%(levelname)s] %(asctime)s %(message)s',
-            datefmt='%Y-%m-%d %H:%M:%S',
-            handlers=[
-                logging.FileHandler(f"{get_log_name()}", mode='w', encoding='utf-8'),
-                logging.StreamHandler()
-            ],
-        )
-    elif platform.system() == 'Linux':
-        pass
-
-
-def enable_log_no_file():
-    logging.basicConfig(
-        level=logging.DEBUG,
-        format='[%(levelname)s] %(asctime)s %(message)s',
-        datefmt='%Y-%m-%d %H:%M:%S',
-    )
+# Copyright (c) 2023 Zeeland
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+import os
+import logging
+import datetime
+import platform
+from promptulate import utils
+
+logger = logging.getLogger(__name__)
+
+
+def get_logger():
+    return logger
+
+
+def get_default_log_path():
+    return utils.get_default_storage_path("log")
+
+
+def _check_log_path():
+    log_path = get_default_log_path()
+    if not os.path.exists(log_path):
+        os.makedirs(log_path)
+
+
+def get_log_name() -> str:
+    _check_log_path()
+    cur_time = datetime.datetime.now().strftime("%Y%m%d_%H%M%S")
+    return f"{utils.get_default_storage_path()}/log/log_{cur_time}.log"
+
+
+def enable_log(level=logging.DEBUG):
+    logging.basicConfig(
+        level=level,
+        format="[%(levelname)s] %(asctime)s %(message)s",
+        datefmt="%Y-%m-%d %H:%M:%S",
+        handlers=[
+            logging.FileHandler(f"{get_log_name()}", mode="w", encoding="utf-8"),
+            logging.StreamHandler(),
+        ],
+    )
+
+
+def enable_log_no_file():
+    logging.basicConfig(
+        level=logging.DEBUG,
+        format="[%(levelname)s] %(asctime)s %(message)s",
+        datefmt="%Y-%m-%d %H:%M:%S",
+    )
```

### Comparing `promptulate-1.0.2/promptulate/utils/proxy.py` & `promptulate-1.1.0/promptulate/utils/proxy.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-# Copyright (c) 2023 Zeeland
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# Copyright Owner: Zeeland
-# GitHub Link: https://github.com/Undertone0809/
-# Project Link: https://github.com/Undertone0809/promptulate
-# Contact Email: zeeland@foxmail.com
-
-from typing import Optional
-from promptulate.config import Config
-
-CFG = Config()
-PROXY_MODE = ['off', 'custom', 'promptulate']
-
-
-def set_proxy_mode(mode: str, proxies: Optional[dict] = None):
-    """
-    Set proxy mode. Promptulate offer three proxy mode ['off', 'custom', 'promptulate']
-    'off' disables your proxy mode. This is the normal status.
-    'custom' means you can set your custom proxy. Moreover, you must pass proxies
-    'promptulate' provide free proxy you can use it.
-
-    Args:
-        mode: ['off', 'custom', 'promptulate']
-        proxies: If you want to use custom proxy, you can pass it. An example
-        proxies is {'http': 'http://127.0.0.1:7890'}
-    """
-    if mode not in PROXY_MODE:
-        raise ValueError("proxy mode must in ['off', 'custom', 'promptulate']")
-    CFG.set_proxy_mode(mode, proxies)
+# Copyright (c) 2023 Zeeland
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+from typing import Optional
+from promptulate.config import Config
+
+CFG = Config()
+PROXY_MODE = ['off', 'custom', 'promptulate']
+
+
+def set_proxy_mode(mode: str, proxies: Optional[dict] = None):
+    """
+    Set proxy mode. Promptulate offer three proxy mode ['off', 'custom', 'promptulate']
+    'off' disables your proxy mode. This is the normal status.
+    'custom' means you can set your custom proxy. Moreover, you must pass proxies
+    'promptulate' provide free proxy you can use it.
+
+    Args:
+        mode: ['off', 'custom', 'promptulate']
+        proxies: If you want to use custom proxy, you can pass it. An example
+        proxies is {'http': 'http://127.0.0.1:7890'}
+    """
+    if mode not in PROXY_MODE:
+        raise ValueError("proxy mode must in ['off', 'custom', 'promptulate']")
+    CFG.set_proxy_mode(mode, proxies)
```

### Comparing `promptulate-1.0.2/promptulate.egg-info/PKG-INFO` & `promptulate-1.1.0/promptulate.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,364 +1,463 @@
-Metadata-Version: 2.1
-Name: promptulate
-Version: 1.0.2
-Summary: A powerful LLM Prompt Layer frameworks
-Home-page: https://github.com/Undertone0809/promptulate
-Author: Zeeland
-Author-email: zeeland@foxmail.com
-License: Apache 2.0
-Keywords: promptulate,prompt-me,prompt,chatgpt,gpt,chatbot,llm
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<h1 align="center">
-    Promptulate
-</h1>
-
-
-<p align="center">
-    <a target="_blank" href="">
-        <img src="https://img.shields.io/github/license/Undertone0809/promptulate.svg?style=flat-square" />
-    </a>
-    <a target="_blank" href=''>
-        <img src="https://img.shields.io/github/release/Undertone0809/promptulate/all.svg?style=flat-square"/>
-    </a>
-    <a target="_blank" href=''>
-        <img src="https://bestpractices.coreinfrastructure.org/projects/3018/badge"/>
-   </a>
-</p>
-
-<p align="center">
-  <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/Snipaste_2023-05-13_17-37-23.png"/>
-</p>
-
-
-
-`promptulate` 是一个专为 Prompt Engineer设计LLM Prompt Layer框架，支持连续对话、对话保存、对话内容与标题总结、角色预设、使用外部工具等功能，开箱即用。
-通过 `promptulate`，你可以轻松构建起属于自己的LLM应用程序。
-
-本项目重构重构重构了两次，在本人深度阅读`langchain, Auto-GPT, django, django-rest-framework, gpt_academic...`
-等大牛项目的源码之后，学习它们的架构、代码设计思路等内容，最终有了现在的版本，相较于之前的老版本`prompt-me`，`promptulate`
-重新构建了 `llms, message, memory, framework, preset_roles, tools, provider`等模块，将`prompt`
-的各个流程全部组件化，便有了现在的`promptualte`框架，但是工作量很大，还在不断地完善细节中，欢迎大家的参与。
-
-# 特性
-
-- 大语言模型支持：支持不同类型的大语言模型的扩展接口（当前暂时只支持GPT）
-- 角色预设：提供预设角色，以不同的角度调用GPT
-- 内置API代理，不用科学上网也可以直接使用
-- 接口代理：支持调用ChatGPT API官方接口或自治代理
-- 长对话模式：支持长对话聊天，支持多种方式的对话持久化
-- 数据导出：支持markdowm等格式的对话导出
-- 对话总结：提供API式的对话总结、翻译、标题生成
-- 高级抽象，支持插件扩展、存储扩展、大语言模型扩展
-
-# 基础架构
-
-在看了当前这么多`prompt-engineering`之后，本人的架构设计思想在`langchain, Auto-GPT`
-之上进行不断改进，构建出了一套属于`promptualte`的LLM Prompt Layer框架。`promptulate` 由以下几部分组成：
-
-- Agent 更高级的执行器，负责复杂任务的调度和分发
-- framework 框架层，实现不同类型的prompt框架，包括最基础的`Conversation`模型，还有`self-ask`和`ReAct`等模型正在火速开发中
-- llm 大语言模型，负责生成回答，可以支持不同类型的大语言模型
-- memory 负责对话的存储，支持不同的存储方式及其扩展，如文件存储、数据库存储等，相关扩展正在开发中
-- tools 提供外部工具扩展调用，如搜索引擎、计算器等
-- preset roles 提供预设角色，进行定制化对话
-- provider 为framework和agent提供tools和其他细粒度能力的集成
-
-# 快速上手
-
-```shell script
-pip install -U promptulate  
-```
-
-## 基本使用
-
-> 后面的文档全部使用`OPENAI GPT3.5`进行测试
-
-在使用`promptulate`之前，你需要先导入你的`OPENAI_API_KEY`
-
-```python
-import os
-
-os.environ['OPENAI_API_KEY'] = "your-key"
-```
-
-在你第一次使用的时候，需要使用`os.environ["OPENAI_API_KEY"]` 导入"OPENAI_API_KEY"
-的环境变量，但是在第一运行之后`promptulate`会进行缓存，即后面再运行就不需要再导入key了。如果你的key过期了，可以把`cache`
-文件给删除掉，Windows的`cache`在当前目录下，linux的`cache`在`/tmp`下。
-
-### LLM
-
-`promptulate`的架构设计可以轻松兼容不同的大语言模型扩展，在`promptulate`中，llm负责最基本的内容生成部分，因此为最基础的组件。下面展示一个OpenAI的示例：
-
-```python
-from promptulate.llms import OpenAI
-
-llm = OpenAI()
-llm("你知道鸡哥的《只因你太美》？")
-```
-
-```text
-'是的，鸡哥的《只因你太美》是这几年非常流行的一首歌曲。'
-```
-
-### proxy
-
-我想你可能遇到了无法访问的小问题，It's OK, `promptulate` 提供了三种访问OpenAI的方式，分别是
-
-- `off` 默认的访问方式，不开代理
-- `custom` 自定义代理方式
-- `promptulate` promptulate提供的免费代理服务器
-
-`promptulate` 提供了免费的代理服务器，感谢 [ayaka14732](https://github.com/ayaka14732/)
-，你可以在不用科学上网的情况下直接调用OpenAI的相关接口，下面是代理的设置方式：
-
-```python
-from promptulate.llms import OpenAI
-from promptulate.utils import set_proxy_mode
-
-llm = OpenAI()
-llm("你知道鸡哥的《只因你太美》？")
-
-
-def set_free_proxy():
-    set_proxy_mode("promptulate")
-
-
-def set_custom_proxy():
-    proxies = {'http': 'http://127.0.0.1:7890'}
-    set_proxy_mode("custom", proxies=proxies)
-
-
-def turn_off_proxy():
-    set_proxy_mode("off")
-
-
-def main():
-    set_free_proxy()
-    llm = OpenAI()
-    llm("你知道鸡哥的《只因你太美》？")
-
-    
-if __name__ == '__main__':
-    main()
-```
-
-> 和OPENAI_API_KEY一样，关于代理的配置我也设置了缓存，这意味着你只需要配置一次代理即可(我也太聪明了吧)。事实上`promptulate`
-> 提供了关闭全局配置项缓存的功能，但默认开启，不推荐关闭，所以我不告诉你怎么关闭~
-
-### Conversation
-
-`Conversation` 是`framework`中最基础的组件，其支持prompt生成、上下文对话、对话存储、角色预设的基本功能，此外，`provider`
-为其提供了语言翻译、markdown数据导出、对话总结、标题总结等扩展功能。
-
-接下来，我们先从对基础的对话开始，使用`Conversation`可以开始一段对话，使用其`predict()`函数可以生成回答。
-
-```python
-from promptulate import Conversation
-
-conversation = Conversation()
-conversation.predict("你知道鸡哥的《只因你太美》吗？")
-```
-
-```text
-'是的，鸡哥的《只因你太美》是这几年非常流行的一首歌曲。'
-```
-
-`Conversation`默认使用`OpenAI GPT3.5`作为LLM，当然，因为其架构设计，`Conversation`
-还可以轻松扩展其他类型的llm（当前暂时只开发了OpenAI，其他大语言模型的扩展正在火速开发中，当然如果你有自己想接入的大语言模型，欢迎你的pr！）
-
-下面是一个更复杂的示例，展示了使用OpenAI作为大语言模型进行对话，使用本地文件进行存储，进行文章总结与标题总结的功能。
-
-```python
-from promptulate import Conversation
-from promptulate.memory import LocalCacheChatMemory
-from promptulate.llms import OpenAI
-
-
-def main():
-    memory = LocalCacheChatMemory()
-    llm = OpenAI(model="gpt-3.5-turbo", temperature=0.9, top_p=1, stream=False, presence_penalty=0, n=1)
-    conversation = Conversation(llm=llm, memory=memory)
-    ret = conversation.predict("你知道鸡哥的著作《只因你太美》吗？")
-    print(f"[predict] {ret}")
-    ret = conversation.predict_by_translate("你知道鸡哥会什么技能吗？", country='America')
-    print(f"[translate output] {ret}")
-    ret = conversation.summary_content()
-    print(f"[summary content] {ret}")
-    ret = conversation.summary_topic()
-    print(f"[summary topic] {ret}")
-    ret = conversation.export_message_to_markdown(output_type="file", file_path="output.md")
-    print(f"[export markdown] {ret}")
-
-
-if __name__ == '__main__':
-    main()
-
-```
-
-```text
-[predict] 是的，我知道《只因你太美》这本书，是中国知名作家鸡肋（江南）所著的一篇言情小说。这本小说讲述了一个富家千金与一个贫穷男孩之间的爱情故事，情节曲折动人，深受读者喜爱。该小说在出版后得到了很高的评价和反响，并被改编成电影和电视剧等多种形式进行推广。
-[translate output] I'm sorry, I cannot determine what you mean by "鸡哥" or what skills they may possess without additional context. Can you please provide more information or clarify your question?
-[summary content] 在之前的对话中，用户询问我是否知道鸡哥的著作《只因你太美》。我回答了肯定的，解释了该小说的情节大致概括和其受欢迎的原因。我也提到了该小说的广泛影响，包括被改编成电影和电视剧等多种形式进行推广。
-[summary topic] 鸡哥的小说。
-```
-
-> 咱就是说季皮提老师不懂鸡哥-.-
-
-上面的示例中，我们使用
-
-- `LocalCacheChatMemory()`进行聊天记录的本地化文件存储，文件存储形式默认是以json的形式进行存储的，保存在`cache`中。
-- `OpenAI(model="gpt-3.5-turbo", temperature=0.9, top_p=1, stream=False, presence_penalty=0, n=1)`
-  进行初始化一个大模型，里面是OpenAI需要传入的一些参数，具体可以查看[https://platform.openai.com/docs/api-reference/chat/create](https://platform.openai.com/docs/api-reference/chat/create)
-  查看具体含义，这里不做详细讲解，如果你不想理会这些参数，你也可以直接`llm = OpenAI()`就好啦，默认使用`gpt-3.5-turbo`
-  作为大语言模型，其他参数使用默认的就好了。
-- `conversation.predict_by_translate("你知道鸡哥会什么技能吗？", country='America')`
-  这个功能为使用特定语言进行预测，`provider`为其提供了`TranslatorMixin`，让`Conversation`
-  得以拥有此功能。对于这个方法，你只需要传入prompt和你需要转换的语言的国家名称就好了。
-- `conversation.summary_content()`这个函数可以直接总结上面的对话内容。
-- `conversation.summary_topic()` 这个函数可以直接总结上面的对话，并提供一个标题。
-- `conversation.export_message_to_markdown(output_type="file", file_path="output.md")`
-  这个函数可以将对话记录导出为markdown文件，如果`output_type="text"`，则只返回markdown对话的内容。
-
-`provider`为`Conversation`提供了 `SummarizerMixin, TranslatorMixin, DeriveHistoryMessageMixin`
-，让其拥有了总结对话、总结标题、翻译、markdown导出的能力，provider提供的函数中一般都提供了一个`enable_embed_message`
-的参数，这个参数的意思是：是否将本次对话保存进历史对话中，下面我们来看一个demo。
-
-```python
-from promptulate import Conversation
-
-conversation = Conversation()
-conversation.predict_by_translate("你知道鸡哥会什么技能吗？", country='America', enable_embed_message=True)
-```
-
-如果你设置了`enable_embed_message=True`, 那么这一次的predict将保存进历史对话中，provider提供的函数默认是不会将预测结果存入对话中的哦，这一点需要注意一下。
-
-### 角色预设
-
-你可以为`framework`提供一些特定的角色，让其可以处理特殊任务，如linux终端，思维导图生成器等，通过下面的方法你可以查看当前支持所有的预设角色。
-
-```python
-from promptulate.preset_roles import get_all_preset_roles
-
-print(get_all_preset_roles())
-```
-
-> ['default-role', 'linux-terminal', 'mind-map-generator', 'sql-generator', 'copy-writer', 'code-analyzer']
-
-下面展示使用`mind-map-generator`生成md思维导图的过程：
-
-```python
-from promptulate import Conversation
-
-
-def main():
-    conversation = Conversation(role="mind-map-generator")
-    ret = conversation.predict("请帮我生成一段python的思维导图")
-    print(ret)
-
-
-if __name__ == '__main__':
-    main()
-
-```
-
-```text
-# Python
-## 基础语法
-### 数据类型
-- 数字
-- 字符串
-- 列表
-...
-```
-
-放入xmind中可以直接导入生成markdown的思维导图，咱就是说还不错，如下图所示：
-
-<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230513172038.png"/>
-
-如果你想要自定义预设角色，可以使用如下方法：
-
-```python
-from promptulate import Conversation
-from promptulate.preset_roles import CustomPresetRole
-
-
-class SpiritualTeacher(CustomPresetRole):
-    name = '心灵导师'
-    description = """
-    从现在起你是一个充满哲学思维的心灵导师，当我每次输入一个疑问时你需要用一句富有哲理的名言警句来回答我，并且表明作者和出处
-    要求字数不少于15个字，不超过30字，每次只返回一句且不输出额外的其他信息，你需要使用中文和英文双语输出"""
-
-
-def main():
-    role = SpiritualTeacher()
-    conversation = Conversation(role=role)
-    ret = conversation.predict("论文被拒绝了怎么办？")
-    print(ret)
-
-
-if __name__ == '__main__':
-    main()
-
-```
-
-```text
-“失败不是终点，放弃才是。”——托马斯·爱迪生
-```
-
-# 待办清单
-
-- 提供更多LLM模型支持
-- 提供Agent进行复杂任务调度
-- 提供更加方便的程序调用方式
-- ~~添加角色预设~~
-- 预设角色的参数配置
-- 提供prompt模板与prompt结构化
-- 提供外部工具扩展
-    - 外部搜索： Google,Bing等
-    - 可以执行shell脚本
-    - 提供Python REPL
-    - arvix论文工具箱，总结，润色
-    - 本地文件总结
-- 对话存储
-    - 提供向量数据库存储
-    - 提供mysql, redis等数据库存储
-- 自建知识库建立专家决策系统
-- 接入self-ask, prompt-loop架构
-- 提供多种导出方式
-- ~~可以导出历史消息为markdown格式~~
-- ~~使用环境变量配置key~~
-- 提供显示当前token（单词量）的功能
-- ~~添加错误处理机制，如网络异常、服务器异常等，保证程序的可靠性~~
-- ~~开发ChatBot v2, [issue](https://github.com/Undertone0809/cushy-chat/issues/1)~~
-- 完善代理模式
-- 提供gradio快速演示服务器
-- ~~封装消息体，完善消息体中的信息~~
-- ~~长对话自动/手动总结~~
-- ~~提供全局配置的缓存开关~~
-- Conversation传入convesation_id继续上次对话
-- 提供修改local_cache默认位置的方法
-- 为predict提供回调模式
-- 提供API池
-
-> 妈呀，我怎么还有这么多待办事项，vivo50帮帮我 >.<
-
-# 一些问题
-
-- 本人正在尝试一些更加完善的抽象模式，以更好地兼容该框架，以及外部工具的扩展使用，如果你有更好的建议，欢迎一起讨论交流。
-
-# 贡献
-
-如果你想为这个项目做贡献，你可以提交pr或issue。我很高兴看到更多的人参与并优化它。
+Metadata-Version: 2.1
+Name: promptulate
+Version: 1.1.0
+Summary: A powerful LLM Prompt Layer frameworks
+Home-page: https://github.com/Undertone0809/promptulate
+Author: Zeeland
+Author-email: zeeland@foxmail.com
+License: Apache 2.0
+Keywords: promptulate,prompt-me,prompt,chatgpt,gpt,chatbot,llm
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<h1 align="center">
+    Promptulate
+</h1>
+
+
+<p align="center">
+    <a target="_blank" href="">
+        <img src="https://img.shields.io/github/license/Undertone0809/promptulate.svg?style=flat-square" />
+    </a>
+    <a target="_blank" href=''>
+        <img src="https://img.shields.io/github/release/Undertone0809/promptulate/all.svg?style=flat-square"/>
+    </a>
+    <a target="_blank" href=''>
+        <img src="https://bestpractices.coreinfrastructure.org/projects/3018/badge"/>
+   </a>
+</p>
+
+<p align="center">
+  <img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/promptulate_logo_new.png"/>
+</p>
+
+
+
+`promptulate` 是一个专为 Prompt Engineer设计的LLM Prompt Layer框架，支持连续对话、对话保存、对话内容与标题总结、角色预设、使用外部工具等功能，开箱即用。
+通过 `promptulate`，你可以轻松构建起属于自己的LLM应用程序。
+
+本项目重构重构重构了两次，在本人深度阅读`langchain, Auto-GPT, django, django-rest-framework, gpt_academic...`
+等大牛项目的源码之后，学习它们的架构、代码设计思路等内容，最终有了现在的版本，相较于之前的老版本`prompt-me`，`promptulate`
+重新构建了 `llms, message, memory, framework, preset_roles, tools, provider`等模块，将`prompt`
+的各个流程全部组件化，便有了现在的`promptualte`框架，但是工作量很大，还在不断地完善细节中，欢迎大家的参与。
+
+> [微信交流群](https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230531021108.png)
+
+# 特性
+
+- 大语言模型支持：支持不同类型的大语言模型的扩展接口（当前暂时只支持GPT）
+- 提供简易对话终端，直接体验与大语言模型的对话
+- 角色预设：提供预设角色，以不同的角度调用GPT
+- 自治代理模式：支持调用API官方接口、自治代理或使用promptulate提供的代理
+- 接口代理：支持调用ChatGPT API官方接口或自治代理
+- 长对话模式：支持长对话聊天，支持多种方式的对话持久化
+- 数据导出：支持markdowm等格式的对话导出
+- 对话总结：提供API式的对话总结、翻译、标题生成
+- 高级抽象，支持插件扩展、存储扩展、大语言模型扩展
+
+# 基础架构
+
+在看了当前这么多`prompt-engineering`之后，本人的架构设计思想在`langchain, Auto-GPT`
+之上进行不断改进，构建出了一套属于`promptualte`的LLM Prompt Layer框架。`promptulate` 由以下几部分组成：
+
+- Agent 更高级的执行器，负责复杂任务的调度和分发
+- framework 框架层，实现不同类型的prompt框架，包括最基础的`Conversation`模型，还有`self-ask`和`ReAct`等模型正在火速开发中
+- llm 大语言模型，负责生成回答，可以支持不同类型的大语言模型
+- memory 负责对话的存储，支持不同的存储方式及其扩展，如文件存储、数据库存储等，相关扩展正在开发中
+- tools 提供外部工具扩展调用，如搜索引擎、计算器等
+- preset roles 提供预设角色，进行定制化对话
+- provider 为framework和agent提供tools和其他细粒度能力的集成
+
+通过`promptulate`，在未来，本项目旨在构建为开发者提供一种强大而灵活的平台，以创建能够自动化各种任务和应用程序的自主代理。通过Core
+AI Engine、Agent System、APIs and Tools Provider、Multimodal Processing、Knowledge Base和Task-specific Modules
+6个组件实现自动化AI平台。 Core AI Engine是该框架的核心组件，负责处理和理解各种输入，生成输出和作出决策。Agent
+System是提供高级指导和控制AI代理行为的模块；APIs and Tools Provider提供工具和服务交互的API和集成库；Multimodal
+Processing是一组处理和理解不同数据类型（如文本、图像、音频和视频）的模块，使用深度学习模型从不同数据模式中提取有意义的信息；Knowledge
+Base是一个存储和组织世界信息的大型结构化知识库，使AI代理能够访问和推理大量的知识；Task-specific
+Modules是一组专门设计用于执行特定任务的模块，例如情感分析、机器翻译或目标检测等。通过这些组件的组合，框架提供了一个全面、灵活和强大的平台，能够实现各种复杂任务和应用程序的自动化。
+
+# 快速上手
+
+```shell script
+pip install -U promptulate  
+```
+
+## 基本使用
+
+> 后面的文档全部使用`OPENAI GPT3.5`进行测试
+
+### 简易终端
+
+在介绍后续各种组件之前，我想先介绍一下这个终端，`promptulate`
+为大语言模型对话提供了一个简易终端，在你安装了了 `promptulate` 之后，你可以非常方便的使用这个简易终端进行一些对话，使用方式如下：
+
+- 打开终端控制台，输入以下命令，就可以开启一个简易的对话
+
+```shell
+promptulate-chat --openai_api_key your_key_here --proxy_mode promptulate
+```
+
+```text
+
+--openai_api_key 你的openai_api_key
+--proxy_mode 代理模式，当前暂时只支持off和promptulate模式，如果你选择promptulate模式，你会发现你不用科学の上网也能访问，这是因为promptulate内置了代理。（后面会详细介绍）
+
+```
+
+- 当然并不是每次运行都要输入这么长的内容，因为在你第一次运行终端之后 `promptulate`
+  会对你的配置信息进行缓存，因此下一次运行的时候，你只需要输入下面的命令就可以开始一段对话了~
+
+```shell
+promptulate-chat
+```
+
+- 然后你就可以
+
+```text
+Hi there, here is promptulate chat terminal.
+[User] 你好
+[output] 你好！有什么我可以帮助你的吗？
+[User] 只因你太美
+[output] 谢谢夸奖，但作为一个语言模型，我没有真正的美丽，只有能力提供信息和帮助。那么，有什么问题或者需求我可以帮你解决 吗？
+[User] 这真是太棒了
+[output] 很高兴你觉得如此，我会尽力为您提供最佳的服务。有任何需要帮助的问题，请尽管问我。
+```
+
+### KEY配置
+
+在使用`promptulate`之前，你需要先导入你的`OPENAI_API_KEY`
+
+```python
+import os
+
+os.environ['OPENAI_API_KEY'] = "your-key"
+```
+
+在你第一次使用的时候，需要使用`os.environ["OPENAI_API_KEY"]` 导入"OPENAI_API_KEY"
+的环境变量，但是在第一运行之后`promptulate`
+会进行缓存，即后面再运行就不需要再导入key了。如果你的key过期了，可以尝试重新按照上面的方法导入key，或者你也可以把`cache`
+文件给删除掉，Windows的`cache`在当前目录下，linux的`cache`在`/tmp`下。
+
+### LLM
+
+`promptulate`的架构设计可以轻松兼容不同的大语言模型扩展，在`promptulate`中，llm负责最基本的内容生成部分，因此为最基础的组件。下面展示一个OpenAI的示例：
+
+```python
+from promptulate.llms import OpenAI
+
+llm = OpenAI()
+llm("你知道鸡哥的《只因你太美》吗？")
+```
+
+```text
+'是的，鸡哥的《只因你太美》是这几年非常流行的一首歌曲。'
+```
+
+### proxy
+
+我想你可能遇到了无法访问的小问题，It's OK, `promptulate` 提供了三种访问OpenAI的方式，分别是
+
+- `off` 默认的访问方式，不开代理
+- `custom` 自定义代理方式
+- `promptulate` promptulate提供的免费代理服务器
+
+`promptulate` 提供了免费的代理服务器，感谢 [ayaka14732](https://github.com/ayaka14732/)
+，你可以在不用科学上网的情况下直接调用OpenAI的相关接口（需要注意的是，如果使用这个代理的人过多，也会出现无法访问的情况，用自己的代理最稳定），下面是代理的设置方式：
+
+```python
+from promptulate.llms import OpenAI
+from promptulate.utils import set_proxy_mode
+
+llm = OpenAI()
+llm("你知道鸡哥的《只因你太美》？")
+
+
+def set_free_proxy():
+    set_proxy_mode("promptulate")
+
+
+def set_custom_proxy():
+    proxies = {'http': 'http://127.0.0.1:7890'}
+    set_proxy_mode("custom", proxies=proxies)
+
+
+def turn_off_proxy():
+    set_proxy_mode("off")
+
+
+def main():
+    set_free_proxy()
+    llm = OpenAI()
+    llm("你知道鸡哥的《只因你太美》？")
+
+
+if __name__ == '__main__':
+    main()
+```
+
+> 和OPENAI_API_KEY一样，关于代理的配置我也设置了缓存，这意味着你只需要配置一次代理即可(我也太聪明了吧)。事实上`promptulate`
+> 提供了关闭全局配置项缓存的功能，但默认开启，不推荐关闭，所以我不告诉你怎么关闭~
+
+### Conversation
+
+上面展示的LLM组件，只提供了最基础的对话生成内容，但是其并不提供上下文对话、文章总结、角色预设等更加复杂的功能，所以接下来我们介绍功能更为强大的`Conversation`。
+
+`Conversation` 是`framework`中最基础的组件，其支持prompt生成、上下文对话、对话存储、角色预设的基本功能，此外，`provider`
+为其提供了语言翻译、markdown数据导出、对话总结、标题总结等扩展功能。
+
+接下来，我们先从对基础的对话开始，使用`Conversation`可以开始一段对话，使用其`predict()`函数可以生成回答。
+
+```python
+from promptulate import Conversation
+
+conversation = Conversation()
+conversation.predict("你知道鸡哥的《只因你太美》吗？")
+```
+
+```text
+'是的，鸡哥的《只因你太美》是这几年非常流行的一首歌曲。'
+```
+
+`Conversation`默认使用`OpenAI GPT3.5`作为LLM，当然，因为其架构设计，`Conversation`
+还可以轻松扩展其他类型的llm（当前暂时只开发了OpenAI，其他大语言模型的扩展正在火速开发中，当然如果你有自己想接入的大语言模型，欢迎你的pr！）
+
+下面是一个更复杂的示例，展示了使用OpenAI作为大语言模型进行对话，使用本地文件进行存储，进行文章总结与标题总结的功能。
+
+```python
+from promptulate import Conversation
+from promptulate.memory import LocalCacheChatMemory
+from promptulate.llms import OpenAI
+
+
+def main():
+    memory = LocalCacheChatMemory()
+    llm = OpenAI(model="gpt-3.5-turbo", temperature=0.9, top_p=1, stream=False, presence_penalty=0, n=1)
+    conversation = Conversation(llm=llm, memory=memory)
+    ret = conversation.predict("你知道鸡哥的著作《只因你太美》吗？")
+    print(f"[predict] {ret}")
+    ret = conversation.predict_by_translate("你知道鸡哥会什么技能吗？", country='America')
+    print(f"[translate output] {ret}")
+    ret = conversation.summary_content()
+    print(f"[summary content] {ret}")
+    ret = conversation.summary_topic()
+    print(f"[summary topic] {ret}")
+    ret = conversation.export_message_to_markdown(output_type="file", file_path="output.md")
+    print(f"[export markdown] {ret}")
+
+
+if __name__ == '__main__':
+    main()
+
+```
+
+```text
+[predict] 是的，我知道《只因你太美》这本书，是中国知名作家鸡肋（江南）所著的一篇言情小说。这本小说讲述了一个富家千金与一个贫穷男孩之间的爱情故事，情节曲折动人，深受读者喜爱。该小说在出版后得到了很高的评价和反响，并被改编成电影和电视剧等多种形式进行推广。
+[translate output] I'm sorry, I cannot determine what you mean by "鸡哥" or what skills they may possess without additional context. Can you please provide more information or clarify your question?
+[summary content] 在之前的对话中，用户询问我是否知道鸡哥的著作《只因你太美》。我回答了肯定的，解释了该小说的情节大致概括和其受欢迎的原因。我也提到了该小说的广泛影响，包括被改编成电影和电视剧等多种形式进行推广。
+[summary topic] 鸡哥的小说。
+```
+
+> 咱就是说季皮提老师不懂鸡哥-.-
+
+上面的示例中，我们使用
+
+- `LocalCacheChatMemory()`进行聊天记录的本地化文件存储，文件存储形式默认是以json的形式进行存储的，保存在`cache`中。
+- `OpenAI(model="gpt-3.5-turbo", temperature=0.9, top_p=1, stream=False, presence_penalty=0, n=1)`
+  进行初始化一个大模型，里面是OpenAI需要传入的一些参数，具体可以查看[https://platform.openai.com/docs/api-reference/chat/create](https://platform.openai.com/docs/api-reference/chat/create)
+  查看具体含义，这里不做详细讲解，如果你不想理会这些参数，你也可以直接`llm = OpenAI()`就好啦，默认使用`gpt-3.5-turbo`
+  作为大语言模型，其他参数使用默认的就好了。
+- `conversation.predict_by_translate("你知道鸡哥会什么技能吗？", country='America')`
+  这个功能为使用特定语言进行预测，`provider`为其提供了`TranslatorMixin`，让`Conversation`
+  得以拥有此功能。对于这个方法，你只需要传入prompt和你需要转换的语言的国家名称就好了。
+- `conversation.summary_content()`这个函数可以直接总结上面的对话内容。
+- `conversation.summary_topic()` 这个函数可以直接总结上面的对话，并提供一个标题。
+- `conversation.export_message_to_markdown(output_type="file", file_path="output.md")`
+  这个函数可以将对话记录导出为markdown文件，如果`output_type="text"`，则只返回markdown对话的内容。
+
+`provider`为`Conversation`提供了 `SummarizerMixin, TranslatorMixin, DeriveHistoryMessageMixin`
+，让其拥有了总结对话、总结标题、翻译、markdown导出的能力，provider提供的函数中一般都提供了一个`enable_embed_message`
+的参数，这个参数的意思是：是否将本次对话保存进历史对话中，下面我们来看一个demo。
+
+```python
+from promptulate import Conversation
+
+conversation = Conversation()
+conversation.predict_by_translate("你知道鸡哥会什么技能吗？", country='America', enable_embed_message=True)
+```
+
+如果你设置了`enable_embed_message=True`, 那么这一次的predict将保存进历史对话中，provider提供的函数默认是不会将预测结果存入对话中的哦，这一点需要注意一下。
+
+### Key池
+
+`promptulate`为OpenAI进行特别优化，构建了Key池，如果你使用的是`GPT3.5`
+5美元的账号，一定会遇到限速的问题，这个时候，如果你有一堆Key，就可以很好的解决这个问题。`promptulate`的LRU
+KEY轮询机制巧妙的解决了限速的问题，你可以使用LLM随意地进行提问（前提是你有够多的key）。此外，如果你既有`GPT4`和`GPT3.5`
+的KEY，KEY池也可以不同模型的KEY调度。下面介绍使用方法：
+
+```python
+from promptulate.llms import OpenAI
+from promptulate.utils import export_openai_key_pool
+
+
+keys = [
+    {"model": "gpt-3.5-turbo", "key": "xxxxx"},
+    {"model": "gpt-3.5-turbo", "key": "xxxxx"},
+    {"model": "gpt-3.5-turbo", "key": "xxxxx"},
+    {"model": "gpt-4.0", "key": "xxxxx"},
+]
+
+export_openai_key_pool(keys)
+llm = OpenAI()
+for i in range(10):
+    llm("你好")
+```
+
+
+### 角色预设
+
+你可以为`framework`提供一些特定的角色，让其可以处理特殊任务，如linux终端，思维导图生成器等，通过下面的方法你可以查看当前支持所有的预设角色。
+
+```python
+from promptulate.preset_roles import get_all_preset_roles
+
+print(get_all_preset_roles())
+```
+
+> ['default-role', 'linux-terminal', 'mind-map-generator', 'sql-generator', 'copy-writer', 'code-analyzer']
+
+下面展示使用`mind-map-generator`生成md思维导图的过程：
+
+```python
+from promptulate import Conversation
+
+
+def main():
+    conversation = Conversation(role="mind-map-generator")
+    ret = conversation.predict("请帮我生成一段python的思维导图")
+    print(ret)
+
+
+if __name__ == '__main__':
+    main()
+
+```
+
+```text
+# Python
+## 基础语法
+### 数据类型
+- 数字
+- 字符串
+- 列表
+...
+```
+
+放入xmind中可以直接导入生成markdown的思维导图，咱就是说还不错，如下图所示：
+
+<img src="https://zeeland-bucket.oss-cn-beijing.aliyuncs.com/images/20230513172038.png"/>
+
+如果你想要自定义预设角色，可以使用如下方法：
+
+```python
+from promptulate import Conversation
+from promptulate.preset_roles import CustomPresetRole
+
+
+class SpiritualTeacher(CustomPresetRole):
+    name = '心灵导师'
+    description = """
+    从现在起你是一个充满哲学思维的心灵导师，当我每次输入一个疑问时你需要用一句富有哲理的名言警句来回答我，并且表明作者和出处
+    要求字数不少于15个字，不超过30字，每次只返回一句且不输出额外的其他信息，你需要使用中文和英文双语输出"""
+
+
+def main():
+    role = SpiritualTeacher()
+    conversation = Conversation(role=role)
+    ret = conversation.predict("论文被拒绝了怎么办？")
+    print(ret)
+
+
+if __name__ == '__main__':
+    main()
+
+```
+
+```text
+“失败不是终点，放弃才是。”——托马斯·爱迪生
+```
+
+# 待办清单
+
+- 提供更多LLM模型支持
+- 提供Agent进行复杂任务调度
+- 提供更加方便的程序调用方式
+- ~~添加角色预设~~
+- 预设角色的参数配置
+- 提供prompt模板与prompt结构化
+- 提供外部工具扩展
+    - ~~外部搜索： Google,Bing等~~
+    - 可以执行shell脚本
+    - ~~提供Python REPL~~
+    - ~~arxiv论文工具箱，总结，润色~~
+    - 本地文件总结
+    - 关系型数据库检索
+    - 图数据库检索
+- 对话存储
+    - 提供向量数据库存储
+    - 提供mysql, redis等数据库存储
+- 自建知识库建立专家决策系统
+- 接入self-ask, prompt-loop, tree of thoughts架构
+- 提供多种导出方式
+- ~~可以导出历史消息为markdown格式~~
+- ~~使用环境变量配置key~~
+- 提供显示当前token（单词量）的功能
+- ~~添加错误处理机制，如网络异常、服务器异常等，保证程序的可靠性~~
+- ~~开发ChatBot v2, [issue](https://github.com/Undertone0809/cushy-chat/issues/1)~~
+- ~~完善代理模式~~
+- 提供gradio快速演示服务器
+- ~~提供简易对话终端~~
+- ~~封装消息体，完善消息体中的信息~~
+- ~~长对话自动/手动总结~~
+- ~~提供全局配置的缓存开关~~
+- ~~提供限速等问题的错误提示~~
+- ~~Conversation传入convesation_id继续上次对话~~
+- 提供修改local_cache默认位置的方法
+- 为predict提供回调模式
+- ~~提供基于LRU算法的API池，解决key限速的问题~~
+- 提供代理池，收集市面上所有可用的免费代理进行轮询
+- 构建结果正确率判别器
+- 设置工作空间
+
+# 设计原则
+
+promptulate框架的设计原则，包括：模块化、可扩展性、互操作性、鲁棒性、可维护性、安全性、效率和可用性。
+
+- 模块化是指以模块为基本单位，允许方便地集成新的组件、模型和工具。
+- 可扩展性是指框架能够处理大量数据、复杂任务和高并发的能力。
+- 互操作性是指该框架与各种外部系统、工具和服务兼容，并且能够实现无缝集成和通信。
+- 鲁棒性是指框架具备强大的错误处理、容错和恢复机制，以确保在各种条件下可靠地运行。
+- 安全性是指框架采用了严格的安全措施，以保护框架、其数据和用户免受未经授权访问和恶意行为的侵害。
+- 效率是指优化框架的性能、资源使用和响应时间，以确保流畅和敏锐的用户体验。
+- 可用性是指该框架采用用户友好的界面和清晰的文档，使其易于使用和理解。
+
+以上原则的遵循，以及最新的人工智能技术的应用，promptulate旨在为创建自动化代理提供强大而灵活的平台。
+
+# 一些问题
+
+- 本人正在尝试一些更加完善的抽象模式，以更好地兼容该框架，以及外部工具的扩展使用，如果你有更好的建议，欢迎一起讨论交流。
+
+# 贡献
+
+如果你想为这个项目做贡献，你可以提交pr或issue。我很高兴看到更多的人参与并优化它。
```

### Comparing `promptulate-1.0.2/setup.py` & `promptulate-1.1.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,64 @@
-# Copyright 2022 Zeeland(https://github.com/Undertone0809/). All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#      http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-import setuptools
-import pathlib
-
-here = pathlib.Path(__file__).parent.resolve()
-long_description = (here / "README.md").read_text(encoding="utf-8")
-
-setuptools.setup(
-    name="promptulate",
-    version="1.0.2",
-    author="Zeeland",
-    author_email="zeeland@foxmail.com",
-    description="A powerful LLM Prompt Layer frameworks",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/Undertone0809/promptulate",
-    packages=setuptools.find_packages(),
-    install_requires=['cushy-storage', 'pydantic', 'requests'],
-    license="Apache 2.0",
-    classifiers=[
-        "Development Status :: 3 - Alpha",
-        "Intended Audience :: Developers",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "Programming Language :: Python :: 3 :: Only",
-        "License :: OSI Approved :: Apache Software License",
-        "Operating System :: OS Independent",
-
-    ],
-    keywords="promptulate, prompt-me, prompt, chatgpt, gpt, chatbot, llm",
-    entry_points={
-        'console_scripts': ['promptulate-chat=promptulate.command.chat:main']
-    },
-)
+# Copyright (c) 2023 Zeeland
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# Copyright Owner: Zeeland
+# GitHub Link: https://github.com/Undertone0809/
+# Project Link: https://github.com/Undertone0809/promptulate
+# Contact Email: zeeland@foxmail.com
+
+import setuptools
+import pathlib
+
+here = pathlib.Path(__file__).parent.resolve()
+long_description = (here / "README.md").read_text(encoding="utf-8")
+
+setuptools.setup(
+    name="promptulate",
+    version="1.1.0",
+    author="Zeeland",
+    author_email="zeeland@foxmail.com",
+    description="A powerful LLM Prompt Layer frameworks",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/Undertone0809/promptulate",
+    packages=setuptools.find_packages(),
+    install_requires=[
+        'cushy-storage',
+        'pydantic',
+        'requests',
+        'duckduckgo_search',
+        'broadcast-service==1.3.2',
+        'arxiv'
+    ],
+    license="Apache 2.0",
+    python_requires='>=3.6',
+    classifiers=[
+        "Development Status :: 3 - Alpha",
+        "Intended Audience :: Developers",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3 :: Only",
+        "License :: OSI Approved :: Apache Software License",
+        "Operating System :: OS Independent",
+
+    ],
+    keywords="promptulate, prompt-me, prompt, chatgpt, gpt, chatbot, llm",
+    entry_points={
+        'console_scripts': ['promptulate-chat=promptulate.command.chat:main']
+    },
+)
```


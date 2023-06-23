# Comparing `tmp/promptops-0.1.8.tar.gz` & `tmp/promptops-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptops-0.1.8.tar", last modified: Fri Jun 23 16:54:02 2023, max compression
+gzip compressed data, was "promptops-0.1.9.tar", last modified: Fri Jun 23 19:47:30 2023, max compression
```

## Comparing `promptops-0.1.8.tar` & `promptops-0.1.9.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 16:54:02.155254 promptops-0.1.8/
--rw-r--r--   0 vasily     (501) staff       (20)    35149 2023-05-24 15:22:16.000000 promptops-0.1.8/LICENSE.txt
--rw-r--r--   0 vasily     (501) staff       (20)     2889 2023-06-23 16:54:02.155423 promptops-0.1.8/PKG-INFO
--rw-r--r--   0 vasily     (501) staff       (20)     2252 2023-06-23 01:46:23.000000 promptops-0.1.8/README.md
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 16:54:02.111145 promptops-0.1.8/local_runner/
--rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.8/local_runner/__init__.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 16:54:02.113987 promptops-0.1.8/local_runner/comms/
--rw-r--r--   0 vasily     (501) staff       (20)      133 2023-05-24 13:48:37.000000 promptops-0.1.8/local_runner/comms/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)      432 2023-05-24 13:48:37.000000 promptops-0.1.8/local_runner/comms/base.py
--rw-r--r--   0 vasily     (501) staff       (20)     2890 2023-05-24 13:48:37.000000 promptops-0.1.8/local_runner/comms/dtos.py
--rw-r--r--   0 vasily     (501) staff       (20)     1536 2023-05-24 13:48:37.000000 promptops-0.1.8/local_runner/comms/http_reporter.py
--rw-r--r--   0 vasily     (501) staff       (20)     1671 2023-06-07 21:55:02.000000 promptops-0.1.8/local_runner/comms/ws.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 16:54:02.115070 promptops-0.1.8/local_runner/config/
--rw-r--r--   0 vasily     (501) staff       (20)       48 2023-05-24 13:48:37.000000 promptops-0.1.8/local_runner/config/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     1720 2023-05-24 13:48:37.000000 promptops-0.1.8/local_runner/config/config.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 16:54:02.115997 promptops-0.1.8/local_runner/creds/
--rw-r--r--   0 vasily     (501) staff       (20)       77 2023-05-24 13:48:37.000000 promptops-0.1.8/local_runner/creds/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     1458 2023-05-24 13:48:37.000000 promptops-0.1.8/local_runner/creds/creds.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 16:54:02.116910 promptops-0.1.8/local_runner/exec/
--rw-r--r--   0 vasily     (501) staff       (20)       54 2023-05-24 13:48:37.000000 promptops-0.1.8/local_runner/exec/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     2317 2023-05-24 13:48:37.000000 promptops-0.1.8/local_runner/exec/manager.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 16:54:02.118124 promptops-0.1.8/local_runner/handler/
--rw-r--r--   0 vasily     (501) staff       (20)       29 2023-05-24 13:48:37.000000 promptops-0.1.8/local_runner/handler/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)      471 2023-05-24 13:48:37.000000 promptops-0.1.8/local_runner/handler/censor.py
--rw-r--r--   0 vasily     (501) staff       (20)     3115 2023-05-24 13:48:37.000000 promptops-0.1.8/local_runner/handler/handler.py
--rw-r--r--   0 vasily     (501) staff       (20)     1361 2023-06-07 21:55:02.000000 promptops-0.1.8/local_runner/main.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 16:54:02.118887 promptops-0.1.8/local_runner/registration/
--rw-r--r--   0 vasily     (501) staff       (20)       56 2023-05-24 13:48:37.000000 promptops-0.1.8/local_runner/registration/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     2523 2023-05-24 13:48:37.000000 promptops-0.1.8/local_runner/registration/registration.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 16:54:02.119722 promptops-0.1.8/local_runner/tokens/
--rw-r--r--   0 vasily     (501) staff       (20)       27 2023-05-24 13:48:37.000000 promptops-0.1.8/local_runner/tokens/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     2235 2023-05-24 13:48:37.000000 promptops-0.1.8/local_runner/tokens/issuer.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 16:54:02.126470 promptops-0.1.8/promptops/
--rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.8/promptops/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     1850 2023-05-24 13:48:37.000000 promptops-0.1.8/promptops/corrections.py
--rw-r--r--   0 vasily     (501) staff       (20)     1033 2023-06-07 21:55:02.000000 promptops-0.1.8/promptops/feedback.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 16:54:02.129624 promptops-0.1.8/promptops/gitaware/
--rw-r--r--   0 vasily     (501) staff       (20)       42 2023-06-07 21:55:02.000000 promptops-0.1.8/promptops/gitaware/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     3161 2023-06-23 16:03:30.000000 promptops-0.1.8/promptops/gitaware/commits.py
--rw-r--r--   0 vasily     (501) staff       (20)      658 2023-06-15 19:15:23.000000 promptops-0.1.8/promptops/gitaware/project.py
--rw-r--r--   0 vasily     (501) staff       (20)     4146 2023-06-07 21:55:02.000000 promptops-0.1.8/promptops/history.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 16:54:02.131459 promptops-0.1.8/promptops/index/
--rw-r--r--   0 vasily     (501) staff       (20)        0 2023-06-07 21:55:02.000000 promptops-0.1.8/promptops/index/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     2691 2023-06-16 22:44:53.000000 promptops-0.1.8/promptops/index/content.py
--rw-r--r--   0 vasily     (501) staff       (20)     2084 2023-06-07 21:55:02.000000 promptops-0.1.8/promptops/index/entry_point.py
--rw-r--r--   0 vasily     (501) staff       (20)     4399 2023-06-07 21:55:02.000000 promptops-0.1.8/promptops/index/index_store.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 16:54:02.136263 promptops-0.1.8/promptops/loading/
--rw-r--r--   0 vasily     (501) staff       (20)      131 2023-05-24 13:48:37.000000 promptops-0.1.8/promptops/loading/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)      745 2023-06-21 21:04:09.000000 promptops-0.1.8/promptops/loading/base.py
--rw-r--r--   0 vasily     (501) staff       (20)     1139 2023-06-15 19:15:23.000000 promptops-0.1.8/promptops/loading/cancellable.py
--rw-r--r--   0 vasily     (501) staff       (20)      481 2023-05-24 13:48:37.000000 promptops-0.1.8/promptops/loading/context.py
--rw-r--r--   0 vasily     (501) staff       (20)     1554 2023-06-15 19:15:23.000000 promptops-0.1.8/promptops/loading/multi.py
--rw-r--r--   0 vasily     (501) staff       (20)     1279 2023-05-24 13:48:37.000000 promptops-0.1.8/promptops/loading/pong.py
--rw-r--r--   0 vasily     (501) staff       (20)     1344 2023-05-24 13:48:37.000000 promptops-0.1.8/promptops/loading/progress.py
--rw-r--r--   0 vasily     (501) staff       (20)     1077 2023-05-24 13:48:37.000000 promptops-0.1.8/promptops/loading/promptops.py
--rw-r--r--   0 vasily     (501) staff       (20)     1051 2023-06-21 21:04:09.000000 promptops-0.1.8/promptops/loading/simple.py
--rw-r--r--   0 vasily     (501) staff       (20)    11413 2023-06-23 16:03:30.000000 promptops-0.1.8/promptops/main.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 16:54:02.140405 promptops-0.1.8/promptops/query/
--rw-r--r--   0 vasily     (501) staff       (20)       28 2023-06-21 01:03:51.000000 promptops-0.1.8/promptops/query/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)      434 2023-06-16 19:21:46.000000 promptops-0.1.8/promptops/query/dtos.py
--rw-r--r--   0 vasily     (501) staff       (20)     4351 2023-05-25 18:38:08.000000 promptops-0.1.8/promptops/query/explanation.py
--rw-r--r--   0 vasily     (501) staff       (20)     4506 2023-06-07 21:55:02.000000 promptops-0.1.8/promptops/query/git_repo.py
--rw-r--r--   0 vasily     (501) staff       (20)     9058 2023-06-23 01:46:23.000000 promptops-0.1.8/promptops/query/lookup.py
--rw-r--r--   0 vasily     (501) staff       (20)     1222 2023-05-24 13:48:37.000000 promptops-0.1.8/promptops/query/messages.py
--rw-r--r--   0 vasily     (501) staff       (20)    19960 2023-06-23 16:03:30.000000 promptops-0.1.8/promptops/query/query.py
--rw-r--r--   0 vasily     (501) staff       (20)     6165 2023-06-23 01:46:23.000000 promptops-0.1.8/promptops/query/suggest_next.py
--rw-r--r--   0 vasily     (501) staff       (20)     1126 2023-05-24 13:48:37.000000 promptops-0.1.8/promptops/query.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 16:54:02.143171 promptops-0.1.8/promptops/recipes/
--rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.8/promptops/recipes/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)    14644 2023-06-21 21:04:09.000000 promptops-0.1.8/promptops/recipes/creation.py
--rw-r--r--   0 vasily     (501) staff       (20)      606 2023-06-16 22:44:53.000000 promptops-0.1.8/promptops/recipes/executor.py
--rw-r--r--   0 vasily     (501) staff       (20)     1076 2023-06-23 01:46:23.000000 promptops-0.1.8/promptops/recipes/run.py
--rw-r--r--   0 vasily     (501) staff       (20)     7585 2023-06-21 01:03:51.000000 promptops-0.1.8/promptops/recipes/terraform.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 16:54:02.144351 promptops-0.1.8/promptops/scrub_secrets/
--rw-r--r--   0 vasily     (501) staff       (20)       55 2023-05-24 13:48:37.000000 promptops-0.1.8/promptops/scrub_secrets/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     2423 2023-05-24 13:48:37.000000 promptops-0.1.8/promptops/scrub_secrets/scrub.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 16:54:02.145410 promptops-0.1.8/promptops/secret/
--rw-r--r--   0 vasily     (501) staff       (20)       55 2023-06-16 22:44:53.000000 promptops-0.1.8/promptops/secret/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     2423 2023-06-16 22:44:53.000000 promptops-0.1.8/promptops/secret/scrub.py
--rw-r--r--   0 vasily     (501) staff       (20)      438 2023-06-23 16:03:30.000000 promptops-0.1.8/promptops/settings.py
--rw-r--r--   0 vasily     (501) staff       (20)     2593 2023-06-23 16:03:30.000000 promptops-0.1.8/promptops/settings_store.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 16:54:02.149282 promptops-0.1.8/promptops/shells/
--rw-r--r--   0 vasily     (501) staff       (20)       46 2023-06-15 19:15:23.000000 promptops-0.1.8/promptops/shells/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     7003 2023-06-23 01:46:23.000000 promptops-0.1.8/promptops/shells/base.py
--rw-r--r--   0 vasily     (501) staff       (20)     1816 2023-06-23 01:46:23.000000 promptops-0.1.8/promptops/shells/bash.py
--rw-r--r--   0 vasily     (501) staff       (20)     1154 2023-06-21 02:44:24.000000 promptops-0.1.8/promptops/shells/common.py
--rw-r--r--   0 vasily     (501) staff       (20)     2410 2023-06-23 01:46:23.000000 promptops-0.1.8/promptops/shells/fish.py
--rw-r--r--   0 vasily     (501) staff       (20)     4012 2023-06-23 01:46:23.000000 promptops-0.1.8/promptops/shells/zsh.py
--rw-r--r--   0 vasily     (501) staff       (20)     3206 2023-06-15 19:15:23.000000 promptops-0.1.8/promptops/similarity.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 16:54:02.152199 promptops-0.1.8/promptops/skills/
--rw-r--r--   0 vasily     (501) staff       (20)        0 2023-06-21 01:03:51.000000 promptops-0.1.8/promptops/skills/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)      108 2023-06-21 01:03:51.000000 promptops-0.1.8/promptops/skills/choice.py
--rw-r--r--   0 vasily     (501) staff       (20)      940 2023-06-22 03:44:33.000000 promptops-0.1.8/promptops/skills/commit_message.py
--rw-r--r--   0 vasily     (501) staff       (20)     9282 2023-06-23 16:03:30.000000 promptops-0.1.8/promptops/skills/dtt.py
--rw-r--r--   0 vasily     (501) staff       (20)      558 2023-06-21 21:04:09.000000 promptops-0.1.8/promptops/skills/next.py
--rw-r--r--   0 vasily     (501) staff       (20)       42 2023-05-24 13:48:37.000000 promptops-0.1.8/promptops/trace.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 16:54:02.154721 promptops-0.1.8/promptops/ui/
--rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.8/promptops/ui/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)      138 2023-06-07 21:55:02.000000 promptops-0.1.8/promptops/ui/input.py
--rw-r--r--   0 vasily     (501) staff       (20)     3070 2023-05-24 13:48:37.000000 promptops-0.1.8/promptops/ui/prompts.py
--rw-r--r--   0 vasily     (501) staff       (20)     9308 2023-06-23 16:03:30.000000 promptops-0.1.8/promptops/ui/selections.py
--rw-r--r--   0 vasily     (501) staff       (20)      621 2023-06-21 01:03:51.000000 promptops-0.1.8/promptops/ui/vim.py
--rw-r--r--   0 vasily     (501) staff       (20)     1099 2023-05-24 13:48:37.000000 promptops-0.1.8/promptops/ui.py
--rw-r--r--   0 vasily     (501) staff       (20)     4570 2023-06-07 21:55:02.000000 promptops-0.1.8/promptops/user.py
--rw-r--r--   0 vasily     (501) staff       (20)       22 2023-06-23 01:46:23.000000 promptops-0.1.8/promptops/version.py
--rw-r--r--   0 vasily     (501) staff       (20)     1632 2023-05-24 13:48:37.000000 promptops-0.1.8/promptops/version_check.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 16:54:02.128338 promptops-0.1.8/promptops.egg-info/
--rw-r--r--   0 vasily     (501) staff       (20)     2889 2023-06-23 16:54:02.000000 promptops-0.1.8/promptops.egg-info/PKG-INFO
--rw-r--r--   0 vasily     (501) staff       (20)     2540 2023-06-23 16:54:02.000000 promptops-0.1.8/promptops.egg-info/SOURCES.txt
--rw-r--r--   0 vasily     (501) staff       (20)        1 2023-06-23 16:54:02.000000 promptops-0.1.8/promptops.egg-info/dependency_links.txt
--rw-r--r--   0 vasily     (501) staff       (20)      120 2023-06-23 16:54:02.000000 promptops-0.1.8/promptops.egg-info/entry_points.txt
--rw-r--r--   0 vasily     (501) staff       (20)      260 2023-06-23 16:54:02.000000 promptops-0.1.8/promptops.egg-info/requires.txt
--rw-r--r--   0 vasily     (501) staff       (20)       23 2023-06-23 16:54:02.000000 promptops-0.1.8/promptops.egg-info/top_level.txt
--rw-r--r--   0 vasily     (501) staff       (20)       87 2023-05-24 14:19:51.000000 promptops-0.1.8/pyproject.toml
--rw-r--r--   0 vasily     (501) staff       (20)       78 2023-06-23 16:54:02.155984 promptops-0.1.8/setup.cfg
--rw-r--r--   0 vasily     (501) staff       (20)     2051 2023-06-23 16:53:44.000000 promptops-0.1.8/setup.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 19:47:30.736026 promptops-0.1.9/
+-rw-r--r--   0 vasily     (501) staff       (20)    35149 2023-05-24 15:22:16.000000 promptops-0.1.9/LICENSE.txt
+-rw-r--r--   0 vasily     (501) staff       (20)     2889 2023-06-23 19:47:30.736189 promptops-0.1.9/PKG-INFO
+-rw-r--r--   0 vasily     (501) staff       (20)     2252 2023-06-23 01:46:23.000000 promptops-0.1.9/README.md
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 19:47:30.707416 promptops-0.1.9/local_runner/
+-rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.9/local_runner/__init__.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 19:47:30.708616 promptops-0.1.9/local_runner/comms/
+-rw-r--r--   0 vasily     (501) staff       (20)      133 2023-05-24 13:48:37.000000 promptops-0.1.9/local_runner/comms/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)      432 2023-05-24 13:48:37.000000 promptops-0.1.9/local_runner/comms/base.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2890 2023-05-24 13:48:37.000000 promptops-0.1.9/local_runner/comms/dtos.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1536 2023-05-24 13:48:37.000000 promptops-0.1.9/local_runner/comms/http_reporter.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1671 2023-06-07 21:55:02.000000 promptops-0.1.9/local_runner/comms/ws.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 19:47:30.709080 promptops-0.1.9/local_runner/config/
+-rw-r--r--   0 vasily     (501) staff       (20)       48 2023-05-24 13:48:37.000000 promptops-0.1.9/local_runner/config/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1720 2023-05-24 13:48:37.000000 promptops-0.1.9/local_runner/config/config.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 19:47:30.709541 promptops-0.1.9/local_runner/creds/
+-rw-r--r--   0 vasily     (501) staff       (20)       77 2023-05-24 13:48:37.000000 promptops-0.1.9/local_runner/creds/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1458 2023-05-24 13:48:37.000000 promptops-0.1.9/local_runner/creds/creds.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 19:47:30.710000 promptops-0.1.9/local_runner/exec/
+-rw-r--r--   0 vasily     (501) staff       (20)       54 2023-05-24 13:48:37.000000 promptops-0.1.9/local_runner/exec/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2317 2023-05-24 13:48:37.000000 promptops-0.1.9/local_runner/exec/manager.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 19:47:30.710744 promptops-0.1.9/local_runner/handler/
+-rw-r--r--   0 vasily     (501) staff       (20)       29 2023-05-24 13:48:37.000000 promptops-0.1.9/local_runner/handler/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)      471 2023-05-24 13:48:37.000000 promptops-0.1.9/local_runner/handler/censor.py
+-rw-r--r--   0 vasily     (501) staff       (20)     3115 2023-05-24 13:48:37.000000 promptops-0.1.9/local_runner/handler/handler.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1361 2023-06-07 21:55:02.000000 promptops-0.1.9/local_runner/main.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 19:47:30.711280 promptops-0.1.9/local_runner/registration/
+-rw-r--r--   0 vasily     (501) staff       (20)       56 2023-05-24 13:48:37.000000 promptops-0.1.9/local_runner/registration/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2523 2023-05-24 13:48:37.000000 promptops-0.1.9/local_runner/registration/registration.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 19:47:30.711770 promptops-0.1.9/local_runner/tokens/
+-rw-r--r--   0 vasily     (501) staff       (20)       27 2023-05-24 13:48:37.000000 promptops-0.1.9/local_runner/tokens/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2235 2023-05-24 13:48:37.000000 promptops-0.1.9/local_runner/tokens/issuer.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 19:47:30.716316 promptops-0.1.9/promptops/
+-rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.9/promptops/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1850 2023-05-24 13:48:37.000000 promptops-0.1.9/promptops/corrections.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1033 2023-06-07 21:55:02.000000 promptops-0.1.9/promptops/feedback.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 19:47:30.719154 promptops-0.1.9/promptops/gitaware/
+-rw-r--r--   0 vasily     (501) staff       (20)       42 2023-06-07 21:55:02.000000 promptops-0.1.9/promptops/gitaware/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     3161 2023-06-23 16:03:30.000000 promptops-0.1.9/promptops/gitaware/commits.py
+-rw-r--r--   0 vasily     (501) staff       (20)      658 2023-06-15 19:15:23.000000 promptops-0.1.9/promptops/gitaware/project.py
+-rw-r--r--   0 vasily     (501) staff       (20)     4146 2023-06-07 21:55:02.000000 promptops-0.1.9/promptops/history.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 19:47:30.720023 promptops-0.1.9/promptops/index/
+-rw-r--r--   0 vasily     (501) staff       (20)        0 2023-06-07 21:55:02.000000 promptops-0.1.9/promptops/index/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2691 2023-06-16 22:44:53.000000 promptops-0.1.9/promptops/index/content.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2084 2023-06-07 21:55:02.000000 promptops-0.1.9/promptops/index/entry_point.py
+-rw-r--r--   0 vasily     (501) staff       (20)     4399 2023-06-07 21:55:02.000000 promptops-0.1.9/promptops/index/index_store.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 19:47:30.722908 promptops-0.1.9/promptops/loading/
+-rw-r--r--   0 vasily     (501) staff       (20)      131 2023-05-24 13:48:37.000000 promptops-0.1.9/promptops/loading/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)      745 2023-06-21 21:04:09.000000 promptops-0.1.9/promptops/loading/base.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1139 2023-06-15 19:15:23.000000 promptops-0.1.9/promptops/loading/cancellable.py
+-rw-r--r--   0 vasily     (501) staff       (20)      481 2023-05-24 13:48:37.000000 promptops-0.1.9/promptops/loading/context.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1554 2023-06-15 19:15:23.000000 promptops-0.1.9/promptops/loading/multi.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1279 2023-05-24 13:48:37.000000 promptops-0.1.9/promptops/loading/pong.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1344 2023-05-24 13:48:37.000000 promptops-0.1.9/promptops/loading/progress.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1077 2023-05-24 13:48:37.000000 promptops-0.1.9/promptops/loading/promptops.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1051 2023-06-21 21:04:09.000000 promptops-0.1.9/promptops/loading/simple.py
+-rw-r--r--   0 vasily     (501) staff       (20)    11413 2023-06-23 16:03:30.000000 promptops-0.1.9/promptops/main.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 19:47:30.726055 promptops-0.1.9/promptops/query/
+-rw-r--r--   0 vasily     (501) staff       (20)       28 2023-06-21 01:03:51.000000 promptops-0.1.9/promptops/query/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)      434 2023-06-16 19:21:46.000000 promptops-0.1.9/promptops/query/dtos.py
+-rw-r--r--   0 vasily     (501) staff       (20)     4351 2023-05-25 18:38:08.000000 promptops-0.1.9/promptops/query/explanation.py
+-rw-r--r--   0 vasily     (501) staff       (20)     4506 2023-06-07 21:55:02.000000 promptops-0.1.9/promptops/query/git_repo.py
+-rw-r--r--   0 vasily     (501) staff       (20)     9058 2023-06-23 01:46:23.000000 promptops-0.1.9/promptops/query/lookup.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1222 2023-05-24 13:48:37.000000 promptops-0.1.9/promptops/query/messages.py
+-rw-r--r--   0 vasily     (501) staff       (20)    19960 2023-06-23 16:03:30.000000 promptops-0.1.9/promptops/query/query.py
+-rw-r--r--   0 vasily     (501) staff       (20)     6896 2023-06-23 19:44:36.000000 promptops-0.1.9/promptops/query/suggest_next.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1126 2023-05-24 13:48:37.000000 promptops-0.1.9/promptops/query.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 19:47:30.728004 promptops-0.1.9/promptops/recipes/
+-rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.9/promptops/recipes/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)    14644 2023-06-21 21:04:09.000000 promptops-0.1.9/promptops/recipes/creation.py
+-rw-r--r--   0 vasily     (501) staff       (20)      606 2023-06-16 22:44:53.000000 promptops-0.1.9/promptops/recipes/executor.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1076 2023-06-23 01:46:23.000000 promptops-0.1.9/promptops/recipes/run.py
+-rw-r--r--   0 vasily     (501) staff       (20)     7585 2023-06-21 01:03:51.000000 promptops-0.1.9/promptops/recipes/terraform.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 19:47:30.728852 promptops-0.1.9/promptops/scrub_secrets/
+-rw-r--r--   0 vasily     (501) staff       (20)       55 2023-05-24 13:48:37.000000 promptops-0.1.9/promptops/scrub_secrets/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2423 2023-05-24 13:48:37.000000 promptops-0.1.9/promptops/scrub_secrets/scrub.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 19:47:30.729651 promptops-0.1.9/promptops/secret/
+-rw-r--r--   0 vasily     (501) staff       (20)       55 2023-06-16 22:44:53.000000 promptops-0.1.9/promptops/secret/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2423 2023-06-16 22:44:53.000000 promptops-0.1.9/promptops/secret/scrub.py
+-rw-r--r--   0 vasily     (501) staff       (20)      438 2023-06-23 16:03:30.000000 promptops-0.1.9/promptops/settings.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2593 2023-06-23 16:03:30.000000 promptops-0.1.9/promptops/settings_store.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 19:47:30.732011 promptops-0.1.9/promptops/shells/
+-rw-r--r--   0 vasily     (501) staff       (20)       46 2023-06-15 19:15:23.000000 promptops-0.1.9/promptops/shells/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     7003 2023-06-23 01:46:23.000000 promptops-0.1.9/promptops/shells/base.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1816 2023-06-23 01:46:23.000000 promptops-0.1.9/promptops/shells/bash.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1154 2023-06-21 02:44:24.000000 promptops-0.1.9/promptops/shells/common.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2410 2023-06-23 01:46:23.000000 promptops-0.1.9/promptops/shells/fish.py
+-rw-r--r--   0 vasily     (501) staff       (20)     4012 2023-06-23 01:46:23.000000 promptops-0.1.9/promptops/shells/zsh.py
+-rw-r--r--   0 vasily     (501) staff       (20)     3206 2023-06-15 19:15:23.000000 promptops-0.1.9/promptops/similarity.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 19:47:30.733772 promptops-0.1.9/promptops/skills/
+-rw-r--r--   0 vasily     (501) staff       (20)        0 2023-06-21 01:03:51.000000 promptops-0.1.9/promptops/skills/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)      108 2023-06-21 01:03:51.000000 promptops-0.1.9/promptops/skills/choice.py
+-rw-r--r--   0 vasily     (501) staff       (20)      940 2023-06-22 03:44:33.000000 promptops-0.1.9/promptops/skills/commit_message.py
+-rw-r--r--   0 vasily     (501) staff       (20)     9282 2023-06-23 16:03:30.000000 promptops-0.1.9/promptops/skills/dtt.py
+-rw-r--r--   0 vasily     (501) staff       (20)      558 2023-06-21 21:04:09.000000 promptops-0.1.9/promptops/skills/next.py
+-rw-r--r--   0 vasily     (501) staff       (20)       42 2023-05-24 13:48:37.000000 promptops-0.1.9/promptops/trace.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 19:47:30.735552 promptops-0.1.9/promptops/ui/
+-rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.9/promptops/ui/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)      138 2023-06-07 21:55:02.000000 promptops-0.1.9/promptops/ui/input.py
+-rw-r--r--   0 vasily     (501) staff       (20)     3070 2023-05-24 13:48:37.000000 promptops-0.1.9/promptops/ui/prompts.py
+-rw-r--r--   0 vasily     (501) staff       (20)     9308 2023-06-23 16:03:30.000000 promptops-0.1.9/promptops/ui/selections.py
+-rw-r--r--   0 vasily     (501) staff       (20)      621 2023-06-21 01:03:51.000000 promptops-0.1.9/promptops/ui/vim.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1099 2023-05-24 13:48:37.000000 promptops-0.1.9/promptops/ui.py
+-rw-r--r--   0 vasily     (501) staff       (20)     4570 2023-06-07 21:55:02.000000 promptops-0.1.9/promptops/user.py
+-rw-r--r--   0 vasily     (501) staff       (20)       22 2023-06-23 19:44:38.000000 promptops-0.1.9/promptops/version.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1632 2023-05-24 13:48:37.000000 promptops-0.1.9/promptops/version_check.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 19:47:30.718140 promptops-0.1.9/promptops.egg-info/
+-rw-r--r--   0 vasily     (501) staff       (20)     2889 2023-06-23 19:47:30.000000 promptops-0.1.9/promptops.egg-info/PKG-INFO
+-rw-r--r--   0 vasily     (501) staff       (20)     2540 2023-06-23 19:47:30.000000 promptops-0.1.9/promptops.egg-info/SOURCES.txt
+-rw-r--r--   0 vasily     (501) staff       (20)        1 2023-06-23 19:47:30.000000 promptops-0.1.9/promptops.egg-info/dependency_links.txt
+-rw-r--r--   0 vasily     (501) staff       (20)      120 2023-06-23 19:47:30.000000 promptops-0.1.9/promptops.egg-info/entry_points.txt
+-rw-r--r--   0 vasily     (501) staff       (20)      248 2023-06-23 19:47:30.000000 promptops-0.1.9/promptops.egg-info/requires.txt
+-rw-r--r--   0 vasily     (501) staff       (20)       23 2023-06-23 19:47:30.000000 promptops-0.1.9/promptops.egg-info/top_level.txt
+-rw-r--r--   0 vasily     (501) staff       (20)       87 2023-05-24 14:19:51.000000 promptops-0.1.9/pyproject.toml
+-rw-r--r--   0 vasily     (501) staff       (20)       78 2023-06-23 19:47:30.736830 promptops-0.1.9/setup.cfg
+-rw-r--r--   0 vasily     (501) staff       (20)     2028 2023-06-23 19:44:38.000000 promptops-0.1.9/setup.py
```

### Comparing `promptops-0.1.8/LICENSE.txt` & `promptops-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/PKG-INFO` & `promptops-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptops
-Version: 0.1.8
+Version: 0.1.9
 Summary: Your CLI assistant. Ask questions, get shell commands.
 Home-page: https://promptops.com/
 Author: CtrlStack inc.
 License: GPLv3
 Project-URL: Documentation, https://docs.promptops.com/cli
 Project-URL: Changelog, https://docs.promptops.com/en/stable/changelog.html
 Project-URL: Live demo, https://promptops.com/
```

### Comparing `promptops-0.1.8/README.md` & `promptops-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/local_runner/comms/dtos.py` & `promptops-0.1.9/local_runner/comms/dtos.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/local_runner/comms/http_reporter.py` & `promptops-0.1.9/local_runner/comms/http_reporter.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/local_runner/comms/ws.py` & `promptops-0.1.9/local_runner/comms/ws.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/local_runner/config/config.py` & `promptops-0.1.9/local_runner/config/config.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/local_runner/creds/creds.py` & `promptops-0.1.9/local_runner/creds/creds.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/local_runner/exec/manager.py` & `promptops-0.1.9/local_runner/exec/manager.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/local_runner/handler/handler.py` & `promptops-0.1.9/local_runner/handler/handler.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/local_runner/main.py` & `promptops-0.1.9/local_runner/main.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/local_runner/registration/registration.py` & `promptops-0.1.9/local_runner/registration/registration.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/local_runner/tokens/issuer.py` & `promptops-0.1.9/local_runner/tokens/issuer.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops/corrections.py` & `promptops-0.1.9/promptops/corrections.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops/feedback.py` & `promptops-0.1.9/promptops/feedback.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops/gitaware/commits.py` & `promptops-0.1.9/promptops/gitaware/commits.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops/gitaware/project.py` & `promptops-0.1.9/promptops/gitaware/project.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops/history.py` & `promptops-0.1.9/promptops/history.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops/index/content.py` & `promptops-0.1.9/promptops/index/content.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops/index/entry_point.py` & `promptops-0.1.9/promptops/index/entry_point.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops/index/index_store.py` & `promptops-0.1.9/promptops/index/index_store.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops/loading/base.py` & `promptops-0.1.9/promptops/loading/base.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops/loading/cancellable.py` & `promptops-0.1.9/promptops/loading/cancellable.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops/loading/multi.py` & `promptops-0.1.9/promptops/loading/multi.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops/loading/pong.py` & `promptops-0.1.9/promptops/loading/pong.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops/loading/progress.py` & `promptops-0.1.9/promptops/loading/progress.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops/loading/promptops.py` & `promptops-0.1.9/promptops/loading/promptops.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops/loading/simple.py` & `promptops-0.1.9/promptops/loading/simple.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops/main.py` & `promptops-0.1.9/promptops/main.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops/query/explanation.py` & `promptops-0.1.9/promptops/query/explanation.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops/query/git_repo.py` & `promptops-0.1.9/promptops/query/git_repo.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops/query/lookup.py` & `promptops-0.1.9/promptops/query/lookup.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops/query/messages.py` & `promptops-0.1.9/promptops/query/messages.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops/query/query.py` & `promptops-0.1.9/promptops/query/query.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops/query/suggest_next.py` & `promptops-0.1.9/promptops/query/suggest_next.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,38 @@
 import fnmatch
 import logging
 import os
 
-import Levenshtein
 import requests
 from typing import List
 from promptops import shells, settings, user, trace
+import shlex
+from thefuzz import fuzz
+
+
+def similarity(cmd1, cmd2):
+    try:
+        tokens1 = shlex.split(cmd1)
+        tokens2 = shlex.split(cmd2)
+    except ValueError:
+        tokens1 = cmd1.strip().split()
+        tokens2 = cmd2.strip().split()
+    if tokens1[0] != tokens2[0]:
+        return 0
+    # naive approach to weigh the tokens
+    max_multiplier = 3
+    m_tokens1 = []
+    for i, token in enumerate(tokens1[1:max_multiplier]):
+        m_tokens1.extend([token] * (max_multiplier - i))
+    m_tokens1.extend(tokens1[max_multiplier:])
+    m_tokens2 = []
+    for i, token in enumerate(tokens2[1:max_multiplier]):
+        m_tokens2.extend([token] * (max_multiplier - i))
+    m_tokens2.extend(tokens2[max_multiplier:])
+    return fuzz.ratio(m_tokens1, m_tokens2) / 100.0
 
 
 class SuffixTree:
     def __init__(self):
         self.roots = {}
         self.build_tree()
 
@@ -27,33 +50,34 @@
     def build_tree(self):
         lines = shells.get_shell().get_recent_history(1000)
         for i, line in enumerate(lines):
             root_cmd = line
             if root_cmd:
                 self.insert(lines[i:i+3])
 
-    def close_enough_node(self, text):
+    def close_enough_node(self, text, cutoff=0.7):
         def count_dicts(d):
             if not isinstance(d, dict):
                 return 0
             return 1 + sum(count_dicts(v) for v in d.values())
 
         close = []
         for s2 in self.roots.keys():
-            score = Levenshtein.jaro_winkler(text, s2, prefix_weight=.3, score_cutoff=.80)
-            if score > 0 and count_dicts(self.roots[s2]) > 1:
-                close.append(self.roots[s2])
+            score = similarity(text, s2)
+            if score > cutoff:
+                if count_dicts(self.roots[s2]) > 1:
+                    close.append(self.roots[s2])
         return close
 
     @staticmethod
-    def closest_next(possible, text):
+    def closest_next(possible, text, cutoff=0.7):
         close = []
         for s2 in possible:
-            score = Levenshtein.jaro_winkler(text, s2, prefix_weight=.3)
-            if score > 0:
+            score = similarity(text, s2)
+            if score > cutoff:
                 close.append((s2, score))
         if len(close) == 0:
             return None
         return max(close, key=lambda x: x[1])[0]
 
     def predict_next_close(self, command_sequence):
         if len(command_sequence) < 1 or command_sequence[0] not in self.roots:
```

### Comparing `promptops-0.1.8/promptops/query.py` & `promptops-0.1.9/promptops/query.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops/recipes/creation.py` & `promptops-0.1.9/promptops/recipes/creation.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops/recipes/executor.py` & `promptops-0.1.9/promptops/recipes/executor.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops/recipes/run.py` & `promptops-0.1.9/promptops/recipes/run.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops/recipes/terraform.py` & `promptops-0.1.9/promptops/recipes/terraform.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops/scrub_secrets/scrub.py` & `promptops-0.1.9/promptops/scrub_secrets/scrub.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops/secret/scrub.py` & `promptops-0.1.9/promptops/secret/scrub.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops/settings_store.py` & `promptops-0.1.9/promptops/settings_store.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops/shells/base.py` & `promptops-0.1.9/promptops/shells/base.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops/shells/bash.py` & `promptops-0.1.9/promptops/shells/bash.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops/shells/common.py` & `promptops-0.1.9/promptops/shells/common.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops/shells/fish.py` & `promptops-0.1.9/promptops/shells/fish.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops/shells/zsh.py` & `promptops-0.1.9/promptops/shells/zsh.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops/similarity.py` & `promptops-0.1.9/promptops/similarity.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops/skills/commit_message.py` & `promptops-0.1.9/promptops/skills/commit_message.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops/skills/dtt.py` & `promptops-0.1.9/promptops/skills/dtt.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops/skills/next.py` & `promptops-0.1.9/promptops/skills/next.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops/ui/prompts.py` & `promptops-0.1.9/promptops/ui/prompts.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops/ui/selections.py` & `promptops-0.1.9/promptops/ui/selections.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops/ui/vim.py` & `promptops-0.1.9/promptops/ui/vim.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops/ui.py` & `promptops-0.1.9/promptops/ui.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops/user.py` & `promptops-0.1.9/promptops/user.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops/version_check.py` & `promptops-0.1.9/promptops/version_check.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/promptops.egg-info/PKG-INFO` & `promptops-0.1.9/promptops.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptops
-Version: 0.1.8
+Version: 0.1.9
 Summary: Your CLI assistant. Ask questions, get shell commands.
 Home-page: https://promptops.com/
 Author: CtrlStack inc.
 License: GPLv3
 Project-URL: Documentation, https://docs.promptops.com/cli
 Project-URL: Changelog, https://docs.promptops.com/en/stable/changelog.html
 Project-URL: Live demo, https://promptops.com/
```

### Comparing `promptops-0.1.8/promptops.egg-info/SOURCES.txt` & `promptops-0.1.9/promptops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `promptops-0.1.8/setup.py` & `promptops-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,20 +42,19 @@
         "websockets~=11.0.3",
         "detect-secrets~=1.4.0",
         "prompt-toolkit~=3.0.38",
         "numpy~=1.25.0",
         "pyperclip~=1.8.2",
         "thefuzz~=0.19.0",
         "psutil~=5.9.5",
-        "levenshtein~=0.21.1",
         "wcwidth~=0.2.6",
         "boto3~=1.26.159",
         "kubernetes~=26.1.0",
         "urllib3>=1.26,<2",  # kubernetes uses google-auth which has urllib3<2
-        "setuptools",
+        "setuptools~=68.0.0",
         "pip",
     ],
     entry_points="""
         [console_scripts]
         promptops=promptops.main:entry_main
         um=promptops.main:entry_alias
         qq=promptops.main:entry_alias
```


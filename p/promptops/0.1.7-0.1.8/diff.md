# Comparing `tmp/promptops-0.1.7.tar.gz` & `tmp/promptops-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptops-0.1.7.tar", last modified: Thu Jun 15 19:16:09 2023, max compression
+gzip compressed data, was "promptops-0.1.8.tar", last modified: Fri Jun 23 16:54:02 2023, max compression
```

## Comparing `promptops-0.1.7.tar` & `promptops-0.1.8.tar`

### file list

```diff
@@ -1,107 +1,116 @@
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-15 19:16:09.988314 promptops-0.1.7/
--rw-r--r--   0 vasily     (501) staff       (20)    35149 2023-05-24 15:22:16.000000 promptops-0.1.7/LICENSE.txt
--rw-r--r--   0 vasily     (501) staff       (20)     2841 2023-06-15 19:16:09.988503 promptops-0.1.7/PKG-INFO
--rw-r--r--   0 vasily     (501) staff       (20)     2204 2023-06-15 19:15:23.000000 promptops-0.1.7/README.md
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-15 19:16:09.949813 promptops-0.1.7/local_runner/
--rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.7/local_runner/__init__.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-15 19:16:09.952491 promptops-0.1.7/local_runner/comms/
--rw-r--r--   0 vasily     (501) staff       (20)      133 2023-05-24 13:48:37.000000 promptops-0.1.7/local_runner/comms/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)      432 2023-05-24 13:48:37.000000 promptops-0.1.7/local_runner/comms/base.py
--rw-r--r--   0 vasily     (501) staff       (20)     2890 2023-05-24 13:48:37.000000 promptops-0.1.7/local_runner/comms/dtos.py
--rw-r--r--   0 vasily     (501) staff       (20)     1536 2023-05-24 13:48:37.000000 promptops-0.1.7/local_runner/comms/http_reporter.py
--rw-r--r--   0 vasily     (501) staff       (20)     1671 2023-06-07 21:55:02.000000 promptops-0.1.7/local_runner/comms/ws.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-15 19:16:09.953475 promptops-0.1.7/local_runner/config/
--rw-r--r--   0 vasily     (501) staff       (20)       48 2023-05-24 13:48:37.000000 promptops-0.1.7/local_runner/config/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     1720 2023-05-24 13:48:37.000000 promptops-0.1.7/local_runner/config/config.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-15 19:16:09.954411 promptops-0.1.7/local_runner/creds/
--rw-r--r--   0 vasily     (501) staff       (20)       77 2023-05-24 13:48:37.000000 promptops-0.1.7/local_runner/creds/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     1458 2023-05-24 13:48:37.000000 promptops-0.1.7/local_runner/creds/creds.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-15 19:16:09.955319 promptops-0.1.7/local_runner/exec/
--rw-r--r--   0 vasily     (501) staff       (20)       54 2023-05-24 13:48:37.000000 promptops-0.1.7/local_runner/exec/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     2317 2023-05-24 13:48:37.000000 promptops-0.1.7/local_runner/exec/manager.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-15 19:16:09.956605 promptops-0.1.7/local_runner/handler/
--rw-r--r--   0 vasily     (501) staff       (20)       29 2023-05-24 13:48:37.000000 promptops-0.1.7/local_runner/handler/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)      471 2023-05-24 13:48:37.000000 promptops-0.1.7/local_runner/handler/censor.py
--rw-r--r--   0 vasily     (501) staff       (20)     3115 2023-05-24 13:48:37.000000 promptops-0.1.7/local_runner/handler/handler.py
--rw-r--r--   0 vasily     (501) staff       (20)     1361 2023-06-07 21:55:02.000000 promptops-0.1.7/local_runner/main.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-15 19:16:09.957591 promptops-0.1.7/local_runner/registration/
--rw-r--r--   0 vasily     (501) staff       (20)       56 2023-05-24 13:48:37.000000 promptops-0.1.7/local_runner/registration/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     2523 2023-05-24 13:48:37.000000 promptops-0.1.7/local_runner/registration/registration.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-15 19:16:09.958502 promptops-0.1.7/local_runner/tokens/
--rw-r--r--   0 vasily     (501) staff       (20)       27 2023-05-24 13:48:37.000000 promptops-0.1.7/local_runner/tokens/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     2235 2023-05-24 13:48:37.000000 promptops-0.1.7/local_runner/tokens/issuer.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-15 19:16:09.965985 promptops-0.1.7/promptops/
--rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     1850 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/corrections.py
--rw-r--r--   0 vasily     (501) staff       (20)     1033 2023-06-07 21:55:02.000000 promptops-0.1.7/promptops/feedback.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-15 19:16:09.969292 promptops-0.1.7/promptops/gitaware/
--rw-r--r--   0 vasily     (501) staff       (20)       42 2023-06-07 21:55:02.000000 promptops-0.1.7/promptops/gitaware/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)      658 2023-06-15 19:15:23.000000 promptops-0.1.7/promptops/gitaware/project.py
--rw-r--r--   0 vasily     (501) staff       (20)     4146 2023-06-07 21:55:02.000000 promptops-0.1.7/promptops/history.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-15 19:16:09.971118 promptops-0.1.7/promptops/index/
--rw-r--r--   0 vasily     (501) staff       (20)        0 2023-06-07 21:55:02.000000 promptops-0.1.7/promptops/index/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     2692 2023-06-07 21:55:02.000000 promptops-0.1.7/promptops/index/content.py
--rw-r--r--   0 vasily     (501) staff       (20)     2084 2023-06-07 21:55:02.000000 promptops-0.1.7/promptops/index/entry_point.py
--rw-r--r--   0 vasily     (501) staff       (20)     4399 2023-06-07 21:55:02.000000 promptops-0.1.7/promptops/index/index_store.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-15 19:16:09.975540 promptops-0.1.7/promptops/loading/
--rw-r--r--   0 vasily     (501) staff       (20)      131 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/loading/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)      677 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/loading/base.py
--rw-r--r--   0 vasily     (501) staff       (20)     1139 2023-06-15 19:15:23.000000 promptops-0.1.7/promptops/loading/cancellable.py
--rw-r--r--   0 vasily     (501) staff       (20)      481 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/loading/context.py
--rw-r--r--   0 vasily     (501) staff       (20)     1554 2023-06-15 19:15:23.000000 promptops-0.1.7/promptops/loading/multi.py
--rw-r--r--   0 vasily     (501) staff       (20)     1279 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/loading/pong.py
--rw-r--r--   0 vasily     (501) staff       (20)     1344 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/loading/progress.py
--rw-r--r--   0 vasily     (501) staff       (20)     1077 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/loading/promptops.py
--rw-r--r--   0 vasily     (501) staff       (20)     1025 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/loading/simple.py
--rw-r--r--   0 vasily     (501) staff       (20)     9999 2023-06-15 19:15:23.000000 promptops-0.1.7/promptops/main.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-15 19:16:09.979297 promptops-0.1.7/promptops/query/
--rw-r--r--   0 vasily     (501) staff       (20)       30 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/query/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)      434 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/query/dtos.py
--rw-r--r--   0 vasily     (501) staff       (20)     4351 2023-05-25 18:38:08.000000 promptops-0.1.7/promptops/query/explanation.py
--rw-r--r--   0 vasily     (501) staff       (20)     4506 2023-06-07 21:55:02.000000 promptops-0.1.7/promptops/query/git_repo.py
--rw-r--r--   0 vasily     (501) staff       (20)     9075 2023-06-15 19:15:23.000000 promptops-0.1.7/promptops/query/lookup.py
--rw-r--r--   0 vasily     (501) staff       (20)     1222 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/query/messages.py
--rw-r--r--   0 vasily     (501) staff       (20)    19626 2023-06-15 19:15:23.000000 promptops-0.1.7/promptops/query/query.py
--rw-r--r--   0 vasily     (501) staff       (20)     1126 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/query.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-15 19:16:09.980926 promptops-0.1.7/promptops/recipes/
--rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/recipes/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)    12414 2023-06-15 19:15:23.000000 promptops-0.1.7/promptops/recipes/creation.py
--rw-r--r--   0 vasily     (501) staff       (20)      998 2023-06-15 19:15:23.000000 promptops-0.1.7/promptops/recipes/run.py
--rw-r--r--   0 vasily     (501) staff       (20)     6555 2023-06-15 19:15:23.000000 promptops-0.1.7/promptops/recipes/terraform.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-15 19:16:09.981801 promptops-0.1.7/promptops/scrub_secrets/
--rw-r--r--   0 vasily     (501) staff       (20)       55 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/scrub_secrets/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     2423 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/scrub_secrets/scrub.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-15 19:16:09.982798 promptops-0.1.7/promptops/secrets/
--rw-r--r--   0 vasily     (501) staff       (20)       55 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/secrets/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     2423 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/secrets/scrub.py
--rw-r--r--   0 vasily     (501) staff       (20)      364 2023-06-07 21:55:02.000000 promptops-0.1.7/promptops/settings.py
--rw-r--r--   0 vasily     (501) staff       (20)     2440 2023-06-07 21:55:02.000000 promptops-0.1.7/promptops/settings_store.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-15 19:16:09.985464 promptops-0.1.7/promptops/shells/
--rw-r--r--   0 vasily     (501) staff       (20)       46 2023-06-15 19:15:23.000000 promptops-0.1.7/promptops/shells/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)     4861 2023-06-07 21:55:02.000000 promptops-0.1.7/promptops/shells/base.py
--rw-r--r--   0 vasily     (501) staff       (20)     1245 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/shells/bash.py
--rw-r--r--   0 vasily     (501) staff       (20)     1154 2023-06-15 19:15:23.000000 promptops-0.1.7/promptops/shells/common.py
--rw-r--r--   0 vasily     (501) staff       (20)     1946 2023-06-07 21:55:02.000000 promptops-0.1.7/promptops/shells/fish.py
--rw-r--r--   0 vasily     (501) staff       (20)     2767 2023-06-07 21:55:02.000000 promptops-0.1.7/promptops/shells/zsh.py
--rw-r--r--   0 vasily     (501) staff       (20)     3206 2023-06-15 19:15:23.000000 promptops-0.1.7/promptops/similarity.py
--rw-r--r--   0 vasily     (501) staff       (20)       42 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/trace.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-15 19:16:09.987900 promptops-0.1.7/promptops/ui/
--rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/ui/__init__.py
--rw-r--r--   0 vasily     (501) staff       (20)      138 2023-06-07 21:55:02.000000 promptops-0.1.7/promptops/ui/input.py
--rw-r--r--   0 vasily     (501) staff       (20)     3070 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/ui/prompts.py
--rw-r--r--   0 vasily     (501) staff       (20)     8990 2023-06-07 21:55:02.000000 promptops-0.1.7/promptops/ui/selections.py
--rw-r--r--   0 vasily     (501) staff       (20)      460 2023-06-07 21:55:02.000000 promptops-0.1.7/promptops/ui/vim.py
--rw-r--r--   0 vasily     (501) staff       (20)     1099 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/ui.py
--rw-r--r--   0 vasily     (501) staff       (20)     4570 2023-06-07 21:55:02.000000 promptops-0.1.7/promptops/user.py
--rw-r--r--   0 vasily     (501) staff       (20)       22 2023-06-15 19:15:23.000000 promptops-0.1.7/promptops/version.py
--rw-r--r--   0 vasily     (501) staff       (20)     1632 2023-05-24 13:48:37.000000 promptops-0.1.7/promptops/version_check.py
-drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-15 19:16:09.968311 promptops-0.1.7/promptops.egg-info/
--rw-r--r--   0 vasily     (501) staff       (20)     2841 2023-06-15 19:16:09.000000 promptops-0.1.7/promptops.egg-info/PKG-INFO
--rw-r--r--   0 vasily     (501) staff       (20)     2310 2023-06-15 19:16:09.000000 promptops-0.1.7/promptops.egg-info/SOURCES.txt
--rw-r--r--   0 vasily     (501) staff       (20)        1 2023-06-15 19:16:09.000000 promptops-0.1.7/promptops.egg-info/dependency_links.txt
--rw-r--r--   0 vasily     (501) staff       (20)      120 2023-06-15 19:16:09.000000 promptops-0.1.7/promptops.egg-info/entry_points.txt
--rw-r--r--   0 vasily     (501) staff       (20)      225 2023-06-15 19:16:09.000000 promptops-0.1.7/promptops.egg-info/requires.txt
--rw-r--r--   0 vasily     (501) staff       (20)       23 2023-06-15 19:16:09.000000 promptops-0.1.7/promptops.egg-info/top_level.txt
--rw-r--r--   0 vasily     (501) staff       (20)       87 2023-05-24 14:19:51.000000 promptops-0.1.7/pyproject.toml
--rw-r--r--   0 vasily     (501) staff       (20)       78 2023-06-15 19:16:09.989123 promptops-0.1.7/setup.cfg
--rw-r--r--   0 vasily     (501) staff       (20)     1994 2023-06-15 19:15:23.000000 promptops-0.1.7/setup.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 16:54:02.155254 promptops-0.1.8/
+-rw-r--r--   0 vasily     (501) staff       (20)    35149 2023-05-24 15:22:16.000000 promptops-0.1.8/LICENSE.txt
+-rw-r--r--   0 vasily     (501) staff       (20)     2889 2023-06-23 16:54:02.155423 promptops-0.1.8/PKG-INFO
+-rw-r--r--   0 vasily     (501) staff       (20)     2252 2023-06-23 01:46:23.000000 promptops-0.1.8/README.md
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 16:54:02.111145 promptops-0.1.8/local_runner/
+-rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.8/local_runner/__init__.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 16:54:02.113987 promptops-0.1.8/local_runner/comms/
+-rw-r--r--   0 vasily     (501) staff       (20)      133 2023-05-24 13:48:37.000000 promptops-0.1.8/local_runner/comms/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)      432 2023-05-24 13:48:37.000000 promptops-0.1.8/local_runner/comms/base.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2890 2023-05-24 13:48:37.000000 promptops-0.1.8/local_runner/comms/dtos.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1536 2023-05-24 13:48:37.000000 promptops-0.1.8/local_runner/comms/http_reporter.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1671 2023-06-07 21:55:02.000000 promptops-0.1.8/local_runner/comms/ws.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 16:54:02.115070 promptops-0.1.8/local_runner/config/
+-rw-r--r--   0 vasily     (501) staff       (20)       48 2023-05-24 13:48:37.000000 promptops-0.1.8/local_runner/config/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1720 2023-05-24 13:48:37.000000 promptops-0.1.8/local_runner/config/config.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 16:54:02.115997 promptops-0.1.8/local_runner/creds/
+-rw-r--r--   0 vasily     (501) staff       (20)       77 2023-05-24 13:48:37.000000 promptops-0.1.8/local_runner/creds/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1458 2023-05-24 13:48:37.000000 promptops-0.1.8/local_runner/creds/creds.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 16:54:02.116910 promptops-0.1.8/local_runner/exec/
+-rw-r--r--   0 vasily     (501) staff       (20)       54 2023-05-24 13:48:37.000000 promptops-0.1.8/local_runner/exec/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2317 2023-05-24 13:48:37.000000 promptops-0.1.8/local_runner/exec/manager.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 16:54:02.118124 promptops-0.1.8/local_runner/handler/
+-rw-r--r--   0 vasily     (501) staff       (20)       29 2023-05-24 13:48:37.000000 promptops-0.1.8/local_runner/handler/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)      471 2023-05-24 13:48:37.000000 promptops-0.1.8/local_runner/handler/censor.py
+-rw-r--r--   0 vasily     (501) staff       (20)     3115 2023-05-24 13:48:37.000000 promptops-0.1.8/local_runner/handler/handler.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1361 2023-06-07 21:55:02.000000 promptops-0.1.8/local_runner/main.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 16:54:02.118887 promptops-0.1.8/local_runner/registration/
+-rw-r--r--   0 vasily     (501) staff       (20)       56 2023-05-24 13:48:37.000000 promptops-0.1.8/local_runner/registration/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2523 2023-05-24 13:48:37.000000 promptops-0.1.8/local_runner/registration/registration.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 16:54:02.119722 promptops-0.1.8/local_runner/tokens/
+-rw-r--r--   0 vasily     (501) staff       (20)       27 2023-05-24 13:48:37.000000 promptops-0.1.8/local_runner/tokens/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2235 2023-05-24 13:48:37.000000 promptops-0.1.8/local_runner/tokens/issuer.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 16:54:02.126470 promptops-0.1.8/promptops/
+-rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.8/promptops/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1850 2023-05-24 13:48:37.000000 promptops-0.1.8/promptops/corrections.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1033 2023-06-07 21:55:02.000000 promptops-0.1.8/promptops/feedback.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 16:54:02.129624 promptops-0.1.8/promptops/gitaware/
+-rw-r--r--   0 vasily     (501) staff       (20)       42 2023-06-07 21:55:02.000000 promptops-0.1.8/promptops/gitaware/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     3161 2023-06-23 16:03:30.000000 promptops-0.1.8/promptops/gitaware/commits.py
+-rw-r--r--   0 vasily     (501) staff       (20)      658 2023-06-15 19:15:23.000000 promptops-0.1.8/promptops/gitaware/project.py
+-rw-r--r--   0 vasily     (501) staff       (20)     4146 2023-06-07 21:55:02.000000 promptops-0.1.8/promptops/history.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 16:54:02.131459 promptops-0.1.8/promptops/index/
+-rw-r--r--   0 vasily     (501) staff       (20)        0 2023-06-07 21:55:02.000000 promptops-0.1.8/promptops/index/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2691 2023-06-16 22:44:53.000000 promptops-0.1.8/promptops/index/content.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2084 2023-06-07 21:55:02.000000 promptops-0.1.8/promptops/index/entry_point.py
+-rw-r--r--   0 vasily     (501) staff       (20)     4399 2023-06-07 21:55:02.000000 promptops-0.1.8/promptops/index/index_store.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 16:54:02.136263 promptops-0.1.8/promptops/loading/
+-rw-r--r--   0 vasily     (501) staff       (20)      131 2023-05-24 13:48:37.000000 promptops-0.1.8/promptops/loading/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)      745 2023-06-21 21:04:09.000000 promptops-0.1.8/promptops/loading/base.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1139 2023-06-15 19:15:23.000000 promptops-0.1.8/promptops/loading/cancellable.py
+-rw-r--r--   0 vasily     (501) staff       (20)      481 2023-05-24 13:48:37.000000 promptops-0.1.8/promptops/loading/context.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1554 2023-06-15 19:15:23.000000 promptops-0.1.8/promptops/loading/multi.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1279 2023-05-24 13:48:37.000000 promptops-0.1.8/promptops/loading/pong.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1344 2023-05-24 13:48:37.000000 promptops-0.1.8/promptops/loading/progress.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1077 2023-05-24 13:48:37.000000 promptops-0.1.8/promptops/loading/promptops.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1051 2023-06-21 21:04:09.000000 promptops-0.1.8/promptops/loading/simple.py
+-rw-r--r--   0 vasily     (501) staff       (20)    11413 2023-06-23 16:03:30.000000 promptops-0.1.8/promptops/main.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 16:54:02.140405 promptops-0.1.8/promptops/query/
+-rw-r--r--   0 vasily     (501) staff       (20)       28 2023-06-21 01:03:51.000000 promptops-0.1.8/promptops/query/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)      434 2023-06-16 19:21:46.000000 promptops-0.1.8/promptops/query/dtos.py
+-rw-r--r--   0 vasily     (501) staff       (20)     4351 2023-05-25 18:38:08.000000 promptops-0.1.8/promptops/query/explanation.py
+-rw-r--r--   0 vasily     (501) staff       (20)     4506 2023-06-07 21:55:02.000000 promptops-0.1.8/promptops/query/git_repo.py
+-rw-r--r--   0 vasily     (501) staff       (20)     9058 2023-06-23 01:46:23.000000 promptops-0.1.8/promptops/query/lookup.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1222 2023-05-24 13:48:37.000000 promptops-0.1.8/promptops/query/messages.py
+-rw-r--r--   0 vasily     (501) staff       (20)    19960 2023-06-23 16:03:30.000000 promptops-0.1.8/promptops/query/query.py
+-rw-r--r--   0 vasily     (501) staff       (20)     6165 2023-06-23 01:46:23.000000 promptops-0.1.8/promptops/query/suggest_next.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1126 2023-05-24 13:48:37.000000 promptops-0.1.8/promptops/query.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 16:54:02.143171 promptops-0.1.8/promptops/recipes/
+-rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.8/promptops/recipes/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)    14644 2023-06-21 21:04:09.000000 promptops-0.1.8/promptops/recipes/creation.py
+-rw-r--r--   0 vasily     (501) staff       (20)      606 2023-06-16 22:44:53.000000 promptops-0.1.8/promptops/recipes/executor.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1076 2023-06-23 01:46:23.000000 promptops-0.1.8/promptops/recipes/run.py
+-rw-r--r--   0 vasily     (501) staff       (20)     7585 2023-06-21 01:03:51.000000 promptops-0.1.8/promptops/recipes/terraform.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 16:54:02.144351 promptops-0.1.8/promptops/scrub_secrets/
+-rw-r--r--   0 vasily     (501) staff       (20)       55 2023-05-24 13:48:37.000000 promptops-0.1.8/promptops/scrub_secrets/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2423 2023-05-24 13:48:37.000000 promptops-0.1.8/promptops/scrub_secrets/scrub.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 16:54:02.145410 promptops-0.1.8/promptops/secret/
+-rw-r--r--   0 vasily     (501) staff       (20)       55 2023-06-16 22:44:53.000000 promptops-0.1.8/promptops/secret/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2423 2023-06-16 22:44:53.000000 promptops-0.1.8/promptops/secret/scrub.py
+-rw-r--r--   0 vasily     (501) staff       (20)      438 2023-06-23 16:03:30.000000 promptops-0.1.8/promptops/settings.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2593 2023-06-23 16:03:30.000000 promptops-0.1.8/promptops/settings_store.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 16:54:02.149282 promptops-0.1.8/promptops/shells/
+-rw-r--r--   0 vasily     (501) staff       (20)       46 2023-06-15 19:15:23.000000 promptops-0.1.8/promptops/shells/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)     7003 2023-06-23 01:46:23.000000 promptops-0.1.8/promptops/shells/base.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1816 2023-06-23 01:46:23.000000 promptops-0.1.8/promptops/shells/bash.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1154 2023-06-21 02:44:24.000000 promptops-0.1.8/promptops/shells/common.py
+-rw-r--r--   0 vasily     (501) staff       (20)     2410 2023-06-23 01:46:23.000000 promptops-0.1.8/promptops/shells/fish.py
+-rw-r--r--   0 vasily     (501) staff       (20)     4012 2023-06-23 01:46:23.000000 promptops-0.1.8/promptops/shells/zsh.py
+-rw-r--r--   0 vasily     (501) staff       (20)     3206 2023-06-15 19:15:23.000000 promptops-0.1.8/promptops/similarity.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 16:54:02.152199 promptops-0.1.8/promptops/skills/
+-rw-r--r--   0 vasily     (501) staff       (20)        0 2023-06-21 01:03:51.000000 promptops-0.1.8/promptops/skills/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)      108 2023-06-21 01:03:51.000000 promptops-0.1.8/promptops/skills/choice.py
+-rw-r--r--   0 vasily     (501) staff       (20)      940 2023-06-22 03:44:33.000000 promptops-0.1.8/promptops/skills/commit_message.py
+-rw-r--r--   0 vasily     (501) staff       (20)     9282 2023-06-23 16:03:30.000000 promptops-0.1.8/promptops/skills/dtt.py
+-rw-r--r--   0 vasily     (501) staff       (20)      558 2023-06-21 21:04:09.000000 promptops-0.1.8/promptops/skills/next.py
+-rw-r--r--   0 vasily     (501) staff       (20)       42 2023-05-24 13:48:37.000000 promptops-0.1.8/promptops/trace.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 16:54:02.154721 promptops-0.1.8/promptops/ui/
+-rw-r--r--   0 vasily     (501) staff       (20)        0 2023-05-24 13:48:37.000000 promptops-0.1.8/promptops/ui/__init__.py
+-rw-r--r--   0 vasily     (501) staff       (20)      138 2023-06-07 21:55:02.000000 promptops-0.1.8/promptops/ui/input.py
+-rw-r--r--   0 vasily     (501) staff       (20)     3070 2023-05-24 13:48:37.000000 promptops-0.1.8/promptops/ui/prompts.py
+-rw-r--r--   0 vasily     (501) staff       (20)     9308 2023-06-23 16:03:30.000000 promptops-0.1.8/promptops/ui/selections.py
+-rw-r--r--   0 vasily     (501) staff       (20)      621 2023-06-21 01:03:51.000000 promptops-0.1.8/promptops/ui/vim.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1099 2023-05-24 13:48:37.000000 promptops-0.1.8/promptops/ui.py
+-rw-r--r--   0 vasily     (501) staff       (20)     4570 2023-06-07 21:55:02.000000 promptops-0.1.8/promptops/user.py
+-rw-r--r--   0 vasily     (501) staff       (20)       22 2023-06-23 01:46:23.000000 promptops-0.1.8/promptops/version.py
+-rw-r--r--   0 vasily     (501) staff       (20)     1632 2023-05-24 13:48:37.000000 promptops-0.1.8/promptops/version_check.py
+drwxr-xr-x   0 vasily     (501) staff       (20)        0 2023-06-23 16:54:02.128338 promptops-0.1.8/promptops.egg-info/
+-rw-r--r--   0 vasily     (501) staff       (20)     2889 2023-06-23 16:54:02.000000 promptops-0.1.8/promptops.egg-info/PKG-INFO
+-rw-r--r--   0 vasily     (501) staff       (20)     2540 2023-06-23 16:54:02.000000 promptops-0.1.8/promptops.egg-info/SOURCES.txt
+-rw-r--r--   0 vasily     (501) staff       (20)        1 2023-06-23 16:54:02.000000 promptops-0.1.8/promptops.egg-info/dependency_links.txt
+-rw-r--r--   0 vasily     (501) staff       (20)      120 2023-06-23 16:54:02.000000 promptops-0.1.8/promptops.egg-info/entry_points.txt
+-rw-r--r--   0 vasily     (501) staff       (20)      260 2023-06-23 16:54:02.000000 promptops-0.1.8/promptops.egg-info/requires.txt
+-rw-r--r--   0 vasily     (501) staff       (20)       23 2023-06-23 16:54:02.000000 promptops-0.1.8/promptops.egg-info/top_level.txt
+-rw-r--r--   0 vasily     (501) staff       (20)       87 2023-05-24 14:19:51.000000 promptops-0.1.8/pyproject.toml
+-rw-r--r--   0 vasily     (501) staff       (20)       78 2023-06-23 16:54:02.155984 promptops-0.1.8/setup.cfg
+-rw-r--r--   0 vasily     (501) staff       (20)     2051 2023-06-23 16:53:44.000000 promptops-0.1.8/setup.py
```

### Comparing `promptops-0.1.7/LICENSE.txt` & `promptops-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `promptops-0.1.7/PKG-INFO` & `promptops-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptops
-Version: 0.1.7
+Version: 0.1.8
 Summary: Your CLI assistant. Ask questions, get shell commands.
 Home-page: https://promptops.com/
 Author: CtrlStack inc.
 License: GPLv3
 Project-URL: Documentation, https://docs.promptops.com/cli
 Project-URL: Changelog, https://docs.promptops.com/en/stable/changelog.html
 Project-URL: Live demo, https://promptops.com/
@@ -50,15 +50,19 @@
 
 ```shell
 pip3 install promptops
 ```
 
 # Configuration
 
-## Enable extended reverse search (Ctrl+E)
+```shell
+eval "$(um --install)"
+```
+
+## (Optional) Enable extended reverse search (Ctrl+E)
 
 Note: currently works only with Zsh
 
 Add the widget and the key binding to your `.zshrc` file
 ```shell
 cp ~/.zshrc ~/.zshrc.backup
 echo 'eval "$(promptops lookup --config)"' >> ~/.zshrc
```

### Comparing `promptops-0.1.7/README.md` & `promptops-0.1.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,19 @@
 
 ```shell
 pip3 install promptops
 ```
 
 # Configuration
 
-## Enable extended reverse search (Ctrl+E)
+```shell
+eval "$(um --install)"
+```
+
+## (Optional) Enable extended reverse search (Ctrl+E)
 
 Note: currently works only with Zsh
 
 Add the widget and the key binding to your `.zshrc` file
 ```shell
 cp ~/.zshrc ~/.zshrc.backup
 echo 'eval "$(promptops lookup --config)"' >> ~/.zshrc
```

### Comparing `promptops-0.1.7/local_runner/comms/dtos.py` & `promptops-0.1.8/local_runner/comms/dtos.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.7/local_runner/comms/http_reporter.py` & `promptops-0.1.8/local_runner/comms/http_reporter.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.7/local_runner/comms/ws.py` & `promptops-0.1.8/local_runner/comms/ws.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.7/local_runner/config/config.py` & `promptops-0.1.8/local_runner/config/config.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.7/local_runner/creds/creds.py` & `promptops-0.1.8/local_runner/creds/creds.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.7/local_runner/exec/manager.py` & `promptops-0.1.8/local_runner/exec/manager.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.7/local_runner/handler/handler.py` & `promptops-0.1.8/local_runner/handler/handler.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.7/local_runner/main.py` & `promptops-0.1.8/local_runner/main.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.7/local_runner/registration/registration.py` & `promptops-0.1.8/local_runner/registration/registration.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.7/local_runner/tokens/issuer.py` & `promptops-0.1.8/local_runner/tokens/issuer.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.7/promptops/corrections.py` & `promptops-0.1.8/promptops/corrections.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.7/promptops/feedback.py` & `promptops-0.1.8/promptops/feedback.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.7/promptops/gitaware/project.py` & `promptops-0.1.8/promptops/gitaware/project.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.7/promptops/history.py` & `promptops-0.1.8/promptops/history.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.7/promptops/index/content.py` & `promptops-0.1.8/promptops/index/content.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Union, Optional
 import numpy as np
 import requests
 
 from promptops.trace import trace_id
 from promptops import user
 from promptops.loading.progress import ProgressSpinner
-from promptops.secrets import scrub_file
+from promptops.secret import scrub_file
 from promptops import settings
 from promptops.similarity import VectorDB
 
 from .index_store import ItemMetadata
 
 
 def index_content(content: Union[str, bytes], content_type: str) -> VectorDB:
```

### Comparing `promptops-0.1.7/promptops/index/entry_point.py` & `promptops-0.1.8/promptops/index/entry_point.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.7/promptops/index/index_store.py` & `promptops-0.1.8/promptops/index/index_store.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.7/promptops/loading/base.py` & `promptops-0.1.8/promptops/loading/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import sys
 import colorama
 
 LINE_UP = '\033[1A'
 
 
 class LoadingBase(object):
-    def __init__(self):
-        self._stream = sys.stdout
+    def __init__(self, stream=None):
+        if stream is None:
+            stream = sys.stdout
+        self._stream = stream
         self._step = 0
         self._written_lines = 0
 
     def step(self):
         self.clear()
         self._draw()
         self._step += 1
```

### Comparing `promptops-0.1.7/promptops/loading/cancellable.py` & `promptops-0.1.8/promptops/loading/cancellable.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.7/promptops/loading/multi.py` & `promptops-0.1.8/promptops/loading/multi.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.7/promptops/loading/pong.py` & `promptops-0.1.8/promptops/loading/pong.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.7/promptops/loading/progress.py` & `promptops-0.1.8/promptops/loading/progress.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.7/promptops/loading/promptops.py` & `promptops-0.1.8/promptops/loading/promptops.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.7/promptops/loading/simple.py` & `promptops-0.1.8/promptops/loading/simple.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 TWO_DOTS = "⠃⠆⡄⣀⢠⠰⠘⠉"
 THREE_DOTS = "⠇⠦⠴⠸⠙⠋"
 FOUR_DOTS = "⡇⣆⣤⣰⢸⠹⠛⠏"
 
 
 class Simple(LoadingBase):
-    def __init__(self, text: str, style=THREE_DOTS):
-        super().__init__()
+    def __init__(self, text: str, style=THREE_DOTS, stream=None):
+        super().__init__(stream=stream)
         self._style = style
         self._text = text
 
     def _get_text(self):
         char = self._style[self._step % len(self._style)]
         return colorama.Fore.GREEN + char + colorama.Style.RESET_ALL + " " + self._text
```

### Comparing `promptops-0.1.7/promptops/main.py` & `promptops-0.1.8/promptops/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,39 +22,73 @@
 
 import logging
 
 from promptops import settings
 from promptops import settings_store
 from promptops import version_check
 from promptops import user
-from promptops.recipes.creation import recipe_entrypoint
-from promptops.index.entry_point import entry_point as index_entry_point
-from promptops.query.lookup import entry_point as lookup_entry_point
+
+from promptops.feedback import feedback
 
 ENDPOINT_ENV = "PROMPTOPS_ENDPOINT"
 
 
 def runner_mode(args):
-    from promptops.feedback import feedback
     from local_runner.main import entry_point
 
     feedback({"event": "runner_mode"})
     entry_point()
 
 
+def check_if_installed():
+    from promptops.shells import get_shell
+    if not get_shell().is_installed():
+        from prompt_toolkit import print_formatted_text
+        from prompt_toolkit.formatted_text import HTML
+        print()
+        print_formatted_text(HTML("<ansired>Warning: um is not fully configured. To finish the installation, run:</ansired>"))
+        print_formatted_text(HTML("<ansigreen>  eval \"$(um --install)\"</ansigreen>"))
+        print()
+
+
 def query_mode(args):
-    from promptops import query
-    query.query_mode(args)
+    if args.verbose:
+        logging.basicConfig(level=logging.DEBUG)
+    else:
+        logging.basicConfig(level=logging.INFO, format="%(message)s")
+    settings.model = args.mode
+    settings.history_context = args.history_context
+    settings.request_explanation = args.explain
+
+    question = " ".join(args.question)
+    try:
+        if question.strip():
+            feedback({"event": "query_mode"})
+            from promptops import query
+            query.do_query(question)
+        else:
+            feedback({"event": "dtt_mode"})
+            from promptops.skills import dtt
+            dtt.entry_point()
+    except KeyboardInterrupt:
+        pass
+    if settings_store.is_changed():
+        for _ in range(3):
+            answer = input("save the current settings? [y/n]")
+            if answer == "y":
+                settings_store.save()
+                break
+            elif answer == "n":
+                break
+    check_if_installed()
 
 
 def lookup_mode(args):
-    from promptops.feedback import feedback
     from promptops.query.lookup import entry_point as lookup_entry_point
 
-    feedback({"event": "lookup_mode"})
     lookup_entry_point(args)
 
 
 def recipe_mode(args):
     from promptops.recipes.creation import recipe_entrypoint
     recipe_entrypoint(args)
 
@@ -99,14 +133,16 @@
         prog=alias,
         usage=f"{alias} [options] <question>\nexample: {alias} list running ec2 instances",
         description=f"{alias}: a command line assistant",
     )
     parser.add_argument("--verbose", "-v", action="store_true", help="verbose output")
     parser.add_argument("--version", action="store_true", help="print version and exit")
     parser.add_argument("--config", action="store_true", help="reconfigure")
+    parser.add_argument("--shell-config", action="store_true", help="print configuration for your shell")
+    parser.add_argument("--install", action="store_true", help="print install script")
     parser.add_argument(
         "--history-context",
         default=settings.history_context,
         type=int,
         help="past commands to include in the query (default: %(default)s)",
     )
     parser.add_argument(
@@ -125,28 +161,40 @@
     )
     parser.add_argument(
         "--mode", default=settings.model, choices=["fast", "accurate"], help="fast or accurate (default: %(default)s)"
     )
     parser.add_argument("question", nargs=REMAINDER, help="the question to ask")
     registered = user.has_registered()
     args = parser.parse_args()
+
+    if args.shell_config:
+        from promptops.shells import get_shell
+        print(get_shell().get_config())
+        sys.exit(0)
+    if args.install:
+        from promptops.shells import get_shell
+        print(get_shell().install())
+        sys.exit(0)
+
     if args.version:
         from promptops.version import __version__
 
         print(__version__)
         r = version_check.version_check()
         if not r.update_required:
             print("latest version:", r.latest_version)
+        check_if_installed()
         sys.exit(0)
 
     if args.verbose:
         logging.basicConfig(level=logging.DEBUG)
     else:
         logging.basicConfig(level=logging.INFO, format="%(message)s")
     version_check.version_check()
+
     if not registered or args.config:
         user.register()
         args.history_context = settings.history_context
     else:
         from promptops import history
 
         history.update_history()
@@ -205,14 +253,16 @@
         action="store_false",
         default=settings.request_explanation,
         help="get faster response",
     )
     parser_question.add_argument(
         "--mode", default=settings.model, choices=["fast", "accurate"], help="fast or accurate (default: %(default)s)"
     )
+    parser_question.add_argument("--shell-config", action="store_true", help="print configuration for your shell")
+    parser_question.add_argument("--install", action="store_true", help="print install script")
     parser_question.add_argument("question", nargs=REMAINDER, help="the question to ask")
     parser_question.set_defaults(func=query_mode)
 
     parser_runner = subparsers.add_parser("runner", help="run commands from slack")
     parser_runner.set_defaults(func=runner_mode)
 
     parser_workflow = subparsers.add_parser("recipe", help="run a complex or multi-stepped script")
@@ -226,19 +276,14 @@
     parser_index.set_defaults(func=index_mode)
 
     parser_lookup = subparsers.add_parser("lookup", help="extended reverse search, use --config to configure in your shell")
     parser_lookup.add_argument("--config", action="store_true", help="print configuration for your shell")
     parser_lookup.add_argument("command", nargs=REMAINDER, help="the command to lookup")
     parser_lookup.set_defaults(func=lookup_mode)
 
-    parser_lookup = subparsers.add_parser("lookup", help="extended reverse search, use --config to configure in your shell")
-    parser_lookup.add_argument("--config", help="print configuration for your shell")
-    parser_lookup.add_argument("command", nargs=REMAINDER, help="the command to lookup")
-    parser_lookup.set_defaults(func=lookup_entry_point)
-
     args = parser.parse_args()
 
     registered = user.has_registered()
 
     if not hasattr(args, "func"):
         if args.version:
             from promptops.version import __version__
```

### Comparing `promptops-0.1.7/promptops/query/explanation.py` & `promptops-0.1.8/promptops/query/explanation.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.7/promptops/query/git_repo.py` & `promptops-0.1.8/promptops/query/git_repo.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.7/promptops/query/lookup.py` & `promptops-0.1.8/promptops/query/lookup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import sys
 import threading
 import queue
+
+from promptops.feedback import feedback
+
 from promptops.similarity import embedding
 from promptops.history import get_history_db
 from promptops.corrections import get_db
 from thefuzz import process, fuzz
 from promptops.shells import get_shell_name
 
 
@@ -149,18 +152,14 @@
 
                 self.options = [match for match, _ in matches[:self._max_items]]
                 self.render()
             except Exception as e:
                 self.options = [str(e)]
                 self._loading = False
                 self.render()
-            except Exception as e:
-                self.options = [str(e)]
-                self._loading = False
-                self.render()
 
     def render(self):
         with self._lock:
             if self._raw_mode:
                 import termios
                 fd = sys.stdin.fileno()
                 termios.tcsetattr(fd, termios.TCSADRAIN, self._old_stdin_attrs)
@@ -245,20 +244,22 @@
             sys.exit(1)
         if shell_name in CONFIG_SCRIPTS:
             sys.stdout.write(CONFIG_SCRIPTS[shell_name])
             sys.stdout.flush()
             return
         sys.exit(1)
 
+    feedback({"event": "lookup_mode"})
     # give us some space
     max_results = 10
     sys.stderr.write("\n"*(max_results + 1))
     sys.stderr.write(f"\x1b[{max_results}A")
 
     try:
         text = App(max_items=max_results).run()
     except KeyboardInterrupt:
+        feedback({"event": "lookup-cancel"})
         sys.exit(1)
     if text is None:
         sys.exit(1)
     sys.stdout.write(text)
     sys.stdout.flush()
```

### Comparing `promptops-0.1.7/promptops/query/messages.py` & `promptops-0.1.8/promptops/query/messages.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.7/promptops/query/query.py` & `promptops-0.1.8/promptops/query/query.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,28 +10,27 @@
 from typing import Optional
 
 import colorama
 import requests
 from prompt_toolkit import print_formatted_text
 from prompt_toolkit.patch_stdout import patch_stdout
 from prompt_toolkit.formatted_text import HTML, to_formatted_text
-import prompt_toolkit
+from promptops.shells import get_shell
 
 from promptops import settings
 from promptops import trace
 from promptops import user
 from promptops.ui import prompts
 from promptops.ui import selections
 from promptops.loading import Simple, loading_animation
 from promptops import similarity
 from promptops import corrections
 from promptops.corrections import get_correction
 from promptops.feedback import feedback
 from promptops import history
-from promptops import settings_store
 from promptops import scrub_secrets
 from promptops import shells
 from promptops.index import index_store
 from promptops import gitaware
 from .dtos import Result
 from .explanation import get_explanation, ReturningThread
 from . import messages
@@ -73,16 +72,17 @@
         thread_out.join()
         thread_err.join()
 
         sys.stdout.write("\n")
         sys.stdout.flush()
 
         process.wait()
-
+        get_shell().add_to_history(cmd.script)
         history.add(scrub_secrets.scrub_line(".bash_history", cmd.script), process.returncode)
+
         return process.returncode, "".join(stderr)
     else:
         raise NotImplementedError(f"{cmd.lang} not implemented yet")
 
 
 def corrections_search(embedding):
     db = corrections.get_db()
@@ -103,15 +103,15 @@
     return similar
 
 
 def make_revise_option():
     return "\x1b[3m💭️ don't see what you're looking for? try providing more context\x1b[0m"
 
 
-ORIGIN_SYMBOLS = {"history": "📖", "promptops": "✨"}
+ORIGIN_SYMBOLS = {"history": "📖", "promptops": "✨", "curated": "📚"}
 
 
 def ellipsis_if_needed(text, max_width, more="..."):
     if len(text) <= max_width:
         return text
     return text[:max_width - len(more)] + more
 
@@ -175,53 +175,64 @@
                 corrected_results=[qa for qa, _ in similar_corrections],
                 prev_results=prev_results,
                 similar_history=[r.script for r in history_results],
                 history_context=history_context,
                 relevant_indexed_data=relevant_indexed_data,
             ),
             daemon=True,
+        ),
+        ReturningThread(
+            curated,
+            kwargs=dict(
+                q=questions[-1],
+            ),
+            daemon=True,
         )
     ]
     num_running = len(tasks)
 
     def update_results(extra):
         with update_lock:
             nonlocal num_running
+            nonlocal ui
             num_running -= 1
-            # TODO: deduplicate
             results.extend(extra)
+            options = [pretty_result(r) for r in deduplicate(results)]
+            if num_running == 0:
+                if len(results) == 0:
+                    feedback({"event": "no-results"})
+                    print("couldn't find any results, try rephrasing your question or providing more context")
+                    selected = prompts.confirm_clarify("")
+                    if selected == prompts.EXIT:
+                        raise KeyboardInterrupt()
+                    return ConfirmResult(question=selected, options=[])
+                options += [make_revise_option()]
             if ui:
-                options = [pretty_result(r) for r in results]
-                if num_running == 0:
-                    options += [make_revise_option()]
                 ui.reset_options(options, is_loading=num_running > 0)
+            else:
+                ui = selections.UI(
+                    options,
+                    num_running > 0,
+                    loading_text=random.choice(messages.QUERY),
+                    actions={
+                        "\x08": remove_entry,
+                        "\x7F": remove_entry,
+                    },
+                )
 
     def done_callback(thread: ReturningThread):
         try:
             update_results(thread.result())
         except Exception as exc:
             logging.exception(exc)
 
     for task in tasks:
         task.add_done_callback(done_callback)
         task.start()
 
-    if len(results) == 0:
-        with loading_animation(Simple("thinking...")):
-            results = [r for t in tasks for r in t.join()]
-        num_running = 0
-        results = deduplicate(results)
-        if len(results) == 0:
-            feedback({"event": "no-results"})
-            print("couldn't find any results, try rephrasing your question or providing more context")
-            selected = prompts.confirm_clarify("")
-            if selected == prompts.EXIT:
-                raise KeyboardInterrupt()
-            return ConfirmResult(question=selected, options=[])
-
     def remove_entry(_, ui: selections.UI):
         with update_lock:
             if ui.selected >= len(results):
                 return
             result = results[ui.selected]
             if result.origin == "history":
                 results.pop(ui.selected)
@@ -236,23 +247,26 @@
         hdb.save(os.path.expanduser(settings.history_db_path))
 
     while True:
         with update_lock:
             options = [pretty_result(r) for r in results]
             if num_running == 0:
                 options += [make_revise_option()]
-            ui = selections.UI(
-                options,
-                num_running > 0,
-                loading_text=random.choice(messages.QUERY),
-                actions={
-                    "\x08": remove_entry,
-                    "\x7F": remove_entry,
-                },
-            )
+            if ui:
+                ui.reset_options(options, is_loading=num_running > 0)
+            else:
+                ui = selections.UI(
+                    options,
+                    num_running > 0,
+                    loading_text=random.choice(messages.QUERY),
+                    actions={
+                        "\x08": remove_entry,
+                        "\x7F": remove_entry,
+                    },
+                )
         index = ui.input()
         print()
         if index == len(results):
             selected = prompts.confirm_clarify("")
             if selected == prompts.GO_BACK:
                 continue
             elif selected == prompts.EXIT:
@@ -372,57 +386,36 @@
 
 def do_query(question: str):
     if git_root := gitaware.git_root():
         from .git_repo import offer_to_index
         offer_to_index(git_root)
 
     question = question.strip()
-    if question == "":
-        feedback({"event": "empty-initial-query"})
-        for i in range(2):
-            if i > 0:
-                print("please enter a question")
-            bottom_toolbar = HTML("<b>[enter]</b> confirm <b>[ctrl+c]</b> exit")
-            # get the name of the calling script
-            alias = os.path.basename(sys.argv[0])
-            question = prompt_toolkit.prompt(f"{alias}: ", bottom_toolbar=bottom_toolbar)
-            question = question.strip()
-            if question != "":
-                break
-        else:
-            print("no question entered")
-            sys.exit(0)
-
     questions = [question]
     prev_results = []
 
     print()
 
     def input_loop():
         history_context = shells.get_shell().get_recent_history(settings.history_context) if settings.history_context else []
         while True:
-            try:
-                results = revise_loop(questions, prev_results, history_context)
-                if results.result:
-                    return results.result, results.confirmed
-                else:
-                    print()
-                    feedback({"event": "revise"})
-                    questions.append(results.question)
-                    prev_results.append(results.options)
-            except KeyboardInterrupt:
+            results = revise_loop(questions, prev_results, history_context)
+            if results.result:
+                return results.result, results.confirmed
+            else:
                 print()
-                feedback({"event": "cancelled"})
-                sys.exit(1)
+                feedback({"event": "revise"})
+                questions.append(results.question)
+                prev_results.append(results.options)
 
     try:
         cmd, confirmed = input_loop()
     except KeyboardInterrupt:
         feedback({"event": "cancelled"})
-        sys.exit(1)
+        return
 
     if cmd.lang == "text":
         return
 
     if confirmed:
         # the user corrected the script
         db = corrections.get_db()
@@ -451,36 +444,14 @@
             vector = similarity.embedding(text=q)
             db.update_or_add(vector, corrections.QATuple(question=q, answer=cmd.script, corrected=corrected_cmd.script).to_dict(), equals=lambda a, b: a["question"] == b["question"])
             logging.debug("added correction to db")
             db.save(os.path.expanduser(settings.corrections_db_path))
         feedback({"event": "finished", "rc": rc, "corrected": True})
 
 
-def query_mode(args):
-    if args.verbose:
-        logging.basicConfig(level=logging.DEBUG)
-    else:
-        logging.basicConfig(level=logging.INFO, format="%(message)s")
-    settings.model = args.mode
-    settings.history_context = args.history_context
-    settings.request_explanation = args.explain
-    try:
-        do_query(" ".join(args.question))
-        if settings_store.is_changed():
-            for _ in range(3):
-                answer = input("save the current settings? [y/n]")
-                if answer == "y":
-                    settings_store.save()
-                    break
-                elif answer == "n":
-                    break
-    except KeyboardInterrupt:
-        pass
-
-
 def query(
     *,
     q: str,
     prev_questions: list[str],
     prev_results: list[list[str]],
     corrected_results: list[corrections.QATuple],
     history_context: list[str],
@@ -532,7 +503,50 @@
     try:
         message = data.get("message")
     except KeyError:
         message = "-"
         logging.debug("no message in response: %s", json.dumps(data, indent=2))
 
     return [Result(script=message, lang="text", explanation="-")]
+
+
+def curated(*, q: str) -> list[Result]:
+    req = {
+        "query": q,
+        "trace_id": trace.trace_id,
+        "platform": sys.platform,
+        "shell": os.environ.get("SHELL"),
+    }
+    logging.debug("curated query with request: %s", req)
+    response = requests.post(
+        settings.endpoint + "/curated",
+        json=req,
+        headers={
+            "user-agent": f"promptops-cli; user_id={user.user_id()}",
+        },
+    )
+    if response.status_code != 200:
+        # this exception completely destroys the ui
+        return []
+        # raise Exception(f"there was problem with the response, status: {response.status_code}, text: {response.text}")
+
+    data = response.json()
+    try:
+        return [content_to_result(entry["content"]) for entry in data["items"] if entry["score"] >= 0.75]
+    except KeyError:
+        logging.debug("no suggestions in response: %s", json.dumps(data, indent=2))
+
+    try:
+        message = data.get("message")
+    except KeyError:
+        message = "-"
+        logging.debug("no message in response: %s", json.dumps(data, indent=2))
+
+    return [Result(script=message, lang="text", explanation="-")]
+
+
+def content_to_result(content) -> Result:
+    return Result(
+        script=content["content"],
+        lang="shell",
+        origin="curated",
+    )
```

### Comparing `promptops-0.1.7/promptops/query.py` & `promptops-0.1.8/promptops/query.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.7/promptops/recipes/creation.py` & `promptops-0.1.8/promptops/recipes/creation.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import logging
 import os
 import queue
 import subprocess
+import time
 
 import colorama
 import requests
 import sys
 
 from typing import Optional
 from promptops import settings
@@ -21,14 +22,19 @@
 from promptops.ui.vim import edit_with_vim
 
 LANG_SHELL = 'shell'
 LANG_TF = 'terraform'
 LANG_OPTIONS = [LANG_TF, LANG_SHELL]
 
 
+class StreamException(Exception):
+    pass
+
+
+
 def handle_execution_response(recipe, response, loading):
     completed_queue = queue.Queue()
     started_queue = queue.Queue()
     file_loader = None
     loading_parameters = False
     for line in response.iter_lines():
         if line:
@@ -45,14 +51,16 @@
                 recipe.setdefault('execution', []).append(json_line)
                 completed_queue.put(json_line.get('key'))
             elif json_line.get('parameter'):
                 if not loading_parameters:
                     started_queue.put('gathering parameters')
                     loading_parameters = True
                 recipe.setdefault('parameters', []).append(json_line)
+            elif json_line.get('error'):
+                raise StreamException
             else:
                 logging.debug('unknown json object', json_line)
 
     if file_loader:
         file_loader.stop()
     return recipe
 
@@ -121,14 +129,16 @@
     for line in response.iter_lines():
         if line:
             if loading:
                 loading.stop()
             json_line = json.loads(line.decode('utf-8'))
             if json_line.get('id'):
                 recipe['id'] = json_line.get('id')
+            elif json_line.get('error'):
+                raise StreamException
             elif json_line.get('step'):
                 if len(recipe['steps']) == 0:
                     print("Based on your requirements & extra details, I've set the project outline to include the following steps: ")
                 recipe['steps'].append(json_line.get('step'))
                 prefix, step_num = json_line.get("prefix", ""), ""
                 if prefix == " -- ":
                     prefix = colorama.Fore.RED + prefix + colorama.Style.RESET_ALL
@@ -177,14 +187,16 @@
     for line in response.iter_lines():
         if line:
             if loading:
                 loading.stop()
             json_line = json.loads(line.decode('utf-8'))
             if json_line.get('id'):
                 recipe['id'] = json_line.get('id')
+            elif json_line.get('error'):
+                raise StreamException
             elif json_line.get('step'):
                 if len(recipe['steps']) == 0:
                     print("Based on your requirements, I've set the project outline to include the following steps: ")
                 recipe['steps'].append(json_line.get('step'))
                 print(f"{len(recipe['steps'])}. {json_line.get('step')}")
             if loading:
                 loading.start()
@@ -289,16 +301,46 @@
     )
 
     if response.status_code != 200:
         print("error", response.json())
         raise Exception(f"there was problem with the response, status: {response.status_code}")
 
 
+def edit_parameters(recipe):
+    parameter_names = [p.get('parameter') for p in recipe.get('parameters')]
+    options = parameter_names + ['exit']
+
+    while True:
+        print("Do you want to set defaults or modify any of the parameters?\n")
+
+        ui = selections.UI(options, is_loading=False)
+        selection = ui.input()
+
+        if selection == len(options) - 1:
+            break
+
+        parameter = recipe.get('parameters')[selection]
+        print(f"{parameter.get('name')}: {parameter.get('description')}")
+        modify = ['set a default value', 'modify the question', 'go back']
+        selection = None
+        while selection != 2:
+            print()
+            ui = selections.UI(modify, is_loading=False)
+            selection = ui.input()
+            if selection == 0:
+                parameter['default'] = non_empty_input('enter a default value: ')
+            elif selection == 1:
+                parameter['description'] = non_empty_input('enter a new question for the parameter: ')
+    return recipe
+
+
 def save_flow(recipe):
     print()
+    recipe = edit_parameters(recipe)
+
     req = {
         'id': recipe.get('id'),
         'trace_id': trace.trace_id,
         'name': non_empty_input("Enter a name for the saved workflow: "),
         'parameters': recipe.get('parameters'),
         'execution': recipe.get('execution')
     }
@@ -348,47 +390,67 @@
             selected = recipes[recipe_selection]
         else:
             print("\nSelect from available recipes: ")
     return selected
 
 
 def recipe_entrypoint(args):
+    last = "recipe-entrypoint"
     try:
         new_recipe = True
         if not args or len(args.question) < 2:
             new_recipe = False
+            last = "recipe-list"
             recipe = available_recipes()
             if not recipe:
                 return
             recipe = get_recipe(recipe['prompt'], recipe['language'], recipe['id'])
+            last = "recipe-select"
         else:
             prompt = " ".join(args.question[1:])
 
             print("Recipes currently utilize Terraform. Support for more methods coming soon.\n")
             # ui = selections.UI(LANG_OPTIONS, is_loading=False)
             # selection = ui.input()
             # print()
             selection = 0
-
+            last = "recipe-init"
             recipe = init_recipe(prompt, LANG_OPTIONS[selection], loading=CancellableSimpleLoader("getting an outline ready..."))
+            last = "recipe-edit-steps"
             recipe = edit_steps(recipe)
 
+            last = "recipe-get"
             loading = CancellableSimpleLoader("generating files, please be patient as this can take several minutes...")
             recipe = get_recipe_execution(recipe, loading)
 
+        last = "recipe-load-execution"
         executor = TerraformExecutor(recipe, regenerate_recipe_execution)
         result = executor.run()
+        last = "recipe-execute"
         feedback({"event": "recipe-execute", "id": recipe.get('id'), "result": result})
 
         if new_recipe:
             print()
             print("Would you like to save this as a reusable recipe?")
             print()
             ui = selections.UI(["save", "exit"], is_loading=False)
             selection = ui.input()
             if selection == 0:
+                last = "recipe-save"
+
+                print("Would you like us to save the changes you made to the files?")
+                ui = selections.UI(["save", "skip"], is_loading=False)
+                selection = ui.input()
+
+                if selection == 0:
+                    recipe = executor.update()
+
                 save_flow(recipe)
                 print()
                 print("To use a saved recipe, simply type 'um recipe'")
             print()
     except KeyboardInterrupt:
+        feedback({"event": "recipe-cancel", "last_executed": last, "time": time.time()})
         pass
+    except StreamException:
+        print("Failed to stream the response back successfully, please try again")
+        feedback({"event": "recipe-error", "error": "failed to stream"})
```

### Comparing `promptops-0.1.7/promptops/recipes/run.py` & `promptops-0.1.8/promptops/recipes/run.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import subprocess
 import sys
 import threading
 from typing import Tuple
 
+from promptops.shells import get_shell
+
 
 def run_command(script, directory) -> Tuple[bool, str]:
+
     def printer(pipe, func):
         for line in iter(pipe.readline, b''):
             line_decoded = line.decode()
             sys.stdout.write(line_decoded)
             sys.stdout.flush()
             func(line)
         pipe.close()
@@ -27,11 +30,10 @@
     thread_out.join()
     thread_err.join()
 
     sys.stdout.write("\n")
     sys.stdout.flush()
 
     process.wait()
+    get_shell().add_to_history(script)
 
     return process.returncode == 0, "".join(stderr)
-
-
```

### Comparing `promptops-0.1.7/promptops/recipes/terraform.py` & `promptops-0.1.8/promptops/recipes/terraform.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import os
 from dataclasses import dataclass
 from typing import Tuple
-
-from promptops.loading import Simple
 from promptops.loading.cancellable import CancellableSimpleLoader
+from promptops.recipes.executor import Executor
 from promptops.recipes.run import run_command
 from promptops.ui import selections
 from promptops.ui.input import non_empty_input
 from promptops.ui.prompts import confirm, GO_BACK
 
 
 @dataclass
 class Step:
     file: str
     content: str
 
 
-class TerraformExecutor:
+class TerraformExecutor(Executor):
     def __init__(self, recipe, regen):
         self.recipe = recipe
         self.execution_steps = [Step(i.get('key'), i.get('value')) for i in recipe.get('execution')]
         self.parameters = recipe.get('parameters')
         directory = non_empty_input("enter a relative directory to store the terraform module in: ").strip()
         directory = directory if directory[0] != "/" else directory[1:]
         directory = directory if directory[-1] == "/" else directory + "/"
@@ -48,15 +47,15 @@
 
             if selection == 0:
                 break
             elif selection == 1:
                 # todo: Create a cache of parameter values before regenerating!
                 print()
                 clarify = input("Provide more clarification (optional): ")
-                self.recipe = self.regen(self.recipe, clarify, loading=Simple("regenerating terraform files..."))
+                self.recipe = self.regen(self.recipe, clarify, loading=CancellableSimpleLoader("regenerating terraform files..."))
                 self.execution_steps = [Step(i.get('key'), i.get('value')) for i in self.recipe.get('execution')]
                 self.parameters = self.recipe.get('parameters')
                 self.clean()
                 self.write_files()
             elif selection == 2:
                 self.init()
                 success, err = self.plan()
@@ -107,28 +106,31 @@
                     inp = input(f"enter additional values for {parameter.get('parameter')} or hit enter to continue: ").strip()
                     value.append(inp)
 
             parameter['value'] = value
 
         return self.parameters
 
+    @staticmethod
+    def get_tf_value_from_param(parameter):
+        if parameter['type'] == "list":
+            items = [f'"{i}"' for i in parameter['value']]
+            return f"[{' ,'.join(items)}]"
+        else:
+            return f"{parameter['value']}"
+
+
     def execute(self):
         for step in self.execution_steps:
             if not os.path.exists(self.directory + step.file):
                 open(self.directory + step.file, 'w').close()
             for parameter in self.parameters:
-                if parameter['parameter'] in step.content:
-                    if parameter['type'] == "list":
-                        items = [f'"{i}"' for i in parameter['value']]
-                        value = f"[{' ,'.join(items)}]"
-                    else:
-                        value = f"{parameter['value']}"
-
+                if parameter['parameter'] in step.content and parameter['value'].strip() != "":
                     var_name = f"<{parameter['parameter']}>"
-                    step.content = step.content.replace(var_name, value)
+                    step.content = step.content.replace(var_name, self.get_tf_value_from_param(parameter))
 
             with open(self.directory + step.file, "w") as outfile:
                 outfile.write(step.content)
 
     def clean(self):
         for step in self.execution_steps:
             if os.path.exists(self.directory + step.file):
@@ -140,17 +142,40 @@
             return True, ""
         return run_command("terraform init", self.directory)
 
     def plan(self) -> Tuple[bool, str]:
         return run_command("terraform plan", self.directory)
 
     def apply(self) -> Tuple[bool, str]:
-        return run_command("terraform apply", self.directory)
+        return run_command("terraform apply", self.directory)\
 
 
     def fix(self, error):
         self.recipe = self.regen(self.recipe, "an error occurred", error, loading=CancellableSimpleLoader("attempting to fix terraform files..."))
         self.execution_steps = [Step(i.get('key'), i.get('value')) for i in self.recipe.get('execution')]
         self.parameters = self.recipe.get('parameters')
         self.clean()
         self.write_files()
         return
+
+
+    def update(self) -> dict:
+        param_used = {p['parameter']: False for p in self.parameters}
+        for step in self.execution_steps:
+            with open(self.directory + step.file, 'r') as f:
+                edited_lines = "".join(f.readlines())
+
+            for parameter in self.parameters:
+                value = self.get_tf_value_from_param(parameter)
+                if value in edited_lines:
+                    param_used[parameter['parameter']] = True
+                    edited_lines = edited_lines.replace(value, "<" + parameter['parameter'] + ">")
+
+            print(f'before: \n {step.content} \n after: \n {edited_lines}\n')
+
+            step.content = edited_lines
+
+
+        self.recipe['execution'] = [{'key': step.file, 'value': step.content} for step in self.execution_steps]
+        self.parameters = [p for p in self.parameters if param_used[p['parameter']]]
+
+        return self.recipe
```

### Comparing `promptops-0.1.7/promptops/scrub_secrets/scrub.py` & `promptops-0.1.8/promptops/scrub_secrets/scrub.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.7/promptops/secrets/scrub.py` & `promptops-0.1.8/promptops/secret/scrub.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.7/promptops/settings_store.py` & `promptops-0.1.8/promptops/settings_store.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,24 +23,26 @@
     settings.endpoint = data.get("endpoint", settings.endpoint)
     settings.request_explanation = data.get("request_explanation", settings.request_explanation)
     settings.model = data.get("model", settings.model)
     settings.history_context = data.get("history_context", settings.history_context)
     settings.corrections_db_path = data.get("corrections_db_path", settings.corrections_db_path)
     settings.history_db_path = data.get("history_db_path", settings.history_db_path)
     settings.index_history = data.get("index_history", settings.index_history)
+    settings.gen_commit_message = data.get("gen_commit_message", settings.gen_commit_message)
 
 
 def _build_data():
     data = {
         "request_explanation": settings.request_explanation,
         "model": settings.model,
         "history_context": settings.history_context,
         "corrections_db_path": settings.corrections_db_path,
         "history_db_path": settings.history_db_path,
         "index_history": settings.index_history,
+        "gen_commit_message": settings.gen_commit_message,
     }
     if settings.endpoint != settings.DEFAULT_ENDPOINT:
         data["endpoint"] = settings.endpoint
     return data
 
 
 def save():
```

### Comparing `promptops-0.1.7/promptops/shells/bash.py` & `promptops-0.1.8/promptops/shells/bash.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,20 @@
             history_file = os.getenv("HISTFILE", "~/.bash_history")
         super().__init__(history_file)
 
     def get_recent_history(self, look_back: int = 10):
         fname = os.path.expanduser(self.history_file)
         buffer = ""
         commands = []
+        for line in reversed(self._get_added_history()):
+            if len(commands) >= look_back:
+                break
+            if accept_command(line):
+                commands.append(line)
+
         for line in reverse_readline(fname):
             if len(commands) >= look_back:
                 break
             current = line.rstrip()
             if current.endswith("\\"):
                 buffer = current + "\n" + buffer
                 continue
@@ -31,7 +37,23 @@
         commands = []
         for line in lines:
             buffer += "\n" + line.rstrip()
             if not line.endswith("\\"):
                 commands.append(buffer.lstrip())
                 buffer = ""
         return commands
+
+    def get_config(self):
+        return f"""
+function um() {{
+    command um $@
+    if [[ -f {self.temp_history_file} ]]; then
+        while IFS= read -r line; do
+            test -n "$line" && history -s "$line"
+        done < {self.temp_history_file}
+        rm {self.temp_history_file}
+    fi
+}}
+""".strip()
+
+    def _get_config_file(self):
+        return "~/.bashrc"
```

### Comparing `promptops-0.1.7/promptops/shells/common.py` & `promptops-0.1.8/promptops/shells/common.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.7/promptops/shells/fish.py` & `promptops-0.1.8/promptops/shells/fish.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import subprocess
+import time
+
 from .base import Shell
 from .base import reverse_readline, accept_command
 from promptops.scrub_secrets import scrub_lines
 import os
 import logging
 
 
@@ -44,7 +47,23 @@
                 try:
                     cmd = cmd.encode("latin-1", "backslashreplace").decode("unicode-escape")
                     if accept_command(cmd):
                         commands.append(cmd)
                 except UnicodeDecodeError:
                     logging.debug("UnicodeDecodeError at line: ", line)
         return scrub_lines(fname, list(reversed(commands)))
+
+    def add_to_history(self, script):
+        with open(os.path.expanduser(self.history_file), 'a') as history:
+            entry = f'- cmd: {script}\n   when: {time.time()}\n'
+            history.write(entry)
+
+    def get_config(self):
+        return """
+function um -d "your CLI assistant"
+    command um $argv
+    builtin history merge
+end
+""".strip()
+
+    def _get_config_file(self):
+        return "~/.config/fish/config.fish"
```

### Comparing `promptops-0.1.7/promptops/shells/zsh.py` & `promptops-0.1.8/promptops/shells/zsh.py`

 * *Files 26% similar despite different names*

```diff
@@ -33,14 +33,21 @@
             history_file = os.getenv("HISTFILE", "~/.zsh_history")
         super().__init__(history_file)
 
     def get_recent_history(self, look_back: int = 10):
         fname = os.path.expanduser(self.history_file)
         buffer = ""
         commands = []
+
+        for line in reversed(self._get_added_history()):
+            if len(commands) >= look_back:
+                break
+            if accept_command(line):
+                commands.append(line)
+
         starting = True
         for line in reverse_readline(fname, transform=unmetafy):
             if starting and line == "":
                 continue
             starting = False
             if len(commands) >= look_back:
                 break
@@ -52,36 +59,66 @@
                 buffer = ""
                 if accept_command(cmd):
                     commands.append(cmd)
             else:
                 line = line.rstrip()
                 if line.endswith("\\"):
                     line = line[:-1]
-                buffer = "\n" + line + buffer
+                    buffer = "\n" + line + buffer
+                else:
+                    if buffer:
+                        cmd = buffer.lstrip("\n")
+                        if accept_command(cmd):
+                            commands.append(cmd)
+                    buffer = "\n" + line
         return scrub_lines(fname, list(reversed(commands)))
 
     def get_full_history(self):
         fname = os.path.expanduser(self.history_file)
         lines = list(readline(fname, transform=unmetafy))
         commands = filter(accept_command, self._get_cmds_from_lines(lines))
-        return scrub_lines(fname, list(commands))
+        return scrub_lines(fname, list(commands) + list(filter(accept_command, self._get_added_history())))
 
     def _get_cmds_from_lines(self, lines):
         buffer = ""
         commands = []
         # find the index of the last non-empty line
         i = len(lines) - 1
         for i in range(len(lines) - 1, -1, -1):
             if lines[i] != "":
                 break
         for line in lines[:i+1]:
             if _is_zsh_start_line(line):
                 if buffer != "":
                     commands.append(buffer)
                 buffer = line.split(";")[1].rstrip()
+                if buffer.endswith("\\"):
+                    buffer = buffer[:-1]
             else:
-                buffer += "\n" + line.rstrip()
-            if buffer.endswith("\\"):
-                buffer = buffer[:-1]
+                line = line.rstrip()
+                if line.endswith("\\"):
+                    buffer += "\n" + line[:-1]
+                else:
+                    if buffer:
+                        buffer = buffer.lstrip("\n")
+                        commands.append(buffer + "\n" + line)
+                    else:
+                        commands.append(line.lstrip("\n"))
+                    buffer = ""
         if buffer != "" and not buffer.endswith("\\"):
-            commands.append(buffer)
+            commands.append(buffer.lstrip("\n"))
         return commands
+
+    def get_config(self):
+        return f"""
+um() {{
+    command um $@
+    if [[ -f {self.temp_history_file} ]]; then
+        while IFS= read -r line; do
+            test -n "$line" && print -s "$line"
+        done < {self.temp_history_file}
+        rm {self.temp_history_file}
+    fi
+}}""".strip()
+
+    def _get_config_file(self):
+        return "~/.zshrc"
```

### Comparing `promptops-0.1.7/promptops/similarity.py` & `promptops-0.1.8/promptops/similarity.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.7/promptops/ui/prompts.py` & `promptops-0.1.8/promptops/ui/prompts.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.7/promptops/ui/selections.py` & `promptops-0.1.8/promptops/ui/selections.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import sys
 import time
 import threading
 import os
+import re
 import typing
 from promptops.loading.simple import loader
 from prompt_toolkit.formatted_text import to_plain_text, ANSI
 import wcwidth
 import colorama
 
 
@@ -181,16 +182,21 @@
     def options(self):
         return self._options
 
     @property
     def is_loading(self):
         return self._is_loading
 
-    def _get_formatted_text(self, option: str, selected: bool):
-        return f"{colorama.Style.BRIGHT if selected else ''}{option}{colorama.Style.RESET_ALL}"
+    @staticmethod
+    def _get_formatted_text(option: str, selected: bool):
+        opt = "\n".join(
+                [(colorama.Fore.LIGHTYELLOW_EX if re.match("^. *#.*$", line) else colorama.Fore.LIGHTWHITE_EX) + line
+                 for line in option.split("\n")]
+        )
+        return f"{colorama.Style.BRIGHT if selected else ''}{opt}{colorama.Style.RESET_ALL}".replace("\n", "\n      ")
 
     def add_options(self, options, is_loading=False):
         if not self._is_active:
             return
         self._options.extend(options)
         self._is_loading = is_loading
         self.render()
@@ -245,7 +251,11 @@
                 self._is_active = False
                 self._is_loading = False
                 self._footer = None
                 self.render()
                 return self._selected
             elif key in self._actions:
                 self._actions[key](key, self)
+
+    @property
+    def is_active(self):
+        return self._is_active
```

### Comparing `promptops-0.1.7/promptops/ui.py` & `promptops-0.1.8/promptops/ui.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.7/promptops/user.py` & `promptops-0.1.8/promptops/user.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.7/promptops/version_check.py` & `promptops-0.1.8/promptops/version_check.py`

 * *Files identical despite different names*

### Comparing `promptops-0.1.7/promptops.egg-info/PKG-INFO` & `promptops-0.1.8/promptops.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptops
-Version: 0.1.7
+Version: 0.1.8
 Summary: Your CLI assistant. Ask questions, get shell commands.
 Home-page: https://promptops.com/
 Author: CtrlStack inc.
 License: GPLv3
 Project-URL: Documentation, https://docs.promptops.com/cli
 Project-URL: Changelog, https://docs.promptops.com/en/stable/changelog.html
 Project-URL: Live demo, https://promptops.com/
@@ -50,15 +50,19 @@
 
 ```shell
 pip3 install promptops
 ```
 
 # Configuration
 
-## Enable extended reverse search (Ctrl+E)
+```shell
+eval "$(um --install)"
+```
+
+## (Optional) Enable extended reverse search (Ctrl+E)
 
 Note: currently works only with Zsh
 
 Add the widget and the key binding to your `.zshrc` file
 ```shell
 cp ~/.zshrc ~/.zshrc.backup
 echo 'eval "$(promptops lookup --config)"' >> ~/.zshrc
```

### Comparing `promptops-0.1.7/promptops.egg-info/SOURCES.txt` & `promptops-0.1.8/promptops.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 promptops.egg-info/PKG-INFO
 promptops.egg-info/SOURCES.txt
 promptops.egg-info/dependency_links.txt
 promptops.egg-info/entry_points.txt
 promptops.egg-info/requires.txt
 promptops.egg-info/top_level.txt
 promptops/gitaware/__init__.py
+promptops/gitaware/commits.py
 promptops/gitaware/project.py
 promptops/index/__init__.py
 promptops/index/content.py
 promptops/index/entry_point.py
 promptops/index/index_store.py
 promptops/loading/__init__.py
 promptops/loading/base.py
@@ -61,26 +62,33 @@
 promptops/query/__init__.py
 promptops/query/dtos.py
 promptops/query/explanation.py
 promptops/query/git_repo.py
 promptops/query/lookup.py
 promptops/query/messages.py
 promptops/query/query.py
+promptops/query/suggest_next.py
 promptops/recipes/__init__.py
 promptops/recipes/creation.py
+promptops/recipes/executor.py
 promptops/recipes/run.py
 promptops/recipes/terraform.py
 promptops/scrub_secrets/__init__.py
 promptops/scrub_secrets/scrub.py
-promptops/secrets/__init__.py
-promptops/secrets/scrub.py
+promptops/secret/__init__.py
+promptops/secret/scrub.py
 promptops/shells/__init__.py
 promptops/shells/base.py
 promptops/shells/bash.py
 promptops/shells/common.py
 promptops/shells/fish.py
 promptops/shells/zsh.py
+promptops/skills/__init__.py
+promptops/skills/choice.py
+promptops/skills/commit_message.py
+promptops/skills/dtt.py
+promptops/skills/next.py
 promptops/ui/__init__.py
 promptops/ui/input.py
 promptops/ui/prompts.py
 promptops/ui/selections.py
 promptops/ui/vim.py
```

### Comparing `promptops-0.1.7/setup.py` & `promptops-0.1.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,25 +34,27 @@
     },
     license='GPLv3',
     packages=find_packages(exclude=("tests", "tests.*")),
     include_package_data=False,
     python_requires=">=3.9",
     install_requires=[
         "colorama~=0.4.6",
-        "urllib3>=1.26,<2",  # kubernetes uses google-auth which has urllib3<2
-        "requests~=2.29.0",
-        "websockets~=11.0.2",
+        "requests~=2.31.0",
+        "websockets~=11.0.3",
         "detect-secrets~=1.4.0",
         "prompt-toolkit~=3.0.38",
-        "numpy~=1.24.3",
+        "numpy~=1.25.0",
         "pyperclip~=1.8.2",
-        "psutil~=5.9.5",
         "thefuzz~=0.19.0",
-        "boto3~=1.26.131",
+        "psutil~=5.9.5",
+        "levenshtein~=0.21.1",
+        "wcwidth~=0.2.6",
+        "boto3~=1.26.159",
         "kubernetes~=26.1.0",
+        "urllib3>=1.26,<2",  # kubernetes uses google-auth which has urllib3<2
         "setuptools",
         "pip",
     ],
     entry_points="""
         [console_scripts]
         promptops=promptops.main:entry_main
         um=promptops.main:entry_alias
```


# Comparing `tmp/fractal_client-1.3.0a2.tar.gz` & `tmp/fractal_client-1.3.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_client-1.3.0a2.tar", max compression
+gzip compressed data, was "fractal_client-1.3.0a3.tar", max compression
```

## Comparing `fractal_client-1.3.0a2.tar` & `fractal_client-1.3.0a3.tar`

### file list

```diff
@@ -1,106 +1,106 @@
--rw-r--r--   0        0        0     1576 2023-05-09 19:58:57.312677 fractal_client-1.3.0a2/LICENSE
--rw-r--r--   0        0        0     2484 2023-06-12 14:10:42.230233 fractal_client-1.3.0a2/README.md
--rw-r--r--   0        0        0       24 2023-06-12 14:15:35.227390 fractal_client-1.3.0a2/fractal/__init__.py
--rw-r--r--   0        0        0      124 2023-05-26 13:31:24.681931 fractal_client-1.3.0a2/fractal/__main__.py
--rw-r--r--   0        0        0     3448 2023-05-26 13:44:53.339222 fractal_client-1.3.0a2/fractal/authclient.py
--rw-r--r--   0        0        0     3773 2023-05-30 07:19:20.910204 fractal_client-1.3.0a2/fractal/client.py
--rw-r--r--   0        0        0    12216 2023-06-12 14:05:40.809583 fractal_client-1.3.0a2/fractal/cmd/__init__.py
--rw-r--r--   0        0        0     6863 2023-06-05 08:33:35.839631 fractal_client-1.3.0a2/fractal/cmd/_aux_task_caching.py
--rw-r--r--   0        0        0     5795 2023-06-06 12:51:00.225986 fractal_client-1.3.0a2/fractal/cmd/_dataset.py
--rw-r--r--   0        0        0     5115 2023-06-06 12:51:00.229986 fractal_client-1.3.0a2/fractal/cmd/_job.py
--rw-r--r--   0        0        0     4031 2023-06-06 12:51:00.229986 fractal_client-1.3.0a2/fractal/cmd/_project.py
--rw-r--r--   0        0        0     6139 2023-06-12 14:05:40.809583 fractal_client-1.3.0a2/fractal/cmd/_task.py
--rw-r--r--   0        0        0     4620 2023-06-06 12:51:00.229986 fractal_client-1.3.0a2/fractal/cmd/_user.py
--rw-r--r--   0        0        0     9027 2023-06-12 06:40:09.560661 fractal_client-1.3.0a2/fractal/cmd/_workflow.py
--rw-r--r--   0        0        0       42 2023-02-21 08:49:25.750218 fractal_client-1.3.0a2/fractal/common/.git
--rw-r--r--   0        0        0      717 2023-03-06 13:52:20.997699 fractal_client-1.3.0a2/fractal/common/.github/workflows/ci.yml
--rw-r--r--   0        0        0      364 2023-02-21 08:49:27.594201 fractal_client-1.3.0a2/fractal/common/.github/workflows/project-management.yml
--rw-r--r--   0        0        0       34 2023-03-06 13:52:21.001699 fractal_client-1.3.0a2/fractal/common/.gitignore
--rw-r--r--   0        0        0      620 2023-02-21 08:49:27.594201 fractal_client-1.3.0a2/fractal/common/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1964 2023-03-06 13:52:21.001699 fractal_client-1.3.0a2/fractal/common/README.md
--rw-r--r--   0        0        0        0 2023-02-21 08:49:27.594201 fractal_client-1.3.0a2/fractal/common/__init__.py
--rw-r--r--   0        0        0      149 2023-02-21 10:13:04.505672 fractal_client-1.3.0a2/fractal/common/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      147 2023-03-16 09:04:47.705157 fractal_client-1.3.0a2/fractal/common/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0       57 2023-05-26 06:48:59.488787 fractal_client-1.3.0a2/fractal/common/requirements.txt
--rw-r--r--   0        0        0      614 2023-05-25 12:31:57.653940 fractal_client-1.3.0a2/fractal/common/schemas/__init__.py
--rw-r--r--   0        0        0      411 2023-05-25 12:32:05.945818 fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      372 2023-03-16 09:04:47.705157 fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      490 2023-03-03 14:13:42.839064 fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/_validator.cpython-310.pyc
--rw-r--r--   0        0        0     1753 2023-04-20 07:56:22.895496 fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/_validators.cpython-310.pyc
--rw-r--r--   0        0        0     1251 2023-03-16 09:04:47.793156 fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/_validators.cpython-39.pyc
--rw-r--r--   0        0        0     1610 2023-05-26 06:49:58.096032 fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
--rw-r--r--   0        0        0     2027 2023-03-16 09:04:47.705157 fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/applyworkflow.cpython-39.pyc
--rw-r--r--   0        0        0     4068 2023-06-12 13:01:03.378002 fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/manifest.cpython-310.pyc
--rw-r--r--   0        0        0     3515 2023-03-16 09:04:47.797156 fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/manifest.cpython-39.pyc
--rw-r--r--   0        0        0     3537 2023-05-26 06:49:58.132032 fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/project.cpython-310.pyc
--rw-r--r--   0        0        0     3711 2023-03-16 09:04:47.797156 fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/project.cpython-39.pyc
--rw-r--r--   0        0        0     1165 2023-05-26 06:49:58.136032 fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/state.cpython-310.pyc
--rw-r--r--   0        0        0     1185 2023-03-16 09:04:47.801156 fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/state.cpython-39.pyc
--rw-r--r--   0        0        0     2705 2023-06-12 13:01:03.386002 fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/task.cpython-310.pyc
--rw-r--r--   0        0        0     4994 2023-03-16 09:04:47.805156 fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/task.cpython-39.pyc
--rw-r--r--   0        0        0     3292 2023-06-12 13:01:03.390002 fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/task_collection.cpython-310.pyc
--rw-r--r--   0        0        0     1202 2023-05-25 12:32:06.097816 fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/user.cpython-310.pyc
--rw-r--r--   0        0        0     1024 2023-03-16 09:04:47.809156 fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/user.cpython-39.pyc
--rw-r--r--   0        0        0     3882 2023-05-26 06:49:58.328029 fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/workflow.cpython-310.pyc
--rw-r--r--   0        0        0     1616 2023-04-06 11:30:39.096144 fractal_client-1.3.0a2/fractal/common/schemas/_validators.py
--rw-r--r--   0        0        0     1117 2023-05-26 06:48:59.488787 fractal_client-1.3.0a2/fractal/common/schemas/applyworkflow.py
--rw-r--r--   0        0        0     3479 2023-06-12 10:22:50.369047 fractal_client-1.3.0a2/fractal/common/schemas/manifest.py
--rw-r--r--   0        0        0     2483 2023-05-26 06:48:59.488787 fractal_client-1.3.0a2/fractal/common/schemas/project.py
--rw-r--r--   0        0        0      673 2023-05-26 06:48:59.488787 fractal_client-1.3.0a2/fractal/common/schemas/state.py
--rw-r--r--   0        0        0     2578 2023-06-12 10:22:50.369047 fractal_client-1.3.0a2/fractal/common/schemas/task.py
--rw-r--r--   0        0        0     2935 2023-06-12 10:22:50.369047 fractal_client-1.3.0a2/fractal/common/schemas/task_collection.py
--rw-r--r--   0        0        0     1216 2023-05-25 12:31:57.653940 fractal_client-1.3.0a2/fractal/common/schemas/user.py
--rw-r--r--   0        0        0     2457 2023-05-26 06:48:59.488787 fractal_client-1.3.0a2/fractal/common/schemas/workflow.py
--rw-r--r--   0        0        0      415 2023-03-06 13:52:30.189594 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0      415 2023-03-07 09:47:31.002846 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      415 2023-04-20 07:57:03.191274 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      415 2023-06-12 13:01:14.929878 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/conftest.cpython-310-pytest-7.3.2.pyc
--rw-r--r--   0        0        0     1578 2023-03-06 13:52:30.221594 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1578 2023-03-07 09:47:31.038845 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      606 2023-05-15 11:49:28.546463 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      606 2023-06-12 13:01:14.961878 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.2.pyc
--rw-r--r--   0        0        0     3382 2023-03-15 10:53:32.644401 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     3382 2023-04-20 07:57:03.471272 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     3382 2023-06-12 13:01:15.169875 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.2.pyc
--rw-r--r--   0        0        0      859 2023-03-06 13:52:30.469591 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0      859 2023-03-07 09:47:31.354842 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1241 2023-06-12 13:01:03.562000 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1241 2023-06-12 13:01:15.169875 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.2.pyc
--rw-r--r--   0        0        0     2236 2023-03-06 13:52:30.469591 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1164 2023-04-20 07:56:23.111495 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1164 2023-04-20 07:57:03.471272 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1164 2023-06-12 13:01:15.169875 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.2.pyc
--rw-r--r--   0        0        0     1763 2023-03-06 14:08:06.438014 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1763 2023-03-07 09:47:31.358842 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1763 2023-04-20 07:57:03.471272 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1763 2023-06-12 13:01:15.173875 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.2.pyc
--rw-r--r--   0        0        0     2222 2023-03-06 13:52:30.473591 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     2222 2023-03-07 09:47:31.358842 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2792 2023-05-25 12:32:06.297813 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2792 2023-06-12 13:01:15.173875 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.2.pyc
--rw-r--r--   0        0        0     1335 2023-06-12 13:01:03.566000 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_task_collection.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1335 2023-06-12 13:01:15.177875 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_task_collection.cpython-310-pytest-7.3.2.pyc
--rw-r--r--   0        0        0     1317 2023-03-06 13:52:30.473591 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     2213 2023-04-20 07:56:23.115495 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2671 2023-05-25 12:32:06.301813 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2671 2023-06-12 13:01:15.177875 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.2.pyc
--rw-r--r--   0        0        0     2579 2023-03-06 14:43:41.164713 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     3032 2023-04-20 07:56:23.115495 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2911 2023-05-15 11:49:28.882460 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2911 2023-06-12 13:01:15.177875 fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.2.pyc
--rw-r--r--   0        0        0      139 2023-03-06 13:52:21.001699 fractal_client-1.3.0a2/fractal/common/tests/conftest.py
--rw-r--r--   0        0        0      298 2023-05-11 16:07:56.531485 fractal_client-1.3.0a2/fractal/common/tests/test_applyworkflow.py
--rw-r--r--   0        0        0     2144 2023-03-14 13:42:31.592919 fractal_client-1.3.0a2/fractal/common/tests/test_dataset.py
--rw-r--r--   0        0        0     1420 2023-06-12 10:22:50.369047 fractal_client-1.3.0a2/fractal/common/tests/test_manifest.py
--rw-r--r--   0        0        0      525 2023-04-06 11:30:39.096144 fractal_client-1.3.0a2/fractal/common/tests/test_project.py
--rw-r--r--   0        0        0      551 2023-03-06 14:07:44.150418 fractal_client-1.3.0a2/fractal/common/tests/test_state.py
--rw-r--r--   0        0        0     1190 2023-05-25 12:31:57.653940 fractal_client-1.3.0a2/fractal/common/tests/test_task.py
--rw-r--r--   0        0        0      968 2023-06-12 10:22:50.369047 fractal_client-1.3.0a2/fractal/common/tests/test_task_collection.py
--rw-r--r--   0        0        0     1499 2023-05-25 12:31:57.653940 fractal_client-1.3.0a2/fractal/common/tests/test_user.py
--rw-r--r--   0        0        0     2596 2023-05-11 16:07:56.531485 fractal_client-1.3.0a2/fractal/common/tests/test_workflow.py
--rw-r--r--   0        0        0     1285 2023-05-12 13:33:57.004876 fractal_client-1.3.0a2/fractal/config.py
--rw-r--r--   0        0        0     1609 2023-05-09 19:58:57.316677 fractal_client-1.3.0a2/fractal/interface.py
--rw-r--r--   0        0        0    23055 2023-06-12 14:05:40.809583 fractal_client-1.3.0a2/fractal/parser.py
--rw-r--r--   0        0        0     1265 2023-05-09 19:58:57.316677 fractal_client-1.3.0a2/fractal/response.py
--rw-r--r--   0        0        0     1851 2023-06-12 14:15:35.227390 fractal_client-1.3.0a2/pyproject.toml
--rw-r--r--   0        0        0     3329 1970-01-01 00:00:00.000000 fractal_client-1.3.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1576 2023-05-09 19:58:57.312677 fractal_client-1.3.0a3/LICENSE
+-rw-r--r--   0        0        0     2492 2023-06-13 10:01:05.958774 fractal_client-1.3.0a3/README.md
+-rw-r--r--   0        0        0       24 2023-06-13 10:01:20.162621 fractal_client-1.3.0a3/fractal/__init__.py
+-rw-r--r--   0        0        0      124 2023-05-26 13:31:24.681931 fractal_client-1.3.0a3/fractal/__main__.py
+-rw-r--r--   0        0        0     3448 2023-05-26 13:44:53.339222 fractal_client-1.3.0a3/fractal/authclient.py
+-rw-r--r--   0        0        0     3773 2023-05-30 07:19:20.910204 fractal_client-1.3.0a3/fractal/client.py
+-rw-r--r--   0        0        0    12216 2023-06-12 14:05:40.809583 fractal_client-1.3.0a3/fractal/cmd/__init__.py
+-rw-r--r--   0        0        0     6863 2023-06-05 08:33:35.839631 fractal_client-1.3.0a3/fractal/cmd/_aux_task_caching.py
+-rw-r--r--   0        0        0     5795 2023-06-06 12:51:00.225986 fractal_client-1.3.0a3/fractal/cmd/_dataset.py
+-rw-r--r--   0        0        0     5115 2023-06-06 12:51:00.229986 fractal_client-1.3.0a3/fractal/cmd/_job.py
+-rw-r--r--   0        0        0     4031 2023-06-06 12:51:00.229986 fractal_client-1.3.0a3/fractal/cmd/_project.py
+-rw-r--r--   0        0        0     6659 2023-06-13 10:01:05.958774 fractal_client-1.3.0a3/fractal/cmd/_task.py
+-rw-r--r--   0        0        0     4620 2023-06-06 12:51:00.229986 fractal_client-1.3.0a3/fractal/cmd/_user.py
+-rw-r--r--   0        0        0     9027 2023-06-12 06:40:09.560661 fractal_client-1.3.0a3/fractal/cmd/_workflow.py
+-rw-r--r--   0        0        0       42 2023-02-21 08:49:25.750218 fractal_client-1.3.0a3/fractal/common/.git
+-rw-r--r--   0        0        0      717 2023-03-06 13:52:20.997699 fractal_client-1.3.0a3/fractal/common/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      364 2023-02-21 08:49:27.594201 fractal_client-1.3.0a3/fractal/common/.github/workflows/project-management.yml
+-rw-r--r--   0        0        0       34 2023-03-06 13:52:21.001699 fractal_client-1.3.0a3/fractal/common/.gitignore
+-rw-r--r--   0        0        0      620 2023-02-21 08:49:27.594201 fractal_client-1.3.0a3/fractal/common/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1964 2023-03-06 13:52:21.001699 fractal_client-1.3.0a3/fractal/common/README.md
+-rw-r--r--   0        0        0        0 2023-02-21 08:49:27.594201 fractal_client-1.3.0a3/fractal/common/__init__.py
+-rw-r--r--   0        0        0      149 2023-02-21 10:13:04.505672 fractal_client-1.3.0a3/fractal/common/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      147 2023-03-16 09:04:47.705157 fractal_client-1.3.0a3/fractal/common/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0       57 2023-05-26 06:48:59.488787 fractal_client-1.3.0a3/fractal/common/requirements.txt
+-rw-r--r--   0        0        0      614 2023-05-25 12:31:57.653940 fractal_client-1.3.0a3/fractal/common/schemas/__init__.py
+-rw-r--r--   0        0        0      411 2023-05-25 12:32:05.945818 fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      372 2023-03-16 09:04:47.705157 fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      490 2023-03-03 14:13:42.839064 fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/_validator.cpython-310.pyc
+-rw-r--r--   0        0        0     1753 2023-04-20 07:56:22.895496 fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/_validators.cpython-310.pyc
+-rw-r--r--   0        0        0     1251 2023-03-16 09:04:47.793156 fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/_validators.cpython-39.pyc
+-rw-r--r--   0        0        0     1610 2023-05-26 06:49:58.096032 fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
+-rw-r--r--   0        0        0     2027 2023-03-16 09:04:47.705157 fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/applyworkflow.cpython-39.pyc
+-rw-r--r--   0        0        0     4068 2023-06-12 13:01:03.378002 fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/manifest.cpython-310.pyc
+-rw-r--r--   0        0        0     3515 2023-03-16 09:04:47.797156 fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/manifest.cpython-39.pyc
+-rw-r--r--   0        0        0     3537 2023-05-26 06:49:58.132032 fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/project.cpython-310.pyc
+-rw-r--r--   0        0        0     3711 2023-03-16 09:04:47.797156 fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/project.cpython-39.pyc
+-rw-r--r--   0        0        0     1165 2023-05-26 06:49:58.136032 fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/state.cpython-310.pyc
+-rw-r--r--   0        0        0     1185 2023-03-16 09:04:47.801156 fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/state.cpython-39.pyc
+-rw-r--r--   0        0        0     2705 2023-06-12 13:01:03.386002 fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/task.cpython-310.pyc
+-rw-r--r--   0        0        0     4994 2023-03-16 09:04:47.805156 fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/task.cpython-39.pyc
+-rw-r--r--   0        0        0     3292 2023-06-12 13:01:03.390002 fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/task_collection.cpython-310.pyc
+-rw-r--r--   0        0        0     1202 2023-05-25 12:32:06.097816 fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/user.cpython-310.pyc
+-rw-r--r--   0        0        0     1024 2023-03-16 09:04:47.809156 fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/user.cpython-39.pyc
+-rw-r--r--   0        0        0     3882 2023-05-26 06:49:58.328029 fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/workflow.cpython-310.pyc
+-rw-r--r--   0        0        0     1616 2023-04-06 11:30:39.096144 fractal_client-1.3.0a3/fractal/common/schemas/_validators.py
+-rw-r--r--   0        0        0     1117 2023-05-26 06:48:59.488787 fractal_client-1.3.0a3/fractal/common/schemas/applyworkflow.py
+-rw-r--r--   0        0        0     3479 2023-06-12 10:22:50.369047 fractal_client-1.3.0a3/fractal/common/schemas/manifest.py
+-rw-r--r--   0        0        0     2483 2023-05-26 06:48:59.488787 fractal_client-1.3.0a3/fractal/common/schemas/project.py
+-rw-r--r--   0        0        0      673 2023-05-26 06:48:59.488787 fractal_client-1.3.0a3/fractal/common/schemas/state.py
+-rw-r--r--   0        0        0     2578 2023-06-12 10:22:50.369047 fractal_client-1.3.0a3/fractal/common/schemas/task.py
+-rw-r--r--   0        0        0     2935 2023-06-12 10:22:50.369047 fractal_client-1.3.0a3/fractal/common/schemas/task_collection.py
+-rw-r--r--   0        0        0     1216 2023-05-25 12:31:57.653940 fractal_client-1.3.0a3/fractal/common/schemas/user.py
+-rw-r--r--   0        0        0     2457 2023-05-26 06:48:59.488787 fractal_client-1.3.0a3/fractal/common/schemas/workflow.py
+-rw-r--r--   0        0        0      415 2023-03-06 13:52:30.189594 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0      415 2023-03-07 09:47:31.002846 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0      415 2023-04-20 07:57:03.191274 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      415 2023-06-12 13:01:14.929878 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/conftest.cpython-310-pytest-7.3.2.pyc
+-rw-r--r--   0        0        0     1578 2023-03-06 13:52:30.221594 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1578 2023-03-07 09:47:31.038845 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0      606 2023-05-15 11:49:28.546463 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      606 2023-06-12 13:01:14.961878 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.2.pyc
+-rw-r--r--   0        0        0     3382 2023-03-15 10:53:32.644401 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     3382 2023-04-20 07:57:03.471272 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     3382 2023-06-12 13:01:15.169875 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.2.pyc
+-rw-r--r--   0        0        0      859 2023-03-06 13:52:30.469591 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0      859 2023-03-07 09:47:31.354842 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1241 2023-06-12 13:01:03.562000 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1241 2023-06-12 13:01:15.169875 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.2.pyc
+-rw-r--r--   0        0        0     2236 2023-03-06 13:52:30.469591 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1164 2023-04-20 07:56:23.111495 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1164 2023-04-20 07:57:03.471272 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1164 2023-06-12 13:01:15.169875 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.2.pyc
+-rw-r--r--   0        0        0     1763 2023-03-06 14:08:06.438014 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1763 2023-03-07 09:47:31.358842 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1763 2023-04-20 07:57:03.471272 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1763 2023-06-12 13:01:15.173875 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.2.pyc
+-rw-r--r--   0        0        0     2222 2023-03-06 13:52:30.473591 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     2222 2023-03-07 09:47:31.358842 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2792 2023-05-25 12:32:06.297813 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2792 2023-06-12 13:01:15.173875 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.2.pyc
+-rw-r--r--   0        0        0     1335 2023-06-12 13:01:03.566000 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_task_collection.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1335 2023-06-12 13:01:15.177875 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_task_collection.cpython-310-pytest-7.3.2.pyc
+-rw-r--r--   0        0        0     1317 2023-03-06 13:52:30.473591 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     2213 2023-04-20 07:56:23.115495 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2671 2023-05-25 12:32:06.301813 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2671 2023-06-12 13:01:15.177875 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.2.pyc
+-rw-r--r--   0        0        0     2579 2023-03-06 14:43:41.164713 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     3032 2023-04-20 07:56:23.115495 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2911 2023-05-15 11:49:28.882460 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2911 2023-06-12 13:01:15.177875 fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.2.pyc
+-rw-r--r--   0        0        0      139 2023-03-06 13:52:21.001699 fractal_client-1.3.0a3/fractal/common/tests/conftest.py
+-rw-r--r--   0        0        0      298 2023-05-11 16:07:56.531485 fractal_client-1.3.0a3/fractal/common/tests/test_applyworkflow.py
+-rw-r--r--   0        0        0     2144 2023-03-14 13:42:31.592919 fractal_client-1.3.0a3/fractal/common/tests/test_dataset.py
+-rw-r--r--   0        0        0     1420 2023-06-12 10:22:50.369047 fractal_client-1.3.0a3/fractal/common/tests/test_manifest.py
+-rw-r--r--   0        0        0      525 2023-04-06 11:30:39.096144 fractal_client-1.3.0a3/fractal/common/tests/test_project.py
+-rw-r--r--   0        0        0      551 2023-03-06 14:07:44.150418 fractal_client-1.3.0a3/fractal/common/tests/test_state.py
+-rw-r--r--   0        0        0     1190 2023-05-25 12:31:57.653940 fractal_client-1.3.0a3/fractal/common/tests/test_task.py
+-rw-r--r--   0        0        0      968 2023-06-12 10:22:50.369047 fractal_client-1.3.0a3/fractal/common/tests/test_task_collection.py
+-rw-r--r--   0        0        0     1499 2023-05-25 12:31:57.653940 fractal_client-1.3.0a3/fractal/common/tests/test_user.py
+-rw-r--r--   0        0        0     2596 2023-05-11 16:07:56.531485 fractal_client-1.3.0a3/fractal/common/tests/test_workflow.py
+-rw-r--r--   0        0        0     1285 2023-05-12 13:33:57.004876 fractal_client-1.3.0a3/fractal/config.py
+-rw-r--r--   0        0        0     1609 2023-05-09 19:58:57.316677 fractal_client-1.3.0a3/fractal/interface.py
+-rw-r--r--   0        0        0    23275 2023-06-13 10:01:03.054806 fractal_client-1.3.0a3/fractal/parser.py
+-rw-r--r--   0        0        0     1265 2023-05-09 19:58:57.316677 fractal_client-1.3.0a3/fractal/response.py
+-rw-r--r--   0        0        0     1851 2023-06-13 10:01:20.162621 fractal_client-1.3.0a3/pyproject.toml
+-rw-r--r--   0        0        0     3337 1970-01-01 00:00:00.000000 fractal_client-1.3.0a3/PKG-INFO
```

### Comparing `fractal_client-1.3.0a2/LICENSE` & `fractal_client-1.3.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/README.md` & `fractal_client-1.3.0a3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 
 See https://fractal-analytics-platform.github.io/fractal.
 
 # Contributors and license
 
 Unless otherwise stated in each individual module, all Fractal components are released according to a BSD 3-Clause License, and Copyright is with Friedrich Miescher Institute for Biomedical Research and University of Zurich.
 
-Fractal was conceived in the Liberali Lab at the Friedrich Miescher Institute for Biomedical Research and in the Pelkmans Lab at the University of Zurich (both in Switzerland). The project lead is with [@gusqgm](https://github.com/gusqgm) & [@jluethi](https://github.com/jluethi). The core development is done under contract by [eXact lab S.r.l.](exact-lab.it).
+Fractal was conceived in the Liberali Lab at the Friedrich Miescher Institute for Biomedical Research and in the Pelkmans Lab at the University of Zurich (both in Switzerland). The project lead is with [@gusqgm](https://github.com/gusqgm) & [@jluethi](https://github.com/jluethi). The core development is done under contract by [eXact lab S.r.l.](https://exact-lab.it).
```

### Comparing `fractal_client-1.3.0a2/fractal/authclient.py` & `fractal_client-1.3.0a3/fractal/authclient.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/client.py` & `fractal_client-1.3.0a3/fractal/client.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/cmd/__init__.py` & `fractal_client-1.3.0a3/fractal/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/cmd/_aux_task_caching.py` & `fractal_client-1.3.0a3/fractal/cmd/_aux_task_caching.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/cmd/_dataset.py` & `fractal_client-1.3.0a3/fractal/cmd/_dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/cmd/_job.py` & `fractal_client-1.3.0a3/fractal/cmd/_job.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/cmd/_project.py` & `fractal_client-1.3.0a3/fractal/cmd/_project.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/cmd/_task.py` & `fractal_client-1.3.0a3/fractal/cmd/_task.py`

 * *Files 4% similar despite different names*

```diff
@@ -195,8 +195,24 @@
     client: AuthClient,
     *,
     id: Optional[int] = None,
     name: Optional[str] = None,
     version: Optional[str] = None,
 ) -> PrintInterface:
 
-    raise NotImplementedError("task_delete")
+    if id:
+        if version:
+            logging.error(
+                "Too many arguments: cannot provide both `id` and `version`."
+            )
+            sys.exit(1)
+    else:
+        try:
+            id = await get_task_id_from_cache(
+                client=client, task_name=name, version=version
+            )
+        except FractalCacheError as e:
+            print(e)
+            sys.exit(1)
+    res = await client.delete(f"{settings.BASE_URL}/task/{id}")
+    check_response(res, expected_status_code=204)
+    return PrintInterface(retcode=0, data="")
```

### Comparing `fractal_client-1.3.0a2/fractal/cmd/_user.py` & `fractal_client-1.3.0a3/fractal/cmd/_user.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/cmd/_workflow.py` & `fractal_client-1.3.0a3/fractal/cmd/_workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/.github/workflows/ci.yml` & `fractal_client-1.3.0a3/fractal/common/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/.pre-commit-config.yaml` & `fractal_client-1.3.0a3/fractal/common/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/README.md` & `fractal_client-1.3.0a3/fractal/common/README.md`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/schemas/__init__.py` & `fractal_client-1.3.0a3/fractal/common/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/_validators.cpython-310.pyc` & `fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/_validators.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/_validators.cpython-39.pyc` & `fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/_validators.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/applyworkflow.cpython-310.pyc` & `fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/applyworkflow.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/applyworkflow.cpython-39.pyc` & `fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/applyworkflow.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/manifest.cpython-310.pyc` & `fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/manifest.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/manifest.cpython-39.pyc` & `fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/manifest.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/project.cpython-310.pyc` & `fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/project.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/project.cpython-39.pyc` & `fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/project.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/state.cpython-310.pyc` & `fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/state.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/state.cpython-39.pyc` & `fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/state.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/task.cpython-310.pyc` & `fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/task.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/task.cpython-39.pyc` & `fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/task.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/task_collection.cpython-310.pyc` & `fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/task_collection.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/user.cpython-310.pyc` & `fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/user.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/user.cpython-39.pyc` & `fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/user.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/schemas/__pycache__/workflow.cpython-310.pyc` & `fractal_client-1.3.0a3/fractal/common/schemas/__pycache__/workflow.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/schemas/_validators.py` & `fractal_client-1.3.0a3/fractal/common/schemas/_validators.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/schemas/applyworkflow.py` & `fractal_client-1.3.0a3/fractal/common/schemas/applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/schemas/manifest.py` & `fractal_client-1.3.0a3/fractal/common/schemas/manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/schemas/project.py` & `fractal_client-1.3.0a3/fractal/common/schemas/project.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/schemas/state.py` & `fractal_client-1.3.0a3/fractal/common/schemas/state.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/schemas/task.py` & `fractal_client-1.3.0a3/fractal/common/schemas/task.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/schemas/task_collection.py` & `fractal_client-1.3.0a3/fractal/common/schemas/task_collection.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/schemas/user.py` & `fractal_client-1.3.0a3/fractal/common/schemas/user.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/schemas/workflow.py` & `fractal_client-1.3.0a3/fractal/common/schemas/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc` & `fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc` & `fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc` & `fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.2.pyc` & `fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc` & `fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc` & `fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.2.pyc` & `fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc` & `fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc` & `fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc` & `fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.2.pyc` & `fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc` & `fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc` & `fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc` & `fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.2.pyc` & `fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc` & `fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc` & `fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc` & `fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.2.pyc` & `fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc` & `fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc` & `fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc` & `fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.2.pyc` & `fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_task_collection.cpython-310-pytest-7.3.1.pyc` & `fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_task_collection.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_task_collection.cpython-310-pytest-7.3.2.pyc` & `fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_task_collection.cpython-310-pytest-7.3.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc` & `fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc` & `fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc` & `fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.2.pyc` & `fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc` & `fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc` & `fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc` & `fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.2.pyc` & `fractal_client-1.3.0a3/fractal/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/tests/test_dataset.py` & `fractal_client-1.3.0a3/fractal/common/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/tests/test_manifest.py` & `fractal_client-1.3.0a3/fractal/common/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/tests/test_project.py` & `fractal_client-1.3.0a3/fractal/common/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/tests/test_state.py` & `fractal_client-1.3.0a3/fractal/common/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/tests/test_task.py` & `fractal_client-1.3.0a3/fractal/common/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/tests/test_task_collection.py` & `fractal_client-1.3.0a3/fractal/common/tests/test_task_collection.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/tests/test_user.py` & `fractal_client-1.3.0a3/fractal/common/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/common/tests/test_workflow.py` & `fractal_client-1.3.0a3/fractal/common/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/config.py` & `fractal_client-1.3.0a3/fractal/config.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/interface.py` & `fractal_client-1.3.0a3/fractal/interface.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/fractal/parser.py` & `fractal_client-1.3.0a3/fractal/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -294,15 +294,20 @@
         "--package-extras=torch,tensorflow` will trigger the installation of "
         "`fractal-tasks-core[torch,tensorflow]`"
     ),
 )
 task_collect_parser.add_argument(
     "--pinned-dependency",
     action="append",
-    help="List of 'package_name:package_version' to be pinned",  # FIXME
+    help=(
+        "Package/version pair representing a pinned-version dependency, in "
+        "the form `collect fractal-tasks-core --pinned-dependency "
+        "pydantic=1.10.0`. Include `--pinned-dependency` multiple times to "
+        "pin several packages to specific versions."
+    ),
 )
 
 # task check-collection
 task_check_collection_parser = task_subparsers.add_parser(
     "check-collection",
     description="Check status of background task collection processes",
     allow_abbrev=False,
```

### Comparing `fractal_client-1.3.0a2/fractal/response.py` & `fractal_client-1.3.0a3/fractal/response.py`

 * *Files identical despite different names*

### Comparing `fractal_client-1.3.0a2/pyproject.toml` & `fractal_client-1.3.0a3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-client"
-version = "1.3.0a2"
+version = "1.3.0a3"
 description = "Client component of the Fractal analytics platform"
 authors = [
     "Tommaso Comparin <tommaso.comparin@exact-lab.it>",
     "Marco Franzon <marco.franzon@exact-lab.it>",
     "Jacopo Nespolo <jacopo.nespolo@exact-lab.it>",
 ]
 readme = "README.md"
@@ -43,15 +43,15 @@
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 
 [tool.bumpver]
-current_version = "1.3.0a2"
+current_version = "1.3.0a3"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fractal_client-1.3.0a2/PKG-INFO` & `fractal_client-1.3.0a3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-client
-Version: 1.3.0a2
+Version: 1.3.0a3
 Summary: Client component of the Fractal analytics platform
 Home-page: https://github.com/fractal-analytics-platform/fractal
 License: BSD-3-Clause
 Author: Tommaso Comparin
 Author-email: tommaso.comparin@exact-lab.it
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
@@ -40,9 +40,9 @@
 
 See https://fractal-analytics-platform.github.io/fractal.
 
 # Contributors and license
 
 Unless otherwise stated in each individual module, all Fractal components are released according to a BSD 3-Clause License, and Copyright is with Friedrich Miescher Institute for Biomedical Research and University of Zurich.
 
-Fractal was conceived in the Liberali Lab at the Friedrich Miescher Institute for Biomedical Research and in the Pelkmans Lab at the University of Zurich (both in Switzerland). The project lead is with [@gusqgm](https://github.com/gusqgm) & [@jluethi](https://github.com/jluethi). The core development is done under contract by [eXact lab S.r.l.](exact-lab.it).
+Fractal was conceived in the Liberali Lab at the Friedrich Miescher Institute for Biomedical Research and in the Pelkmans Lab at the University of Zurich (both in Switzerland). The project lead is with [@gusqgm](https://github.com/gusqgm) & [@jluethi](https://github.com/jluethi). The core development is done under contract by [eXact lab S.r.l.](https://exact-lab.it).
```


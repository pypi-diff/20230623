# Comparing `tmp/fractal_server-1.3.0a8.tar.gz` & `tmp/fractal_server-1.3.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_server-1.3.0a8.tar", max compression
+gzip compressed data, was "fractal_server-1.3.0a9.tar", max compression
```

## Comparing `fractal_server-1.3.0a8.tar` & `fractal_server-1.3.0a9.tar`

### file list

```diff
@@ -1,135 +1,107 @@
--rw-r--r--   0        0        0     1576 2022-09-07 11:17:53.820970 fractal_server-1.3.0a8/LICENSE
--rw-r--r--   0        0        0     2100 2023-06-19 09:13:19.197654 fractal_server-1.3.0a8/README.md
--rw-r--r--   0        0        0       69 2022-09-07 11:17:53.836969 fractal_server-1.3.0a8/fractal_server/.gitignore
--rw-r--r--   0        0        0       24 2023-06-19 15:00:16.347835 fractal_server-1.3.0a8/fractal_server/__init__.py
--rw-r--r--   0        0        0     2202 2023-05-25 12:06:55.503794 fractal_server-1.3.0a8/fractal_server/__main__.py
--rw-r--r--   0        0        0     3153 2023-02-22 13:06:13.003243 fractal_server-1.3.0a8/fractal_server/alembic.ini
--rw-r--r--   0        0        0        0 2022-09-07 11:17:53.836969 fractal_server-1.3.0a8/fractal_server/app/__init__.py
--rw-r--r--   0        0        0      952 2023-05-12 06:48:40.382595 fractal_server-1.3.0a8/fractal_server/app/api/__init__.py
--rw-r--r--   0        0        0       24 2023-02-22 13:06:13.003243 fractal_server-1.3.0a8/fractal_server/app/api/v1/__init__.py
--rw-r--r--   0        0        0     7616 2023-06-19 09:13:19.197654 fractal_server-1.3.0a8/fractal_server/app/api/v1/_aux_functions.py
--rw-r--r--   0        0        0     7624 2023-05-23 13:25:45.067972 fractal_server-1.3.0a8/fractal_server/app/api/v1/dataset.py
--rw-r--r--   0        0        0     4817 2023-05-15 12:45:48.614516 fractal_server-1.3.0a8/fractal_server/app/api/v1/job.py
--rw-r--r--   0        0        0     8880 2023-05-15 09:02:05.627121 fractal_server-1.3.0a8/fractal_server/app/api/v1/project.py
--rw-r--r--   0        0        0    15912 2023-06-19 09:13:19.197654 fractal_server-1.3.0a8/fractal_server/app/api/v1/task.py
--rw-r--r--   0        0        0    12501 2023-05-29 15:02:27.725371 fractal_server-1.3.0a8/fractal_server/app/api/v1/workflow.py
--rw-r--r--   0        0        0     3081 2023-05-12 06:48:40.382595 fractal_server-1.3.0a8/fractal_server/app/db/__init__.py
--rw-r--r--   0        0        0      372 2023-03-16 13:58:42.445129 fractal_server-1.3.0a8/fractal_server/app/models/__init__.py
--rw-r--r--   0        0        0     3412 2023-05-29 08:51:11.986940 fractal_server-1.3.0a8/fractal_server/app/models/job.py
--rw-r--r--   0        0        0      309 2023-05-12 06:48:40.382595 fractal_server-1.3.0a8/fractal_server/app/models/linkuserproject.py
--rw-r--r--   0        0        0     2355 2023-05-29 08:51:11.986940 fractal_server-1.3.0a8/fractal_server/app/models/project.py
--rw-r--r--   0        0        0     2563 2023-05-29 09:51:02.494983 fractal_server-1.3.0a8/fractal_server/app/models/security.py
--rw-r--r--   0        0        0     1119 2023-05-29 08:51:11.986940 fractal_server-1.3.0a8/fractal_server/app/models/state.py
--rw-r--r--   0        0        0     1591 2023-06-19 14:50:22.446330 fractal_server-1.3.0a8/fractal_server/app/models/task.py
--rw-r--r--   0        0        0     5861 2023-06-19 09:13:19.197654 fractal_server-1.3.0a8/fractal_server/app/models/workflow.py
--rw-r--r--   0        0        0       16 2023-04-11 12:05:21.017629 fractal_server-1.3.0a8/fractal_server/app/runner/.gitignore
--rw-r--r--   0        0        0    10102 2023-06-19 11:56:16.860753 fractal_server-1.3.0a8/fractal_server/app/runner/__init__.py
--rw-r--r--   0        0        0    19523 2023-06-08 09:22:21.105956 fractal_server-1.3.0a8/fractal_server/app/runner/_common.py
--rw-r--r--   0        0        0     5464 2023-05-12 12:34:32.122055 fractal_server-1.3.0a8/fractal_server/app/runner/_local/__init__.py
--rw-r--r--   0        0        0     3245 2023-06-19 09:13:19.197654 fractal_server-1.3.0a8/fractal_server/app/runner/_local/_local_config.py
--rw-r--r--   0        0        0     1631 2023-04-17 13:34:24.748408 fractal_server-1.3.0a8/fractal_server/app/runner/_local/_submit_setup.py
--rw-r--r--   0        0        0     3620 2023-04-17 13:34:24.748408 fractal_server-1.3.0a8/fractal_server/app/runner/_local/executor.py
--rw-r--r--   0        0        0       16 2023-04-11 12:05:21.017629 fractal_server-1.3.0a8/fractal_server/app/runner/_slurm/.gitignore
--rw-r--r--   0        0        0     3839 2023-05-12 12:34:32.122055 fractal_server-1.3.0a8/fractal_server/app/runner/_slurm/__init__.py
--rw-r--r--   0        0        0     8840 2023-04-14 12:55:14.842206 fractal_server-1.3.0a8/fractal_server/app/runner/_slurm/_batching.py
--rw-r--r--   0        0        0     4331 2023-05-15 10:36:57.758906 fractal_server-1.3.0a8/fractal_server/app/runner/_slurm/_executor_wait_thread.py
--rw-r--r--   0        0        0    19766 2023-06-19 09:13:19.197654 fractal_server-1.3.0a8/fractal_server/app/runner/_slurm/_slurm_config.py
--rw-r--r--   0        0        0     2942 2023-04-11 12:05:21.021629 fractal_server-1.3.0a8/fractal_server/app/runner/_slurm/_submit_setup.py
--rw-r--r--   0        0        0     4534 2023-05-03 10:33:21.774484 fractal_server-1.3.0a8/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py
--rw-r--r--   0        0        0    42200 2023-05-18 09:57:35.703959 fractal_server-1.3.0a8/fractal_server/app/runner/_slurm/executor.py
--rw-r--r--   0        0        0     5852 2023-04-14 08:31:16.571080 fractal_server-1.3.0a8/fractal_server/app/runner/_slurm/remote.py
--rw-r--r--   0        0        0     7900 2023-06-08 08:33:26.930560 fractal_server-1.3.0a8/fractal_server/app/runner/common.py
--rw-r--r--   0        0        0    11324 2023-05-12 06:48:40.382595 fractal_server-1.3.0a8/fractal_server/app/security/__init__.py
--rw-r--r--   0        0        0       49 2023-02-22 11:04:15.289972 fractal_server-1.3.0a8/fractal_server/common/.git
--rw-r--r--   0        0        0      717 2023-05-08 12:01:46.018194 fractal_server-1.3.0a8/fractal_server/common/.github/workflows/ci.yml
--rw-r--r--   0        0        0      364 2023-02-22 11:04:15.289972 fractal_server-1.3.0a8/fractal_server/common/.github/workflows/project-management.yml
--rw-r--r--   0        0        0       34 2023-05-08 12:01:46.018194 fractal_server-1.3.0a8/fractal_server/common/.gitignore
--rw-r--r--   0        0        0      620 2023-02-22 11:04:15.289972 fractal_server-1.3.0a8/fractal_server/common/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1964 2023-05-08 12:01:46.018194 fractal_server-1.3.0a8/fractal_server/common/README.md
--rw-r--r--   0        0        0        0 2023-02-22 11:04:15.289972 fractal_server-1.3.0a8/fractal_server/common/__init__.py
--rw-r--r--   0        0        0      163 2023-02-22 12:30:35.511172 fractal_server-1.3.0a8/fractal_server/common/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      179 2023-02-23 12:52:36.416846 fractal_server-1.3.0a8/fractal_server/common/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0       57 2023-05-26 06:41:57.297956 fractal_server-1.3.0a8/fractal_server/common/requirements.txt
--rw-r--r--   0        0        0      614 2023-05-26 06:41:57.297956 fractal_server-1.3.0a8/fractal_server/common/schemas/__init__.py
--rw-r--r--   0        0        0      425 2023-05-26 06:49:50.432129 fractal_server-1.3.0a8/fractal_server/common/schemas/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      593 2023-02-23 12:52:36.416846 fractal_server-1.3.0a8/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      504 2023-03-03 14:24:46.376001 fractal_server-1.3.0a8/fractal_server/common/schemas/__pycache__/_validator.cpython-310.pyc
--rw-r--r--   0        0        0     1767 2023-05-08 12:02:12.593892 fractal_server-1.3.0a8/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc
--rw-r--r--   0        0        0     1624 2023-06-12 09:13:31.352825 fractal_server-1.3.0a8/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
--rw-r--r--   0        0        0     2325 2023-02-23 12:52:36.416846 fractal_server-1.3.0a8/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc
--rw-r--r--   0        0        0     4082 2023-06-12 09:13:31.356825 fractal_server-1.3.0a8/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc
--rw-r--r--   0        0        0     4433 2023-02-23 12:52:36.420846 fractal_server-1.3.0a8/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc
--rw-r--r--   0        0        0     3551 2023-05-26 06:49:50.436129 fractal_server-1.3.0a8/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc
--rw-r--r--   0        0        0     5221 2023-02-23 12:52:36.420846 fractal_server-1.3.0a8/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc
--rw-r--r--   0        0        0     1179 2023-05-26 06:49:50.444129 fractal_server-1.3.0a8/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc
--rw-r--r--   0        0        0     1877 2023-02-23 12:52:36.428846 fractal_server-1.3.0a8/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc
--rw-r--r--   0        0        0     2719 2023-06-12 09:13:31.364825 fractal_server-1.3.0a8/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc
--rw-r--r--   0        0        0     6570 2023-02-23 12:52:36.428846 fractal_server-1.3.0a8/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc
--rw-r--r--   0        0        0     3306 2023-06-12 09:13:31.368826 fractal_server-1.3.0a8/fractal_server/common/schemas/__pycache__/task_collection.cpython-310.pyc
--rw-r--r--   0        0        0     1216 2023-05-26 06:49:50.448129 fractal_server-1.3.0a8/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc
--rw-r--r--   0        0        0     1200 2023-02-23 12:52:36.432846 fractal_server-1.3.0a8/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc
--rw-r--r--   0        0        0     3896 2023-05-26 06:49:50.452129 fractal_server-1.3.0a8/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc
--rw-r--r--   0        0        0     4596 2023-02-23 12:52:36.432846 fractal_server-1.3.0a8/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc
--rw-r--r--   0        0        0     1616 2023-05-08 12:01:46.018194 fractal_server-1.3.0a8/fractal_server/common/schemas/_validators.py
--rw-r--r--   0        0        0     1117 2023-06-12 09:12:04.406676 fractal_server-1.3.0a8/fractal_server/common/schemas/applyworkflow.py
--rw-r--r--   0        0        0     3479 2023-06-12 09:12:04.406676 fractal_server-1.3.0a8/fractal_server/common/schemas/manifest.py
--rw-r--r--   0        0        0     2483 2023-05-26 06:41:57.297956 fractal_server-1.3.0a8/fractal_server/common/schemas/project.py
--rw-r--r--   0        0        0      673 2023-05-26 06:41:57.297956 fractal_server-1.3.0a8/fractal_server/common/schemas/state.py
--rw-r--r--   0        0        0     2578 2023-06-12 09:12:04.406676 fractal_server-1.3.0a8/fractal_server/common/schemas/task.py
--rw-r--r--   0        0        0     2935 2023-06-12 09:12:04.406676 fractal_server-1.3.0a8/fractal_server/common/schemas/task_collection.py
--rw-r--r--   0        0        0     1216 2023-05-26 06:41:57.297956 fractal_server-1.3.0a8/fractal_server/common/schemas/user.py
--rw-r--r--   0        0        0     2457 2023-05-26 06:41:57.297956 fractal_server-1.3.0a8/fractal_server/common/schemas/workflow.py
--rw-r--r--   0        0        0      429 2023-03-09 14:38:27.388159 fractal_server-1.3.0a8/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0      429 2023-03-24 12:58:52.898563 fractal_server-1.3.0a8/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      429 2023-05-08 12:02:12.937888 fractal_server-1.3.0a8/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1592 2023-03-09 14:38:27.444159 fractal_server-1.3.0a8/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1592 2023-03-24 12:58:52.954562 fractal_server-1.3.0a8/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      620 2023-05-09 18:15:54.737187 fractal_server-1.3.0a8/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     3396 2023-03-15 08:26:08.661090 fractal_server-1.3.0a8/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     3396 2023-03-24 12:58:52.978562 fractal_server-1.3.0a8/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     3396 2023-05-08 12:02:13.009887 fractal_server-1.3.0a8/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      873 2023-03-09 14:38:27.472158 fractal_server-1.3.0a8/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0      873 2023-03-24 12:58:52.978562 fractal_server-1.3.0a8/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1255 2023-06-15 11:41:13.549879 fractal_server-1.3.0a8/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1272 2023-03-15 08:26:08.665089 fractal_server-1.3.0a8/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1178 2023-04-06 08:33:24.349041 fractal_server-1.3.0a8/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1178 2023-05-08 12:02:13.013887 fractal_server-1.3.0a8/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1777 2023-03-09 14:38:27.476158 fractal_server-1.3.0a8/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1777 2023-03-24 12:58:52.982562 fractal_server-1.3.0a8/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1777 2023-05-08 12:02:13.013887 fractal_server-1.3.0a8/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2236 2023-03-09 14:38:27.480158 fractal_server-1.3.0a8/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     2236 2023-03-24 12:58:52.982562 fractal_server-1.3.0a8/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2806 2023-05-26 06:49:50.864124 fractal_server-1.3.0a8/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1349 2023-06-15 11:41:13.553879 fractal_server-1.3.0a8/fractal_server/common/tests/__pycache__/test_task_collection.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1331 2023-03-09 14:38:27.480158 fractal_server-1.3.0a8/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     2227 2023-04-06 08:33:24.353041 fractal_server-1.3.0a8/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2685 2023-05-26 06:49:50.868124 fractal_server-1.3.0a8/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2593 2023-03-09 14:38:27.480158 fractal_server-1.3.0a8/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     3046 2023-03-24 12:58:52.986562 fractal_server-1.3.0a8/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2925 2023-05-09 18:15:54.765188 fractal_server-1.3.0a8/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      139 2023-05-08 12:01:46.018194 fractal_server-1.3.0a8/fractal_server/common/tests/conftest.py
--rw-r--r--   0        0        0      298 2023-05-09 11:24:30.681084 fractal_server-1.3.0a8/fractal_server/common/tests/test_applyworkflow.py
--rw-r--r--   0        0        0     2144 2023-05-08 12:01:46.018194 fractal_server-1.3.0a8/fractal_server/common/tests/test_dataset.py
--rw-r--r--   0        0        0     1420 2023-06-12 09:12:04.406676 fractal_server-1.3.0a8/fractal_server/common/tests/test_manifest.py
--rw-r--r--   0        0        0      525 2023-05-08 12:01:46.018194 fractal_server-1.3.0a8/fractal_server/common/tests/test_project.py
--rw-r--r--   0        0        0      551 2023-05-08 12:01:46.018194 fractal_server-1.3.0a8/fractal_server/common/tests/test_state.py
--rw-r--r--   0        0        0     1190 2023-05-26 06:41:57.297956 fractal_server-1.3.0a8/fractal_server/common/tests/test_task.py
--rw-r--r--   0        0        0      968 2023-06-12 09:12:04.410676 fractal_server-1.3.0a8/fractal_server/common/tests/test_task_collection.py
--rw-r--r--   0        0        0     1499 2023-05-26 06:41:57.297956 fractal_server-1.3.0a8/fractal_server/common/tests/test_user.py
--rw-r--r--   0        0        0     2596 2023-05-09 11:24:30.681084 fractal_server-1.3.0a8/fractal_server/common/tests/test_workflow.py
--rw-r--r--   0        0        0    12432 2023-06-19 09:13:19.197654 fractal_server-1.3.0a8/fractal_server/config.py
--rw-r--r--   0        0        0     4562 2023-04-14 12:55:14.846206 fractal_server-1.3.0a8/fractal_server/logger.py
--rw-r--r--   0        0        0     5935 2023-06-19 09:13:19.197654 fractal_server-1.3.0a8/fractal_server/main.py
--rw-r--r--   0        0        0       59 2022-09-08 11:49:20.993046 fractal_server-1.3.0a8/fractal_server/migrations/README
--rw-r--r--   0        0        0     2330 2023-06-19 14:49:54.798636 fractal_server-1.3.0a8/fractal_server/migrations/env.py
--rw-r--r--   0        0        0      550 2022-09-08 11:49:30.768918 fractal_server-1.3.0a8/fractal_server/migrations/script.py.mako
--rw-r--r--   0        0        0      954 2023-06-08 09:21:57.166713 fractal_server-1.3.0a8/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py
--rw-r--r--   0        0        0     8770 2023-05-29 15:02:27.725371 fractal_server-1.3.0a8/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py
--rw-r--r--   0        0        0      746 2023-06-08 09:21:57.166713 fractal_server-1.3.0a8/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py
--rw-r--r--   0        0        0        0 2022-11-02 11:51:16.322067 fractal_server-1.3.0a8/fractal_server/py.typed
--rw-r--r--   0        0        0     2786 2023-04-11 12:05:21.021629 fractal_server-1.3.0a8/fractal_server/syringe.py
--rw-r--r--   0        0        0       72 2023-04-11 12:05:21.021629 fractal_server-1.3.0a8/fractal_server/tasks/__init__.py
--rw-r--r--   0        0        0    17581 2023-06-12 14:10:58.230055 fractal_server-1.3.0a8/fractal_server/tasks/collection.py
--rw-r--r--   0        0        0     2115 2023-05-03 10:43:26.232421 fractal_server-1.3.0a8/fractal_server/utils.py
--rw-r--r--   0        0        0     2704 2023-06-19 15:00:16.347835 fractal_server-1.3.0a8/pyproject.toml
--rw-r--r--   0        0        0     3546 1970-01-01 00:00:00.000000 fractal_server-1.3.0a8/PKG-INFO
+-rw-r--r--   0        0        0     1576 2022-12-15 19:55:06.212112 fractal_server-1.3.0a9/LICENSE
+-rw-r--r--   0        0        0     2100 2023-06-20 19:21:04.815875 fractal_server-1.3.0a9/README.md
+-rw-r--r--   0        0        0       69 2022-12-15 19:55:06.216112 fractal_server-1.3.0a9/fractal_server/.gitignore
+-rw-r--r--   0        0        0       24 2023-06-21 08:32:07.752695 fractal_server-1.3.0a9/fractal_server/__init__.py
+-rw-r--r--   0        0        0     2202 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/__main__.py
+-rw-r--r--   0        0        0     3153 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/alembic.ini
+-rw-r--r--   0        0        0        0 2022-12-15 19:55:06.216112 fractal_server-1.3.0a9/fractal_server/app/__init__.py
+-rw-r--r--   0        0        0      952 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/api/__init__.py
+-rw-r--r--   0        0        0       24 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/api/v1/__init__.py
+-rw-r--r--   0        0        0     7616 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/api/v1/_aux_functions.py
+-rw-r--r--   0        0        0     7624 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/api/v1/dataset.py
+-rw-r--r--   0        0        0     4817 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/api/v1/job.py
+-rw-r--r--   0        0        0     8880 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/api/v1/project.py
+-rw-r--r--   0        0        0    15912 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/api/v1/task.py
+-rw-r--r--   0        0        0    12866 2023-06-21 08:31:20.096225 fractal_server-1.3.0a9/fractal_server/app/api/v1/workflow.py
+-rw-r--r--   0        0        0     3081 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/db/__init__.py
+-rw-r--r--   0        0        0      372 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/models/__init__.py
+-rw-r--r--   0        0        0     3412 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/models/job.py
+-rw-r--r--   0        0        0      309 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/models/linkuserproject.py
+-rw-r--r--   0        0        0     2355 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/models/project.py
+-rw-r--r--   0        0        0     2563 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/models/security.py
+-rw-r--r--   0        0        0     1119 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/models/state.py
+-rw-r--r--   0        0        0     2535 2023-06-21 08:31:20.096225 fractal_server-1.3.0a9/fractal_server/app/models/task.py
+-rw-r--r--   0        0        0     5205 2023-06-21 08:31:20.096225 fractal_server-1.3.0a9/fractal_server/app/models/workflow.py
+-rw-r--r--   0        0        0       16 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/runner/.gitignore
+-rw-r--r--   0        0        0    10102 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/runner/__init__.py
+-rw-r--r--   0        0        0    19523 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/runner/_common.py
+-rw-r--r--   0        0        0     5464 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/runner/_local/__init__.py
+-rw-r--r--   0        0        0     3245 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/runner/_local/_local_config.py
+-rw-r--r--   0        0        0     1631 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/runner/_local/_submit_setup.py
+-rw-r--r--   0        0        0     3620 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/runner/_local/executor.py
+-rw-r--r--   0        0        0       16 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/runner/_slurm/.gitignore
+-rw-r--r--   0        0        0     3839 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/runner/_slurm/__init__.py
+-rw-r--r--   0        0        0     8840 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/runner/_slurm/_batching.py
+-rw-r--r--   0        0        0     4331 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/runner/_slurm/_executor_wait_thread.py
+-rw-r--r--   0        0        0    19766 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/runner/_slurm/_slurm_config.py
+-rw-r--r--   0        0        0     2942 2023-06-20 19:21:04.819876 fractal_server-1.3.0a9/fractal_server/app/runner/_slurm/_submit_setup.py
+-rw-r--r--   0        0        0     4534 2023-06-20 19:21:04.823876 fractal_server-1.3.0a9/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py
+-rw-r--r--   0        0        0    42200 2023-06-20 19:21:04.823876 fractal_server-1.3.0a9/fractal_server/app/runner/_slurm/executor.py
+-rw-r--r--   0        0        0     5852 2023-06-20 19:21:04.823876 fractal_server-1.3.0a9/fractal_server/app/runner/_slurm/remote.py
+-rw-r--r--   0        0        0     7900 2023-06-20 19:21:04.823876 fractal_server-1.3.0a9/fractal_server/app/runner/common.py
+-rw-r--r--   0        0        0    11324 2023-06-20 19:21:04.823876 fractal_server-1.3.0a9/fractal_server/app/security/__init__.py
+-rw-r--r--   0        0        0       49 2023-06-20 20:07:43.590964 fractal_server-1.3.0a9/fractal_server/common/.git
+-rw-r--r--   0        0        0      717 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      364 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/.github/workflows/project-management.yml
+-rw-r--r--   0        0        0       34 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/.gitignore
+-rw-r--r--   0        0        0      620 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1964 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/README.md
+-rw-r--r--   0        0        0        0 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/__init__.py
+-rw-r--r--   0        0        0      163 2023-06-20 20:09:45.855554 fractal_server-1.3.0a9/fractal_server/common/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0       57 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/requirements.txt
+-rw-r--r--   0        0        0      614 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/schemas/__init__.py
+-rw-r--r--   0        0        0      425 2023-06-20 20:09:08.951386 fractal_server-1.3.0a9/fractal_server/common/schemas/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1767 2023-06-20 20:09:08.971386 fractal_server-1.3.0a9/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc
+-rw-r--r--   0        0        0     1624 2023-06-20 20:09:08.951386 fractal_server-1.3.0a9/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
+-rw-r--r--   0        0        0     4082 2023-06-20 20:09:08.975386 fractal_server-1.3.0a9/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc
+-rw-r--r--   0        0        0     3551 2023-06-20 20:09:08.975386 fractal_server-1.3.0a9/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc
+-rw-r--r--   0        0        0     1179 2023-06-20 20:09:08.983386 fractal_server-1.3.0a9/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc
+-rw-r--r--   0        0        0     2719 2023-06-20 20:09:08.983386 fractal_server-1.3.0a9/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc
+-rw-r--r--   0        0        0     3306 2023-06-20 20:09:08.991386 fractal_server-1.3.0a9/fractal_server/common/schemas/__pycache__/task_collection.cpython-310.pyc
+-rw-r--r--   0        0        0     1216 2023-06-20 20:09:08.991386 fractal_server-1.3.0a9/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc
+-rw-r--r--   0        0        0     3896 2023-06-20 20:09:09.235387 fractal_server-1.3.0a9/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc
+-rw-r--r--   0        0        0     1616 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/schemas/_validators.py
+-rw-r--r--   0        0        0     1117 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/schemas/applyworkflow.py
+-rw-r--r--   0        0        0     3479 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/schemas/manifest.py
+-rw-r--r--   0        0        0     2483 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/schemas/project.py
+-rw-r--r--   0        0        0      673 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/schemas/state.py
+-rw-r--r--   0        0        0     2578 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/schemas/task.py
+-rw-r--r--   0        0        0     2935 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/schemas/task_collection.py
+-rw-r--r--   0        0        0     1216 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/schemas/user.py
+-rw-r--r--   0        0        0     2457 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/schemas/workflow.py
+-rw-r--r--   0        0        0      429 2023-06-20 20:09:08.927385 fractal_server-1.3.0a9/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      620 2023-06-20 20:09:08.947386 fractal_server-1.3.0a9/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     3396 2023-06-20 20:09:09.247387 fractal_server-1.3.0a9/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1255 2023-06-20 20:09:09.247387 fractal_server-1.3.0a9/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1178 2023-06-20 20:09:09.251387 fractal_server-1.3.0a9/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1777 2023-06-20 20:09:09.251387 fractal_server-1.3.0a9/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2806 2023-06-20 20:09:09.255387 fractal_server-1.3.0a9/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1349 2023-06-20 20:09:09.259387 fractal_server-1.3.0a9/fractal_server/common/tests/__pycache__/test_task_collection.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2685 2023-06-20 20:09:09.263387 fractal_server-1.3.0a9/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2925 2023-06-20 20:09:09.263387 fractal_server-1.3.0a9/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      139 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/tests/conftest.py
+-rw-r--r--   0        0        0      298 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/tests/test_applyworkflow.py
+-rw-r--r--   0        0        0     2144 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/tests/test_dataset.py
+-rw-r--r--   0        0        0     1420 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/tests/test_manifest.py
+-rw-r--r--   0        0        0      525 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/tests/test_project.py
+-rw-r--r--   0        0        0      551 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/tests/test_state.py
+-rw-r--r--   0        0        0     1190 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/tests/test_task.py
+-rw-r--r--   0        0        0      968 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/tests/test_task_collection.py
+-rw-r--r--   0        0        0     1499 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/tests/test_user.py
+-rw-r--r--   0        0        0     2596 2023-06-20 20:08:58.767338 fractal_server-1.3.0a9/fractal_server/common/tests/test_workflow.py
+-rw-r--r--   0        0        0    12432 2023-06-20 19:21:04.823876 fractal_server-1.3.0a9/fractal_server/config.py
+-rw-r--r--   0        0        0     4562 2023-06-20 19:21:04.823876 fractal_server-1.3.0a9/fractal_server/logger.py
+-rw-r--r--   0        0        0     5935 2023-06-20 19:21:04.823876 fractal_server-1.3.0a9/fractal_server/main.py
+-rw-r--r--   0        0        0       59 2022-12-15 19:55:06.216112 fractal_server-1.3.0a9/fractal_server/migrations/README
+-rw-r--r--   0        0        0     2330 2023-06-20 19:21:04.823876 fractal_server-1.3.0a9/fractal_server/migrations/env.py
+-rw-r--r--   0        0        0      550 2022-12-15 19:55:06.216112 fractal_server-1.3.0a9/fractal_server/migrations/script.py.mako
+-rw-r--r--   0        0        0      954 2023-06-20 19:21:04.823876 fractal_server-1.3.0a9/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py
+-rw-r--r--   0        0        0     8770 2023-06-20 19:21:04.823876 fractal_server-1.3.0a9/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py
+-rw-r--r--   0        0        0      746 2023-06-20 19:21:04.823876 fractal_server-1.3.0a9/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py
+-rw-r--r--   0        0        0        0 2022-12-15 19:55:06.216112 fractal_server-1.3.0a9/fractal_server/py.typed
+-rw-r--r--   0        0        0     2786 2023-06-20 19:21:04.823876 fractal_server-1.3.0a9/fractal_server/syringe.py
+-rw-r--r--   0        0        0       72 2023-06-20 19:21:04.823876 fractal_server-1.3.0a9/fractal_server/tasks/__init__.py
+-rw-r--r--   0        0        0    17581 2023-06-20 19:21:04.823876 fractal_server-1.3.0a9/fractal_server/tasks/collection.py
+-rw-r--r--   0        0        0     2115 2023-06-20 19:21:04.823876 fractal_server-1.3.0a9/fractal_server/utils.py
+-rw-r--r--   0        0        0     2704 2023-06-21 08:32:07.752695 fractal_server-1.3.0a9/pyproject.toml
+-rw-r--r--   0        0        0     3546 1970-01-01 00:00:00.000000 fractal_server-1.3.0a9/PKG-INFO
```

### Comparing `fractal_server-1.3.0a8/LICENSE` & `fractal_server-1.3.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/README.md` & `fractal_server-1.3.0a9/README.md`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/__main__.py` & `fractal_server-1.3.0a9/fractal_server/__main__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/alembic.ini` & `fractal_server-1.3.0a9/fractal_server/alembic.ini`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/app/api/__init__.py` & `fractal_server-1.3.0a9/fractal_server/app/api/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/app/api/v1/_aux_functions.py` & `fractal_server-1.3.0a9/fractal_server/app/api/v1/_aux_functions.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/app/api/v1/dataset.py` & `fractal_server-1.3.0a9/fractal_server/app/api/v1/dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/app/api/v1/job.py` & `fractal_server-1.3.0a9/fractal_server/app/api/v1/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/app/api/v1/project.py` & `fractal_server-1.3.0a9/fractal_server/app/api/v1/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/app/api/v1/task.py` & `fractal_server-1.3.0a9/fractal_server/app/api/v1/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/app/api/v1/workflow.py` & `fractal_server-1.3.0a9/fractal_server/app/api/v1/workflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -364,17 +364,27 @@
         workflow_id=workflow_id,
         user_id=user.id,
         db=db,
     )
 
     for key, value in workflow_task_update.dict(exclude_unset=True).items():
         if key == "args":
-            current_args = deepcopy(db_workflow_task.args) or {}
-            current_args.update(value)
-            setattr(db_workflow_task, key, current_args)
+
+            # Get default arguments via a Task property method
+            default_args = deepcopy(
+                db_workflow_task.task.default_args_from_args_schema
+            )
+            # Override default_args with args value items
+            actual_args = default_args.copy()
+            if value is not None:
+                for k, v in value.items():
+                    actual_args[k] = v
+            if not actual_args:
+                actual_args = None
+            setattr(db_workflow_task, key, actual_args)
         elif key == "meta":
             current_meta = deepcopy(db_workflow_task.meta) or {}
             current_meta.update(value)
             setattr(db_workflow_task, key, current_meta)
         else:
             raise HTTPException(
                 status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
```

### Comparing `fractal_server-1.3.0a8/fractal_server/app/db/__init__.py` & `fractal_server-1.3.0a9/fractal_server/app/db/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/app/models/job.py` & `fractal_server-1.3.0a9/fractal_server/app/models/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/app/models/project.py` & `fractal_server-1.3.0a9/fractal_server/app/models/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/app/models/security.py` & `fractal_server-1.3.0a9/fractal_server/app/models/security.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/app/models/state.py` & `fractal_server-1.3.0a9/fractal_server/app/models/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/app/models/workflow.py` & `fractal_server-1.3.0a9/fractal_server/app/models/workflow.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import json
-import logging
 from typing import Any
 from typing import Optional
 from typing import Union
 
 from pydantic import validator
 from sqlalchemy import Column
 from sqlalchemy.ext.orderinglist import ordering_list
@@ -137,31 +135,18 @@
             order: TBD
             db: TBD
             commit: TBD
         """
         if order is None:
             order = len(self.task_list)
 
-        # Get task from db, extract the JSON Schema for its arguments (if any),
-        # read default values and set them in default_args
+        # Get task from db, and extract default arguments via a Task property
+        # method
         db_task = await db.get(Task, task_id)
-        default_args = {}
-        if db_task.args_schema is not None:
-            try:
-                properties = db_task.args_schema["properties"]
-                for prop_name, prop_schema in properties.items():
-                    default_value = prop_schema.get("default", None)
-                    if default_value:
-                        default_args[prop_name] = default_value
-            except KeyError as e:
-                logging.warning(
-                    "Cannot set default_args from args_schema="
-                    f"{json.dumps(db_task.args_schema)}\n"
-                    f"Original KeyError: {str(e)}"
-                )
+        default_args = db_task.default_args_from_args_schema
         # Override default_args with args
         actual_args = default_args.copy()
         if args is not None:
             for k, v in args.items():
                 actual_args[k] = v
         if not actual_args:
             actual_args = None
```

### Comparing `fractal_server-1.3.0a8/fractal_server/app/runner/__init__.py` & `fractal_server-1.3.0a9/fractal_server/app/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/app/runner/_common.py` & `fractal_server-1.3.0a9/fractal_server/app/runner/_common.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/app/runner/_local/__init__.py` & `fractal_server-1.3.0a9/fractal_server/app/runner/_local/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/app/runner/_local/_local_config.py` & `fractal_server-1.3.0a9/fractal_server/app/runner/_local/_local_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/app/runner/_local/_submit_setup.py` & `fractal_server-1.3.0a9/fractal_server/app/runner/_local/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/app/runner/_local/executor.py` & `fractal_server-1.3.0a9/fractal_server/app/runner/_local/executor.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/app/runner/_slurm/__init__.py` & `fractal_server-1.3.0a9/fractal_server/app/runner/_slurm/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/app/runner/_slurm/_batching.py` & `fractal_server-1.3.0a9/fractal_server/app/runner/_slurm/_batching.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/app/runner/_slurm/_executor_wait_thread.py` & `fractal_server-1.3.0a9/fractal_server/app/runner/_slurm/_executor_wait_thread.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/app/runner/_slurm/_slurm_config.py` & `fractal_server-1.3.0a9/fractal_server/app/runner/_slurm/_slurm_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/app/runner/_slurm/_submit_setup.py` & `fractal_server-1.3.0a9/fractal_server/app/runner/_slurm/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py` & `fractal_server-1.3.0a9/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/app/runner/_slurm/executor.py` & `fractal_server-1.3.0a9/fractal_server/app/runner/_slurm/executor.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/app/runner/_slurm/remote.py` & `fractal_server-1.3.0a9/fractal_server/app/runner/_slurm/remote.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/app/runner/common.py` & `fractal_server-1.3.0a9/fractal_server/app/runner/common.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/app/security/__init__.py` & `fractal_server-1.3.0a9/fractal_server/app/security/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/common/.github/workflows/ci.yml` & `fractal_server-1.3.0a9/fractal_server/common/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/common/.pre-commit-config.yaml` & `fractal_server-1.3.0a9/fractal_server/common/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/common/README.md` & `fractal_server-1.3.0a9/fractal_server/common/README.md`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/common/schemas/__init__.py` & `fractal_server-1.3.0a9/fractal_server/common/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc` & `fractal_server-1.3.0a9/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon May  8 12:01:46 2023 UTC, .py size: 1616 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 aae4 5864 5006 0000  o.........XdP...
+00000000: 6f0d 0d0a 0000 0000 5a07 9264 5006 0000  o.......Z..dP...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
 00000030: 6401 6c00 5a00 6402 6501 6602 6403 6404  d.l.Z.d.e.f.d.d.
 00000040: 8404 5a02 640b 6402 6501 6406 6503 6604  ..Z.d.d.e.d.e.f.
 00000050: 6407 6408 8405 5a04 6402 6501 6602 6409  d.d...Z.d.e.f.d.
 00000060: 640a 8404 5a05 6401 5300 290c e900 0000  d...Z.d.S.).....
 00000070: 004e da09 6174 7472 6962 7574 6563 0100  .N..attributec..
```

### Comparing `fractal_server-1.3.0a8/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc` & `fractal_server-1.3.0a9/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jun 12 09:12:04 2023 UTC, .py size: 1117 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 64e1 8664 5d04 0000  o.......d..d]...
+00000000: 6f0d 0d0a 0000 0000 5a07 9264 5d04 0000  o.......Z..d]...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
 00000030: 6401 6c00 6d00 5a00 0100 6400 6402 6c01  d.l.m.Z...d.d.l.
 00000040: 6d02 5a02 0100 6400 6403 6c03 6d04 5a04  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c03 6d05 5a05 0100 6405  ..d.d.l.m.Z...d.
 00000060: 6406 6c06 6d07 5a07 0100 6407 5a08 4700  d.l.m.Z...d.Z.G.
 00000070: 6408 6409 8400 6409 6504 8303 5a09 4700  d.d...d.e...Z.G.
@@ -39,64 +39,64 @@
 00000260: 6865 6d61 732f 6170 706c 7977 6f72 6b66  hemas/applyworkf
 00000270: 6c6f 772e 7079 7208 0000 0010 0000 0073  low.pyr........s
 00000280: 0600 0000 0a00 0401 1007 7208 0000 0063  ..........r....c
 00000290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000002a0: 0400 0000 4000 0000 7320 0000 0065 005a  ....@...s ...e.Z
 000002b0: 0164 005a 0265 0364 0164 0264 038d 0265  .d.Z.e.d.d.d...e
 000002c0: 0464 0183 0183 015a 0564 0453 0029 0572  .d.....Z.d.S.).r
-000002d0: 0900 0000 720b 0000 0054 2901 da0b 616c  ....r....T)...al
+000002d0: 0900 0000 720b 0000 0054 2901 5a0b 616c  ....r....T).Z.al
 000002e0: 6c6f 775f 7265 7573 654e 2906 720c 0000  low_reuseN).r...
 000002f0: 0072 0d00 0000 720e 0000 0072 0500 0000  .r....r....r....
-00000300: 7207 0000 00da 0c5f 776f 726b 6572 5f69  r......_worker_i
+00000300: 7207 0000 005a 0c5f 776f 726b 6572 5f69  r....Z._worker_i
 00000310: 6e69 7472 1200 0000 7212 0000 0072 1200  nitr....r....r..
 00000320: 0000 7213 0000 0072 0900 0000 1b00 0000  ..r....r........
 00000330: 7308 0000 0008 000a 0306 0108 ff72 0900  s............r..
 00000340: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
 00000350: 0000 0003 0000 0040 0000 0073 8e00 0000  .......@...s....
 00000360: 6500 5a01 6400 5a02 5500 6503 6504 6401  e.Z.d.Z.U.e.e.d.
 00000370: 3c00 6503 6504 6402 3c00 6503 6504 6403  <.e.e.d.<.e.e.d.
 00000380: 3c00 6503 6504 6404 3c00 6503 6504 6405  <.e.e.d.<.e.e.d.
 00000390: 3c00 6505 6504 6406 3c00 6506 6505 1900  <.e.e.d.<.e.e...
 000003a0: 6504 6407 3c00 6507 6504 6408 3c00 6506  e.d.<.e.e.d.<.e.
 000003b0: 6507 1900 6504 6409 3c00 6506 6508 6507  e...e.d.<.e.e.e.
 000003c0: 1900 1900 6504 640a 3c00 6506 6507 1900  ....e.d.<.e.e...
 000003d0: 6504 640b 3c00 6506 6507 1900 6504 640c  e.d.<.e.e...e.d.
 000003e0: 3c00 640d 640e 8400 5a09 640f 5300 2910  <.d.d...Z.d.S.).
-000003f0: 720a 0000 00da 0269 64da 0a70 726f 6a65  r......id..proje
-00000400: 6374 5f69 64da 0b77 6f72 6b66 6c6f 775f  ct_id..workflow_
-00000410: 6964 da10 696e 7075 745f 6461 7461 7365  id..input_datase
-00000420: 745f 6964 da11 6f75 7470 7574 5f64 6174  t_id..output_dat
+000003f0: 720a 0000 00da 0269 645a 0a70 726f 6a65  r......idZ.proje
+00000400: 6374 5f69 645a 0b77 6f72 6b66 6c6f 775f  ct_idZ.workflow_
+00000410: 6964 5a10 696e 7075 745f 6461 7461 7365  idZ.input_datase
+00000420: 745f 6964 5a11 6f75 7470 7574 5f64 6174  t_idZ.output_dat
 00000430: 6173 6574 5f69 64da 0f73 7461 7274 5f74  aset_id..start_t
 00000440: 696d 6573 7461 6d70 da0d 656e 645f 7469  imestamp..end_ti
 00000450: 6d65 7374 616d 70da 0673 7461 7475 73da  mestamp..status.
-00000460: 036c 6f67 da07 6869 7374 6f72 79da 0b77  .log..history..w
-00000470: 6f72 6b69 6e67 5f64 6972 da10 776f 726b  orking_dir..work
+00000460: 036c 6f67 da07 6869 7374 6f72 795a 0b77  .log..historyZ.w
+00000470: 6f72 6b69 6e67 5f64 6972 5a10 776f 726b  orking_dirZ.work
 00000480: 696e 675f 6469 725f 7573 6572 6301 0000  ing_dir_userc...
 00000490: 0000 0000 0000 0000 0002 0000 0003 0000  ................
 000004a0: 0043 0000 0073 2800 0000 7c00 a000 a100  .C...s(...|.....
 000004b0: 7d01 7401 7c00 6a02 8301 7c01 6401 3c00  }.t.|.j...|.d.<.
 000004c0: 7401 7c00 6a03 8301 7c01 6402 3c00 7c01  t.|.j...|.d.<.|.
-000004d0: 5300 2903 4e72 1b00 0000 721c 0000 0029  S.).Nr....r....)
-000004e0: 04da 0464 6963 7472 1000 0000 721b 0000  ...dictr....r...
-000004f0: 0072 1c00 0000 2902 da04 7365 6c66 da01  .r....)...self..
+000004d0: 5300 2903 4e72 1500 0000 7216 0000 0029  S.).Nr....r....)
+000004e0: 04da 0464 6963 7472 1000 0000 7215 0000  ...dictr....r...
+000004f0: 0072 1600 0000 2902 da04 7365 6c66 da01  .r....)...self..
 00000500: 6472 1200 0000 7212 0000 0072 1300 0000  dr....r....r....
 00000510: da0e 7361 6e69 7469 7365 645f 6469 6374  ..sanitised_dict
 00000520: 3100 0000 7308 0000 0008 010e 010e 0104  1...s...........
 00000530: 017a 2041 7070 6c79 576f 726b 666c 6f77  .z ApplyWorkflow
 00000540: 5265 6164 2e73 616e 6974 6973 6564 5f64  Read.sanitised_d
 00000550: 6963 744e 290a 720c 0000 0072 0d00 0000  ictN).r....r....
 00000560: 720e 0000 00da 0369 6e74 7211 0000 0072  r......intr....r
 00000570: 0200 0000 7203 0000 0072 1000 0000 da04  ....r....r......
-00000580: 6c69 7374 7225 0000 0072 1200 0000 7212  listr%...r....r.
+00000580: 6c69 7374 721d 0000 0072 1200 0000 7212  listr....r....r.
 00000590: 0000 0072 1200 0000 7213 0000 0072 0a00  ...r....r....r..
 000005a0: 0000 2300 0000 731c 0000 000a 0008 0108  ..#...s.........
 000005b0: 0108 0108 0108 0108 010c 0108 010c 0110  ................
 000005c0: 010c 010c 010c 0272 0a00 0000 4e29 0c72  .......r....N).r
 000005d0: 0200 0000 da06 7479 7069 6e67 7203 0000  ......typingr...
-000005e0: 00da 0870 7964 616e 7469 6372 0400 0000  ...pydanticr....
+000005e0: 005a 0870 7964 616e 7469 6372 0400 0000  .Z.pydanticr....
 000005f0: 7205 0000 00da 0b5f 7661 6c69 6461 746f  r......_validato
 00000600: 7273 7207 0000 00da 075f 5f61 6c6c 5f5f  rsr......__all__
 00000610: 7208 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
 00000620: 1200 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
 00000630: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
 00000640: 0073 1200 0000 0c00 0c01 0c02 0c01 0c02  .s..............
 00000650: 0402 1007 100b 1408                      ........
```

### Comparing `fractal_server-1.3.0a8/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc` & `fractal_server-1.3.0a9/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jun 12 09:12:04 2023 UTC, .py size: 3479 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 64e1 8664 970d 0000  o.......d..d....
+00000000: 6f0d 0d0a 0000 0000 5a07 9264 970d 0000  o.......Z..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 a800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c00  d.l.m.Z...d.d.l.
 00000040: 6d02 5a02 0100 6400 6403 6c00 6d03 5a03  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c04 6d06 5a06 0100 6400 6406 6c04  d.l.m.Z...d.d.l.
 00000070: 6d07 5a07 0100 6400 6407 6c04 6d08 5a08  m.Z...d.d.l.m.Z.
@@ -78,25 +78,25 @@
 000004d0: 206e 6565 645f 6770 753d 5472 7565 292c   need_gpu=True),
 000004e0: 0a20 2020 2020 2020 2020 2020 2065 7463  .            etc
 000004f0: 2e0a 2020 2020 2020 2020 6172 6773 5f73  ..        args_s
 00000500: 6368 656d 613a 0a20 2020 2020 2020 2020  chema:.         
 00000510: 2020 204a 534f 4e20 5363 6865 6d61 2066     JSON Schema f
 00000520: 6f72 2074 6173 6b20 6172 6775 6d65 6e74  or task argument
 00000530: 730a 2020 2020 da04 6e61 6d65 da0a 6578  s.    ..name..ex
-00000540: 6563 7574 6162 6c65 da0a 696e 7075 745f  ecutable..input_
+00000540: 6563 7574 6162 6c65 5a0a 696e 7075 745f  ecutableZ.input_
 00000550: 7479 7065 da0b 6f75 7470 7574 5f74 7970  type..output_typ
 00000560: 6529 01da 0f64 6566 6175 6c74 5f66 6163  e)...default_fac
 00000570: 746f 7279 da04 6d65 7461 da0b 6172 6773  tory..meta..args
 00000580: 5f73 6368 656d 614e 290b da08 5f5f 6e61  _schemaN)...__na
 00000590: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
 000005a0: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
 000005b0: 5f5f 646f 635f 5fda 0373 7472 da0f 5f5f  __doc__..str..__
 000005c0: 616e 6e6f 7461 7469 6f6e 735f 5f72 0600  annotations__r..
-000005d0: 0000 da04 6469 6374 7211 0000 0072 0300  ....dictr....r..
-000005e0: 0000 7202 0000 00a9 0072 1a00 0000 721a  ..r......r....r.
+000005d0: 0000 da04 6469 6374 7210 0000 0072 0300  ....dictr....r..
+000005e0: 0000 7202 0000 00a9 0072 1900 0000 7219  ..r......r....r.
 000005f0: 0000 00fa 4e2f 686f 6d65 2f74 6f6d 6d61  ....N/home/tomma
 00000600: 736f 2f46 7261 6374 616c 2f66 7261 6374  so/Fractal/fract
 00000610: 616c 2d73 6572 7665 722f 6672 6163 7461  al-server/fracta
 00000620: 6c5f 7365 7276 6572 2f63 6f6d 6d6f 6e2f  l_server/common/
 00000630: 7363 6865 6d61 732f 6d61 6e69 6665 7374  schemas/manifest
 00000640: 2e70 7972 0b00 0000 0e00 0000 7310 0000  .pyr........s...
 00000650: 000a 0004 0108 1b08 0108 0108 011e 0118  ................
@@ -174,83 +174,83 @@
 00000ad0: 656c 206f 6620 686f 7720 6061 7267 735f  el of how `args_
 00000ae0: 7363 6865 6d61 6073 2077 6572 6520 6765  schema`s were ge
 00000af0: 6e65 7261 7465 6420 2865 2e67 2e20 6070  nerated (e.g. `p
 00000b00: 7964 616e 7469 635f 7631 6029 2e0a 2020  ydantic_v1`)..  
 00000b10: 2020 da10 6d61 6e69 6665 7374 5f76 6572    ..manifest_ver
 00000b20: 7369 6f6e da09 7461 736b 5f6c 6973 7446  sion..task_listF
 00000b30: da10 6861 735f 6172 6773 5f73 6368 656d  ..has_args_schem
-00000b40: 6173 da13 6172 6773 5f73 6368 656d 615f  as..args_schema_
+00000b40: 6173 5a13 6172 6773 5f73 6368 656d 615f  asZ.args_schema_
 00000b50: 7665 7273 696f 6e63 0200 0000 0000 0000  versionc........
 00000b60: 0000 0000 0500 0000 0900 0000 4300 0000  ............C...
 00000b70: 734c 0000 007c 0164 0119 007d 027c 0164  sL...|.d...}.|.d
 00000b80: 0219 007d 037c 0272 247c 0344 005d 177d  ...}.|.r$|.D.].}
 00000b90: 047c 046a 0064 0075 0072 2374 0164 037c  .|.j.d.u.r#t.d.|
 00000ba0: 029b 0064 047c 046a 029b 0064 057c 046a  ...d.|.j...d.|.j
 00000bb0: 009b 0064 069d 0783 0182 0171 0c7c 0153  ...d.......q.|.S
-00000bc0: 0029 074e 7221 0000 0072 2000 0000 7a11  .).Nr!...r ...z.
+00000bc0: 0029 074e 7220 0000 0072 1f00 0000 7a11  .).Nr ...r....z.
 00000bd0: 6861 735f 6172 6773 5f73 6368 656d 6173  has_args_schemas
 00000be0: 3d7a 0b20 6275 7420 7461 736b 2022 7a12  =z. but task "z.
 00000bf0: 2220 6861 7320 6172 6773 5f73 6368 656d  " has args_schem
-00000c00: 613d da01 2e29 0372 1200 0000 da0a 5661  a=...).r......Va
+00000c00: 613d da01 2e29 0372 1100 0000 da0a 5661  a=...).r......Va
 00000c10: 6c75 6545 7272 6f72 720c 0000 0029 05da  lueErrorr....)..
-00000c20: 0363 6c73 da06 7661 6c75 6573 7221 0000  .cls..valuesr!..
-00000c30: 0072 2000 0000 da04 7461 736b 721a 0000  .r .....taskr...
-00000c40: 0072 1a00 0000 721b 0000 00da 1f5f 6368  .r....r......_ch
+00000c20: 0363 6c73 da06 7661 6c75 6573 7220 0000  .cls..valuesr ..
+00000c30: 0072 1f00 0000 da04 7461 736b 7219 0000  .r......taskr...
+00000c40: 0072 1900 0000 721a 0000 00da 1f5f 6368  .r....r......_ch
 00000c50: 6563 6b5f 6172 6773 5f73 6368 656d 6173  eck_args_schemas
 00000c60: 5f61 7265 5f70 7265 7365 6e74 5400 0000  _are_presentT...
 00000c70: 731c 0000 0008 0208 0104 0108 010a 0102  s...............
 00000c80: 0108 0104 0104 ff04 0106 ff04 ff02 ff04  ................
 00000c90: 057a 2d5f 4d61 6e69 6665 7374 4261 7365  .z-_ManifestBase
 00000ca0: 2e5f 6368 6563 6b5f 6172 6773 5f73 6368  ._check_args_sch
 00000cb0: 656d 6173 5f61 7265 5f70 7265 7365 6e74  emas_are_present
-00000cc0: 4e29 0d72 1300 0000 7214 0000 0072 1500  N).r....r....r..
-00000cd0: 0000 7216 0000 0072 1700 0000 7218 0000  ..r....r....r...
-00000ce0: 00da 046c 6973 7472 1c00 0000 7221 0000  ...listr....r!..
+00000cc0: 4e29 0d72 1200 0000 7213 0000 0072 1400  N).r....r....r..
+00000cd0: 0000 7215 0000 0072 1600 0000 7217 0000  ..r....r....r...
+00000ce0: 00da 046c 6973 7472 1b00 0000 7220 0000  ...listr....r ..
 00000cf0: 00da 0462 6f6f 6c72 0300 0000 7207 0000  ...boolr....r...
-00000d00: 0072 2800 0000 721a 0000 0072 1a00 0000  .r(...r....r....
-00000d10: 721a 0000 0072 1b00 0000 721e 0000 0035  r....r....r....5
+00000d00: 0072 2600 0000 7219 0000 0072 1900 0000  .r&...r....r....
+00000d10: 7219 0000 0072 1a00 0000 721d 0000 0035  r....r....r....5
 00000d20: 0000 0073 1000 0000 0a00 0401 0819 0c01  ...s............
-00000d30: 0c01 0c01 0402 0e01 721e 0000 0063 0000  ........r....c..
+00000d30: 0c01 0c01 0402 0e01 721d 0000 0063 0000  ........r....c..
 00000d40: 0000 0000 0000 0000 0000 0000 0000 0100  ................
 00000d50: 0000 4000 0000 730c 0000 0065 005a 0164  ..@...s....e.Z.d
 00000d60: 005a 0264 0153 0029 0272 0900 0000 4e29  .Z.d.S.).r....N)
-00000d70: 0372 1300 0000 7214 0000 0072 1500 0000  .r....r....r....
-00000d80: 721a 0000 0072 1a00 0000 721a 0000 0072  r....r....r....r
-00000d90: 1b00 0000 7209 0000 0062 0000 0073 0400  ....r....b...s..
+00000d70: 0372 1200 0000 7213 0000 0072 1400 0000  .r....r....r....
+00000d80: 7219 0000 0072 1900 0000 7219 0000 0072  r....r....r....r
+00000d90: 1a00 0000 7209 0000 0062 0000 0073 0400  ....r....b...s..
 00000da0: 0000 0800 0401 7209 0000 0063 0000 0000  ......r....c....
 00000db0: 0000 0000 0000 0000 0000 0000 0300 0000  ................
 00000dc0: 4000 0000 732e 0000 0065 005a 0164 005a  @...s....e.Z.d.Z
 00000dd0: 0255 0064 015a 0365 0465 0519 0065 0664  .U.d.Z.e.e...e.d
 00000de0: 023c 0065 0764 0383 0164 0464 0584 0083  .<.e.d...d.d....
 00000df0: 015a 0864 0653 0029 0772 0a00 0000 7a23  .Z.d.S.).r....z#
 00000e00: 0a20 2020 204d 616e 6966 6573 7420 7363  .    Manifest sc
 00000e10: 6865 6d61 2076 6572 7369 6f6e 2031 0a20  hema version 1. 
-00000e20: 2020 2072 2000 0000 721f 0000 0063 0200     r ...r....c..
+00000e20: 2020 2072 1f00 0000 721e 0000 0063 0200     r....r....c..
 00000e30: 0000 0000 0000 0000 0000 0200 0000 0400  ................
 00000e40: 0000 4300 0000 731c 0000 007c 0164 016b  ..C...s....|.d.k
 00000e50: 0372 0c74 0064 027c 019b 0064 039d 0383  .r.t.d.|...d....
 00000e60: 0182 0164 0053 0029 044e da01 317a 1e57  ...d.S.).N..1z.W
 00000e70: 726f 6e67 206d 616e 6966 6573 7420 7665  rong manifest ve
 00000e80: 7273 696f 6e20 2867 6976 656e 20fa 0129  rsion (given ..)
-00000e90: 2901 7224 0000 0029 0272 2500 0000 da05  ).r$...).r%.....
-00000ea0: 7661 6c75 6572 1a00 0000 721a 0000 0072  valuer....r....r
-00000eb0: 1b00 0000 da12 6d61 6e69 6665 7374 5f76  ......manifest_v
+00000e90: 2901 7222 0000 0029 0272 2300 0000 da05  ).r"...).r#.....
+00000ea0: 7661 6c75 6572 1900 0000 7219 0000 0072  valuer....r....r
+00000eb0: 1a00 0000 da12 6d61 6e69 6665 7374 5f76  ......manifest_v
 00000ec0: 6572 7369 6f6e 5f31 6d00 0000 7306 0000  ersion_1m...s...
 00000ed0: 0008 0210 0104 ff7a 1d4d 616e 6966 6573  .......z.Manifes
 00000ee0: 7456 312e 6d61 6e69 6665 7374 5f76 6572  tV1.manifest_ver
-00000ef0: 7369 6f6e 5f31 4e29 0972 1300 0000 7214  sion_1N).r....r.
-00000f00: 0000 0072 1500 0000 7216 0000 0072 2900  ...r....r....r).
-00000f10: 0000 7209 0000 0072 1800 0000 7208 0000  ..r....r....r...
-00000f20: 0072 2e00 0000 721a 0000 0072 1a00 0000  .r....r....r....
-00000f30: 721a 0000 0072 1b00 0000 720a 0000 0066  r....r....r....f
+00000ef0: 7369 6f6e 5f31 4e29 0972 1200 0000 7213  sion_1N).r....r.
+00000f00: 0000 0072 1400 0000 7215 0000 0072 2700  ...r....r....r'.
+00000f10: 0000 7209 0000 0072 1700 0000 7208 0000  ..r....r....r...
+00000f20: 0072 2c00 0000 7219 0000 0072 1900 0000  .r,...r....r....
+00000f30: 7219 0000 0072 1a00 0000 720a 0000 0066  r....r....r....f
 00000f40: 0000 0073 0a00 0000 0a00 0401 0c04 0602  ...s............
 00000f50: 0e01 720a 0000 004e 290f da06 7479 7069  ..r....N)...typi
 00000f60: 6e67 7202 0000 0072 0300 0000 7204 0000  ngr....r....r...
 00000f70: 00da 0870 7964 616e 7469 6372 0500 0000  ...pydanticr....
 00000f80: 7206 0000 0072 0700 0000 7208 0000 00da  r....r....r.....
-00000f90: 075f 5f61 6c6c 5f5f 720b 0000 0072 1c00  .__all__r....r..
-00000fa0: 0000 721e 0000 0072 0900 0000 720a 0000  ..r....r....r...
-00000fb0: 0072 1a00 0000 721a 0000 0072 1a00 0000  .r....r....r....
-00000fc0: 721b 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00000f90: 075f 5f61 6c6c 5f5f 720b 0000 0072 1b00  .__all__r....r..
+00000fa0: 0000 721d 0000 0072 0900 0000 720a 0000  ..r....r....r...
+00000fb0: 0072 1900 0000 7219 0000 0072 1900 0000  .r....r....r....
+00000fc0: 721a 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
 00000fd0: 0000 0073 1a00 0000 0c00 0c01 0c01 0c02  ...s............
 00000fe0: 0c01 0c01 0c01 0403 1003 0c24 1003 102d  ...........$...-
 00000ff0: 1404                                     ..
```

### Comparing `fractal_server-1.3.0a8/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc` & `fractal_server-1.3.0a9/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri May 26 06:41:57 2023 UTC, .py size: 2483 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b554 7064 b309 0000  o........Tpd....
+00000000: 6f0d 0d0a 0000 0000 5a07 9264 b309 0000  o.......Z..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 1c01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c00  d.l.m.Z...d.d.l.
 00000040: 6d02 5a02 0100 6400 6403 6c03 6d04 5a04  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c03 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c03 6d06 5a06 0100 6406 6407 6c07  d.l.m.Z...d.d.l.
 00000070: 6d08 5a08 0100 6406 6408 6c07 6d09 5a09  m.Z...d.d.l.m.Z.
@@ -68,15 +68,15 @@
 00000430: 721e 0000 004e 7220 0000 0072 1b00 0000  r....Nr ...r....
 00000440: 721b 0000 0072 1b00 0000 721c 0000 0072  r....r....r....r
 00000450: 1200 0000 2900 0000 7222 0000 0072 1200  ....)...r"...r..
 00000460: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
 00000470: 0000 0003 0000 0040 0000 0073 1e00 0000  .......@...s....
 00000480: 6500 5a01 6400 5a02 5500 6503 6504 6401  e.Z.d.Z.U.e.e.d.
 00000490: 3c00 6503 6504 6402 3c00 6403 5300 2904  <.e.e.d.<.d.S.).
-000004a0: 7211 0000 00da 0269 64da 0a64 6174 6173  r......id..datas
+000004a0: 7211 0000 00da 0269 645a 0a64 6174 6173  r......idZ.datas
 000004b0: 6574 5f69 644e 2905 7215 0000 0072 1600  et_idN).r....r..
 000004c0: 0000 7217 0000 00da 0369 6e74 721a 0000  ..r......intr...
 000004d0: 0072 1b00 0000 721b 0000 0072 1b00 0000  .r....r....r....
 000004e0: 721c 0000 0072 1100 0000 2e00 0000 7306  r....r........s.
 000004f0: 0000 000a 0008 010c 0172 1100 0000 6300  .........r....c.
 00000500: 0000 0000 0000 0000 0000 0000 0000 0003  ................
 00000510: 0000 0040 0000 0073 4c00 0000 6500 5a01  ...@...sL...e.Z.
@@ -94,129 +94,129 @@
 000005d0: 2020 206d 6574 613a 2054 4244 0a20 2020     meta: TBD.   
 000005e0: 2020 2020 2072 6561 645f 6f6e 6c79 3a20       read_only: 
 000005f0: 5442 440a 2020 2020 da04 6e61 6d65 da04  TBD.    ..name..
 00000600: 7479 7065 2901 da07 6465 6661 756c 74da  type)...default.
 00000610: 046d 6574 6146 da09 7265 6164 5f6f 6e6c  .metaF..read_onl
 00000620: 794e 290d 7215 0000 0072 1600 0000 7217  yN).r....r....r.
 00000630: 0000 0072 1800 0000 7219 0000 0072 1a00  ...r....r....r..
-00000640: 0000 7203 0000 0072 0500 0000 722a 0000  ..r....r....r*..
-00000650: 00da 0464 6963 7472 0200 0000 722b 0000  ...dictr....r+..
+00000640: 0000 7203 0000 0072 0500 0000 7229 0000  ..r....r....r)..
+00000650: 00da 0464 6963 7472 0200 0000 722a 0000  ...dictr....r*..
 00000660: 00da 0462 6f6f 6c72 1b00 0000 721b 0000  ...boolr....r...
-00000670: 0072 1b00 0000 721c 0000 0072 2600 0000  .r....r....r&...
+00000670: 0072 1b00 0000 721c 0000 0072 2500 0000  .r....r....r%...
 00000680: 3600 0000 730c 0000 000a 0004 0108 0a0c  6...s...........
-00000690: 011a 0110 0172 2600 0000 6300 0000 0000  .....r&...c.....
+00000690: 011a 0110 0172 2500 0000 6300 0000 0000  .....r%...c.....
 000006a0: 0000 0000 0000 0000 0000 0004 0000 0040  ...............@
 000006b0: 0000 0073 6600 0000 6500 5a01 6400 5a02  ...sf...e.Z.d.Z.
 000006c0: 5500 6503 6504 1900 6505 6401 3c00 6402  U.e.e...e.d.<.d.
 000006d0: 5a06 6503 6507 6504 6508 6602 1900 1900  Z.e.e.e.e.f.....
 000006e0: 6505 6403 3c00 6503 6509 1900 6505 6404  e.d.<.e.e...e.d.
 000006f0: 3c00 650a 6401 6405 6406 8d02 650b 6401  <.e.d.d.d...e.d.
 00000700: 8301 8301 5a0c 650a 6407 6405 6406 8d02  ....Z.e.d.d.d...
 00000710: 650b 6407 8301 8301 5a0d 6402 5300 2908  e.d.....Z.d.S.).
-00000720: 720d 0000 0072 2700 0000 4e72 2a00 0000  r....r'...Nr*...
-00000730: 722b 0000 0054 721e 0000 0072 2800 0000  r+...Tr....r(...
+00000720: 720d 0000 0072 2600 0000 4e72 2900 0000  r....r&...Nr)...
+00000730: 722a 0000 0054 721e 0000 0072 2700 0000  r*...Tr....r'...
 00000740: 290e 7215 0000 0072 1600 0000 7217 0000  ).r....r....r...
 00000750: 0072 0300 0000 7219 0000 0072 1a00 0000  .r....r....r....
-00000760: 722a 0000 0072 2c00 0000 7202 0000 0072  r*...r,...r....r
-00000770: 2d00 0000 7206 0000 0072 0900 0000 da05  -...r....r......
+00000760: 7229 0000 0072 2b00 0000 7202 0000 0072  r)...r+...r....r
+00000770: 2c00 0000 7206 0000 0072 0900 0000 da05  ,...r....r......
 00000780: 5f6e 616d 65da 055f 7479 7065 721b 0000  _name.._typer...
 00000790: 0072 1b00 0000 721b 0000 0072 1c00 0000  .r....r....r....
 000007a0: 720d 0000 0047 0000 0073 0c00 0000 0a00  r....G...s......
 000007b0: 0c01 1801 0c01 1403 1801 720d 0000 0063  ..........r....c
 000007c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000007d0: 0400 0000 4000 0000 7334 0000 0065 005a  ....@...s4...e.Z
 000007e0: 0164 005a 0265 0364 0164 0264 038d 0265  .d.Z.e.d.d.d...e
 000007f0: 0464 0183 0183 015a 0565 0364 0464 0264  .d.....Z.e.d.d.d
 00000800: 038d 0265 0464 0483 0183 015a 0664 0553  ...e.d.....Z.d.S
-00000810: 0029 0672 0e00 0000 7227 0000 0054 721e  .).r....r'...Tr.
-00000820: 0000 0072 2800 0000 4e29 0772 1500 0000  ...r(...N).r....
+00000810: 0029 0672 0e00 0000 7226 0000 0054 721e  .).r....r&...Tr.
+00000820: 0000 0072 2700 0000 4e29 0772 1500 0000  ...r'...N).r....
 00000830: 7216 0000 0072 1700 0000 7206 0000 0072  r....r....r....r
-00000840: 0900 0000 722e 0000 0072 2f00 0000 721b  ....r....r/...r.
+00000840: 0900 0000 722d 0000 0072 2e00 0000 721b  ....r-...r....r.
 00000850: 0000 0072 1b00 0000 721b 0000 0072 1c00  ...r....r....r..
 00000860: 0000 720e 0000 0051 0000 0073 0600 0000  ..r....Q...s....
 00000870: 0800 1402 1801 720e 0000 0063 0000 0000  ......r....c....
 00000880: 0000 0000 0000 0000 0000 0000 0300 0000  ................
 00000890: 4000 0000 7332 0000 0065 005a 0164 005a  @...s2...e.Z.d.Z
 000008a0: 0255 0065 0365 0464 013c 0065 0565 0619  .U.e.e.d.<.e.e..
 000008b0: 0065 0464 023c 0065 0365 0464 033c 0065  .e.d.<.e.e.d.<.e
 000008c0: 0765 0464 043c 0064 0553 0029 0672 0f00  .e.d.<.d.S.).r..
-000008d0: 0000 7223 0000 00da 0d72 6573 6f75 7263  ..r#.....resourc
+000008d0: 0000 7223 0000 005a 0d72 6573 6f75 7263  ..r#...Z.resourc
 000008e0: 655f 6c69 7374 da0a 7072 6f6a 6563 745f  e_list..project_
-000008f0: 6964 722b 0000 004e 2908 7215 0000 0072  idr+...N).r....r
-00000900: 1600 0000 7217 0000 0072 2500 0000 721a  ....r....r%...r.
-00000910: 0000 00da 046c 6973 7472 1100 0000 722d  .....listr....r-
+000008f0: 6964 722a 0000 004e 2908 7215 0000 0072  idr*...N).r....r
+00000900: 1600 0000 7217 0000 0072 2400 0000 721a  ....r....r$...r.
+00000910: 0000 00da 046c 6973 7472 1100 0000 722c  .....listr....r,
 00000920: 0000 0072 1b00 0000 721b 0000 0072 1b00  ...r....r....r..
 00000930: 0000 721c 0000 0072 0f00 0000 5700 0000  ..r....r....W...
 00000940: 730a 0000 000a 0008 010c 0108 010c 0172  s..............r
 00000950: 0f00 0000 6300 0000 0000 0000 0000 0000  ....c...........
 00000960: 0000 0000 0003 0000 0040 0000 0073 2600  .........@...s&.
 00000970: 0000 6500 5a01 6400 5a02 5500 6401 5a03  ..e.Z.d.Z.U.d.Z.
 00000980: 6504 6505 6402 3c00 6403 5a06 6507 6505  e.e.d.<.d.Z.e.e.
 00000990: 6404 3c00 6405 5300 2906 da0c 5f50 726f  d.<.d.S.)..._Pro
 000009a0: 6a65 6374 4261 7365 7a5a 0a20 2020 2042  jectBasezZ.    B
 000009b0: 6173 6520 636c 6173 7320 666f 7220 5072  ase class for Pr
 000009c0: 6f6a 6563 740a 0a20 2020 2041 7474 7269  oject..    Attri
 000009d0: 6275 7465 733a 0a20 2020 2020 2020 206e  butes:.        n
 000009e0: 616d 653a 2054 4244 0a20 2020 2020 2020  ame: TBD.       
 000009f0: 2072 6561 645f 6f6e 6c79 3a20 5442 440a   read_only: TBD.
-00000a00: 2020 2020 7227 0000 0046 722b 0000 004e      r'...Fr+...N
+00000a00: 2020 2020 7226 0000 0046 722a 0000 004e      r&...Fr*...N
 00000a10: 2908 7215 0000 0072 1600 0000 7217 0000  ).r....r....r...
 00000a20: 0072 1800 0000 7219 0000 0072 1a00 0000  .r....r....r....
-00000a30: 722b 0000 0072 2d00 0000 721b 0000 0072  r+...r-...r....r
-00000a40: 1b00 0000 721b 0000 0072 1c00 0000 7233  ....r....r....r3
+00000a30: 722a 0000 0072 2c00 0000 721b 0000 0072  r*...r,...r....r
+00000a40: 1b00 0000 721b 0000 0072 1c00 0000 7231  ....r....r....r1
 00000a50: 0000 0061 0000 0073 0800 0000 0a00 0401  ...a...s........
-00000a60: 0808 1001 7233 0000 0063 0000 0000 0000  ....r3...c......
+00000a60: 0808 1001 7231 0000 0063 0000 0000 0000  ....r1...c......
 00000a70: 0000 0000 0000 0000 0000 0400 0000 4000  ..............@.
 00000a80: 0000 7346 0000 0065 005a 0164 005a 0255  ..sF...e.Z.d.Z.U
 00000a90: 0064 015a 0365 0465 0519 0065 0664 023c  .d.Z.e.e...e.d.<
 00000aa0: 0065 0764 0364 0464 058d 0265 0864 0383  .e.d.d.d...e.d..
 00000ab0: 0183 015a 0965 0764 0264 0464 058d 0265  ...Z.e.d.d.d...e
 00000ac0: 0864 0283 0183 015a 0a64 0653 0029 0772  .d.....Z.d.S.).r
-00000ad0: 0a00 0000 7229 0000 00da 1464 6566 6175  ....r).....defau
+00000ad0: 0a00 0000 7228 0000 00da 1464 6566 6175  ....r(.....defau
 00000ae0: 6c74 5f64 6174 6173 6574 5f6e 616d 6572  lt_dataset_namer
-00000af0: 2700 0000 5472 1e00 0000 4e29 0b72 1500  '...Tr....N).r..
-00000b00: 0000 7216 0000 0072 1700 0000 7234 0000  ..r....r....r4..
+00000af0: 2600 0000 5472 1e00 0000 4e29 0b72 1500  &...Tr....N).r..
+00000b00: 0000 7216 0000 0072 1700 0000 7232 0000  ..r....r....r2..
 00000b10: 0072 0300 0000 7219 0000 0072 1a00 0000  .r....r....r....
-00000b20: 7206 0000 0072 0900 0000 722e 0000 00da  r....r....r.....
+00000b20: 7206 0000 0072 0900 0000 722d 0000 005a  r....r....r-...Z
 00000b30: 155f 6465 6661 756c 745f 6461 7461 7365  ._default_datase
 00000b40: 745f 6e61 6d65 721b 0000 0072 1b00 0000  t_namer....r....
 00000b50: 721b 0000 0072 1c00 0000 720a 0000 006e  r....r....r....n
 00000b60: 0000 0073 1000 0000 0a00 1001 1403 0201  ...s............
 00000b70: 0401 04ff 0602 08fe 720a 0000 0063 0000  ........r....c..
 00000b80: 0000 0000 0000 0000 0000 0000 0000 0300  ................
 00000b90: 0000 4000 0000 7326 0000 0065 005a 0164  ..@...s&...e.Z.d
 00000ba0: 005a 0255 0065 0365 0464 013c 0067 005a  .Z.U.e.e.d.<.g.Z
 00000bb0: 0565 0665 0719 0065 0464 023c 0064 0353  .e.e...e.d.<.d.S
 00000bc0: 0029 0472 0b00 0000 7223 0000 00da 0c64  .).r....r#.....d
 00000bd0: 6174 6173 6574 5f6c 6973 744e 2908 7215  ataset_listN).r.
-00000be0: 0000 0072 1600 0000 7217 0000 0072 2500  ...r....r....r%.
-00000bf0: 0000 721a 0000 0072 3600 0000 7232 0000  ..r....r6...r2..
+00000be0: 0000 0072 1600 0000 7217 0000 0072 2400  ...r....r....r$.
+00000bf0: 0000 721a 0000 0072 3300 0000 7230 0000  ..r....r3...r0..
 00000c00: 0072 0f00 0000 721b 0000 0072 1b00 0000  .r....r....r....
 00000c10: 721b 0000 0072 1c00 0000 720b 0000 0078  r....r....r....x
 00000c20: 0000 0073 0600 0000 0a00 0801 1401 720b  ...s..........r.
 00000c30: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
 00000c40: 0000 0000 0400 0000 4000 0000 733a 0000  ........@...s:..
 00000c50: 0065 005a 0164 005a 0255 0065 0365 0419  .e.Z.d.Z.U.e.e..
 00000c60: 0065 0564 013c 0065 0365 0619 0065 0564  .e.d.<.e.e...e.d
 00000c70: 023c 0065 0764 0164 0364 048d 0265 0864  .<.e.d.d.d...e.d
 00000c80: 0183 0183 015a 0964 0553 0029 0672 0c00  .....Z.d.S.).r..
-00000c90: 0000 7227 0000 0072 2b00 0000 5472 1e00  ..r'...r+...Tr..
+00000c90: 0000 7226 0000 0072 2a00 0000 5472 1e00  ..r&...r*...Tr..
 00000ca0: 0000 4e29 0a72 1500 0000 7216 0000 0072  ..N).r....r....r
 00000cb0: 1700 0000 7203 0000 0072 1900 0000 721a  ....r....r....r.
-00000cc0: 0000 0072 2d00 0000 7206 0000 0072 0900  ...r-...r....r..
-00000cd0: 0000 722e 0000 0072 1b00 0000 721b 0000  ..r....r....r...
+00000cc0: 0000 0072 2c00 0000 7206 0000 0072 0900  ...r,...r....r..
+00000cd0: 0000 722d 0000 0072 1b00 0000 721b 0000  ..r-...r....r...
 00000ce0: 0072 1b00 0000 721c 0000 0072 0c00 0000  .r....r....r....
 00000cf0: 7d00 0000 7308 0000 000a 000c 010c 0118  }...s...........
 00000d00: 0372 0c00 0000 4e29 17da 0674 7970 696e  .r....N)...typin
 00000d10: 6772 0200 0000 7203 0000 00da 0870 7964  gr....r......pyd
 00000d20: 616e 7469 6372 0400 0000 7205 0000 0072  anticr....r....r
 00000d30: 0600 0000 da0b 5f76 616c 6964 6174 6f72  ......_validator
 00000d40: 7372 0800 0000 7209 0000 00da 075f 5f61  sr....r......__a
 00000d50: 6c6c 5f5f 7213 0000 0072 1000 0000 7212  ll__r....r....r.
-00000d60: 0000 0072 1100 0000 7226 0000 0072 0d00  ...r....r&...r..
-00000d70: 0000 720e 0000 0072 0f00 0000 7233 0000  ..r....r....r3..
+00000d60: 0000 0072 1100 0000 7225 0000 0072 0d00  ...r....r%...r..
+00000d70: 0000 720e 0000 0072 0f00 0000 7231 0000  ..r....r....r1..
 00000d80: 0072 0a00 0000 720b 0000 0072 0c00 0000  .r....r....r....
 00000d90: 721b 0000 0072 1b00 0000 721b 0000 0072  r....r....r....r
 00000da0: 1c00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
 00000db0: 0000 7328 0000 000c 000c 010c 020c 010c  ..s(............
 00000dc0: 010c 020c 0104 0310 1010 0810 0510 0510  ................
 00000dd0: 0810 1110 0a10 0610 0a10 0d10 0a14 05    ...............
```

### Comparing `fractal_server-1.3.0a8/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc` & `fractal_server-1.3.0a9/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri May 26 06:41:57 2023 UTC, .py size: 673 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b554 7064 a102 0000  o........Tpd....
+00000000: 6f0d 0d0a 0000 0000 5a07 9264 a102 0000  o.......Z..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5800 0000 6400  .....@...sX...d.
 00000030: 6401 6c00 6d00 5a00 0100 6400 6402 6c01  d.l.m.Z...d.d.l.
 00000040: 6d02 5a02 0100 6400 6403 6c01 6d03 5a03  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c04 6d05 5a05 0100 6405  ..d.d.l.m.Z...d.
 00000060: 5a06 4700 6406 6407 8400 6407 6505 8303  Z.G.d.d...d.e...
 00000070: 5a07 4700 6408 6409 8400 6409 6507 8303  Z.G.d.d...d.e...
```

### Comparing `fractal_server-1.3.0a8/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc` & `fractal_server-1.3.0a9/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jun 12 09:12:04 2023 UTC, .py size: 2578 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 64e1 8664 120a 0000  o.......d..d....
+00000000: 6f0d 0d0a 0000 0000 5a07 9264 120a 0000  o.......Z..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 b000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c00  d.l.m.Z...d.d.l.
 00000040: 6d02 5a02 0100 6400 6403 6c03 6d04 5a04  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c03 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c03 6d06 5a06 0100 6406 6407 6c07  d.l.m.Z...d.d.l.
 00000070: 6d08 5a08 0100 6408 5a09 4700 6409 640a  m.Z...d.Z.G.d.d.
@@ -147,15 +147,15 @@
 00000920: 0000 0072 2000 0000 7221 0000 0072 2200  ...r ...r!...r".
 00000930: 0000 5472 1000 0000 4e29 1272 1200 0000  ..Tr....N).r....
 00000940: 7213 0000 0072 1400 0000 7216 0000 0072  r....r....r....r
 00000950: 1700 0000 7205 0000 0072 1f00 0000 7203  ....r....r....r.
 00000960: 0000 0072 2300 0000 7202 0000 0072 0600  ...r#...r....r..
 00000970: 0000 7208 0000 0072 2400 0000 7225 0000  ..r....r$...r%..
 00000980: 0072 2600 0000 7227 0000 0072 2800 0000  .r&...r'...r(...
-00000990: da14 5f61 7267 735f 7363 6865 6d61 5f76  .._args_schema_v
+00000990: 5a14 5f61 7267 735f 7363 6865 6d61 5f76  Z._args_schema_v
 000009a0: 6572 7369 6f6e 7219 0000 0072 1900 0000  ersionr....r....
 000009b0: 7219 0000 0072 1a00 0000 7209 0000 004e  r....r....r....N
 000009c0: 0000 0073 2a00 0000 0a00 0801 0801 0801  ...s*...........
 000009d0: 0801 1e01 0c01 1401 0c01 1403 0a01 0601  ................
 000009e0: 04ff 0a03 0601 04ff 1403 1401 0a01 0601  ................
 000009f0: 08ff 7209 0000 004e 2910 da06 7479 7069  ..r....N)...typi
 00000a00: 6e67 7202 0000 0072 0300 0000 da08 7079  ngr....r......py
```

### Comparing `fractal_server-1.3.0a8/fractal_server/common/schemas/__pycache__/task_collection.cpython-310.pyc` & `fractal_server-1.3.0a9/fractal_server/common/schemas/__pycache__/task_collection.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jun 12 09:12:04 2023 UTC, .py size: 2935 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 64e1 8664 770b 0000  o.......d..dw...
+00000000: 6f0d 0d0a 0000 0000 5a07 9264 770b 0000  o.......Z..dw...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 9800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c02 6d04 5a04  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c05 6d06 5a06 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c05 6d07 5a07 0100 6400 6406 6c05  d.l.m.Z...d.d.l.
 00000070: 6d08 5a08 0100 6407 6408 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
@@ -131,17 +131,17 @@
 00000820: 6f6c 6c65 6374 5069 702e 7061 636b 6167  ollectPip.packag
 00000830: 655f 7661 6c69 6461 746f 7229 1272 0e00  e_validator).r..
 00000840: 0000 720f 0000 0072 1000 0000 da07 5f5f  ..r....r......__
 00000850: 646f 635f 5fda 0373 7472 da0f 5f5f 616e  doc__..str..__an
 00000860: 6e6f 7461 7469 6f6e 735f 5f72 1400 0000  notations__r....
 00000870: 7204 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
 00000880: 1700 0000 da04 6469 6374 7207 0000 0072  ......dictr....r
-00000890: 0900 0000 da10 5f70 6163 6b61 6765 5f76  ......_package_v
-000008a0: 6572 7369 6f6e da0f 5f70 6163 6b61 6765  ersion.._package
-000008b0: 5f65 7874 7261 73da 0f5f 7079 7468 6f6e  _extras.._python
+00000890: 0900 0000 5a10 5f70 6163 6b61 6765 5f76  ....Z._package_v
+000008a0: 6572 7369 6f6e 5a0f 5f70 6163 6b61 6765  ersionZ._package
+000008b0: 5f65 7874 7261 735a 0f5f 7079 7468 6f6e  _extrasZ._python
 000008c0: 5f76 6572 7369 6f6e 721f 0000 0072 1100  _versionr....r..
 000008d0: 0000 7211 0000 0072 1100 0000 7212 0000  ..r....r....r...
 000008e0: 0072 0b00 0000 1600 0000 7324 0000 000a  .r........s$....
 000008f0: 0004 0108 1a10 0110 0110 0118 010a 0206  ................
 00000900: 0104 ff0a 0306 0104 ff0a 0306 0104 ff06  ................
 00000910: 040e 0172 0b00 0000 6300 0000 0000 0000  ...r....c.......
 00000920: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
@@ -159,41 +159,41 @@
 000009e0: 7475 733a 2054 4244 0a20 2020 2020 2020  tus: TBD.       
 000009f0: 2070 6163 6b61 6765 3a20 5442 440a 2020   package: TBD.  
 00000a00: 2020 2020 2020 7665 6e76 5f70 6174 683a        venv_path:
 00000a10: 2054 4244 0a20 2020 2020 2020 2074 6173   TBD.        tas
 00000a20: 6b5f 6c69 7374 3a20 5442 440a 2020 2020  k_list: TBD.    
 00000a30: 2020 2020 6c6f 673a 2054 4244 0a20 2020      log: TBD.   
 00000a40: 2020 2020 2069 6e66 6f3a 2054 4244 0a20       info: TBD. 
-00000a50: 2020 2029 05da 0770 656e 6469 6e67 da0a     )...pending..
-00000a60: 696e 7374 616c 6c69 6e67 da0a 636f 6c6c  installing..coll
+00000a50: 2020 2029 05da 0770 656e 6469 6e67 5a0a     )...pendingZ.
+00000a60: 696e 7374 616c 6c69 6e67 5a0a 636f 6c6c  installingZ.coll
 00000a70: 6563 7469 6e67 da04 6661 696c da02 4f4b  ecting..fail..OK
 00000a80: da06 7374 6174 7573 7213 0000 00da 0976  ..statusr......v
 00000a90: 656e 765f 7061 7468 2901 da07 6465 6661  env_path)...defa
 00000aa0: 756c 74da 0974 6173 6b5f 6c69 7374 da03  ult..task_list..
 00000ab0: 6c6f 67da 0469 6e66 6f63 0100 0000 0000  log..infoc......
 00000ac0: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
 00000ad0: 0000 731a 0000 007c 00a0 00a1 007d 0174  ..s....|.....}.t
 00000ae0: 017c 006a 0283 017c 0164 013c 007c 0153  .|.j...|.d.<.|.S
 00000af0: 0029 027a 510a 2020 2020 2020 2020 5265  .).zQ.        Re
 00000b00: 7475 726e 2060 7365 6c66 2e64 6963 7428  turn `self.dict(
 00000b10: 2960 2061 6674 6572 2063 6173 7469 6e67  )` after casting
 00000b20: 2060 7365 6c66 2e76 656e 765f 7061 7468   `self.venv_path
 00000b30: 6020 746f 2061 2073 7472 696e 670a 2020  ` to a string.  
-00000b40: 2020 2020 2020 722d 0000 0029 0372 2300        r-...).r#.
-00000b50: 0000 7221 0000 0072 2d00 0000 2902 da04  ..r!...r-...)...
+00000b40: 2020 2020 2020 7228 0000 0029 0372 2300        r(...).r#.
+00000b50: 0000 7221 0000 0072 2800 0000 2902 da04  ..r!...r(...)...
 00000b60: 7365 6c66 da01 6472 1100 0000 7211 0000  self..dr....r...
 00000b70: 0072 1200 0000 da0e 7361 6e69 7469 7365  .r......sanitise
 00000b80: 645f 6469 6374 6400 0000 7306 0000 0008  d_dictd...s.....
 00000b90: 040e 0104 017a 2054 6173 6b43 6f6c 6c65  .....z TaskColle
 00000ba0: 6374 5374 6174 7573 2e73 616e 6974 6973  ctStatus.sanitis
 00000bb0: 6564 5f64 6963 744e 290e 720e 0000 0072  ed_dictN).r....r
 00000bc0: 0f00 0000 7210 0000 0072 2000 0000 7203  ....r....r ...r.
 00000bd0: 0000 0072 2200 0000 7221 0000 0072 0200  ...r"...r!...r..
-00000be0: 0000 7206 0000 0072 2f00 0000 7204 0000  ..r....r/...r...
-00000bf0: 00da 046c 6973 7472 0a00 0000 7234 0000  ...listr....r4..
+00000be0: 0000 7206 0000 0072 2a00 0000 7204 0000  ..r....r*...r...
+00000bf0: 00da 046c 6973 7472 0a00 0000 722f 0000  ...listr....r/..
 00000c00: 0072 1100 0000 7211 0000 0072 1100 0000  .r....r....r....
 00000c10: 7212 0000 0072 0c00 0000 5000 0000 7312  r....r....P...s.
 00000c20: 0000 000a 0004 010c 0c08 0108 011a 010c  ................
 00000c30: 010c 010c 0272 0c00 0000 4e29 11da 0770  .....r....N)...p
 00000c40: 6174 686c 6962 7202 0000 00da 0674 7970  athlibr......typ
 00000c50: 696e 6772 0300 0000 7204 0000 00da 0870  ingr....r......p
 00000c60: 7964 616e 7469 6372 0500 0000 7206 0000  ydanticr....r...
```

### Comparing `fractal_server-1.3.0a8/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc` & `fractal_server-1.3.0a9/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri May 26 06:41:57 2023 UTC, .py size: 1216 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b554 7064 c004 0000  o........Tpd....
+00000000: 6f0d 0d0a 0000 0000 5a07 9264 c004 0000  o.......Z..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 7e00 0000 6400  .....@...s~...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6404 6405 6c06 6d07 5a07 0100 6404  ..d.d.l.m.Z...d.
 00000060: 6406 6c06 6d08 5a08 0100 6407 5a09 4700  d.l.m.Z...d.Z.G.
 00000070: 6408 6409 8400 6409 6503 6a0a 650b 1900  d.d...d.e.j.e...
@@ -44,33 +44,33 @@
 000002b0: 6404 6405 8d02 6507 6403 8301 8301 5a09  d.d...e.d.....Z.
 000002c0: 6506 6402 6404 6405 8d02 650a 6402 8301  e.d.d.d...e.d...
 000002d0: 8301 5a0b 6406 5300 2907 7209 0000 0072  ..Z.d.S.).r....r
 000002e0: 0b00 0000 720c 0000 0072 0d00 0000 54a9  ....r....r....T.
 000002f0: 01da 0b61 6c6c 6f77 5f72 6575 7365 4ea9  ...allow_reuseN.
 00000300: 0c72 0e00 0000 720f 0000 0072 1000 0000  .r....r....r....
 00000310: 7202 0000 0072 1100 0000 7212 0000 0072  r....r....r....r
-00000320: 0400 0000 7207 0000 00da 0b5f 736c 7572  ....r......_slur
-00000330: 6d5f 7573 6572 da09 5f75 7365 726e 616d  m_user.._usernam
-00000340: 6572 0600 0000 da0a 5f63 6163 6865 5f64  er......_cache_d
+00000320: 0400 0000 7207 0000 005a 0b5f 736c 7572  ....r....Z._slur
+00000330: 6d5f 7573 6572 5a09 5f75 7365 726e 616d  m_userZ._usernam
+00000340: 6572 0600 0000 5a0a 5f63 6163 6865 5f64  er....Z._cache_d
 00000350: 6972 7213 0000 0072 1300 0000 7213 0000  irr....r....r...
 00000360: 0072 1400 0000 7209 0000 0017 0000 00f3  .r....r.........
 00000370: 1600 0000 0a00 0c01 0c01 0c01 0a03 0601  ................
 00000380: 04ff 1403 0a01 0601 08ff 7209 0000 0063  ..........r....c
 00000390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003a0: 0400 0000 4000 0000 7215 0000 0029 0772  ....@...r....).r
 000003b0: 0a00 0000 720b 0000 0072 0c00 0000 720d  ....r....r....r.
 000003c0: 0000 0054 7216 0000 004e 7218 0000 0072  ...Tr....Nr....r
 000003d0: 1300 0000 7213 0000 0072 1300 0000 7214  ....r....r....r.
-000003e0: 0000 0072 0a00 0000 2600 0000 721c 0000  ...r....&...r...
+000003e0: 0000 0072 0a00 0000 2600 0000 7219 0000  ...r....&...r...
 000003f0: 0072 0a00 0000 4e29 11da 0674 7970 696e  .r....N)...typin
-00000400: 6772 0200 0000 da0d 6661 7374 6170 695f  gr......fastapi_
+00000400: 6772 0200 0000 5a0d 6661 7374 6170 695f  gr....Z.fastapi_
 00000410: 7573 6572 7372 0300 0000 da08 7079 6461  usersr......pyda
 00000420: 6e74 6963 7204 0000 00da 0b5f 7661 6c69  nticr......_vali
 00000430: 6461 746f 7273 7206 0000 0072 0700 0000  datorsr....r....
-00000440: da07 5f5f 616c 6c5f 5fda 0842 6173 6555  ..__all__..BaseU
-00000450: 7365 72da 0369 6e74 7208 0000 00da 0e42  ser..intr......B
+00000440: da07 5f5f 616c 6c5f 5f5a 0842 6173 6555  ..__all__Z.BaseU
+00000450: 7365 72da 0369 6e74 7208 0000 005a 0e42  ser..intr....Z.B
 00000460: 6173 6555 7365 7255 7064 6174 6572 0900  aseUserUpdater..
-00000470: 0000 da0e 4261 7365 5573 6572 4372 6561  ....BaseUserCrea
+00000470: 0000 5a0e 4261 7365 5573 6572 4372 6561  ..Z.BaseUserCrea
 00000480: 7465 720a 0000 0072 1300 0000 7213 0000  ter....r....r...
 00000490: 0072 1300 0000 7214 0000 00da 083c 6d6f  .r....r......<mo
 000004a0: 6475 6c65 3e01 0000 0073 1200 0000 0c00  dule>....s......
 000004b0: 0c02 0c01 0c02 0c01 0403 1607 1206 160f  ................
```

### Comparing `fractal_server-1.3.0a8/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc` & `fractal_server-1.3.0a9/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri May 26 06:41:57 2023 UTC, .py size: 2457 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b554 7064 9909 0000  o........Tpd....
+00000000: 6f0d 0d0a 0000 0000 5a07 9264 9909 0000  o.......Z..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3401 0000 6400  .....@...s4...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c00  d.l.m.Z...d.d.l.
 00000040: 6d02 5a02 0100 6400 6403 6c03 6d04 5a04  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c03 6d05 5a05 0100 6405  ..d.d.l.m.Z...d.
 00000060: 6406 6c06 6d07 5a07 0100 6405 6407 6c06  d.l.m.Z...d.d.l.
 00000070: 6d08 5a08 0100 6405 6408 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
@@ -105,15 +105,15 @@
 00000680: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
 00000690: 0000 0300 0000 4000 0000 731c 0000 0065  ......@...s....e
 000006a0: 005a 0164 005a 0265 0364 0183 0164 0264  .Z.d.Z.e.d...d.d
 000006b0: 0384 0083 015a 0464 0453 0029 0572 1500  .....Z.d.S.).r..
 000006c0: 0000 7217 0000 0063 0200 0000 0000 0000  ..r....c........
 000006d0: 0000 0000 0200 0000 0200 0000 4300 0000  ............C...
 000006e0: 7314 0000 0064 017c 0176 0072 0874 0064  s....d.|.v.r.t.d
-000006f0: 0283 0182 017c 0153 0029 034e da15 7061  .....|.S.).N..pa
+000006f0: 0283 0182 017c 0153 0029 034e 5a15 7061  .....|.S.).NZ.pa
 00000700: 7261 6c6c 656c 697a 6174 696f 6e5f 6c65  rallelization_le
 00000710: 7665 6c7a 3b4f 7665 7272 6964 696e 6720  velz;Overriding 
 00000720: 7461 736b 2070 6172 616c 6c65 6c69 7a61  task paralleliza
 00000730: 7469 6f6e 206c 6576 656c 2063 7572 7265  tion level curre
 00000740: 6e74 6c79 206e 6f74 2061 6c6c 6f77 6564  ntly not allowed
 00000750: 2901 da0a 5661 6c75 6545 7272 6f72 2902  )...ValueError).
 00000760: da03 636c 73da 016d 721f 0000 0072 1f00  ..cls..mr....r..
@@ -121,25 +121,25 @@
 00000780: 6f5f 7061 7261 6c6c 656c 6973 6174 696f  o_parallelisatio
 00000790: 6e5f 6c65 7665 6c3a 0000 0073 0a00 0000  n_level:...s....
 000007a0: 0802 0201 0201 04ff 0403 7a31 576f 726b  ..........z1Work
 000007b0: 666c 6f77 5461 736b 5570 6461 7465 2e63  flowTaskUpdate.c
 000007c0: 6865 636b 5f6e 6f5f 7061 7261 6c6c 656c  heck_no_parallel
 000007d0: 6973 6174 696f 6e5f 6c65 7665 6c4e 2905  isation_levelN).
 000007e0: 7219 0000 0072 1a00 0000 721b 0000 0072  r....r....r....r
-000007f0: 0500 0000 7231 0000 0072 1f00 0000 721f  ....r1...r....r.
+000007f0: 0500 0000 7230 0000 0072 1f00 0000 721f  ....r0...r....r.
 00000800: 0000 0072 1f00 0000 7220 0000 0072 1500  ...r....r ...r..
 00000810: 0000 3800 0000 7306 0000 0008 0006 020e  ..8...s.........
 00000820: 0172 1500 0000 6300 0000 0000 0000 0000  .r....c.........
 00000830: 0000 0000 0000 0003 0000 0040 0000 0072  ...........@...r
 00000840: 2b00 0000 2903 da0d 5f57 6f72 6b66 6c6f  +...)..._Workflo
 00000850: 7742 6173 65da 046e 616d 654e 2905 7219  wBase..nameN).r.
 00000860: 0000 0072 1a00 0000 721b 0000 0072 1d00  ...r....r....r..
 00000870: 0000 721e 0000 0072 1f00 0000 721f 0000  ..r....r....r...
-00000880: 0072 1f00 0000 7220 0000 0072 3200 0000  .r....r ...r2...
-00000890: 4300 0000 722c 0000 0072 3200 0000 6300  C...r,...r2...c.
+00000880: 0072 1f00 0000 7220 0000 0072 3100 0000  .r....r ...r1...
+00000890: 4300 0000 722c 0000 0072 3100 0000 6300  C...r,...r1...c.
 000008a0: 0000 0000 0000 0000 0000 0000 0000 0003  ................
 000008b0: 0000 0040 0000 0073 2a00 0000 6500 5a01  ...@...s*...e.Z.
 000008c0: 6400 5a02 5500 6503 6504 6401 3c00 6503  d.Z.U.e.e.d.<.e.
 000008d0: 6504 6402 3c00 6505 6506 1900 6504 6403  e.d.<.e.e...e.d.
 000008e0: 3c00 6404 5300 2905 720d 0000 0072 2700  <.d.S.).r....r'.
 000008f0: 0000 da0a 7072 6f6a 6563 745f 6964 da09  ....project_id..
 00000900: 7461 736b 5f6c 6973 744e 2907 7219 0000  task_listN).r...
@@ -148,28 +148,28 @@
 00000930: 721f 0000 0072 1f00 0000 721f 0000 0072  r....r....r....r
 00000940: 2000 0000 720d 0000 0047 0000 0073 0800   ...r....G...s..
 00000950: 0000 0a00 0801 0801 1001 720d 0000 0063  ..........r....c
 00000960: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000970: 0400 0000 4000 0000 7320 0000 0065 005a  ....@...s ...e.Z
 00000980: 0164 005a 0265 0364 0164 0264 038d 0265  .d.Z.e.d.d.d...e
 00000990: 0464 0183 0183 015a 0564 0453 0029 0572  .d.....Z.d.S.).r
-000009a0: 0c00 0000 7233 0000 0054 7222 0000 004e  ....r3...Tr"...N
+000009a0: 0c00 0000 7232 0000 0054 7222 0000 004e  ....r2...Tr"...N
 000009b0: 2906 7219 0000 0072 1a00 0000 721b 0000  ).r....r....r...
 000009c0: 0072 0500 0000 7208 0000 00da 055f 6e61  .r....r......_na
 000009d0: 6d65 721f 0000 0072 1f00 0000 721f 0000  mer....r....r...
 000009e0: 0072 2000 0000 720c 0000 004d 0000 0073  .r ...r....M...s
 000009f0: 0400 0000 0800 1802 720c 0000 0063 0000  ........r....c..
 00000a00: 0000 0000 0000 0000 0000 0000 0000 0400  ................
 00000a10: 0000 4000 0000 734e 0000 0065 005a 0164  ..@...sN...e.Z.d
 00000a20: 005a 0255 0065 0365 0419 0065 0564 013c  .Z.U.e.e...e.d.<
 00000a30: 0065 0365 0665 0719 0019 0065 0564 023c  .e.e.e.....e.d.<
 00000a40: 0065 0864 0164 0364 048d 0265 0964 0183  .e.d.d.d...e.d..
 00000a50: 0183 015a 0a65 0864 0283 0164 0564 0684  ...Z.e.d...d.d..
 00000a60: 0083 015a 0b64 0753 0029 0872 0e00 0000  ...Z.d.S.).r....
-00000a70: 7233 0000 00da 1a72 656f 7264 6572 6564  r3.....reordered
+00000a70: 7232 0000 005a 1a72 656f 7264 6572 6564  r2...Z.reordered
 00000a80: 5f77 6f72 6b66 6c6f 7774 6173 6b5f 6964  _workflowtask_id
 00000a90: 7354 7222 0000 0063 0200 0000 0000 0000  sTr"...c........
 00000aa0: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
 00000ab0: 733a 0000 0074 0064 0164 0284 007c 0144  s:...t.d.d...|.D
 00000ac0: 0083 0183 0172 0d74 0164 0383 0182 0174  .....r.t.d.....t
 00000ad0: 027c 0183 0174 0274 037c 0183 0183 016b  .|...t.t.|.....k
 00000ae0: 0372 1b74 0164 0483 0182 017c 0153 0029  .r.t.d.....|.S.)
@@ -186,59 +186,59 @@
 00000b90: 3c6c 6f63 616c 733e 2e3c 6765 6e65 7870  <locals>.<genexp
 00000ba0: 723e 7a2d 4e65 6761 7469 7665 2060 6964  r>z-Negative `id
 00000bb0: 6020 696e 2060 7265 6f72 6465 7265 645f  ` in `reordered_
 00000bc0: 776f 726b 666c 6f77 7461 736b 5f69 6473  workflowtask_ids
 00000bd0: 607a 2c60 7265 6f72 6465 7265 645f 776f  `z,`reordered_wo
 00000be0: 726b 666c 6f77 7461 736b 5f69 6473 6020  rkflowtask_ids` 
 00000bf0: 6861 7320 7265 7065 7469 7469 6f6e 7329  has repetitions)
-00000c00: 04da 0361 6e79 722e 0000 00da 036c 656e  ...anyr......len
-00000c10: da03 7365 7429 0272 2f00 0000 da05 7661  ..set).r/.....va
+00000c00: 04da 0361 6e79 722d 0000 00da 036c 656e  ...anyr-.....len
+00000c10: da03 7365 7429 0272 2e00 0000 da05 7661  ..set).r......va
 00000c20: 6c75 6572 1f00 0000 721f 0000 0072 2000  luer....r....r .
 00000c30: 0000 da19 6368 6563 6b5f 706f 7369 7469  ....check_positi
 00000c40: 7665 5f61 6e64 5f75 6e69 7175 6559 0000  ve_and_uniqueY..
 00000c50: 0073 0a00 0000 1202 0801 1401 0801 0401  .s..............
 00000c60: 7a28 576f 726b 666c 6f77 5570 6461 7465  z(WorkflowUpdate
 00000c70: 2e63 6865 636b 5f70 6f73 6974 6976 655f  .check_positive_
 00000c80: 616e 645f 756e 6971 7565 4e29 0c72 1900  and_uniqueN).r..
 00000c90: 0000 721a 0000 0072 1b00 0000 7203 0000  ..r....r....r...
-00000ca0: 0072 1d00 0000 721e 0000 0072 3600 0000  .r....r....r6...
+00000ca0: 0072 1d00 0000 721e 0000 0072 3500 0000  .r....r....r5...
 00000cb0: 7225 0000 0072 0500 0000 7208 0000 0072  r%...r....r....r
-00000cc0: 3700 0000 7240 0000 0072 1f00 0000 721f  7...r@...r....r.
+00000cc0: 3600 0000 723e 0000 0072 1f00 0000 721f  6...r>...r....r.
 00000cd0: 0000 0072 1f00 0000 7220 0000 0072 0e00  ...r....r ...r..
 00000ce0: 0000 5200 0000 730c 0000 000a 000c 0110  ..R...s.........
 00000cf0: 0114 0306 020e 0172 0e00 0000 6300 0000  .......r....c...
 00000d00: 0000 0000 0000 0000 0000 0000 0004 0000  ................
 00000d10: 0040 0000 0073 2e00 0000 6500 5a01 6400  .@...s....e.Z.d.
 00000d20: 5a02 5500 6503 6504 1900 6505 6401 3c00  Z.U.e.e...e.d.<.
 00000d30: 6506 6402 6403 6404 8d02 6507 6402 8301  e.d.d.d...e.d...
 00000d40: 8301 5a08 6405 5300 2906 720f 0000 0072  ..Z.d.S.).r....r
-00000d50: 3500 0000 7233 0000 0054 7222 0000 004e  5...r3...Tr"...N
+00000d50: 3400 0000 7232 0000 0054 7222 0000 004e  4...r2...Tr"...N
 00000d60: 2909 7219 0000 0072 1a00 0000 721b 0000  ).r....r....r...
-00000d70: 0072 3600 0000 7212 0000 0072 1e00 0000  .r6...r....r....
-00000d80: 7205 0000 0072 0800 0000 7237 0000 0072  r....r....r7...r
+00000d70: 0072 3500 0000 7212 0000 0072 1e00 0000  .r5...r....r....
+00000d80: 7205 0000 0072 0800 0000 7236 0000 0072  r....r....r6...r
 00000d90: 1f00 0000 721f 0000 0072 1f00 0000 7220  ....r....r....r 
 00000da0: 0000 0072 0f00 0000 6200 0000 7306 0000  ...r....b...s...
 00000db0: 000a 000c 0118 0372 0f00 0000 6300 0000  .......r....c...
 00000dc0: 0000 0000 0000 0000 0000 0000 0003 0000  ................
 00000dd0: 0040 0000 0073 1a00 0000 6500 5a01 6400  .@...s....e.Z.d.
 00000de0: 5a02 5500 6503 6504 1900 6505 6401 3c00  Z.U.e.e...e.d.<.
-00000df0: 6402 5300 2903 7210 0000 0072 3500 0000  d.S.).r....r5...
+00000df0: 6402 5300 2903 7210 0000 0072 3400 0000  d.S.).r....r4...
 00000e00: 4e29 0672 1900 0000 721a 0000 0072 1b00  N).r....r....r..
-00000e10: 0000 7236 0000 0072 1300 0000 721e 0000  ..r6...r....r...
+00000e10: 0000 7235 0000 0072 1300 0000 721e 0000  ..r5...r....r...
 00000e20: 0072 1f00 0000 721f 0000 0072 1f00 0000  .r....r....r....
 00000e30: 7220 0000 0072 1000 0000 6900 0000 7304  r ...r....i...s.
 00000e40: 0000 000a 0010 0172 1000 0000 4e29 1ada  .......r....N)..
 00000e50: 0674 7970 696e 6772 0200 0000 7203 0000  .typingr....r...
 00000e60: 00da 0870 7964 616e 7469 6372 0400 0000  ...pydanticr....
 00000e70: 7205 0000 00da 0b5f 7661 6c69 6461 746f  r......_validato
 00000e80: 7273 7207 0000 0072 0800 0000 722a 0000  rsr....r....r*..
 00000e90: 0072 0900 0000 720a 0000 0072 0b00 0000  .r....r....r....
 00000ea0: da07 5f5f 616c 6c5f 5f72 1600 0000 7211  ..__all__r....r.
 00000eb0: 0000 0072 1400 0000 7212 0000 0072 1300  ...r....r....r..
-00000ec0: 0000 7215 0000 0072 3200 0000 720d 0000  ..r....r2...r...
+00000ec0: 0000 7215 0000 0072 3100 0000 720d 0000  ..r....r1...r...
 00000ed0: 0072 0c00 0000 720e 0000 0072 0f00 0000  .r....r....r....
 00000ee0: 7210 0000 0072 1f00 0000 721f 0000 0072  r....r....r....r
 00000ef0: 1f00 0000 7220 0000 00da 083c 6d6f 6475  ....r .....<modu
 00000f00: 6c65 3e01 0000 0073 2c00 0000 0c00 0c01  le>....s,.......
 00000f10: 0c02 0c01 0c02 0c01 0c01 0c01 0c01 0403  ................
 00000f20: 100e 1006 1006 1008 1004 1004 100b 1004  ................
 00000f30: 1006 1005 1010 1407                      ........
```

### Comparing `fractal_server-1.3.0a8/fractal_server/common/schemas/_validators.py` & `fractal_server-1.3.0a9/fractal_server/common/schemas/_validators.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/common/schemas/applyworkflow.py` & `fractal_server-1.3.0a9/fractal_server/common/schemas/applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/common/schemas/manifest.py` & `fractal_server-1.3.0a9/fractal_server/common/schemas/manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/common/schemas/project.py` & `fractal_server-1.3.0a9/fractal_server/common/schemas/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/common/schemas/state.py` & `fractal_server-1.3.0a9/fractal_server/common/schemas/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/common/schemas/task.py` & `fractal_server-1.3.0a9/fractal_server/common/schemas/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/common/schemas/task_collection.py` & `fractal_server-1.3.0a9/fractal_server/common/schemas/task_collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/common/schemas/user.py` & `fractal_server-1.3.0a9/fractal_server/common/schemas/user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/common/schemas/workflow.py` & `fractal_server-1.3.0a9/fractal_server/common/schemas/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a9/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Mar  6 16:04:10 2023 UTC, .py size: 1065 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,100 +1,74 @@
-00000000: 6f0d 0d0a 0000 0000 fa0e 0664 2904 0000  o..........d)...
+00000000: 6f0d 0d0a 0000 0000 5a07 9264 0d02 0000  o.......Z..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6400 6402 6c07 6d08 5a08 0100 6400 6403  d.d.l.m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 0100 6400 6404 6c0b 6d0c  l.m.Z...d.d.l.m.
 00000070: 5a0c 0100 6405 6406 8400 5a0d 6401 5300  Z...d.d...Z.d.S.
 00000080: 2907 e900 0000 004e 2901 da05 6465 6275  )......N)...debu
 00000090: 6729 01da 0f56 616c 6964 6174 696f 6e45  g)...ValidationE
-000000a0: 7272 6f72 2901 da13 4170 706c 7957 6f72  rror)...ApplyWor
-000000b0: 6b66 6c6f 7743 7265 6174 6563 0000 0000  kflowCreatec....
-000000c0: 0000 0000 0000 0000 0a00 0000 0900 0000  ................
-000000d0: 4300 0000 737e 0100 0074 0064 0164 0164  C...s~...t.d.d.d
-000000e0: 0264 0364 0464 058d 057d 0074 0164 1169  .d.d.d...}.t.d.i
-000000f0: 007c 00a4 018e 017d 0174 027c 0183 0101  .|.....}.t.|....
-00000100: 007c 016a 037d 0264 007d 037c 027c 0375  .|.j.}.d.}.|.|.u
-00000110: 007d 047c 0473 5374 04a0 0564 067c 0466  .}.|.sSt...d.|.f
-00000120: 0164 077c 027c 0366 02a1 0464 0874 06a0  .d.|.|.f...d.t..
-00000130: 07a1 0076 0073 3474 04a0 087c 01a1 0172  ...v.s4t...|...r
-00000140: 3974 04a0 097c 01a1 016e 0164 0874 04a0  9t...|...n.d.t..
-00000150: 097c 02a1 0174 04a0 097c 03a1 0164 099c  .|...t...|...d..
-00000160: 0316 007d 0564 0a64 0b7c 0569 0116 007d  ...}.d.d.|.i...}
-00000170: 0674 0a74 04a0 0b7c 06a1 0183 0182 0164  .t.t...|.......d
-00000180: 0004 007d 0204 007d 047d 0364 027c 0064  ...}...}.}.d.|.d
-00000190: 0c3c 0074 0164 1169 007c 00a4 018e 017d  .<.t.d.i.|.....}
-000001a0: 0174 027c 0183 0101 007c 016a 037d 027c  .t.|.....|.j.}.|
-000001b0: 0273 8e64 0d64 0874 06a0 07a1 0076 0073  .s.d.d.t.....v.s
-000001c0: 7974 04a0 087c 01a1 0172 7e74 04a0 097c  yt...|...r~t...|
-000001d0: 01a1 016e 0164 0874 04a0 097c 02a1 0164  ...n.d.t...|...d
-000001e0: 0e9c 0216 007d 0774 0a74 04a0 0b7c 07a1  .....}.t.t...|..
-000001f0: 0183 0182 0164 007d 0264 0f44 005d 2a7d  .....d.}.d.D.]*}
-00000200: 087c 00a0 0ca1 007d 0964 107c 097c 083c  .|.....}.d.|.|.<
-00000210: 0074 027c 0983 0101 0074 0da0 0e74 0fa1  .t.|.....t...t..
-00000220: 018f 0f01 0074 0164 1169 007c 09a4 018e  .....t.d.i.|....
-00000230: 0101 0057 0064 0004 0004 0083 0301 006e  ...W.d.........n
-00000240: 0831 0073 b777 0101 0001 0001 0059 0001  .1.s.w.......Y..
-00000250: 0071 9264 0053 0029 124e e901 0000 00e9  .q.d.S.).N......
-00000260: 0300 0000 547a 0b57 4f52 4b45 5220 494e  ....Tz.WORKER IN
-00000270: 4954 2905 da0a 7072 6f6a 6563 745f 6964  IT)...project_id
-00000280: da10 696e 7075 745f 6461 7461 7365 745f  ..input_dataset_
-00000290: 6964 da0b 776f 726b 666c 6f77 5f69 64da  id..workflow_id.
-000002a0: 0f6f 7665 7277 7269 7465 5f69 6e70 7574  .overwrite_input
-000002b0: da0b 776f 726b 6572 5f69 6e69 7429 01da  ..worker_init)..
-000002c0: 0269 7329 017a 3925 2870 7932 2973 0a7b  .is).z9%(py2)s.{
-000002d0: 2528 7079 3229 7320 3d20 2528 7079 3029  %(py2)s = %(py0)
-000002e0: 732e 6f75 7470 7574 5f64 6174 6173 6574  s.output_dataset
-000002f0: 5f69 640a 7d20 6973 2025 2870 7935 2973  _id.} is %(py5)s
-00000300: da03 6a6f 6229 03da 0370 7930 da03 7079  ..job)...py0..py
-00000310: 32da 0370 7935 7a0e 6173 7365 7274 2025  2..py5z.assert %
-00000320: 2870 7937 2973 da03 7079 37da 116f 7574  (py7)s..py7..out
-00000330: 7075 745f 6461 7461 7365 745f 6964 7a35  put_dataset_idz5
-00000340: 6173 7365 7274 2025 2870 7932 2973 0a7b  assert %(py2)s.{
-00000350: 2528 7079 3229 7320 3d20 2528 7079 3029  %(py2)s = %(py0)
-00000360: 732e 6f75 7470 7574 5f64 6174 6173 6574  s.output_dataset
-00000370: 5f69 640a 7d29 0272 0e00 0000 720f 0000  _id.}).r....r...
-00000380: 0029 0472 0700 0000 7208 0000 0072 1200  .).r....r....r..
-00000390: 0000 7209 0000 00e9 ffff ffff a900 2910  ..r...........).
-000003a0: da04 6469 6374 7204 0000 0072 0200 0000  ..dictr....r....
-000003b0: 7212 0000 00da 0a40 7079 7465 7374 5f61  r......@pytest_a
-000003c0: 72da 115f 6361 6c6c 5f72 6570 7263 6f6d  r.._call_reprcom
-000003d0: 7061 7265 da0c 4070 795f 6275 696c 7469  pare..@py_builti
-000003e0: 6e73 da06 6c6f 6361 6c73 da18 5f73 686f  ns..locals.._sho
-000003f0: 756c 645f 7265 7072 5f67 6c6f 6261 6c5f  uld_repr_global_
-00000400: 6e61 6d65 da09 5f73 6166 6572 6570 72da  name.._saferepr.
-00000410: 0e41 7373 6572 7469 6f6e 4572 726f 72da  .AssertionError.
-00000420: 135f 666f 726d 6174 5f65 7870 6c61 6e61  ._format_explana
-00000430: 7469 6f6e da04 636f 7079 da06 7079 7465  tion..copy..pyte
-00000440: 7374 da06 7261 6973 6573 7203 0000 0029  st..raisesr....)
-00000450: 0ada 0a76 616c 6964 5f61 7267 7372 0d00  ...valid_argsr..
-00000460: 0000 da0b 4070 795f 6173 7365 7274 31da  ....@py_assert1.
-00000470: 0b40 7079 5f61 7373 6572 7434 da0b 4070  .@py_assert4..@p
-00000480: 795f 6173 7365 7274 33da 0b40 7079 5f66  y_assert3..@py_f
-00000490: 6f72 6d61 7436 da0b 4070 795f 666f 726d  ormat6..@py_form
-000004a0: 6174 38da 0b40 7079 5f66 6f72 6d61 7433  at8..@py_format3
-000004b0: da03 6b65 79da 0c69 6e76 616c 6964 5f61  ..key..invalid_a
-000004c0: 7267 7372 1400 0000 7214 0000 00fa 562f  rgsr....r.....V/
-000004d0: 686f 6d65 2f74 6f6d 6d61 736f 2f46 7261  home/tommaso/Fra
-000004e0: 6374 616c 2f66 7261 6374 616c 2d73 6572  ctal/fractal-ser
-000004f0: 7665 722f 6672 6163 7461 6c5f 7365 7276  ver/fractal_serv
-00000500: 6572 2f63 6f6d 6d6f 6e2f 7465 7374 732f  er/common/tests/
-00000510: 7465 7374 5f61 7070 6c79 776f 726b 666c  test_applyworkfl
-00000520: 6f77 2e70 79da 1a74 6573 745f 6170 706c  ow.py..test_appl
-00000530: 795f 776f 726b 666c 6f77 5f63 7265 6174  y_workflow_creat
-00000540: 6508 0000 0073 2e00 0000 0202 0201 0201  e....s..........
-00000550: 0201 0201 0201 06fb 0e07 0801 8a01 0802  ................
-00000560: 0e01 0801 5001 0802 0806 0801 0801 0c01  ....P...........
-00000570: 1001 1cff 0280 04f7 722b 0000 0029 0eda  ........r+...)..
-00000580: 0862 7569 6c74 696e 7372 1800 0000 da19  .builtinsr......
-00000590: 5f70 7974 6573 742e 6173 7365 7274 696f  _pytest.assertio
-000005a0: 6e2e 7265 7772 6974 65da 0961 7373 6572  n.rewrite..asser
-000005b0: 7469 6f6e da07 7265 7772 6974 6572 1600  tion..rewriter..
-000005c0: 0000 721f 0000 00da 0864 6576 746f 6f6c  ..r......devtool
-000005d0: 7372 0200 0000 da17 7079 6461 6e74 6963  sr......pydantic
-000005e0: 2e65 7272 6f72 5f77 7261 7070 6572 7372  .error_wrappersr
-000005f0: 0300 0000 da07 7363 6865 6d61 7372 0400  ......schemasr..
-00000600: 0000 722b 0000 0072 1400 0000 7214 0000  ..r+...r....r...
-00000610: 0072 1400 0000 722a 0000 00da 083c 6d6f  .r....r*.....<mo
-00000620: 6475 6c65 3e01 0000 0073 0a00 0000 2200  dule>....s....".
-00000630: 0c01 0c01 0c02 0c03                      ........
+000000a0: 7272 6f72 2901 da0d 5072 6f6a 6563 7443  rror)...ProjectC
+000000b0: 7265 6174 6563 0000 0000 0000 0000 0000  reatec..........
+000000c0: 0000 0600 0000 0800 0000 4300 0000 7306  ..........C...s.
+000000d0: 0100 0074 0064 0164 028d 017d 0074 017c  ...t.d.d...}.t.|
+000000e0: 0083 0101 0064 037d 0174 0064 047c 019b  .....d.}.t.d.|..
+000000f0: 0064 049d 0364 028d 017d 0074 017c 0083  .d...d...}.t.|..
+00000100: 0101 007c 006a 027d 027c 027c 016b 027d  ...|.j.}.|.|.k.}
+00000110: 037c 0373 6274 03a0 0464 057c 0366 0164  .|.sbt...d.|.f.d
+00000120: 067c 027c 0166 02a1 0464 0774 05a0 06a1  .|.|.f...d.t....
+00000130: 0076 0073 3674 03a0 077c 00a1 0172 3b74  .v.s6t...|...r;t
+00000140: 03a0 087c 00a1 016e 0164 0774 03a0 087c  ...|...n.d.t...|
+00000150: 02a1 0164 0874 05a0 06a1 0076 0073 4b74  ...d.t.....v.sKt
+00000160: 03a0 077c 01a1 0172 5074 03a0 087c 01a1  ...|...rPt...|..
+00000170: 016e 0164 0864 099c 0316 007d 0464 0a64  .n.d.d.....}.d.d
+00000180: 0b7c 0469 0116 007d 0574 0974 03a0 0a7c  .|.i...}.t.t...|
+00000190: 05a1 0183 0182 0164 0004 007d 027d 0374  .......d...}.}.t
+000001a0: 0ba0 0c74 0da1 018f 0e01 0074 0064 0464  ...t.......t.d.d
+000001b0: 028d 0101 0057 0064 0004 0004 0083 0301  .....W.d........
+000001c0: 0064 0053 0031 0073 7c77 0101 0001 0001  .d.S.1.s|w......
+000001d0: 0059 0001 0064 0053 0029 0c4e 7a0a 6d79  .Y...d.S.).Nz.my
+000001e0: 2070 726f 6a65 6374 2901 da04 6e61 6d65   project)...name
+000001f0: 7a11 736f 6d65 2070 726f 6a65 6374 206e  z.some project n
+00000200: 616d 657a 0220 2029 01fa 023d 3d29 017a  amez.  )...==).z
+00000210: 2c25 2870 7932 2973 0a7b 2528 7079 3229  ,%(py2)s.{%(py2)
+00000220: 7320 3d20 2528 7079 3029 732e 6e61 6d65  s = %(py0)s.name
+00000230: 0a7d 203d 3d20 2528 7079 3429 73da 0170  .} == %(py4)s..p
+00000240: da04 4e41 4d45 2903 da03 7079 30da 0370  ..NAME)...py0..p
+00000250: 7932 da03 7079 347a 0e61 7373 6572 7420  y2..py4z.assert 
+00000260: 2528 7079 3629 73da 0370 7936 290e 7204  %(py6)s..py6).r.
+00000270: 0000 0072 0200 0000 7205 0000 00da 0a40  ...r....r......@
+00000280: 7079 7465 7374 5f61 72da 115f 6361 6c6c  pytest_ar.._call
+00000290: 5f72 6570 7263 6f6d 7061 7265 da0c 4070  _reprcompare..@p
+000002a0: 795f 6275 696c 7469 6e73 da06 6c6f 6361  y_builtins..loca
+000002b0: 6c73 da18 5f73 686f 756c 645f 7265 7072  ls.._should_repr
+000002c0: 5f67 6c6f 6261 6c5f 6e61 6d65 da09 5f73  _global_name.._s
+000002d0: 6166 6572 6570 72da 0e41 7373 6572 7469  aferepr..Asserti
+000002e0: 6f6e 4572 726f 72da 135f 666f 726d 6174  onError.._format
+000002f0: 5f65 7870 6c61 6e61 7469 6f6e da06 7079  _explanation..py
+00000300: 7465 7374 da06 7261 6973 6573 7203 0000  test..raisesr...
+00000310: 0029 0672 0700 0000 7208 0000 00da 0b40  .).r....r......@
+00000320: 7079 5f61 7373 6572 7431 da0b 4070 795f  py_assert1..@py_
+00000330: 6173 7365 7274 33da 0b40 7079 5f66 6f72  assert3..@py_for
+00000340: 6d61 7435 da0b 4070 795f 666f 726d 6174  mat5..@py_format
+00000350: 37a9 0072 1b00 0000 fa50 2f68 6f6d 652f  7..r.....P/home/
+00000360: 746f 6d6d 6173 6f2f 4672 6163 7461 6c2f  tommaso/Fractal/
+00000370: 6672 6163 7461 6c2d 7365 7276 6572 2f66  fractal-server/f
+00000380: 7261 6374 616c 5f73 6572 7665 722f 636f  ractal_server/co
+00000390: 6d6d 6f6e 2f74 6573 7473 2f74 6573 745f  mmon/tests/test_
+000003a0: 7072 6f6a 6563 742e 7079 da13 7465 7374  project.py..test
+000003b0: 5f70 726f 6a65 6374 5f63 7265 6174 6508  _project_create.
+000003c0: 0000 0073 1200 0000 0a02 0801 0402 1201  ...s............
+000003d0: 0801 9c01 0c02 0c01 22ff 721d 0000 0029  ........".r....)
+000003e0: 0eda 0862 7569 6c74 696e 7372 0f00 0000  ...builtinsr....
+000003f0: da19 5f70 7974 6573 742e 6173 7365 7274  .._pytest.assert
+00000400: 696f 6e2e 7265 7772 6974 65da 0961 7373  ion.rewrite..ass
+00000410: 6572 7469 6f6e da07 7265 7772 6974 6572  ertion..rewriter
+00000420: 0d00 0000 7215 0000 00da 0864 6576 746f  ....r......devto
+00000430: 6f6c 7372 0200 0000 da17 7079 6461 6e74  olsr......pydant
+00000440: 6963 2e65 7272 6f72 5f77 7261 7070 6572  ic.error_wrapper
+00000450: 7372 0300 0000 da07 7363 6865 6d61 7372  sr......schemasr
+00000460: 0400 0000 721d 0000 0072 1b00 0000 721b  ....r....r....r.
+00000470: 0000 0072 1b00 0000 721c 0000 00da 083c  ...r....r......<
+00000480: 6d6f 6475 6c65 3e01 0000 0073 0a00 0000  module>....s....
+00000490: 2200 0c01 0c01 0c02 0c03                 ".........
```

### Comparing `fractal_server-1.3.0a8/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a9/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue May  9 11:24:30 2023 UTC, .py size: 298 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-00000000: 6f0d 0d0a 0000 0000 6e2d 5a64 2a01 0000  o.......n-Zd*...
+00000000: 6f0d 0d0a 0000 0000 5a07 9264 2a01 0000  o.......Z..d*...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 3e00 0000 6400  .....@...s>...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6400 6403 6c08 6d09 5a09 0100  Z...d.d.l.m.Z...
 00000060: 6404 6405 8400 5a0a 6401 5300 2906 e900  d.d...Z.d.S.)...
 00000070: 0000 004e 2901 da05 6465 6275 6729 01da  ...N)...debug)..
 00000080: 1341 7070 6c79 576f 726b 666c 6f77 4372  .ApplyWorkflowCr
 00000090: 6561 7465 6300 0000 0000 0000 0000 0000  eatec...........
 000000a0: 0002 0000 0004 0000 0043 0000 0073 2600  .........C...s&.
 000000b0: 0000 7400 6401 6402 6403 8d02 7d00 7401  ..t.d.d.d...}.t.
 000000c0: 6404 6900 7c00 a401 8e01 7d01 7402 7c01  d.i.|.....}.t.|.
 000000d0: 8301 0100 6400 5300 2905 4e54 7a0b 574f  ....d.S.).NTz.WO
-000000e0: 524b 4552 2049 4e49 5429 02da 0f6f 7665  RKER INIT)...ove
-000000f0: 7277 7269 7465 5f69 6e70 7574 da0b 776f  rwrite_input..wo
+000000e0: 524b 4552 2049 4e49 5429 025a 0f6f 7665  RKER INIT).Z.ove
+000000f0: 7277 7269 7465 5f69 6e70 7574 5a0b 776f  rwrite_inputZ.wo
 00000100: 726b 6572 5f69 6e69 74a9 0029 03da 0464  rker_init..)...d
-00000110: 6963 7472 0300 0000 7202 0000 0029 02da  ictr....r....)..
-00000120: 0a76 616c 6964 5f61 7267 73da 036a 6f62  .valid_args..job
-00000130: 7206 0000 0072 0600 0000 fa56 2f68 6f6d  r....r.....V/hom
+00000110: 6963 7472 0300 0000 7202 0000 0029 025a  ictr....r....).Z
+00000120: 0a76 616c 6964 5f61 7267 735a 036a 6f62  .valid_argsZ.job
+00000130: 7204 0000 0072 0400 0000 fa56 2f68 6f6d  r....r.....V/hom
 00000140: 652f 746f 6d6d 6173 6f2f 4672 6163 7461  e/tommaso/Fracta
 00000150: 6c2f 6672 6163 7461 6c2d 7365 7276 6572  l/fractal-server
 00000160: 2f66 7261 6374 616c 5f73 6572 7665 722f  /fractal_server/
 00000170: 636f 6d6d 6f6e 2f74 6573 7473 2f74 6573  common/tests/tes
 00000180: 745f 6170 706c 7977 6f72 6b66 6c6f 772e  t_applyworkflow.
 00000190: 7079 da1a 7465 7374 5f61 7070 6c79 5f77  py..test_apply_w
 000001a0: 6f72 6b66 6c6f 775f 6372 6561 7465 0600  orkflow_create..
 000001b0: 0000 730c 0000 0002 0202 0102 0106 fe0e  ..s.............
-000001c0: 040c 0172 0b00 0000 290b da08 6275 696c  ...r....)...buil
+000001c0: 040c 0172 0700 0000 290b da08 6275 696c  ...r....)...buil
 000001d0: 7469 6e73 da0c 4070 795f 6275 696c 7469  tins..@py_builti
 000001e0: 6e73 da19 5f70 7974 6573 742e 6173 7365  ns.._pytest.asse
 000001f0: 7274 696f 6e2e 7265 7772 6974 65da 0961  rtion.rewrite..a
 00000200: 7373 6572 7469 6f6e da07 7265 7772 6974  ssertion..rewrit
-00000210: 65da 0a40 7079 7465 7374 5f61 72da 0864  e..@pytest_ar..d
+00000210: 65da 0a40 7079 7465 7374 5f61 725a 0864  e..@pytest_arZ.d
 00000220: 6576 746f 6f6c 7372 0200 0000 da07 7363  evtoolsr......sc
-00000230: 6865 6d61 7372 0300 0000 720b 0000 0072  hemasr....r....r
-00000240: 0600 0000 7206 0000 0072 0600 0000 720a  ....r....r....r.
+00000230: 6865 6d61 7372 0300 0000 7207 0000 0072  hemasr....r....r
+00000240: 0400 0000 7204 0000 0072 0400 0000 7206  ....r....r....r.
 00000250: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
 00000260: 0073 0600 0000 2600 0c02 0c03            .s....&.....
```

### Comparing `fractal_server-1.3.0a8/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a9/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Mar 15 08:25:43 2023 UTC, .py size: 2144 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0781 1164 6008 0000  o..........d`...
+00000000: 6f0d 0d0a 0000 0000 5a07 9264 6008 0000  o.......Z..d`...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 8600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6400 6402 6c07 6d08 5a08 0100 6400 6403  d.d.l.m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 0100 6400 6404 6c0b 6d0c  l.m.Z...d.d.l.m.
 00000070: 5a0c 0100 6400 6405 6c0b 6d0d 5a0d 0100  Z...d.d.l.m.Z...
@@ -89,19 +89,19 @@
 00000580: da01 6e54 2905 da02 6964 da0a 7072 6f6a  ..nT)...id..proj
 00000590: 6563 745f 6964 da0d 7265 736f 7572 6365  ect_id..resource
 000005a0: 5f6c 6973 7472 0800 0000 721a 0000 007a  _listr....r....z
 000005b0: 0a2f 736f 6d65 7468 696e 6729 0372 2700  ./something).r'.
 000005c0: 0000 da0a 6461 7461 7365 745f 6964 da04  ....dataset_id..
 000005d0: 7061 7468 4629 0372 0500 0000 7202 0000  pathF).r....r...
 000005e0: 0072 0700 0000 2904 720c 0000 00da 0272  .r....).r......r
-000005f0: 31da 0272 32da 0572 6c69 7374 7222 0000  1..r2..rlistr"..
+000005f0: 31da 0272 325a 0572 6c69 7374 7222 0000  1..r2Z.rlistr"..
 00000600: 0072 2200 0000 7223 0000 00da 1174 6573  .r"...r#.....tes
 00000610: 745f 6461 7461 7365 745f 7265 6164 1b00  t_dataset_read..
 00000620: 0000 7316 0000 0002 020a 0106 ff08 030e  ..s.............
-00000630: 020e 0108 0102 010a 0106 ff0c 0372 2f00  .............r/.
+00000630: 020e 0108 0102 010a 0106 ff0c 0372 2e00  .............r..
 00000640: 0000 6300 0000 0000 0000 0000 0000 0009  ..c.............
 00000650: 0000 0009 0000 0043 0000 0073 0204 0000  .......C...s....
 00000660: 7400 6401 6402 8d01 7d00 7401 6410 6900  t.d.d...}.t.d.i.
 00000670: 7c00 a401 8e01 6a00 6403 6404 8d01 7d01  |.....j.d.d...}.
 00000680: 7402 7c01 8301 0100 7c01 6a03 7d02 7c02  t.|.....|.j.}.|.
 00000690: 8300 7d03 7c00 6a03 7d04 7c04 8300 7d05  ..}.|.j.}.|...}.
 000006a0: 7c03 7c05 6b02 7d06 7c06 7373 7404 a005  |.|.k.}.|.sst...
@@ -173,41 +173,41 @@
 00000ac0: 0a7d 203d 3d20 2528 7079 3130 2973 0a7b  .} == %(py10)s.{
 00000ad0: 2528 7079 3130 2973 203d 2025 2870 7938  %(py10)s = %(py8
 00000ae0: 2973 0a7b 2528 7079 3829 7320 3d20 2528  )s.{%(py8)s = %(
 00000af0: 7079 3629 732e 6b65 7973 0a7d 2829 0a7d  py6)s.keys.}().}
 00000b00: da13 6461 7461 7365 745f 7570 6461 7465  ..dataset_update
 00000b10: 5f64 6963 74da 0770 6179 6c6f 6164 2906  _dict..payload).
 00000b20: 720e 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
-00000b30: 1100 0000 da03 7079 38da 0470 7931 307a  ......py8..py10z
+00000b30: 1100 0000 5a03 7079 385a 0470 7931 307a  ....Z.py8Z.py10z
 00000b40: 0f61 7373 6572 7420 2528 7079 3132 2973  .assert %(py12)s
-00000b50: da04 7079 3132 da04 7479 7065 2901 7236  ..py12..type).r6
+00000b50: 5a04 7079 3132 da04 7479 7065 2901 7232  Z.py12..type).r2
 00000b60: 0000 0029 0172 1a00 0000 2902 721a 0000  ...).r....).r...
 00000b70: 0072 0800 0000 7222 0000 0029 0cda 0464  .r....r"...)...d
 00000b80: 6963 7472 0600 0000 7202 0000 00da 046b  ictr....r......k
 00000b90: 6579 7372 1200 0000 7213 0000 0072 1400  eysr....r....r..
 00000ba0: 0000 7215 0000 0072 1600 0000 7217 0000  ..r....r....r...
-00000bb0: 0072 1800 0000 7219 0000 0029 0972 3200  .r....r....).r2.
-00000bc0: 0000 7231 0000 0072 1d00 0000 721e 0000  ..r1...r....r...
-00000bd0: 00da 0b40 7079 5f61 7373 6572 7437 da0b  ...@py_assert7..
-00000be0: 4070 795f 6173 7365 7274 39da 0b40 7079  @py_assert9..@py
-00000bf0: 5f61 7373 6572 7435 da0c 4070 795f 666f  _assert5..@py_fo
-00000c00: 726d 6174 3131 da0c 4070 795f 666f 726d  rmat11..@py_form
+00000bb0: 0072 1800 0000 7219 0000 0029 0972 3100  .r....r....).r1.
+00000bc0: 0000 7230 0000 0072 1d00 0000 721e 0000  ..r0...r....r...
+00000bd0: 005a 0b40 7079 5f61 7373 6572 7437 5a0b  .Z.@py_assert7Z.
+00000be0: 4070 795f 6173 7365 7274 395a 0b40 7079  @py_assert9Z.@py
+00000bf0: 5f61 7373 6572 7435 5a0c 4070 795f 666f  _assert5Z.@py_fo
+00000c00: 726d 6174 3131 5a0c 4070 795f 666f 726d  rmat11Z.@py_form
 00000c10: 6174 3133 7222 0000 0072 2200 0000 7223  at13r"...r"...r#
 00000c20: 0000 00da 1374 6573 745f 6461 7461 7365  .....test_datase
 00000c30: 745f 7570 6461 7465 2b00 0000 7320 0000  t_update+...s ..
 00000c40: 000a 0416 0108 01d2 010a 0216 0108 01d2  ................
 00000c50: 010a 0216 0108 01dc 010c 0216 0108 01e0  ................
-00000c60: 0172 3e00 0000 2913 da08 6275 696c 7469  .r>...)...builti
+00000c60: 0172 3500 0000 2913 da08 6275 696c 7469  .r5...)...builti
 00000c70: 6e73 7214 0000 00da 195f 7079 7465 7374  nsr......_pytest
 00000c80: 2e61 7373 6572 7469 6f6e 2e72 6577 7269  .assertion.rewri
 00000c90: 7465 da09 6173 7365 7274 696f 6eda 0772  te..assertion..r
 00000ca0: 6577 7269 7465 7212 0000 0072 1b00 0000  ewriter....r....
 00000cb0: da08 6465 7674 6f6f 6c73 7202 0000 00da  ..devtoolsr.....
 00000cc0: 1770 7964 616e 7469 632e 6572 726f 725f  .pydantic.error_
 00000cd0: 7772 6170 7065 7273 7203 0000 00da 0773  wrappersr......s
 00000ce0: 6368 656d 6173 7204 0000 0072 0500 0000  chemasr....r....
 00000cf0: 7206 0000 0072 0700 0000 7224 0000 0072  r....r....r$...r
-00000d00: 2f00 0000 723e 0000 0072 2200 0000 7222  /...r>...r"...r"
+00000d00: 2e00 0000 7235 0000 0072 2200 0000 7222  ....r5...r"...r"
 00000d10: 0000 0072 2200 0000 7223 0000 00da 083c  ...r"...r#.....<
 00000d20: 6d6f 6475 6c65 3e01 0000 0073 1400 0000  module>....s....
 00000d30: 2200 0c01 0c01 0c02 0c01 0c01 0c01 0803  "...............
 00000d40: 0810 0c10                                ....
```

### Comparing `fractal_server-1.3.0a8/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a9/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jun 12 09:12:04 2023 UTC, .py size: 1420 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 64e1 8664 8c05 0000  o.......d..d....
+00000000: 6f0d 0d0a 0000 0000 5a07 9264 8c05 0000  o.......Z..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5e00 0000 6400  .....@...s^...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6400 6402 6c07 6d08 5a08 0100 6400 6403  d.d.l.m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 0100 6400 6404 6c0b 6d0c  l.m.Z...d.d.l.m.
 00000070: 5a0c 0100 6400 6405 6c0b 6d0d 5a0d 0100  Z...d.d.l.m.Z...
@@ -31,49 +31,49 @@
 000001e0: 0100 5900 0100 6400 5300 2913 4e7a 0654  ..Y...d.S.).Nz.T
 000001f0: 6173 6b20 41da 0a65 7865 6375 7461 626c  ask A..executabl
 00000200: 65da 0a69 6e70 7574 5f74 7970 65da 0b6f  e..input_type..o
 00000210: 7574 7075 745f 7479 7065 da03 6172 67da  utput_type..arg.
 00000220: 0376 616c 2905 da04 6e61 6d65 7206 0000  .val)...namer...
 00000230: 0072 0700 0000 7208 0000 00da 0c64 6566  .r....r......def
 00000240: 6175 6c74 5f61 7267 737a 0654 6173 6b20  ault_argsz.Task 
-00000250: 42da 0973 6f6d 6574 6869 6e67 da04 656c  B..something..el
+00000250: 425a 0973 6f6d 6574 6869 6e67 da04 656c  BZ.something..el
 00000260: 7365 2906 720b 0000 0072 0600 0000 7207  se).r....r....r.
 00000270: 0000 0072 0800 0000 720c 0000 00da 0b61  ...r....r......a
 00000280: 7267 735f 7363 6865 6d61 da01 3129 02da  rgs_schema..1)..
 00000290: 106d 616e 6966 6573 745f 7665 7273 696f  .manifest_versio
 000002a0: 6eda 0974 6173 6b5f 6c69 7374 4629 0372  n..task_listF).r
-000002b0: 1100 0000 da10 6861 735f 6172 6773 5f73  ......has_args_s
-000002c0: 6368 656d 6173 7212 0000 0054 2903 7211  chemasr....T).r.
-000002d0: 0000 0072 1200 0000 7213 0000 00da 0132  ...r....r......2
+000002b0: 1000 0000 da10 6861 735f 6172 6773 5f73  ......has_args_s
+000002c0: 6368 656d 6173 7211 0000 0054 2903 7210  chemasr....T).r.
+000002d0: 0000 0072 1100 0000 7212 0000 00da 0132  ...r....r......2
 000002e0: 2907 7205 0000 0072 0400 0000 7202 0000  ).r....r....r...
 000002f0: 00da 0670 7974 6573 74da 0672 6169 7365  ...pytest..raise
-00000300: 7372 0300 0000 da05 7661 6c75 6529 04da  sr......value)..
+00000300: 7372 0300 0000 da05 7661 6c75 6529 045a  sr......value).Z
 00000310: 1874 6173 6b5f 7769 7468 6f75 745f 6172  .task_without_ar
-00000320: 6773 5f73 6368 656d 61da 1574 6173 6b5f  gs_schema..task_
+00000320: 6773 5f73 6368 656d 615a 1574 6173 6b5f  gs_schemaZ.task_
 00000330: 7769 7468 5f61 7267 735f 7363 6865 6d61  with_args_schema
-00000340: da01 6dda 0165 a900 721c 0000 00fa 512f  ..m..e..r.....Q/
+00000340: da01 6dda 0165 a900 7219 0000 00fa 512f  ..m..e..r.....Q/
 00000350: 686f 6d65 2f74 6f6d 6d61 736f 2f46 7261  home/tommaso/Fra
 00000360: 6374 616c 2f66 7261 6374 616c 2d73 6572  ctal/fractal-ser
 00000370: 7665 722f 6672 6163 7461 6c5f 7365 7276  ver/fractal_serv
 00000380: 6572 2f63 6f6d 6d6f 6e2f 7465 7374 732f  er/common/tests/
 00000390: 7465 7374 5f6d 616e 6966 6573 742e 7079  test_manifest.py
 000003a0: da0f 7465 7374 5f4d 616e 6966 6573 7456  ..test_ManifestV
 000003b0: 3109 0000 0073 5600 0000 0202 0201 0201  1....sV.........
 000003c0: 0201 0201 0601 06fb 0207 0201 0201 0201  ................
 000003d0: 0201 0601 0601 06fa 0209 0201 0401 06fe  ................
 000003e0: 0804 0201 0201 0201 0401 06fd 0805 0201  ................
 000003f0: 0201 0201 0401 06fd 0805 0c02 0201 0201  ................
 00000400: 0601 0201 08fd 1cff 0a06 0c02 1001 22ff  ..............".
-00000410: 721e 0000 0029 0fda 0862 7569 6c74 696e  r....)...builtin
+00000410: 721b 0000 0029 0fda 0862 7569 6c74 696e  r....)...builtin
 00000420: 73da 0c40 7079 5f62 7569 6c74 696e 73da  s..@py_builtins.
 00000430: 195f 7079 7465 7374 2e61 7373 6572 7469  ._pytest.asserti
 00000440: 6f6e 2e72 6577 7269 7465 da09 6173 7365  on.rewrite..asse
 00000450: 7274 696f 6eda 0772 6577 7269 7465 da0a  rtion..rewrite..
-00000460: 4070 7974 6573 745f 6172 7215 0000 00da  @pytest_arr.....
+00000460: 4070 7974 6573 745f 6172 7214 0000 00da  @pytest_arr.....
 00000470: 0864 6576 746f 6f6c 7372 0200 0000 da17  .devtoolsr......
 00000480: 7079 6461 6e74 6963 2e65 7272 6f72 5f77  pydantic.error_w
 00000490: 7261 7070 6572 7372 0300 0000 da07 7363  rappersr......sc
 000004a0: 6865 6d61 7372 0400 0000 7205 0000 0072  hemasr....r....r
-000004b0: 1e00 0000 721c 0000 0072 1c00 0000 721c  ....r....r....r.
-000004c0: 0000 0072 1d00 0000 da08 3c6d 6f64 756c  ...r......<modul
+000004b0: 1b00 0000 7219 0000 0072 1900 0000 7219  ....r....r....r.
+000004c0: 0000 0072 1a00 0000 da08 3c6d 6f64 756c  ...r......<modul
 000004d0: 653e 0100 0000 730c 0000 0022 000c 010c  e>....s...."....
 000004e0: 010c 020c 010c 03                        .......
```

### Comparing `fractal_server-1.3.0a8/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a9/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr  6 08:31:17 2023 UTC, .py size: 525 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,74 +1,112 @@
-00000000: 6f0d 0d0a 0000 0000 5583 2e64 0d02 0000  o.......U..d....
+00000000: 6f0d 0d0a 0000 0000 5a07 9264 2702 0000  o.......Z..d'...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
+00000020: 0002 0000 0040 0000 0073 5e00 0000 6400  .....@...s^...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
-00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
-00000050: 6400 6402 6c07 6d08 5a08 0100 6400 6403  d.d.l.m.Z...d.d.
-00000060: 6c09 6d0a 5a0a 0100 6400 6404 6c0b 6d0c  l.m.Z...d.d.l.m.
-00000070: 5a0c 0100 6405 6406 8400 5a0d 6401 5300  Z...d.d...Z.d.S.
-00000080: 2907 e900 0000 004e 2901 da05 6465 6275  )......N)...debu
-00000090: 6729 01da 0f56 616c 6964 6174 696f 6e45  g)...ValidationE
-000000a0: 7272 6f72 2901 da0d 5072 6f6a 6563 7443  rror)...ProjectC
-000000b0: 7265 6174 6563 0000 0000 0000 0000 0000  reatec..........
-000000c0: 0000 0600 0000 0800 0000 4300 0000 7306  ..........C...s.
-000000d0: 0100 0074 0064 0164 028d 017d 0074 017c  ...t.d.d...}.t.|
-000000e0: 0083 0101 0064 037d 0174 0064 047c 019b  .....d.}.t.d.|..
-000000f0: 0064 049d 0364 028d 017d 0074 017c 0083  .d...d...}.t.|..
-00000100: 0101 007c 006a 027d 027c 027c 016b 027d  ...|.j.}.|.|.k.}
-00000110: 037c 0373 6274 03a0 0464 057c 0366 0164  .|.sbt...d.|.f.d
-00000120: 067c 027c 0166 02a1 0464 0774 05a0 06a1  .|.|.f...d.t....
-00000130: 0076 0073 3674 03a0 077c 00a1 0172 3b74  .v.s6t...|...r;t
-00000140: 03a0 087c 00a1 016e 0164 0774 03a0 087c  ...|...n.d.t...|
-00000150: 02a1 0164 0874 05a0 06a1 0076 0073 4b74  ...d.t.....v.sKt
-00000160: 03a0 077c 01a1 0172 5074 03a0 087c 01a1  ...|...rPt...|..
-00000170: 016e 0164 0864 099c 0316 007d 0464 0a64  .n.d.d.....}.d.d
-00000180: 0b7c 0469 0116 007d 0574 0974 03a0 0a7c  .|.i...}.t.t...|
-00000190: 05a1 0183 0182 0164 0004 007d 027d 0374  .......d...}.}.t
-000001a0: 0ba0 0c74 0da1 018f 0e01 0074 0064 0464  ...t.......t.d.d
-000001b0: 028d 0101 0057 0064 0004 0004 0083 0301  .....W.d........
-000001c0: 0064 0053 0031 0073 7c77 0101 0001 0001  .d.S.1.s|w......
-000001d0: 0059 0001 0064 0053 0029 0c4e 7a0a 6d79  .Y...d.S.).Nz.my
-000001e0: 2070 726f 6a65 6374 2901 da04 6e61 6d65   project)...name
-000001f0: 7a11 736f 6d65 2070 726f 6a65 6374 206e  z.some project n
-00000200: 616d 657a 0220 2029 01fa 023d 3d29 017a  amez.  )...==).z
-00000210: 2c25 2870 7932 2973 0a7b 2528 7079 3229  ,%(py2)s.{%(py2)
-00000220: 7320 3d20 2528 7079 3029 732e 6e61 6d65  s = %(py0)s.name
-00000230: 0a7d 203d 3d20 2528 7079 3429 73da 0170  .} == %(py4)s..p
-00000240: da04 4e41 4d45 2903 da03 7079 30da 0370  ..NAME)...py0..p
-00000250: 7932 da03 7079 347a 0e61 7373 6572 7420  y2..py4z.assert 
-00000260: 2528 7079 3629 73da 0370 7936 290e 7204  %(py6)s..py6).r.
-00000270: 0000 0072 0200 0000 7205 0000 00da 0a40  ...r....r......@
-00000280: 7079 7465 7374 5f61 72da 115f 6361 6c6c  pytest_ar.._call
-00000290: 5f72 6570 7263 6f6d 7061 7265 da0c 4070  _reprcompare..@p
-000002a0: 795f 6275 696c 7469 6e73 da06 6c6f 6361  y_builtins..loca
-000002b0: 6c73 da18 5f73 686f 756c 645f 7265 7072  ls.._should_repr
-000002c0: 5f67 6c6f 6261 6c5f 6e61 6d65 da09 5f73  _global_name.._s
-000002d0: 6166 6572 6570 72da 0e41 7373 6572 7469  aferepr..Asserti
-000002e0: 6f6e 4572 726f 72da 135f 666f 726d 6174  onError.._format
-000002f0: 5f65 7870 6c61 6e61 7469 6f6e da06 7079  _explanation..py
-00000300: 7465 7374 da06 7261 6973 6573 7203 0000  test..raisesr...
-00000310: 0029 0672 0700 0000 7208 0000 00da 0b40  .).r....r......@
-00000320: 7079 5f61 7373 6572 7431 da0b 4070 795f  py_assert1..@py_
-00000330: 6173 7365 7274 33da 0b40 7079 5f66 6f72  assert3..@py_for
-00000340: 6d61 7435 da0b 4070 795f 666f 726d 6174  mat5..@py_format
-00000350: 37a9 0072 1b00 0000 fa50 2f68 6f6d 652f  7..r.....P/home/
-00000360: 746f 6d6d 6173 6f2f 4672 6163 7461 6c2f  tommaso/Fractal/
-00000370: 6672 6163 7461 6c2d 7365 7276 6572 2f66  fractal-server/f
-00000380: 7261 6374 616c 5f73 6572 7665 722f 636f  ractal_server/co
-00000390: 6d6d 6f6e 2f74 6573 7473 2f74 6573 745f  mmon/tests/test_
-000003a0: 7072 6f6a 6563 742e 7079 da13 7465 7374  project.py..test
-000003b0: 5f70 726f 6a65 6374 5f63 7265 6174 6508  _project_create.
-000003c0: 0000 0073 1200 0000 0a02 0801 0402 1201  ...s............
-000003d0: 0801 9c01 0c02 0c01 22ff 721d 0000 0029  ........".r....)
-000003e0: 0eda 0862 7569 6c74 696e 7372 0f00 0000  ...builtinsr....
-000003f0: da19 5f70 7974 6573 742e 6173 7365 7274  .._pytest.assert
-00000400: 696f 6e2e 7265 7772 6974 65da 0961 7373  ion.rewrite..ass
-00000410: 6572 7469 6f6e da07 7265 7772 6974 6572  ertion..rewriter
-00000420: 0d00 0000 7215 0000 00da 0864 6576 746f  ....r......devto
-00000430: 6f6c 7372 0200 0000 da17 7079 6461 6e74  olsr......pydant
-00000440: 6963 2e65 7272 6f72 5f77 7261 7070 6572  ic.error_wrapper
-00000450: 7372 0300 0000 da07 7363 6865 6d61 7372  sr......schemasr
-00000460: 0400 0000 721d 0000 0072 1b00 0000 721b  ....r....r....r.
-00000470: 0000 0072 1b00 0000 721c 0000 00da 083c  ...r....r......<
-00000480: 6d6f 6475 6c65 3e01 0000 0073 0a00 0000  module>....s....
-00000490: 2200 0c01 0c01 0c02 0c03                 ".........
+00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d06  ..m.Z...d.d.l.m.
+00000050: 5a06 0100 6400 6403 6c07 6d08 5a08 0100  Z...d.d.l.m.Z...
+00000060: 6400 6404 6c09 6d0a 5a0a 0100 6400 6405  d.d.l.m.Z...d.d.
+00000070: 6c09 6d0b 5a0b 0100 6406 6407 8400 5a0c  l.m.Z...d.d...Z.
+00000080: 6408 6409 8400 5a0d 6401 5300 290a e900  d.d...Z.d.S.)...
+00000090: 0000 004e 2901 da08 6461 7465 7469 6d65  ...N)...datetime
+000000a0: 2901 da05 6465 6275 6729 01da 0a5f 5374  )...debug)..._St
+000000b0: 6174 6542 6173 6529 01da 0953 7461 7465  ateBase)...State
+000000c0: 5265 6164 6300 0000 0000 0000 0000 0000  Readc...........
+000000d0: 0004 0000 0007 0000 0043 0000 0073 ba00  .........C...s..
+000000e0: 0000 7400 6401 6402 6901 7401 a002 a100  ..t.d.d.i.t.....
+000000f0: 6403 8d02 7d00 7403 7c00 8301 0100 7403  d...}.t.|.....t.
+00000100: 7c00 a004 a100 8301 0100 7c00 a004 a100  |.........|.....
+00000110: 6404 1900 7d01 7405 7c01 7406 8302 7d02  d...}.t.|.t...}.
+00000120: 7c02 7357 6405 6406 7407 a008 a100 7600  |.sWd.d.t.....v.
+00000130: 732d 7409 a00a 7405 a101 7232 7409 a00b  s-t...t...r2t...
+00000140: 7405 a101 6e01 6406 7409 a00b 7c01 a101  t...n.d.t...|...
+00000150: 6407 7407 a008 a100 7600 7342 7409 a00a  d.t.....v.sBt...
+00000160: 7406 a101 7247 7409 a00b 7406 a101 6e01  t...rGt...t...n.
+00000170: 6407 7409 a00b 7c02 a101 6408 9c04 1600  d.t...|...d.....
+00000180: 7d03 740c 7409 a00d 7c03 a101 8301 8201  }.t.t...|.......
+00000190: 6400 0400 7d01 7d02 6400 5300 2909 4eda  d...}.}.d.S.).N.
+000001a0: 0473 6f6d 65da 0574 6869 6e67 a902 da04  .some..thing....
+000001b0: 6461 7461 da09 7469 6d65 7374 616d 7072  data..timestampr
+000001c0: 0a00 0000 7a35 6173 7365 7274 2025 2870  ....z5assert %(p
+000001d0: 7935 2973 0a7b 2528 7079 3529 7320 3d20  y5)s.{%(py5)s = 
+000001e0: 2528 7079 3029 7328 2528 7079 3229 732c  %(py0)s(%(py2)s,
+000001f0: 2025 2870 7933 2973 290a 7dda 0a69 7369   %(py3)s).}..isi
+00000200: 6e73 7461 6e63 65da 0373 7472 2904 da03  nstance..str)...
+00000210: 7079 30da 0370 7932 da03 7079 33da 0370  py0..py2..py3..p
+00000220: 7935 290e 7204 0000 0072 0200 0000 da03  y5).r....r......
+00000230: 6e6f 7772 0300 0000 da0e 7361 6e69 7469  nowr......saniti
+00000240: 7365 645f 6469 6374 720b 0000 0072 0c00  sed_dictr....r..
+00000250: 0000 da0c 4070 795f 6275 696c 7469 6e73  ....@py_builtins
+00000260: da06 6c6f 6361 6c73 da0a 4070 7974 6573  ..locals..@pytes
+00000270: 745f 6172 da18 5f73 686f 756c 645f 7265  t_ar.._should_re
+00000280: 7072 5f67 6c6f 6261 6c5f 6e61 6d65 da09  pr_global_name..
+00000290: 5f73 6166 6572 6570 72da 0e41 7373 6572  _saferepr..Asser
+000002a0: 7469 6f6e 4572 726f 72da 135f 666f 726d  tionError.._form
+000002b0: 6174 5f65 7870 6c61 6e61 7469 6f6e 2904  at_explanation).
+000002c0: da01 73da 0b40 7079 5f61 7373 6572 7431  ..s..@py_assert1
+000002d0: da0b 4070 795f 6173 7365 7274 34da 0b40  ..@py_assert4..@
+000002e0: 7079 5f66 6f72 6d61 7436 a900 721e 0000  py_format6..r...
+000002f0: 00fa 4e2f 686f 6d65 2f74 6f6d 6d61 736f  ..N/home/tommaso
+00000300: 2f46 7261 6374 616c 2f66 7261 6374 616c  /Fractal/fractal
+00000310: 2d73 6572 7665 722f 6672 6163 7461 6c5f  -server/fractal_
+00000320: 7365 7276 6572 2f63 6f6d 6d6f 6e2f 7465  server/common/te
+00000330: 7374 732f 7465 7374 5f73 7461 7465 2e70  sts/test_state.p
+00000340: 79da 0a74 6573 745f 7374 6174 6509 0000  y..test_state...
+00000350: 0073 0800 0000 1401 0801 0c01 9201 7220  .s............r 
+00000360: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00000370: 0600 0000 0700 0000 4300 0000 7352 0100  ........C...sR..
+00000380: 0074 0064 0164 0269 0174 01a0 02a1 0064  .t.d.d.i.t.....d
+00000390: 038d 027d 0074 037c 0083 0101 007c 006a  ...}.t.|.....|.j
+000003a0: 047d 0164 007d 027c 017c 0275 007d 037c  .}.d.}.|.|.u.}.|
+000003b0: 0373 4d74 05a0 0664 047c 0366 0164 057c  .sMt...d.|.f.d.|
+000003c0: 017c 0266 02a1 0464 0674 07a0 08a1 0076  .|.f...d.t.....v
+000003d0: 0073 2e74 05a0 097c 00a1 0172 3374 05a0  .s.t...|...r3t..
+000003e0: 0a7c 00a1 016e 0164 0674 05a0 0a7c 01a1  .|...n.d.t...|..
+000003f0: 0174 05a0 0a7c 02a1 0164 079c 0316 007d  .t...|...d.....}
+00000400: 0464 0864 097c 0469 0116 007d 0574 0b74  .d.d.|.i...}.t.t
+00000410: 05a0 0c7c 05a1 0183 0182 0164 0004 007d  ...|.......d...}
+00000420: 0104 007d 037d 0274 0064 0164 0269 0174  ...}.}.t.d.d.i.t
+00000430: 01a0 02a1 0064 0a64 0b8d 037d 0074 037c  .....d.d...}.t.|
+00000440: 0083 0101 007c 006a 047d 0164 0a7d 027c  .....|.j.}.d.}.|
+00000450: 017c 026b 027d 037c 0373 a174 05a0 0664  .|.k.}.|.s.t...d
+00000460: 0c7c 0366 0164 0d7c 017c 0266 02a1 0464  .|.f.d.|.|.f...d
+00000470: 0674 07a0 08a1 0076 0073 8274 05a0 097c  .t.....v.s.t...|
+00000480: 00a1 0172 8774 05a0 0a7c 00a1 016e 0164  ...r.t...|...n.d
+00000490: 0674 05a0 0a7c 01a1 0174 05a0 0a7c 02a1  .t...|...t...|..
+000004a0: 0164 079c 0316 007d 0464 0864 097c 0469  .d.....}.d.d.|.i
+000004b0: 0116 007d 0574 0b74 05a0 0c7c 05a1 0183  ...}.t.t...|....
+000004c0: 0182 0164 0004 007d 0104 007d 037d 0264  ...d...}...}.}.d
+000004d0: 0053 0029 0e4e 7206 0000 0072 0700 0000  .S.).Nr....r....
+000004e0: 7208 0000 0029 01da 0269 7329 017a 2a25  r....)...is).z*%
+000004f0: 2870 7932 2973 0a7b 2528 7079 3229 7320  (py2)s.{%(py2)s 
+00000500: 3d20 2528 7079 3029 732e 6964 0a7d 2069  = %(py0)s.id.} i
+00000510: 7320 2528 7079 3529 7372 1a00 0000 2903  s %(py5)sr....).
+00000520: 720d 0000 0072 0e00 0000 7210 0000 007a  r....r....r....z
+00000530: 0e61 7373 6572 7420 2528 7079 3729 73da  .assert %(py7)s.
+00000540: 0370 7937 e901 0000 0029 0372 0900 0000  .py7.....).r....
+00000550: 720a 0000 00da 0269 6429 01fa 023d 3d29  r......id)...==)
+00000560: 017a 2a25 2870 7932 2973 0a7b 2528 7079  .z*%(py2)s.{%(py
+00000570: 3229 7320 3d20 2528 7079 3029 732e 6964  2)s = %(py0)s.id
+00000580: 0a7d 203d 3d20 2528 7079 3529 7329 0d72  .} == %(py5)s).r
+00000590: 0500 0000 7202 0000 0072 1100 0000 7203  ....r....r....r.
+000005a0: 0000 0072 2400 0000 7215 0000 00da 115f  ...r$...r......_
+000005b0: 6361 6c6c 5f72 6570 7263 6f6d 7061 7265  call_reprcompare
+000005c0: 7213 0000 0072 1400 0000 7216 0000 0072  r....r....r....r
+000005d0: 1700 0000 7218 0000 0072 1900 0000 2906  ....r....r....).
+000005e0: 721a 0000 0072 1b00 0000 721c 0000 00da  r....r....r.....
+000005f0: 0b40 7079 5f61 7373 6572 7433 721d 0000  .@py_assert3r...
+00000600: 00da 0b40 7079 5f66 6f72 6d61 7438 721e  ...@py_format8r.
+00000610: 0000 0072 1e00 0000 721f 0000 00da 0f74  ...r....r......t
+00000620: 6573 745f 7374 6174 655f 7265 6164 1000  est_state_read..
+00000630: 0000 730c 0000 0014 0108 018a 0116 0208  ..s.............
+00000640: 018e 0172 2900 0000 290e da08 6275 696c  ...r)...)...buil
+00000650: 7469 6e73 7213 0000 00da 195f 7079 7465  tinsr......_pyte
+00000660: 7374 2e61 7373 6572 7469 6f6e 2e72 6577  st.assertion.rew
+00000670: 7269 7465 da09 6173 7365 7274 696f 6eda  rite..assertion.
+00000680: 0772 6577 7269 7465 7215 0000 0072 0200  .rewriter....r..
+00000690: 0000 da08 6465 7674 6f6f 6c73 7203 0000  ....devtoolsr...
+000006a0: 00da 0773 6368 656d 6173 7204 0000 0072  ...schemasr....r
+000006b0: 0500 0000 7220 0000 0072 2900 0000 721e  ....r ...r)...r.
+000006c0: 0000 0072 1e00 0000 721e 0000 0072 1f00  ...r....r....r..
+000006d0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+000006e0: 730c 0000 0026 000c 020c 020c 0108 030c  s....&..........
+000006f0: 07                                       .
```

### Comparing `fractal_server-1.3.0a8/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a9/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Mar  6 16:04:10 2023 UTC, .py size: 748 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-00000000: 6f0d 0d0a 0000 0000 fa0e 0664 ec02 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 5a07 9264 a604 0000  o.......Z..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6400 6402 6c07 6d08 5a08 0100 6400 6403  d.d.l.m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 0100 6400 6404 6c0b 6d0c  l.m.Z...d.d.l.m.
 00000070: 5a0c 0100 6400 6405 6c0b 6d0d 5a0d 0100  Z...d.d.l.m.Z...
 00000080: 6406 6407 8400 5a0e 6408 6409 8400 5a0f  d.d...Z.d.d...Z.
 00000090: 6401 5300 290a e900 0000 004e 2901 da05  d.S.)......N)...
 000000a0: 6465 6275 6729 01da 0f56 616c 6964 6174  debug)...Validat
 000000b0: 696f 6e45 7272 6f72 2901 da0a 5461 736b  ionError)...Task
 000000c0: 4372 6561 7465 2901 da0a 5461 736b 5570  Create)...TaskUp
 000000d0: 6461 7465 6300 0000 0000 0000 0000 0000  datec...........
-000000e0: 000b 0000 000c 0000 0043 0000 0073 3002  .........C...s0.
+000000e0: 000d 0000 000c 0000 0043 0000 0073 6203  .........C...sb.
 000000f0: 0000 7400 6401 6402 8d01 7d00 7401 7c00  ..t.d.d...}.t.|.
 00000100: 8301 0100 7c00 6a02 7d01 6403 7d02 7c01  ....|.j.}.d.}.|.
 00000110: 7c02 6404 8d01 7d03 7c03 6a03 7d04 7c04  |.d...}.|.j.}.|.
 00000120: 8300 7d05 7404 7c05 8301 7d06 6401 6701  ..}.t.|...}.d.g.
 00000130: 7d07 7c06 7c07 6b02 7d08 7c08 737f 7405  }.|.|.k.}.|.s.t.
 00000140: a006 6405 7c08 6601 6406 7c06 7c07 6602  ..d.|.f.d.|.|.f.
 00000150: a104 6407 7407 a008 a100 7600 733b 7405  ..d.t.....v.s;t.
@@ -43,98 +43,134 @@
 000002a0: 6e01 6408 7405 a00a 7c01 a101 7405 a00a  n.d.t...|...t...
 000002b0: 7c02 a101 7405 a00a 7c03 a101 7405 a00a  |...t...|...t...
 000002c0: 7c04 a101 7405 a00a 7c05 a101 7405 a00a  |...t...|...t...
 000002d0: 7c06 a101 7405 a00a 7c07 a101 6409 9c09  |...t...|...d...
 000002e0: 1600 7d09 640a 640b 7c09 6901 1600 7d0a  ..}.d.d.|.i...}.
 000002f0: 740b 7405 a00c 7c0a a101 8301 8201 6400  t.t...|.......d.
 00000300: 0400 7d01 0400 7d02 0400 7d03 0400 7d04  ..}...}...}...}.
-00000310: 0400 7d05 0400 7d06 0400 7d08 7d07 6400  ..}...}...}.}.d.
-00000320: 5300 290e 4eda 046e 616d 6529 0172 0600  S.).N..name).r..
-00000330: 0000 5429 01da 0c65 7863 6c75 6465 5f6e  ..T)...exclude_n
-00000340: 6f6e 6529 01fa 023d 3d29 017a ab25 2870  one)...==).z.%(p
-00000350: 7931 3329 730a 7b25 2870 7931 3329 7320  y13)s.{%(py13)s 
-00000360: 3d20 2528 7079 3029 7328 2528 7079 3131  = %(py0)s(%(py11
-00000370: 2973 0a7b 2528 7079 3131 2973 203d 2025  )s.{%(py11)s = %
-00000380: 2870 7939 2973 0a7b 2528 7079 3929 7320  (py9)s.{%(py9)s 
-00000390: 3d20 2528 7079 3729 730a 7b25 2870 7937  = %(py7)s.{%(py7
-000003a0: 2973 203d 2025 2870 7933 2973 0a7b 2528  )s = %(py3)s.{%(
-000003b0: 7079 3329 7320 3d20 2528 7079 3129 732e  py3)s = %(py1)s.
-000003c0: 6469 6374 0a7d 2865 7863 6c75 6465 5f6e  dict.}(exclude_n
-000003d0: 6f6e 653d 2528 7079 3529 7329 0a7d 2e6b  one=%(py5)s).}.k
-000003e0: 6579 730a 7d28 290a 7d29 0a7d 203d 3d20  eys.}().}).} == 
-000003f0: 2528 7079 3136 2973 da04 6c69 7374 da01  %(py16)s..list..
-00000400: 7429 09da 0370 7930 da03 7079 31da 0370  t)...py0..py1..p
-00000410: 7933 da03 7079 35da 0370 7937 da03 7079  y3..py5..py7..py
-00000420: 39da 0470 7931 31da 0470 7931 33da 0470  9..py11..py13..p
-00000430: 7931 367a 0f61 7373 6572 7420 2528 7079  y16z.assert %(py
-00000440: 3138 2973 da04 7079 3138 2901 da0d 6578  18)s..py18)...ex
-00000450: 636c 7564 655f 756e 7365 7429 017a ac25  clude_unset).z.%
-00000460: 2870 7931 3329 730a 7b25 2870 7931 3329  (py13)s.{%(py13)
-00000470: 7320 3d20 2528 7079 3029 7328 2528 7079  s = %(py0)s(%(py
-00000480: 3131 2973 0a7b 2528 7079 3131 2973 203d  11)s.{%(py11)s =
-00000490: 2025 2870 7939 2973 0a7b 2528 7079 3929   %(py9)s.{%(py9)
-000004a0: 7320 3d20 2528 7079 3729 730a 7b25 2870  s = %(py7)s.{%(p
-000004b0: 7937 2973 203d 2025 2870 7933 2973 0a7b  y7)s = %(py3)s.{
-000004c0: 2528 7079 3329 7320 3d20 2528 7079 3129  %(py3)s = %(py1)
-000004d0: 732e 6469 6374 0a7d 2865 7863 6c75 6465  s.dict.}(exclude
-000004e0: 5f75 6e73 6574 3d25 2870 7935 2973 290a  _unset=%(py5)s).
-000004f0: 7d2e 6b65 7973 0a7d 2829 0a7d 290a 7d20  }.keys.}().}).} 
-00000500: 3d3d 2025 2870 7931 3629 7329 0d72 0500  == %(py16)s).r..
-00000510: 0000 7202 0000 00da 0464 6963 74da 046b  ..r......dict..k
-00000520: 6579 7372 0900 0000 da0a 4070 7974 6573  eysr......@pytes
-00000530: 745f 6172 da11 5f63 616c 6c5f 7265 7072  t_ar.._call_repr
-00000540: 636f 6d70 6172 65da 0c40 7079 5f62 7569  compare..@py_bui
-00000550: 6c74 696e 73da 066c 6f63 616c 73da 185f  ltins..locals.._
-00000560: 7368 6f75 6c64 5f72 6570 725f 676c 6f62  should_repr_glob
-00000570: 616c 5f6e 616d 65da 095f 7361 6665 7265  al_name.._safere
-00000580: 7072 da0e 4173 7365 7274 696f 6e45 7272  pr..AssertionErr
-00000590: 6f72 da13 5f66 6f72 6d61 745f 6578 706c  or.._format_expl
-000005a0: 616e 6174 696f 6e29 0b72 0a00 0000 da0b  anation).r......
-000005b0: 4070 795f 6173 7365 7274 32da 0b40 7079  @py_assert2..@py
-000005c0: 5f61 7373 6572 7434 da0b 4070 795f 6173  _assert4..@py_as
-000005d0: 7365 7274 36da 0b40 7079 5f61 7373 6572  sert6..@py_asser
-000005e0: 7438 da0c 4070 795f 6173 7365 7274 3130  t8..@py_assert10
-000005f0: da0c 4070 795f 6173 7365 7274 3132 da0c  ..@py_assert12..
-00000600: 4070 795f 6173 7365 7274 3135 da0c 4070  @py_assert15..@p
-00000610: 795f 6173 7365 7274 3134 da0c 4070 795f  y_assert14..@py_
-00000620: 666f 726d 6174 3137 da0c 4070 795f 666f  format17..@py_fo
-00000630: 726d 6174 3139 a900 722a 0000 00fa 4d2f  rmat19..r*....M/
-00000640: 686f 6d65 2f74 6f6d 6d61 736f 2f46 7261  home/tommaso/Fra
-00000650: 6374 616c 2f66 7261 6374 616c 2d73 6572  ctal/fractal-ser
-00000660: 7665 722f 6672 6163 7461 6c5f 7365 7276  ver/fractal_serv
-00000670: 6572 2f63 6f6d 6d6f 6e2f 7465 7374 732f  er/common/tests/
-00000680: 7465 7374 5f74 6173 6b2e 7079 da10 7465  test_task.py..te
-00000690: 7374 5f74 6173 6b5f 7570 6461 7465 0900  st_task_update..
-000006a0: 0000 730c 0000 000a 0208 01fe 010e 00fe  ..s.............
-000006b0: 0114 0072 2c00 0000 6300 0000 0000 0000  ...r,...c.......
-000006c0: 0000 0000 0001 0000 0008 0000 0043 0000  .............C..
-000006d0: 0073 5600 0000 7400 6401 6402 6403 6404  .sV...t.d.d.d.d.
-000006e0: 6405 6406 8d05 7d00 7401 7c00 8301 0100  d.d...}.t.|.....
-000006f0: 7402 a003 7404 a101 8f0f 0100 7400 6401  t...t.......t.d.
-00000700: 6402 6407 8d02 0100 5700 6400 0400 0400  d.d.....W.d.....
-00000710: 8303 0100 6400 5300 3100 7324 7701 0100  ....d.S.1.s$w...
-00000720: 0100 0100 5900 0100 6400 5300 2908 4eda  ....Y...d.S.).N.
-00000730: 0474 6173 6bda 0673 6f75 7263 65da 0763  .task..source..c
-00000740: 6f6d 6d61 6e64 da0a 696e 7075 745f 7479  ommand..input_ty
-00000750: 7065 da0b 6f75 7470 7574 5f74 7970 6529  pe..output_type)
-00000760: 0572 0600 0000 722e 0000 0072 2f00 0000  .r....r....r/...
-00000770: 7230 0000 0072 3100 0000 2902 7206 0000  r0...r1...).r...
-00000780: 0072 2e00 0000 2905 7204 0000 0072 0200  .r....).r....r..
-00000790: 0000 da06 7079 7465 7374 da06 7261 6973  ....pytest..rais
-000007a0: 6573 7203 0000 0029 0172 0a00 0000 722a  esr....).r....r*
-000007b0: 0000 0072 2a00 0000 722b 0000 00da 1074  ...r*...r+.....t
-000007c0: 6573 745f 7461 736b 5f63 7265 6174 6511  est_task_create.
-000007d0: 0000 0073 1600 0000 0202 0201 0201 0201  ...s............
-000007e0: 0201 0201 06fb 0807 0c02 0e01 22ff 7234  ............".r4
-000007f0: 0000 0029 10da 0862 7569 6c74 696e 7372  ...)...builtinsr
-00000800: 1a00 0000 da19 5f70 7974 6573 742e 6173  ......_pytest.as
-00000810: 7365 7274 696f 6e2e 7265 7772 6974 65da  sertion.rewrite.
-00000820: 0961 7373 6572 7469 6f6e da07 7265 7772  .assertion..rewr
-00000830: 6974 6572 1800 0000 7232 0000 00da 0864  iter....r2.....d
-00000840: 6576 746f 6f6c 7372 0200 0000 da17 7079  evtoolsr......py
-00000850: 6461 6e74 6963 2e65 7272 6f72 5f77 7261  dantic.error_wra
-00000860: 7070 6572 7372 0300 0000 da07 7363 6865  ppersr......sche
-00000870: 6d61 7372 0400 0000 7205 0000 0072 2c00  masr....r....r,.
-00000880: 0000 7234 0000 0072 2a00 0000 722a 0000  ..r4...r*...r*..
-00000890: 0072 2a00 0000 722b 0000 00da 083c 6d6f  .r*...r+.....<mo
-000008a0: 6475 6c65 3e01 0000 0073 0e00 0000 2200  dule>....s....".
-000008b0: 0c01 0c01 0c02 0c01 0803 0c08            ............
+00000310: 0400 7d05 0400 7d06 0400 7d08 7d07 740d  ..}...}...}.}.t.
+00000320: a00e 740f a101 8f0e 0100 7400 640e 640f  ..t.......t.d.d.
+00000330: 6410 8d02 0100 5700 6400 0400 0400 8303  d.....W.d.......
+00000340: 0100 6e09 3100 9001 732d 7701 0100 0100  ..n.1...s-w.....
+00000350: 0100 5900 0100 740d a00e 740f a101 8f0e  ..Y...t...t.....
+00000360: 0100 7400 640e 6400 6410 8d02 0100 5700  ..t.d.d.d.....W.
+00000370: 6400 0400 0400 8303 0100 6e09 3100 9001  d.........n.1...
+00000380: 7349 7701 0100 0100 0100 5900 0100 7400  sIw.......Y...t.
+00000390: 640e 6411 6412 6413 8d03 7d00 7401 7c00  d.d.d.d...}.t.|.
+000003a0: 8301 0100 7c00 6a10 7d0b 7c0b 9001 7382  ....|.j.}.|...s.
+000003b0: 6414 6408 7407 a008 a100 7600 9001 736d  d.d.t.....v...sm
+000003c0: 7405 a009 7c00 a101 9001 7272 7405 a00a  t...|.....rrt...
+000003d0: 7c00 a101 6e01 6408 7405 a00a 7c0b a101  |...n.d.t...|...
+000003e0: 6415 9c02 1600 7d0c 740b 7405 a00c 7c0c  d.....}.t.t...|.
+000003f0: a101 8301 8201 6400 7d0b 7c00 6a11 7d0b  ......d.}.|.j.}.
+00000400: 7c0b 9001 73ad 6416 6408 7407 a008 a100  |...s.d.d.t.....
+00000410: 7600 9001 7398 7405 a009 7c00 a101 9001  v...s.t...|.....
+00000420: 729d 7405 a00a 7c00 a101 6e01 6408 7405  r.t...|...n.d.t.
+00000430: a00a 7c0b a101 6415 9c02 1600 7d0c 740b  ..|...d.....}.t.
+00000440: 7405 a00c 7c0c a101 8301 8201 6400 7d0b  t...|.......d.}.
+00000450: 6400 5300 2917 4eda 046e 616d 6529 0172  d.S.).N..name).r
+00000460: 0600 0000 5429 01da 0c65 7863 6c75 6465  ....T)...exclude
+00000470: 5f6e 6f6e 6529 01fa 023d 3d29 017a ab25  _none)...==).z.%
+00000480: 2870 7931 3329 730a 7b25 2870 7931 3329  (py13)s.{%(py13)
+00000490: 7320 3d20 2528 7079 3029 7328 2528 7079  s = %(py0)s(%(py
+000004a0: 3131 2973 0a7b 2528 7079 3131 2973 203d  11)s.{%(py11)s =
+000004b0: 2025 2870 7939 2973 0a7b 2528 7079 3929   %(py9)s.{%(py9)
+000004c0: 7320 3d20 2528 7079 3729 730a 7b25 2870  s = %(py7)s.{%(p
+000004d0: 7937 2973 203d 2025 2870 7933 2973 0a7b  y7)s = %(py3)s.{
+000004e0: 2528 7079 3329 7320 3d20 2528 7079 3129  %(py3)s = %(py1)
+000004f0: 732e 6469 6374 0a7d 2865 7863 6c75 6465  s.dict.}(exclude
+00000500: 5f6e 6f6e 653d 2528 7079 3529 7329 0a7d  _none=%(py5)s).}
+00000510: 2e6b 6579 730a 7d28 290a 7d29 0a7d 203d  .keys.}().}).} =
+00000520: 3d20 2528 7079 3136 2973 da04 6c69 7374  = %(py16)s..list
+00000530: da01 7429 09da 0370 7930 da03 7079 31da  ..t)...py0..py1.
+00000540: 0370 7933 da03 7079 35da 0370 7937 5a03  .py3..py5..py7Z.
+00000550: 7079 395a 0470 7931 315a 0470 7931 335a  py9Z.py11Z.py13Z
+00000560: 0470 7931 367a 0f61 7373 6572 7420 2528  .py16z.assert %(
+00000570: 7079 3138 2973 5a04 7079 3138 2901 da0d  py18)sZ.py18)...
+00000580: 6578 636c 7564 655f 756e 7365 7429 017a  exclude_unset).z
+00000590: ac25 2870 7931 3329 730a 7b25 2870 7931  .%(py13)s.{%(py1
+000005a0: 3329 7320 3d20 2528 7079 3029 7328 2528  3)s = %(py0)s(%(
+000005b0: 7079 3131 2973 0a7b 2528 7079 3131 2973  py11)s.{%(py11)s
+000005c0: 203d 2025 2870 7939 2973 0a7b 2528 7079   = %(py9)s.{%(py
+000005d0: 3929 7320 3d20 2528 7079 3729 730a 7b25  9)s = %(py7)s.{%
+000005e0: 2870 7937 2973 203d 2025 2870 7933 2973  (py7)s = %(py3)s
+000005f0: 0a7b 2528 7079 3329 7320 3d20 2528 7079  .{%(py3)s = %(py
+00000600: 3129 732e 6469 6374 0a7d 2865 7863 6c75  1)s.dict.}(exclu
+00000610: 6465 5f75 6e73 6574 3d25 2870 7935 2973  de_unset=%(py5)s
+00000620: 290a 7d2e 6b65 7973 0a7d 2829 0a7d 290a  ).}.keys.}().}).
+00000630: 7d20 3d3d 2025 2870 7931 3629 73da 0474  } == %(py16)s..t
+00000640: 6173 6bda 0029 0272 0600 0000 da07 7665  ask..).r......ve
+00000650: 7273 696f 6efa 0531 2e32 2e33 da07 736f  rsion..1.2.3..so
+00000660: 6d65 6f6e 6529 0372 0600 0000 7213 0000  meone).r....r...
+00000670: 00da 056f 776e 6572 7a28 6173 7365 7274  ...ownerz(assert
+00000680: 2025 2870 7932 2973 0a7b 2528 7079 3229   %(py2)s.{%(py2)
+00000690: 7320 3d20 2528 7079 3029 732e 6e61 6d65  s = %(py0)s.name
+000006a0: 0a7d 2902 720b 0000 00da 0370 7932 7a2b  .}).r......py2z+
+000006b0: 6173 7365 7274 2025 2870 7932 2973 0a7b  assert %(py2)s.{
+000006c0: 2528 7079 3229 7320 3d20 2528 7079 3029  %(py2)s = %(py0)
+000006d0: 732e 7665 7273 696f 6e0a 7d29 1272 0500  s.version.}).r..
+000006e0: 0000 7202 0000 00da 0464 6963 74da 046b  ..r......dict..k
+000006f0: 6579 7372 0900 0000 da0a 4070 7974 6573  eysr......@pytes
+00000700: 745f 6172 da11 5f63 616c 6c5f 7265 7072  t_ar.._call_repr
+00000710: 636f 6d70 6172 65da 0c40 7079 5f62 7569  compare..@py_bui
+00000720: 6c74 696e 73da 066c 6f63 616c 73da 185f  ltins..locals.._
+00000730: 7368 6f75 6c64 5f72 6570 725f 676c 6f62  should_repr_glob
+00000740: 616c 5f6e 616d 65da 095f 7361 6665 7265  al_name.._safere
+00000750: 7072 da0e 4173 7365 7274 696f 6e45 7272  pr..AssertionErr
+00000760: 6f72 da13 5f66 6f72 6d61 745f 6578 706c  or.._format_expl
+00000770: 616e 6174 696f 6eda 0670 7974 6573 74da  anation..pytest.
+00000780: 0672 6169 7365 7372 0300 0000 7206 0000  .raisesr....r...
+00000790: 0072 1300 0000 290d 720a 0000 00da 0b40  .r....).r......@
+000007a0: 7079 5f61 7373 6572 7432 da0b 4070 795f  py_assert2..@py_
+000007b0: 6173 7365 7274 345a 0b40 7079 5f61 7373  assert4Z.@py_ass
+000007c0: 6572 7436 5a0b 4070 795f 6173 7365 7274  ert6Z.@py_assert
+000007d0: 385a 0c40 7079 5f61 7373 6572 7431 305a  8Z.@py_assert10Z
+000007e0: 0c40 7079 5f61 7373 6572 7431 325a 0c40  .@py_assert12Z.@
+000007f0: 7079 5f61 7373 6572 7431 355a 0c40 7079  py_assert15Z.@py
+00000800: 5f61 7373 6572 7431 345a 0c40 7079 5f66  _assert14Z.@py_f
+00000810: 6f72 6d61 7431 375a 0c40 7079 5f66 6f72  ormat17Z.@py_for
+00000820: 6d61 7431 39da 0b40 7079 5f61 7373 6572  mat19..@py_asser
+00000830: 7431 da0b 4070 795f 666f 726d 6174 33a9  t1..@py_format3.
+00000840: 0072 2800 0000 fa4d 2f68 6f6d 652f 746f  .r(....M/home/to
+00000850: 6d6d 6173 6f2f 4672 6163 7461 6c2f 6672  mmaso/Fractal/fr
+00000860: 6163 7461 6c2d 7365 7276 6572 2f66 7261  actal-server/fra
+00000870: 6374 616c 5f73 6572 7665 722f 636f 6d6d  ctal_server/comm
+00000880: 6f6e 2f74 6573 7473 2f74 6573 745f 7461  on/tests/test_ta
+00000890: 736b 2e70 79da 1074 6573 745f 7461 736b  sk.py..test_task
+000008a0: 5f75 7064 6174 6509 0000 0073 2800 0000  _update....s(...
+000008b0: 0a02 0801 fe01 0e00 fe01 1000 0c02 0e01  ................
+000008c0: 1eff 0c02 0e01 1eff 0203 0201 0201 0201  ................
+000008d0: 06fd 0805 5601 5a01 722a 0000 0063 0000  ....V.Z.r*...c..
+000008e0: 0000 0000 0000 0000 0000 0100 0000 0900  ................
+000008f0: 0000 4300 0000 735a 0000 0074 0064 0164  ..C...sZ...t.d.d
+00000900: 0264 0364 0464 0564 0664 0764 088d 077d  .d.d.d.d.d.d...}
+00000910: 0074 017c 0083 0101 0074 02a0 0374 04a1  .t.|.....t...t..
+00000920: 018f 0f01 0074 0064 0164 0264 098d 0201  .....t.d.d.d....
+00000930: 0057 0064 0004 0004 0083 0301 0064 0053  .W.d.........d.S
+00000940: 0031 0073 2677 0101 0001 0001 0059 0001  .1.s&w.......Y..
+00000950: 0064 0053 0029 0a4e 7211 0000 00da 0673  .d.S.).Nr......s
+00000960: 6f75 7263 65da 0763 6f6d 6d61 6e64 da0a  ource..command..
+00000970: 696e 7075 745f 7479 7065 da0b 6f75 7470  input_type..outp
+00000980: 7574 5f74 7970 6572 1400 0000 7215 0000  ut_typer....r...
+00000990: 0029 0772 0600 0000 722b 0000 0072 2c00  .).r....r+...r,.
+000009a0: 0000 722d 0000 0072 2e00 0000 7213 0000  ..r-...r....r...
+000009b0: 0072 1600 0000 2902 7206 0000 0072 2b00  .r....).r....r+.
+000009c0: 0000 2905 7204 0000 0072 0200 0000 7222  ..).r....r....r"
+000009d0: 0000 0072 2300 0000 7203 0000 0029 0172  ...r#...r....).r
+000009e0: 0a00 0000 7228 0000 0072 2800 0000 7229  ....r(...r(...r)
+000009f0: 0000 00da 1074 6573 745f 7461 736b 5f63  .....test_task_c
+00000a00: 7265 6174 651f 0000 0073 1a00 0000 0202  reate....s......
+00000a10: 0201 0201 0201 0201 0201 0201 0201 06f9  ................
+00000a20: 0809 0c02 0e01 22ff 722f 0000 0029 10da  ......".r/...)..
+00000a30: 0862 7569 6c74 696e 7372 1c00 0000 da19  .builtinsr......
+00000a40: 5f70 7974 6573 742e 6173 7365 7274 696f  _pytest.assertio
+00000a50: 6e2e 7265 7772 6974 65da 0961 7373 6572  n.rewrite..asser
+00000a60: 7469 6f6e da07 7265 7772 6974 6572 1a00  tion..rewriter..
+00000a70: 0000 7222 0000 00da 0864 6576 746f 6f6c  ..r".....devtool
+00000a80: 7372 0200 0000 da17 7079 6461 6e74 6963  sr......pydantic
+00000a90: 2e65 7272 6f72 5f77 7261 7070 6572 7372  .error_wrappersr
+00000aa0: 0300 0000 da07 7363 6865 6d61 7372 0400  ......schemasr..
+00000ab0: 0000 7205 0000 0072 2a00 0000 722f 0000  ..r....r*...r/..
+00000ac0: 0072 2800 0000 7228 0000 0072 2800 0000  .r(...r(...r(...
+00000ad0: 7229 0000 00da 083c 6d6f 6475 6c65 3e01  r).....<module>.
+00000ae0: 0000 0073 0e00 0000 2200 0c01 0c01 0c02  ...s....".......
+00000af0: 0c01 0803 0c16                           ......
```

### Comparing `fractal_server-1.3.0a8/fractal_server/common/tests/__pycache__/test_task_collection.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a9/fractal_server/common/tests/__pycache__/test_task_collection.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jun 12 09:12:04 2023 UTC, .py size: 968 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 64e1 8664 c803 0000  o.......d..d....
+00000000: 6f0d 0d0a 0000 0000 5a07 9264 c803 0000  o.......Z..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6400 6402 6c07 6d08 5a08 0100 6400 6403  d.d.l.m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 0100 6400 6404 6c0b 6d0c  l.m.Z...d.d.l.m.
 00000070: 5a0c 0100 6405 6406 8400 5a0d 6401 5300  Z...d.d...Z.d.S.
@@ -54,32 +54,32 @@
 00000350: 696e 73da 066c 6f63 616c 73da 0a40 7079  ins..locals..@py
 00000360: 7465 7374 5f61 72da 185f 7368 6f75 6c64  test_ar.._should
 00000370: 5f72 6570 725f 676c 6f62 616c 5f6e 616d  _repr_global_nam
 00000380: 65da 095f 7361 6665 7265 7072 da0e 4173  e.._saferepr..As
 00000390: 7365 7274 696f 6e45 7272 6f72 da13 5f66  sertionError.._f
 000003a0: 6f72 6d61 745f 6578 706c 616e 6174 696f  ormat_explanatio
 000003b0: 6eda 0670 7974 6573 74da 0672 6169 7365  n..pytest..raise
-000003c0: 7372 0300 0000 2902 7207 0000 00da 0b40  sr....).r......@
-000003d0: 7079 5f66 6f72 6d61 7431 a900 7216 0000  py_format1..r...
+000003c0: 7372 0300 0000 2902 7207 0000 005a 0b40  sr....).r....Z.@
+000003d0: 7079 5f66 6f72 6d61 7431 a900 7215 0000  py_format1..r...
 000003e0: 00fa 582f 686f 6d65 2f74 6f6d 6d61 736f  ..X/home/tommaso
 000003f0: 2f46 7261 6374 616c 2f66 7261 6374 616c  /Fractal/fractal
 00000400: 2d73 6572 7665 722f 6672 6163 7461 6c5f  -server/fractal_
 00000410: 7365 7276 6572 2f63 6f6d 6d6f 6e2f 7465  server/common/te
 00000420: 7374 732f 7465 7374 5f74 6173 6b5f 636f  sts/test_task_co
 00000430: 6c6c 6563 7469 6f6e 2e70 79da 1374 6573  llection.py..tes
 00000440: 745f 5461 736b 436f 6c6c 6563 7450 6970  t_TaskCollectPip
 00000450: 0800 0000 732c 0000 000a 0208 013e 010a  ....s,.......>..
 00000460: 0108 013e 010c 020c 011c ff0c 020c 011c  ...>............
 00000470: ff0c 020e 011c ff0c 020e 011c ff0c 030c  ................
-00000480: 010e 0122 ff72 1800 0000 290e da08 6275  ...".r....)...bu
+00000480: 010e 0122 ff72 1700 0000 290e da08 6275  ...".r....)...bu
 00000490: 696c 7469 6e73 720c 0000 00da 195f 7079  iltinsr......_py
 000004a0: 7465 7374 2e61 7373 6572 7469 6f6e 2e72  test.assertion.r
 000004b0: 6577 7269 7465 da09 6173 7365 7274 696f  ewrite..assertio
 000004c0: 6eda 0772 6577 7269 7465 720e 0000 0072  n..rewriter....r
 000004d0: 1300 0000 da08 6465 7674 6f6f 6c73 7202  ......devtoolsr.
 000004e0: 0000 00da 1770 7964 616e 7469 632e 6572  .....pydantic.er
 000004f0: 726f 725f 7772 6170 7065 7273 7203 0000  ror_wrappersr...
 00000500: 00da 0773 6368 656d 6173 7204 0000 0072  ...schemasr....r
-00000510: 1800 0000 7216 0000 0072 1600 0000 7216  ....r....r....r.
-00000520: 0000 0072 1700 0000 da08 3c6d 6f64 756c  ...r......<modul
+00000510: 1700 0000 7215 0000 0072 1500 0000 7215  ....r....r....r.
+00000520: 0000 0072 1600 0000 da08 3c6d 6f64 756c  ...r......<modul
 00000530: 653e 0100 0000 730a 0000 0022 000c 010c  e>....s...."....
 00000540: 010c 020c 03                             .....
```

### Comparing `fractal_server-1.3.0a8/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a9/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Apr  6 07:41:00 2023 UTC, .py size: 1224 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-00000000: 6f0d 0d0a 0000 0000 8c77 2e64 c804 0000  o........w.d....
+00000000: 6f0d 0d0a 0000 0000 5a07 9264 db05 0000  o.......Z..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6400 6402 6c07 6d08 5a08 0100 6400 6403  d.d.l.m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 0100 6400 6404 6c0b 6d0c  l.m.Z...d.d.l.m.
 00000070: 5a0c 0100 6405 6406 8400 5a0d 6401 5300  Z...d.d...Z.d.S.
 00000080: 2907 e900 0000 004e 2901 da05 6465 6275  )......N)...debu
 00000090: 6729 01da 0f56 616c 6964 6174 696f 6e45  g)...ValidationE
 000000a0: 7272 6f72 2901 da0a 5573 6572 4372 6561  rror)...UserCrea
 000000b0: 7465 6300 0000 0000 0000 0000 0000 000d  tec.............
-000000c0: 0000 0008 0000 0043 0000 0073 6803 0000  .......C...sh...
+000000c0: 0000 0008 0000 0043 0000 0073 8404 0000  .......C...s....
 000000d0: 7400 6401 6402 6403 8d02 7d00 7401 7c00  t.d.d.d...}.t.|.
 000000e0: 8301 0100 7c00 6a02 7d01 6400 7d02 7c01  ....|.j.}.d.}.|.
 000000f0: 7c02 7500 7d03 7c03 7349 7403 a004 6404  |.u.}.|.sIt...d.
 00000100: 7c03 6601 6405 7c01 7c02 6602 a104 6406  |.f.d.|.|.f...d.
 00000110: 7405 a006 a100 7600 732a 7403 a007 7c00  t.....v.s*t...|.
 00000120: a101 722f 7403 a008 7c00 a101 6e01 6406  ..r/t...|...n.d.
 00000130: 7403 a008 7c01 a101 7403 a008 7c02 a101  t...|...t...|...
@@ -61,80 +61,108 @@
 000003c0: 7d0b 7c0a 6a0f a010 a100 6419 1900 641a  }.|.j.....d...d.
 000003d0: 1900 7d03 7c0b 7c03 7600 7d0c 7c0c 9001  ..}.|.|.v.}.|...
 000003e0: 73ac 7403 a004 641b 7c0c 6601 641c 7c0b  s.t...d.|.f.d.|.
 000003f0: 7c03 6602 a104 7403 a008 7c0b a101 7403  |.f...t...|...t.
 00000400: a008 7c03 a101 641d 9c02 1600 7d08 6416  ..|...d.....}.d.
 00000410: 6417 7c08 6901 1600 7d09 7409 7403 a00a  d.|.i...}.t.t...
 00000420: 7c09 a101 8301 8201 6400 0400 7d0b 0400  |.......d...}...
-00000430: 7d0c 7d03 6400 5300 2920 4e7a 0561 4062  }.}.d.S.) Nz.a@b
-00000440: 2e63 da03 6173 6429 02da 0565 6d61 696c  .c..asd)...email
-00000450: da08 7061 7373 776f 7264 2901 da02 6973  ..password)...is
-00000460: 2901 7a32 2528 7079 3229 730a 7b25 2870  ).z2%(py2)s.{%(p
-00000470: 7932 2973 203d 2025 2870 7930 2973 2e73  y2)s = %(py0)s.s
-00000480: 6c75 726d 5f75 7365 720a 7d20 6973 2025  lurm_user.} is %
-00000490: 2870 7935 2973 da01 7529 03da 0370 7930  (py5)s..u)...py0
-000004a0: da03 7079 32da 0370 7935 7a0e 6173 7365  ..py2..py5z.asse
-000004b0: 7274 2025 2870 7937 2973 da03 7079 37da  rt %(py7)s..py7.
-000004c0: 0a73 6c75 726d 5f75 7365 7229 0372 0600  .slurm_user).r..
-000004d0: 0000 7207 0000 0072 0e00 0000 7a2e 6173  ..r....r....z.as
-000004e0: 7365 7274 2025 2870 7932 2973 0a7b 2528  sert %(py2)s.{%(
-000004f0: 7079 3229 7320 3d20 2528 7079 3029 732e  py2)s = %(py0)s.
-00000500: 736c 7572 6d5f 7573 6572 0a7d 2902 720a  slurm_user.}).r.
-00000510: 0000 0072 0b00 0000 7a02 2020 7a04 2f78  ...r....z.  z./x
-00000520: 7878 7a03 2020 2029 0372 0600 0000 7207  xxz.   ).r....r.
-00000530: 0000 00da 0963 6163 6865 5f64 6972 2901  .....cache_dir).
-00000540: fa02 3d3d 2901 7a31 2528 7079 3229 730a  ..==).z1%(py2)s.
-00000550: 7b25 2870 7932 2973 203d 2025 2870 7930  {%(py2)s = %(py0
-00000560: 2973 2e63 6163 6865 5f64 6972 0a7d 203d  )s.cache_dir.} =
-00000570: 3d20 2528 7079 3429 73da 0943 4143 4845  = %(py4)s..CACHE
-00000580: 5f44 4952 2903 720a 0000 0072 0b00 0000  _DIR).r....r....
-00000590: da03 7079 347a 0e61 7373 6572 7420 2528  ..py4z.assert %(
-000005a0: 7079 3629 73da 0370 7936 7a0f 6361 6e6e  py6)s..py6z.cann
-000005b0: 6f74 2062 6520 656d 7074 7972 0100 0000  ot be emptyr....
-000005c0: da03 6d73 6729 01da 0269 6e29 017a 1225  ..msg)...in).z.%
-000005d0: 2870 7931 2973 2069 6e20 2528 7079 3429  (py1)s in %(py4)
-000005e0: 7329 02da 0370 7931 7212 0000 00da 0378  s)...py1r......x
-000005f0: 7878 7a18 6d75 7374 2062 6520 616e 2061  xxz.must be an a
-00000600: 6273 6f6c 7574 6520 7061 7468 2911 7204  bsolute path).r.
-00000610: 0000 0072 0200 0000 720e 0000 00da 0a40  ...r....r......@
-00000620: 7079 7465 7374 5f61 72da 115f 6361 6c6c  pytest_ar.._call
-00000630: 5f72 6570 7263 6f6d 7061 7265 da0c 4070  _reprcompare..@p
-00000640: 795f 6275 696c 7469 6e73 da06 6c6f 6361  y_builtins..loca
-00000650: 6c73 da18 5f73 686f 756c 645f 7265 7072  ls.._should_repr
-00000660: 5f67 6c6f 6261 6c5f 6e61 6d65 da09 5f73  _global_name.._s
-00000670: 6166 6572 6570 72da 0e41 7373 6572 7469  aferepr..Asserti
-00000680: 6f6e 4572 726f 72da 135f 666f 726d 6174  onError.._format
-00000690: 5f65 7870 6c61 6e61 7469 6f6e da06 7079  _explanation..py
-000006a0: 7465 7374 da06 7261 6973 6573 7203 0000  test..raisesr...
-000006b0: 0072 0f00 0000 da05 7661 6c75 65da 0665  .r......value..e
-000006c0: 7272 6f72 7329 0d72 0900 0000 da0b 4070  rrors).r......@p
-000006d0: 795f 6173 7365 7274 31da 0b40 7079 5f61  y_assert1..@py_a
-000006e0: 7373 6572 7434 da0b 4070 795f 6173 7365  ssert4..@py_asse
-000006f0: 7274 33da 0b40 7079 5f66 6f72 6d61 7436  rt3..@py_format6
-00000700: da0b 4070 795f 666f 726d 6174 38da 0b40  ..@py_format8..@
-00000710: 7079 5f66 6f72 6d61 7433 7211 0000 00da  py_format3r.....
-00000720: 0b40 7079 5f66 6f72 6d61 7435 da0b 4070  .@py_format5..@p
-00000730: 795f 666f 726d 6174 37da 0165 da0b 4070  y_format7..e..@p
-00000740: 795f 6173 7365 7274 30da 0b40 7079 5f61  y_assert0..@py_a
-00000750: 7373 6572 7432 a900 722f 0000 00fa 4d2f  ssert2..r/....M/
-00000760: 686f 6d65 2f74 6f6d 6d61 736f 2f46 7261  home/tommaso/Fra
-00000770: 6374 616c 2f66 7261 6374 616c 2d73 6572  ctal/fractal-ser
-00000780: 7665 722f 6672 6163 7461 6c5f 7365 7276  ver/fractal_serv
-00000790: 6572 2f63 6f6d 6d6f 6e2f 7465 7374 732f  er/common/tests/
-000007a0: 7465 7374 5f75 7365 722e 7079 da10 7465  test_user.py..te
-000007b0: 7374 5f75 7365 725f 6372 6561 7465 0800  st_user_create..
-000007c0: 0000 732c 0000 000c 0208 018a 010e 0208  ..s,............
-000007d0: 0150 010c 0210 011c ff04 0314 019c 010c  .P..............
-000007e0: 0210 011e ff0a 0276 010c 0210 011e ff0a  .......v........
-000007f0: 027a 0172 3100 0000 290e da08 6275 696c  .z.r1...)...buil
-00000800: 7469 6e73 721a 0000 00da 195f 7079 7465  tinsr......_pyte
-00000810: 7374 2e61 7373 6572 7469 6f6e 2e72 6577  st.assertion.rew
-00000820: 7269 7465 da09 6173 7365 7274 696f 6eda  rite..assertion.
-00000830: 0772 6577 7269 7465 7218 0000 0072 2000  .rewriter....r .
-00000840: 0000 da08 6465 7674 6f6f 6c73 7202 0000  ....devtoolsr...
-00000850: 00da 1770 7964 616e 7469 632e 6572 726f  ...pydantic.erro
-00000860: 725f 7772 6170 7065 7273 7203 0000 00da  r_wrappersr.....
-00000870: 0773 6368 656d 6173 7204 0000 0072 3100  .schemasr....r1.
-00000880: 0000 722f 0000 0072 2f00 0000 722f 0000  ..r/...r/...r/..
-00000890: 0072 3000 0000 da08 3c6d 6f64 756c 653e  .r0.....<module>
-000008a0: 0100 0000 730a 0000 0022 000c 010c 010c  ....s...."......
-000008b0: 020c 03                                  ...
+00000430: 7d0c 7d03 7400 6401 6420 640a 6421 6422  }.}.t.d.d d.d!d"
+00000440: 6423 8d05 7d00 7401 7c00 8301 0100 7c00  d#..}.t.|.....|.
+00000450: 6a02 7d01 7c01 9001 73e8 640c 6406 7405  j.}.|...s.d.d.t.
+00000460: a006 a100 7600 9001 73d3 7403 a007 7c00  ....v...s.t...|.
+00000470: a101 9001 72d8 7403 a008 7c00 a101 6e01  ....r.t...|...n.
+00000480: 6406 7403 a008 7c01 a101 640d 9c02 1600  d.t...|...d.....
+00000490: 7d06 7409 7403 a00a 7c06 a101 8301 8201  }.t.t...|.......
+000004a0: 6400 7d01 7c00 6a0e 7d01 7c01 9002 7313  d.}.|.j.}.|...s.
+000004b0: 6424 6406 7405 a006 a100 7600 9001 73fe  d$d.t.....v...s.
+000004c0: 7403 a007 7c00 a101 9002 7203 7403 a008  t...|.....r.t...
+000004d0: 7c00 a101 6e01 6406 7403 a008 7c01 a101  |...n.d.t...|...
+000004e0: 640d 9c02 1600 7d06 7409 7403 a00a 7c06  d.....}.t.t...|.
+000004f0: a101 8301 8201 6400 7d01 7c00 6a11 7d01  ......d.}.|.j.}.
+00000500: 7c01 9002 733e 6425 6406 7405 a006 a100  |...s>d%d.t.....
+00000510: 7600 9002 7329 7403 a007 7c00 a101 9002  v...s)t...|.....
+00000520: 722e 7403 a008 7c00 a101 6e01 6406 7403  r.t...|...n.d.t.
+00000530: a008 7c01 a101 640d 9c02 1600 7d06 7409  ..|...d.....}.t.
+00000540: 7403 a00a 7c06 a101 8301 8201 6400 7d01  t...|.......d.}.
+00000550: 6400 5300 2926 4e7a 0561 4062 2e63 5a03  d.S.)&Nz.a@b.cZ.
+00000560: 6173 6429 02da 0565 6d61 696c da08 7061  asd)...email..pa
+00000570: 7373 776f 7264 2901 da02 6973 2901 7a32  ssword)...is).z2
+00000580: 2528 7079 3229 730a 7b25 2870 7932 2973  %(py2)s.{%(py2)s
+00000590: 203d 2025 2870 7930 2973 2e73 6c75 726d   = %(py0)s.slurm
+000005a0: 5f75 7365 720a 7d20 6973 2025 2870 7935  _user.} is %(py5
+000005b0: 2973 da01 7529 03da 0370 7930 da03 7079  )s..u)...py0..py
+000005c0: 32da 0370 7935 7a0e 6173 7365 7274 2025  2..py5z.assert %
+000005d0: 2870 7937 2973 da03 7079 37da 0a73 6c75  (py7)s..py7..slu
+000005e0: 726d 5f75 7365 7229 0372 0500 0000 7206  rm_user).r....r.
+000005f0: 0000 0072 0d00 0000 7a2e 6173 7365 7274  ...r....z.assert
+00000600: 2025 2870 7932 2973 0a7b 2528 7079 3229   %(py2)s.{%(py2)
+00000610: 7320 3d20 2528 7079 3029 732e 736c 7572  s = %(py0)s.slur
+00000620: 6d5f 7573 6572 0a7d 2902 7209 0000 0072  m_user.}).r....r
+00000630: 0a00 0000 7a02 2020 7a04 2f78 7878 7a03  ....z.  z./xxxz.
+00000640: 2020 2029 0372 0500 0000 7206 0000 00da     ).r....r.....
+00000650: 0963 6163 6865 5f64 6972 2901 fa02 3d3d  .cache_dir)...==
+00000660: 2901 7a31 2528 7079 3229 730a 7b25 2870  ).z1%(py2)s.{%(p
+00000670: 7932 2973 203d 2025 2870 7930 2973 2e63  y2)s = %(py0)s.c
+00000680: 6163 6865 5f64 6972 0a7d 203d 3d20 2528  ache_dir.} == %(
+00000690: 7079 3429 73da 0943 4143 4845 5f44 4952  py4)s..CACHE_DIR
+000006a0: 2903 7209 0000 0072 0a00 0000 da03 7079  ).r....r......py
+000006b0: 347a 0e61 7373 6572 7420 2528 7079 3629  4z.assert %(py6)
+000006c0: 73da 0370 7936 7a0f 6361 6e6e 6f74 2062  s..py6z.cannot b
+000006d0: 6520 656d 7074 7972 0100 0000 da03 6d73  e emptyr......ms
+000006e0: 6729 01da 0269 6e29 017a 1225 2870 7931  g)...in).z.%(py1
+000006f0: 2973 2069 6e20 2528 7079 3429 7329 02da  )s in %(py4)s)..
+00000700: 0370 7931 7211 0000 005a 0378 7878 7a18  .py1r....Z.xxxz.
+00000710: 6d75 7374 2062 6520 616e 2061 6273 6f6c  must be an absol
+00000720: 7574 6520 7061 7468 da03 7077 64da 0875  ute path..pwd..u
+00000730: 7365 726e 616d 657a 0a2f 736f 6d65 2f70  sernamez./some/p
+00000740: 6174 6829 0572 0500 0000 7206 0000 0072  ath).r....r....r
+00000750: 0d00 0000 7217 0000 0072 0e00 0000 7a2d  ....r....r....z-
+00000760: 6173 7365 7274 2025 2870 7932 2973 0a7b  assert %(py2)s.{
+00000770: 2528 7079 3229 7320 3d20 2528 7079 3029  %(py2)s = %(py0)
+00000780: 732e 6361 6368 655f 6469 720a 7d7a 2c61  s.cache_dir.}z,a
+00000790: 7373 6572 7420 2528 7079 3229 730a 7b25  ssert %(py2)s.{%
+000007a0: 2870 7932 2973 203d 2025 2870 7930 2973  (py2)s = %(py0)s
+000007b0: 2e75 7365 726e 616d 650a 7d29 1272 0400  .username.}).r..
+000007c0: 0000 7202 0000 0072 0d00 0000 da0a 4070  ..r....r......@p
+000007d0: 7974 6573 745f 6172 da11 5f63 616c 6c5f  ytest_ar.._call_
+000007e0: 7265 7072 636f 6d70 6172 65da 0c40 7079  reprcompare..@py
+000007f0: 5f62 7569 6c74 696e 73da 066c 6f63 616c  _builtins..local
+00000800: 73da 185f 7368 6f75 6c64 5f72 6570 725f  s.._should_repr_
+00000810: 676c 6f62 616c 5f6e 616d 65da 095f 7361  global_name.._sa
+00000820: 6665 7265 7072 da0e 4173 7365 7274 696f  ferepr..Assertio
+00000830: 6e45 7272 6f72 da13 5f66 6f72 6d61 745f  nError.._format_
+00000840: 6578 706c 616e 6174 696f 6eda 0670 7974  explanation..pyt
+00000850: 6573 74da 0672 6169 7365 7372 0300 0000  est..raisesr....
+00000860: 720e 0000 00da 0576 616c 7565 da06 6572  r......value..er
+00000870: 726f 7273 7217 0000 0029 0d72 0800 0000  rorsr....).r....
+00000880: da0b 4070 795f 6173 7365 7274 31da 0b40  ..@py_assert1..@
+00000890: 7079 5f61 7373 6572 7434 da0b 4070 795f  py_assert4..@py_
+000008a0: 6173 7365 7274 33da 0b40 7079 5f66 6f72  assert3..@py_for
+000008b0: 6d61 7436 da0b 4070 795f 666f 726d 6174  mat6..@py_format
+000008c0: 38da 0b40 7079 5f66 6f72 6d61 7433 7210  8..@py_format3r.
+000008d0: 0000 00da 0b40 7079 5f66 6f72 6d61 7435  .....@py_format5
+000008e0: da0b 4070 795f 666f 726d 6174 37da 0165  ..@py_format7..e
+000008f0: 5a0b 4070 795f 6173 7365 7274 30da 0b40  Z.@py_assert0..@
+00000900: 7079 5f61 7373 6572 7432 a900 722e 0000  py_assert2..r...
+00000910: 00fa 4d2f 686f 6d65 2f74 6f6d 6d61 736f  ..M/home/tommaso
+00000920: 2f46 7261 6374 616c 2f66 7261 6374 616c  /Fractal/fractal
+00000930: 2d73 6572 7665 722f 6672 6163 7461 6c5f  -server/fractal_
+00000940: 7365 7276 6572 2f63 6f6d 6d6f 6e2f 7465  server/common/te
+00000950: 7374 732f 7465 7374 5f75 7365 722e 7079  sts/test_user.py
+00000960: da10 7465 7374 5f75 7365 725f 6372 6561  ..test_user_crea
+00000970: 7465 0800 0000 7342 0000 000c 0208 018a  te....sB........
+00000980: 010e 0208 0150 010c 0210 011c ff04 0314  .....P..........
+00000990: 019c 010c 0210 011e ff0a 0276 010c 0210  ...........v....
+000009a0: 011e ff0a 0276 0102 0202 0102 0102 0102  .....v..........
+000009b0: 0102 0106 fb08 0756 0156 015a 0172 3000  .......V.V.Z.r0.
+000009c0: 0000 290e da08 6275 696c 7469 6e73 721a  ..)...builtinsr.
+000009d0: 0000 00da 195f 7079 7465 7374 2e61 7373  ....._pytest.ass
+000009e0: 6572 7469 6f6e 2e72 6577 7269 7465 da09  ertion.rewrite..
+000009f0: 6173 7365 7274 696f 6eda 0772 6577 7269  assertion..rewri
+00000a00: 7465 7218 0000 0072 2000 0000 da08 6465  ter....r .....de
+00000a10: 7674 6f6f 6c73 7202 0000 00da 1770 7964  vtoolsr......pyd
+00000a20: 616e 7469 632e 6572 726f 725f 7772 6170  antic.error_wrap
+00000a30: 7065 7273 7203 0000 00da 0773 6368 656d  persr......schem
+00000a40: 6173 7204 0000 0072 3000 0000 722e 0000  asr....r0...r...
+00000a50: 0072 2e00 0000 722e 0000 0072 2f00 0000  .r....r....r/...
+00000a60: da08 3c6d 6f64 756c 653e 0100 0000 730a  ..<module>....s.
+00000a70: 0000 0022 000c 010c 010c 020c 03         ...".........
```

### Comparing `fractal_server-1.3.0a8/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a9/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Mar  6 16:04:10 2023 UTC, .py size: 2361 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,163 +1,183 @@
-00000000: 6f0d 0d0a 0000 0000 fa0e 0664 3909 0000  o..........d9...
+00000000: 6f0d 0d0a 0000 0000 5a07 9264 240a 0000  o.......Z..d$...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 da00 0000 6400  .....@...s....d.
+00000020: 0002 0000 0040 0000 0073 ee00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6400 6402 6c07 6d08 5a08 0100 6400 6403  d.d.l.m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 0100 6400 6404 6c0b 6d0c  l.m.Z...d.d.l.m.
 00000070: 5a0c 0100 6400 6405 6c0b 6d0d 5a0d 0100  Z...d.d.l.m.Z...
 00000080: 6400 6406 6c0b 6d0e 5a0e 0100 6400 6407  d.d.l.m.Z...d.d.
 00000090: 6c0b 6d0f 5a0f 0100 6400 6408 6c0b 6d10  l.m.Z...d.d.l.m.
 000000a0: 5a10 0100 6400 6409 6c0b 6d11 5a11 0100  Z...d.d.l.m.Z...
 000000b0: 6400 640a 6c0b 6d12 5a12 0100 6400 640b  d.d.l.m.Z...d.d.
 000000c0: 6c0b 6d13 5a13 0100 6400 640c 6c0b 6d14  l.m.Z...d.d.l.m.
-000000d0: 5a14 0100 640d 640e 8400 5a15 640f 6410  Z...d.d...Z.d.d.
-000000e0: 8400 5a16 6411 6412 8400 5a17 6413 6414  ..Z.d.d...Z.d.d.
-000000f0: 8400 5a18 6415 6416 8400 5a19 6417 6418  ..Z.d.d...Z.d.d.
-00000100: 8400 5a1a 6401 5300 2919 e900 0000 004e  ..Z.d.S.)......N
-00000110: 2901 da05 6465 6275 6729 01da 0f56 616c  )...debug)...Val
-00000120: 6964 6174 696f 6e45 7272 6f72 2901 da0a  idationError)...
-00000130: 5461 736b 496d 706f 7274 2901 da08 5461  TaskImport)...Ta
-00000140: 736b 5265 6164 2901 da0e 576f 726b 666c  skRead)...Workfl
-00000150: 6f77 4372 6561 7465 2901 da0e 576f 726b  owCreate)...Work
-00000160: 666c 6f77 496d 706f 7274 2901 da0c 576f  flowImport)...Wo
-00000170: 726b 666c 6f77 5265 6164 2901 da12 576f  rkflowRead)...Wo
-00000180: 726b 666c 6f77 5461 736b 4372 6561 7465  rkflowTaskCreate
-00000190: 2901 da12 576f 726b 666c 6f77 5461 736b  )...WorkflowTask
-000001a0: 496d 706f 7274 2901 da10 576f 726b 666c  Import)...Workfl
-000001b0: 6f77 5461 736b 5265 6164 2901 da12 576f  owTaskRead)...Wo
-000001c0: 726b 666c 6f77 5461 736b 5570 6461 7465  rkflowTaskUpdate
-000001d0: 6300 0000 0000 0000 0000 0000 0001 0000  c...............
-000001e0: 0008 0000 0043 0000 0073 d000 0000 7400  .....C...s....t.
-000001f0: 6401 6402 8d01 7d00 7401 7c00 8301 0100  d.d...}.t.|.....
-00000200: 7402 a003 7404 a101 8f0d 0100 7400 6403  t...t.......t.d.
-00000210: 6402 8d01 0100 5700 6400 0400 0400 8303  d.....W.d.......
-00000220: 0100 6e08 3100 731e 7701 0100 0100 0100  ..n.1.s.w.......
-00000230: 5900 0100 7400 6401 6401 6404 8d02 7d00  Y...t.d.d.d...}.
-00000240: 7400 6401 6405 6404 8d02 7d00 7402 a003  t.d.d.d...}.t...
-00000250: 7404 a101 8f0e 0100 7400 6401 6403 6404  t.......t.d.d.d.
-00000260: 8d02 0100 5700 6400 0400 0400 8303 0100  ....W.d.........
-00000270: 6e08 3100 7345 7701 0100 0100 0100 5900  n.1.sEw.......Y.
-00000280: 0100 7402 a003 7404 a101 8f0f 0100 7400  ..t...t.......t.
-00000290: 6401 6400 6404 8d02 0100 5700 6400 0400  d.d.d.....W.d...
-000002a0: 0400 8303 0100 6400 5300 3100 7361 7701  ......d.S.1.saw.
-000002b0: 0100 0100 0100 5900 0100 6400 5300 2906  ......Y...d.S.).
-000002c0: 4ee9 0100 0000 2901 da07 7461 736b 5f69  N.....)...task_i
-000002d0: 64e9 ffff ffff 2902 720e 0000 00da 056f  d.....).r......o
-000002e0: 7264 6572 7201 0000 0029 0572 0900 0000  rderr....).r....
-000002f0: 7202 0000 00da 0670 7974 6573 74da 0672  r......pytest..r
-00000300: 6169 7365 7372 0300 0000 a901 da01 74a9  aisesr........t.
-00000310: 0072 1500 0000 fa51 2f68 6f6d 652f 746f  .r.....Q/home/to
-00000320: 6d6d 6173 6f2f 4672 6163 7461 6c2f 6672  mmaso/Fractal/fr
-00000330: 6163 7461 6c2d 7365 7276 6572 2f66 7261  actal-server/fra
-00000340: 6374 616c 5f73 6572 7665 722f 636f 6d6d  ctal_server/comm
-00000350: 6f6e 2f74 6573 7473 2f74 6573 745f 776f  on/tests/test_wo
-00000360: 726b 666c 6f77 2e70 79da 1974 6573 745f  rkflow.py..test_
-00000370: 776f 726b 666c 6f77 5f74 6173 6b5f 6372  workflow_task_cr
-00000380: 6561 7465 1000 0000 731a 0000 000a 0208  eate....s.......
-00000390: 010c 020c 011c ff0c 030c 010c 010e 011c  ................
-000003a0: ff0c 020e 0122 ff72 1700 0000 6300 0000  .....".r....c...
-000003b0: 0000 0000 0000 0000 0001 0000 0008 0000  ................
-000003c0: 0043 0000 0073 5600 0000 7400 7401 6401  .C...sV...t.t.d.
-000003d0: 6402 8d01 6403 8d01 7d00 7402 a003 7404  d...d...}.t...t.
-000003e0: a101 8f10 0100 7400 7401 6404 6405 8d01  ......t.t.d.d...
-000003f0: 6403 8d01 7d00 5700 6400 0400 0400 8303  d...}.W.d.......
-00000400: 0100 6e08 3100 7320 7701 0100 0100 0100  ..n.1.s w.......
-00000410: 5900 0100 7405 7c00 8301 0100 6400 5300  Y...t.|.....d.S.
-00000420: 2906 4eda 0465 6c73 65a9 01da 0973 6f6d  ).N..else....som
-00000430: 6574 6869 6e67 2901 da04 6d65 7461 da03  ething)...meta..
-00000440: 6e65 7729 01da 1570 6172 616c 6c65 6c69  new)...paralleli
-00000450: 7a61 7469 6f6e 5f6c 6576 656c 2906 720c  zation_level).r.
-00000460: 0000 00da 0464 6963 7472 1100 0000 7212  .....dictr....r.
-00000470: 0000 0072 0300 0000 7202 0000 0072 1300  ...r....r....r..
-00000480: 0000 7215 0000 0072 1500 0000 7216 0000  ..r....r....r...
-00000490: 00da 1974 6573 745f 776f 726b 666c 6f77  ...test_workflow
-000004a0: 5f74 6173 6b5f 7570 6461 7465 2000 0000  _task_update ...
-000004b0: 730a 0000 0010 020c 0212 011c ff0c 0272  s..............r
-000004c0: 1f00 0000 6300 0000 0000 0000 0000 0000  ....c...........
-000004d0: 0001 0000 0004 0000 0043 0000 0073 1800  .........C...s..
-000004e0: 0000 7400 6401 6402 6403 8d02 7d00 7401  ..t.d.d.d...}.t.
-000004f0: 7c00 8301 0100 6400 5300 2904 4eda 0877  |.....d.S.).N..w
-00000500: 6f72 6b66 6c6f 7772 0d00 0000 2902 da04  orkflowr....)...
-00000510: 6e61 6d65 da0a 7072 6f6a 6563 745f 6964  name..project_id
-00000520: 2902 7206 0000 0072 0200 0000 a901 da01  ).r....r........
-00000530: 7772 1500 0000 7215 0000 0072 1600 0000  wr....r....r....
-00000540: da14 7465 7374 5f77 6f72 6b66 6c6f 775f  ..test_workflow_
-00000550: 6372 6561 7465 2900 0000 7304 0000 000c  create)...s.....
-00000560: 010c 0172 2500 0000 6300 0000 0000 0000  ...r%...c.......
-00000570: 0000 0000 0003 0000 0008 0000 0043 0000  .............C..
-00000580: 0073 6a00 0000 7400 6401 6402 6403 8d02  .sj...t.d.d.d...
-00000590: 7d00 7401 7c00 6404 8d01 7d01 7402 6405  }.t.|.d...}.t.d.
-000005a0: 7c01 6701 6406 8d02 7d02 7403 7c02 8301  |.g.d...}.t.|...
-000005b0: 0100 7404 a005 7406 a101 8f10 0100 7402  ..t...t.......t.
-000005c0: 6407 7c01 6701 6406 8d02 0100 5700 6400  d.|.g.d.....W.d.
-000005d0: 0400 0400 8303 0100 6400 5300 3100 732e  ........d.S.1.s.
-000005e0: 7701 0100 0100 0100 5900 0100 6400 5300  w.......Y...d.S.
-000005f0: 2908 4e72 2100 0000 da06 736f 7572 6365  ).Nr!.....source
-00000600: 2902 7221 0000 0072 2600 0000 2901 da04  ).r!...r&...)...
-00000610: 7461 736b 7220 0000 0029 0272 2100 0000  taskr ...).r!...
-00000620: da09 7461 736b 5f6c 6973 74da 0120 2907  ..task_list.. ).
-00000630: 7204 0000 0072 0a00 0000 7207 0000 0072  r....r....r....r
-00000640: 0200 0000 7211 0000 0072 1200 0000 7203  ....r....r....r.
-00000650: 0000 0029 0372 1400 0000 da03 7766 7472  ...).r......wftr
-00000660: 2400 0000 7215 0000 0072 1500 0000 7216  $...r....r....r.
-00000670: 0000 00da 1474 6573 745f 776f 726b 666c  .....test_workfl
-00000680: 6f77 5f69 6d70 6f72 742e 0000 0073 0e00  ow_import....s..
-00000690: 0000 0c02 0a01 0e01 0801 0c02 1001 22ff  ..............".
-000006a0: 722b 0000 0063 0000 0000 0000 0000 0000  r+...c..........
-000006b0: 0000 0100 0000 0600 0000 4300 0000 731c  ..........C...s.
-000006c0: 0000 0074 0064 0164 0264 0167 0064 038d  ...t.d.d.d.g.d..
-000006d0: 047d 0074 017c 0083 0101 0064 0053 0029  .}.t.|.....d.S.)
-000006e0: 044e 720d 0000 0072 2000 0000 a904 da02  .Nr....r .......
-000006f0: 6964 7221 0000 0072 2200 0000 7228 0000  idr!...r"...r(..
-00000700: 0029 0272 0800 0000 7202 0000 0072 2300  .).r....r....r#.
-00000710: 0000 7215 0000 0072 1500 0000 7216 0000  ..r....r....r...
-00000720: 00da 2274 6573 745f 776f 726b 666c 6f77  .."test_workflow
-00000730: 5f72 6561 645f 656d 7074 795f 7461 736b  _read_empty_task
-00000740: 5f6c 6973 7439 0000 0073 0400 0000 1001  _list9...s......
-00000750: 0c01 722e 0000 0063 0000 0000 0000 0000  ..r....c........
-00000760: 0000 0000 0400 0000 0a00 0000 4300 0000  ............C...
-00000770: 735c 0000 0074 0064 0164 0264 0364 0464  s\...t.d.d.d.d.d
-00000780: 0564 0674 0164 0764 088d 0164 098d 077d  .d.t.d.d...d...}
-00000790: 0074 0264 0a64 0a64 0a7c 0064 0b8d 047d  .t.d.d.d.|.d...}
-000007a0: 0174 0264 0c64 0a64 0a7c 0064 0b8d 047d  .t.d.d.d.|.d...}
-000007b0: 0274 0364 0a64 0d64 0a7c 017c 0267 0264  .t.d.d.d.|.|.g.d
-000007c0: 0e8d 047d 0374 047c 0383 0101 0064 0053  ...}.t.|.....d.S
-000007d0: 0029 0f4e e909 0000 0072 2100 0000 7226  .).N.....r!...r&
-000007e0: 0000 00da 0763 6f6d 6d61 6e64 da0a 696e  .....command..in
-000007f0: 7075 745f 7479 7065 da0b 6f75 7470 7574  put_type..output
-00000800: 5f74 7970 6572 1800 0000 7219 0000 0029  _typer....r....)
-00000810: 0772 2d00 0000 7221 0000 0072 2600 0000  .r-...r!...r&...
-00000820: 7230 0000 0072 3100 0000 7232 0000 0072  r0...r1...r2...r
-00000830: 1b00 0000 720d 0000 0029 0472 2d00 0000  ....r....).r-...
-00000840: 720e 0000 00da 0b77 6f72 6b66 6c6f 775f  r......workflow_
-00000850: 6964 7227 0000 00e9 0200 0000 7220 0000  idr'........r ..
-00000860: 0072 2c00 0000 2905 7205 0000 0072 1e00  .r,...).r....r..
-00000870: 0000 720b 0000 0072 0800 0000 7202 0000  ..r....r....r...
-00000880: 0029 04da 0274 31da 0477 6674 31da 0477  .)...t1..wft1..w
-00000890: 6674 3272 2400 0000 7215 0000 0072 1500  ft2r$...r....r..
-000008a0: 0000 7216 0000 00da 2674 6573 745f 776f  ..r.....&test_wo
-000008b0: 726b 666c 6f77 5f72 6561 645f 6e6f 6e5f  rkflow_read_non_
-000008c0: 656d 7074 795f 7461 736b 5f6c 6973 743e  empty_task_list>
-000008d0: 0000 0073 1e00 0000 0202 0201 0201 0201  ...s............
-000008e0: 0201 0201 0201 0801 06f9 100a 1001 0202  ................
-000008f0: 0c01 06ff 0c03 7238 0000 0029 1bda 0862  ......r8...)...b
-00000900: 7569 6c74 696e 73da 0c40 7079 5f62 7569  uiltins..@py_bui
-00000910: 6c74 696e 73da 195f 7079 7465 7374 2e61  ltins.._pytest.a
-00000920: 7373 6572 7469 6f6e 2e72 6577 7269 7465  ssertion.rewrite
-00000930: da09 6173 7365 7274 696f 6eda 0772 6577  ..assertion..rew
-00000940: 7269 7465 da0a 4070 7974 6573 745f 6172  rite..@pytest_ar
-00000950: 7211 0000 00da 0864 6576 746f 6f6c 7372  r......devtoolsr
-00000960: 0200 0000 da17 7079 6461 6e74 6963 2e65  ......pydantic.e
-00000970: 7272 6f72 5f77 7261 7070 6572 7372 0300  rror_wrappersr..
-00000980: 0000 da07 7363 6865 6d61 7372 0400 0000  ....schemasr....
-00000990: 7205 0000 0072 0600 0000 7207 0000 0072  r....r....r....r
-000009a0: 0800 0000 7209 0000 0072 0a00 0000 720b  ....r....r....r.
-000009b0: 0000 0072 0c00 0000 7217 0000 0072 1f00  ...r....r....r..
-000009c0: 0000 7225 0000 0072 2b00 0000 722e 0000  ..r%...r+...r...
-000009d0: 0072 3800 0000 7215 0000 0072 1500 0000  .r8...r....r....
-000009e0: 7215 0000 0072 1600 0000 da08 3c6d 6f64  r....r......<mod
-000009f0: 756c 653e 0100 0000 7324 0000 0022 000c  ule>....s$..."..
-00000a00: 010c 010c 020c 010c 010c 010c 010c 010c  ................
-00000a10: 010c 010c 0108 0308 1008 0908 0508 0b0c  ................
-00000a20: 05                                       .
+000000d0: 5a14 0100 6400 640d 6c0b 6d15 5a15 0100  Z...d.d.l.m.Z...
+000000e0: 640e 640f 8400 5a16 6410 6411 8400 5a17  d.d...Z.d.d...Z.
+000000f0: 6412 6413 8400 5a18 6414 6415 8400 5a19  d.d...Z.d.d...Z.
+00000100: 6416 6417 8400 5a1a 6418 6419 8400 5a1b  d.d...Z.d.d...Z.
+00000110: 641a 641b 8400 5a1c 6401 5300 291c e900  d.d...Z.d.S.)...
+00000120: 0000 004e 2901 da05 6465 6275 6729 01da  ...N)...debug)..
+00000130: 0f56 616c 6964 6174 696f 6e45 7272 6f72  .ValidationError
+00000140: 2901 da0a 5461 736b 496d 706f 7274 2901  )...TaskImport).
+00000150: da08 5461 736b 5265 6164 2901 da0e 576f  ..TaskRead)...Wo
+00000160: 726b 666c 6f77 4372 6561 7465 2901 da0e  rkflowCreate)...
+00000170: 576f 726b 666c 6f77 496d 706f 7274 2901  WorkflowImport).
+00000180: da0c 576f 726b 666c 6f77 5265 6164 2901  ..WorkflowRead).
+00000190: da12 576f 726b 666c 6f77 5461 736b 4372  ..WorkflowTaskCr
+000001a0: 6561 7465 2901 da12 576f 726b 666c 6f77  eate)...Workflow
+000001b0: 5461 736b 496d 706f 7274 2901 da10 576f  TaskImport)...Wo
+000001c0: 726b 666c 6f77 5461 736b 5265 6164 2901  rkflowTaskRead).
+000001d0: da12 576f 726b 666c 6f77 5461 736b 5570  ..WorkflowTaskUp
+000001e0: 6461 7465 2901 da0e 576f 726b 666c 6f77  date)...Workflow
+000001f0: 5570 6461 7465 6300 0000 0000 0000 0000  Updatec.........
+00000200: 0000 0001 0000 0008 0000 0043 0000 0073  ...........C...s
+00000210: 8000 0000 7400 6401 6402 8d01 7d00 7401  ....t.d.d...}.t.
+00000220: 7c00 8301 0100 7402 a003 7404 a101 8f0d  |.....t...t.....
+00000230: 0100 7400 6403 6402 8d01 0100 5700 6400  ..t.d.d.....W.d.
+00000240: 0400 0400 8303 0100 6e08 3100 731e 7701  ........n.1.s.w.
+00000250: 0100 0100 0100 5900 0100 7402 a003 7404  ......Y...t...t.
+00000260: a101 8f0e 0100 7400 6400 6402 8d01 0100  ......t.d.d.....
+00000270: 5700 6400 0400 0400 8303 0100 6400 5300  W.d.........d.S.
+00000280: 3100 7339 7701 0100 0100 0100 5900 0100  1.s9w.......Y...
+00000290: 6400 5300 2904 4ee9 0100 0000 2901 da05  d.S.).N.....)...
+000002a0: 6f72 6465 72e9 ffff ffff 2905 7209 0000  order.....).r...
+000002b0: 0072 0200 0000 da06 7079 7465 7374 da06  .r......pytest..
+000002c0: 7261 6973 6573 7203 0000 00a9 01da 0174  raisesr........t
+000002d0: a900 7215 0000 00fa 512f 686f 6d65 2f74  ..r.....Q/home/t
+000002e0: 6f6d 6d61 736f 2f46 7261 6374 616c 2f66  ommaso/Fractal/f
+000002f0: 7261 6374 616c 2d73 6572 7665 722f 6672  ractal-server/fr
+00000300: 6163 7461 6c5f 7365 7276 6572 2f63 6f6d  actal_server/com
+00000310: 6d6f 6e2f 7465 7374 732f 7465 7374 5f77  mon/tests/test_w
+00000320: 6f72 6b66 6c6f 772e 7079 da19 7465 7374  orkflow.py..test
+00000330: 5f77 6f72 6b66 6c6f 775f 7461 736b 5f63  _workflow_task_c
+00000340: 7265 6174 6511 0000 0073 1000 0000 0a02  reate....s......
+00000350: 0801 0c02 0c01 1cff 0c02 0c01 22ff 7217  ............".r.
+00000360: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00000370: 0100 0000 0800 0000 4300 0000 7356 0000  ........C...sV..
+00000380: 0074 0074 0164 0164 028d 0164 038d 017d  .t.t.d.d...d...}
+00000390: 0074 02a0 0374 04a1 018f 1001 0074 0074  .t...t.......t.t
+000003a0: 0164 0464 058d 0164 038d 017d 0057 0064  .d.d...d...}.W.d
+000003b0: 0004 0004 0083 0301 006e 0831 0073 2077  .........n.1.s w
+000003c0: 0101 0001 0001 0059 0001 0074 057c 0083  .......Y...t.|..
+000003d0: 0101 0064 0053 0029 064e da04 656c 7365  ...d.S.).N..else
+000003e0: a901 da09 736f 6d65 7468 696e 6729 01da  ....something)..
+000003f0: 046d 6574 61da 036e 6577 2901 da15 7061  .meta..new)...pa
+00000400: 7261 6c6c 656c 697a 6174 696f 6e5f 6c65  rallelization_le
+00000410: 7665 6c29 0672 0c00 0000 da04 6469 6374  vel).r......dict
+00000420: 7211 0000 0072 1200 0000 7203 0000 0072  r....r....r....r
+00000430: 0200 0000 7213 0000 0072 1500 0000 7215  ....r....r....r.
+00000440: 0000 0072 1600 0000 da19 7465 7374 5f77  ...r......test_w
+00000450: 6f72 6b66 6c6f 775f 7461 736b 5f75 7064  orkflow_task_upd
+00000460: 6174 651c 0000 0073 0a00 0000 1002 0c02  ate....s........
+00000470: 1201 1cff 0c02 721f 0000 0063 0000 0000  ......r....c....
+00000480: 0000 0000 0000 0000 0100 0000 0300 0000  ................
+00000490: 4300 0000 7316 0000 0074 0064 0164 028d  C...s....t.d.d..
+000004a0: 017d 0074 017c 0083 0101 0064 0053 0029  .}.t.|.....d.S.)
+000004b0: 034e da08 776f 726b 666c 6f77 a901 da04  .N..workflow....
+000004c0: 6e61 6d65 2902 7206 0000 0072 0200 0000  name).r....r....
+000004d0: a901 da01 7772 1500 0000 7215 0000 0072  ....wr....r....r
+000004e0: 1600 0000 da14 7465 7374 5f77 6f72 6b66  ......test_workf
+000004f0: 6c6f 775f 6372 6561 7465 2500 0000 7304  low_create%...s.
+00000500: 0000 000a 010c 0172 2500 0000 6300 0000  .......r%...c...
+00000510: 0000 0000 0000 0000 0003 0000 0008 0000  ................
+00000520: 0043 0000 0073 6a00 0000 7400 6401 6402  .C...sj...t.d.d.
+00000530: 6403 8d02 7d00 7401 7c00 6404 8d01 7d01  d...}.t.|.d...}.
+00000540: 7402 6405 7c01 6701 6406 8d02 7d02 7403  t.d.|.g.d...}.t.
+00000550: 7c02 8301 0100 7404 a005 7406 a101 8f10  |.....t...t.....
+00000560: 0100 7402 6407 7c01 6701 6406 8d02 0100  ..t.d.|.g.d.....
+00000570: 5700 6400 0400 0400 8303 0100 6400 5300  W.d.........d.S.
+00000580: 3100 732e 7701 0100 0100 0100 5900 0100  1.s.w.......Y...
+00000590: 6400 5300 2908 4e72 2200 0000 da06 736f  d.S.).Nr".....so
+000005a0: 7572 6365 2902 7222 0000 0072 2600 0000  urce).r"...r&...
+000005b0: 2901 da04 7461 736b 7220 0000 0029 0272  )...taskr ...).r
+000005c0: 2200 0000 da09 7461 736b 5f6c 6973 74da  ".....task_list.
+000005d0: 0120 2907 7204 0000 0072 0a00 0000 7207  . ).r....r....r.
+000005e0: 0000 0072 0200 0000 7211 0000 0072 1200  ...r....r....r..
+000005f0: 0000 7203 0000 0029 0372 1400 0000 5a03  ..r....).r....Z.
+00000600: 7766 7472 2400 0000 7215 0000 0072 1500  wftr$...r....r..
+00000610: 0000 7216 0000 00da 1474 6573 745f 776f  ..r......test_wo
+00000620: 726b 666c 6f77 5f69 6d70 6f72 742a 0000  rkflow_import*..
+00000630: 0073 0e00 0000 0c02 0a01 0e01 0801 0c02  .s..............
+00000640: 1001 22ff 722a 0000 0063 0000 0000 0000  ..".r*...c......
+00000650: 0000 0000 0000 0100 0000 0600 0000 4300  ..............C.
+00000660: 0000 731c 0000 0074 0064 0164 0264 0167  ..s....t.d.d.d.g
+00000670: 0064 038d 047d 0074 017c 0083 0101 0064  .d...}.t.|.....d
+00000680: 0053 0029 044e 720e 0000 0072 2000 0000  .S.).Nr....r ...
+00000690: a904 da02 6964 7222 0000 00da 0a70 726f  ....idr".....pro
+000006a0: 6a65 6374 5f69 6472 2800 0000 2902 7208  ject_idr(...).r.
+000006b0: 0000 0072 0200 0000 7223 0000 0072 1500  ...r....r#...r..
+000006c0: 0000 7215 0000 0072 1600 0000 da22 7465  ..r....r....."te
+000006d0: 7374 5f77 6f72 6b66 6c6f 775f 7265 6164  st_workflow_read
+000006e0: 5f65 6d70 7479 5f74 6173 6b5f 6c69 7374  _empty_task_list
+000006f0: 3500 0000 7304 0000 0010 010c 0172 2e00  5...s........r..
+00000700: 0000 6300 0000 0000 0000 0000 0000 0004  ..c.............
+00000710: 0000 000a 0000 0043 0000 0073 5c00 0000  .......C...s\...
+00000720: 7400 6401 6402 6403 6404 6405 6406 7401  t.d.d.d.d.d.d.t.
+00000730: 6407 6408 8d01 6409 8d07 7d00 7402 640a  d.d...d...}.t.d.
+00000740: 640a 640a 7c00 640b 8d04 7d01 7402 640c  d.d.|.d...}.t.d.
+00000750: 640a 640a 7c00 640b 8d04 7d02 7403 640a  d.d.|.d...}.t.d.
+00000760: 640d 640a 7c01 7c02 6702 640e 8d04 7d03  d.d.|.|.g.d...}.
+00000770: 7404 7c03 8301 0100 6400 5300 290f 4ee9  t.|.....d.S.).N.
+00000780: 0900 0000 7222 0000 0072 2600 0000 da07  ....r"...r&.....
+00000790: 636f 6d6d 616e 64da 0a69 6e70 7574 5f74  command..input_t
+000007a0: 7970 65da 0b6f 7574 7075 745f 7479 7065  ype..output_type
+000007b0: 7218 0000 0072 1900 0000 2907 722c 0000  r....r....).r,..
+000007c0: 0072 2200 0000 7226 0000 0072 3000 0000  .r"...r&...r0...
+000007d0: 7231 0000 0072 3200 0000 721b 0000 0072  r1...r2...r....r
+000007e0: 0e00 0000 2904 722c 0000 00da 0774 6173  ....).r,.....tas
+000007f0: 6b5f 6964 da0b 776f 726b 666c 6f77 5f69  k_id..workflow_i
+00000800: 6472 2700 0000 e902 0000 0072 2000 0000  dr'........r ...
+00000810: 722b 0000 0029 0572 0500 0000 721e 0000  r+...).r....r...
+00000820: 0072 0b00 0000 7208 0000 0072 0200 0000  .r....r....r....
+00000830: 2904 da02 7431 5a04 7766 7431 5a04 7766  )...t1Z.wft1Z.wf
+00000840: 7432 7224 0000 0072 1500 0000 7215 0000  t2r$...r....r...
+00000850: 0072 1600 0000 da26 7465 7374 5f77 6f72  .r.....&test_wor
+00000860: 6b66 6c6f 775f 7265 6164 5f6e 6f6e 5f65  kflow_read_non_e
+00000870: 6d70 7479 5f74 6173 6b5f 6c69 7374 3a00  mpty_task_list:.
+00000880: 0000 731e 0000 0002 0202 0102 0102 0102  ..s.............
+00000890: 0102 0102 0108 0106 f910 0a10 0102 020c  ................
+000008a0: 0106 ff0c 0372 3700 0000 6300 0000 0000  .....r7...c.....
+000008b0: 0000 0000 0000 0000 0000 0008 0000 0043  ...............C
+000008c0: 0000 0073 a200 0000 7400 6401 6700 6402  ...s....t.d.g.d.
+000008d0: a201 6403 8d02 0100 7400 6401 6404 8d01  ..d.....t.d.d...
+000008e0: 0100 7400 6700 6402 a201 6405 8d01 0100  ..t.g.d...d.....
+000008f0: 7401 a002 7403 a101 8f10 0100 7400 6401  t...t.......t.d.
+00000900: 6700 6406 a201 6403 8d02 0100 5700 6400  g.d...d.....W.d.
+00000910: 0400 0400 8303 0100 6e08 3100 732c 7701  ........n.1.s,w.
+00000920: 0100 0100 0100 5900 0100 7401 a002 7403  ......Y...t...t.
+00000930: a101 8f11 0100 7400 6401 6700 6407 a201  ......t.d.g.d...
+00000940: 6403 8d02 0100 5700 6400 0400 0400 8303  d.....W.d.......
+00000950: 0100 6400 5300 3100 734a 7701 0100 0100  ..d.S.1.sJw.....
+00000960: 0100 5900 0100 6400 5300 2908 4e72 2000  ..Y...d.S.).Nr .
+00000970: 0000 2904 7201 0000 0072 0e00 0000 e903  ..).r....r......
+00000980: 0000 0072 3500 0000 2902 7222 0000 00da  ...r5...).r"....
+00000990: 1a72 656f 7264 6572 6564 5f77 6f72 6b66  .reordered_workf
+000009a0: 6c6f 7774 6173 6b5f 6964 7372 2100 0000  lowtask_idsr!...
+000009b0: 2901 7239 0000 0029 0372 0e00 0000 7238  ).r9...).r....r8
+000009c0: 0000 0072 0e00 0000 2903 720e 0000 0072  ...r....).r....r
+000009d0: 3800 0000 7210 0000 0029 0472 0d00 0000  8...r....).r....
+000009e0: 7211 0000 0072 1200 0000 7203 0000 0072  r....r....r....r
+000009f0: 1500 0000 7215 0000 0072 1500 0000 7216  ....r....r....r.
+00000a00: 0000 00da 1474 6573 745f 776f 726b 666c  .....test_workfl
+00000a10: 6f77 5f75 7064 6174 654f 0000 0073 1200  ow_updateO...s..
+00000a20: 0000 1001 0a01 0e01 0c01 1201 1cff 0c02  ................
+00000a30: 1201 22ff 723a 0000 0029 1dda 0862 7569  ..".r:...)...bui
+00000a40: 6c74 696e 73da 0c40 7079 5f62 7569 6c74  ltins..@py_built
+00000a50: 696e 73da 195f 7079 7465 7374 2e61 7373  ins.._pytest.ass
+00000a60: 6572 7469 6f6e 2e72 6577 7269 7465 da09  ertion.rewrite..
+00000a70: 6173 7365 7274 696f 6eda 0772 6577 7269  assertion..rewri
+00000a80: 7465 da0a 4070 7974 6573 745f 6172 7211  te..@pytest_arr.
+00000a90: 0000 00da 0864 6576 746f 6f6c 7372 0200  .....devtoolsr..
+00000aa0: 0000 da17 7079 6461 6e74 6963 2e65 7272  ....pydantic.err
+00000ab0: 6f72 5f77 7261 7070 6572 7372 0300 0000  or_wrappersr....
+00000ac0: da07 7363 6865 6d61 7372 0400 0000 7205  ..schemasr....r.
+00000ad0: 0000 0072 0600 0000 7207 0000 0072 0800  ...r....r....r..
+00000ae0: 0000 7209 0000 0072 0a00 0000 720b 0000  ..r....r....r...
+00000af0: 0072 0c00 0000 720d 0000 0072 1700 0000  .r....r....r....
+00000b00: 721f 0000 0072 2500 0000 722a 0000 0072  r....r%...r*...r
+00000b10: 2e00 0000 7237 0000 0072 3a00 0000 7215  ....r7...r:...r.
+00000b20: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
+00000b30: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00000b40: 7328 0000 0022 000c 010c 010c 020c 010c  s(..."..........
+00000b50: 010c 010c 010c 010c 010c 010c 010c 0108  ................
+00000b60: 0308 0b08 0908 0508 0b08 050c 15         .............
```

### Comparing `fractal_server-1.3.0a8/fractal_server/common/tests/test_dataset.py` & `fractal_server-1.3.0a9/fractal_server/common/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/common/tests/test_manifest.py` & `fractal_server-1.3.0a9/fractal_server/common/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/common/tests/test_project.py` & `fractal_server-1.3.0a9/fractal_server/common/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/common/tests/test_state.py` & `fractal_server-1.3.0a9/fractal_server/common/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/common/tests/test_task.py` & `fractal_server-1.3.0a9/fractal_server/common/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/common/tests/test_task_collection.py` & `fractal_server-1.3.0a9/fractal_server/common/tests/test_task_collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/common/tests/test_user.py` & `fractal_server-1.3.0a9/fractal_server/common/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/common/tests/test_workflow.py` & `fractal_server-1.3.0a9/fractal_server/common/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/config.py` & `fractal_server-1.3.0a9/fractal_server/config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/logger.py` & `fractal_server-1.3.0a9/fractal_server/logger.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/main.py` & `fractal_server-1.3.0a9/fractal_server/main.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/migrations/env.py` & `fractal_server-1.3.0a9/fractal_server/migrations/env.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/migrations/script.py.mako` & `fractal_server-1.3.0a9/fractal_server/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py` & `fractal_server-1.3.0a9/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py` & `fractal_server-1.3.0a9/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py` & `fractal_server-1.3.0a9/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/syringe.py` & `fractal_server-1.3.0a9/fractal_server/syringe.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/tasks/collection.py` & `fractal_server-1.3.0a9/fractal_server/tasks/collection.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/fractal_server/utils.py` & `fractal_server-1.3.0a9/fractal_server/utils.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a8/pyproject.toml` & `fractal_server-1.3.0a9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-server"
-version = "1.3.0a8"
+version = "1.3.0a9"
 description = "Server component of the Fractal analytics platform"
 authors = [
     "Jacopo Nespolo <jacopo.nespolo@exact-lab.it>",
     "Marco Franzon <marco.franzon@exact-lab.it>",
     "Tommaso Comparin <tommaso.comparin@exact-lab.it>",
 ]
 readme = "README.md"
@@ -73,15 +73,15 @@
 asyncio_mode = "auto"
 filterwarnings = [
     "error::RuntimeWarning",
     "error::pytest.PytestUnraisableExceptionWarning",
 ]
 
 [tool.bumpver]
-current_version = "1.3.0a8"
+current_version = "1.3.0a9"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fractal_server-1.3.0a8/PKG-INFO` & `fractal_server-1.3.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-server
-Version: 1.3.0a8
+Version: 1.3.0a9
 Summary: Server component of the Fractal analytics platform
 Home-page: https://github.com/fractal-analytics-platform/fractal-server
 License: BSD-3-Clause
 Author: Jacopo Nespolo
 Author-email: jacopo.nespolo@exact-lab.it
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
```


# Comparing `tmp/aiida_core-2.3.1.tar.gz` & `tmp/aiida_core-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida_core-2.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aiida_core-2.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiida_core-2.3.1.tar` & `aiida_core-2.4.0.tar`

### file list

```diff
@@ -1,680 +1,680 @@
--rw-r--r--   0        0        0      539 2023-05-22 21:50:10.259921 aiida_core-2.3.1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0      347 2023-05-22 21:50:10.259921 aiida_core-2.3.1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1056 2023-05-22 21:50:10.259921 aiida_core-2.3.1/.devcontainer/docker-compose.yml
--rw-r--r--   0        0        0       56 2023-05-22 21:50:10.259921 aiida_core-2.3.1/.devcontainer/post_create.sh
--rw-r--r--   0        0        0      759 2023-05-22 21:50:10.259921 aiida_core-2.3.1/.docker/docker-rabbitmq.yml
--rwxr-xr-x   0        0        0       66 2023-05-22 21:50:10.259921 aiida_core-2.3.1/.docker/my_init.d/configure-aiida.sh
--rwxr-xr-x   0        0        0     3773 2023-05-22 21:50:10.259921 aiida_core-2.3.1/.docker/opt/configure-aiida.sh
--rw-r--r--   0        0        0      155 2023-05-22 21:50:10.259921 aiida_core-2.3.1/.dockerignore
--rw-r--r--   0        0        0      649 2023-05-22 21:50:10.259921 aiida_core-2.3.1/.github/CODEOWNERS
--rw-r--r--   0        0        0      972 2023-05-22 21:50:10.259921 aiida_core-2.3.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      275 2023-05-22 21:50:10.259921 aiida_core-2.3.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      434 2023-05-22 21:50:10.259921 aiida_core-2.3.1/.github/ISSUE_TEMPLATE/doc-improvements.md
--rw-r--r--   0        0        0      754 2023-05-22 21:50:10.259921 aiida_core-2.3.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      181 2023-05-22 21:50:10.259921 aiida_core-2.3.1/.github/config/README.md
--rw-r--r--   0        0        0      307 2023-05-22 21:50:10.259921 aiida_core-2.3.1/.github/config/add-singularity.yaml
--rw-r--r--   0        0        0      163 2023-05-22 21:50:10.259921 aiida_core-2.3.1/.github/config/add.yaml
--rwxr-xr-x   0        0        0      347 2023-05-22 21:50:10.259921 aiida_core-2.3.1/.github/config/doubler.sh
--rw-r--r--   0        0        0      199 2023-05-22 21:50:10.259921 aiida_core-2.3.1/.github/config/doubler.yaml
--rw-r--r--   0        0        0       43 2023-05-22 21:50:10.259921 aiida_core-2.3.1/.github/config/localhost-config.yaml
--rw-r--r--   0        0        0      274 2023-05-22 21:50:10.259921 aiida_core-2.3.1/.github/config/localhost.yaml
--rw-r--r--   0        0        0      453 2023-05-22 21:50:10.259921 aiida_core-2.3.1/.github/config/profile.yaml
--rw-r--r--   0        0        0      130 2023-05-22 21:50:10.259921 aiida_core-2.3.1/.github/config/slurm-ssh-config.yaml
--rw-r--r--   0        0        0      275 2023-05-22 21:50:10.259921 aiida_core-2.3.1/.github/config/slurm-ssh.yaml
--rw-r--r--   0        0        0     1679 2023-05-22 21:50:10.259921 aiida_core-2.3.1/.github/config/slurm_rsa
--rw-r--r--   0        0        0      202 2023-05-22 21:50:10.259921 aiida_core-2.3.1/.github/system_tests/README.md
--rw-r--r--   0        0        0     3176 2023-05-22 21:50:10.259921 aiida_core-2.3.1/.github/system_tests/pytest/test_memory_leaks.py
--rw-r--r--   0        0        0     1387 2023-05-22 21:50:10.259921 aiida_core-2.3.1/.github/system_tests/test_containerized_code.py
--rw-r--r--   0        0        0    24024 2023-05-22 21:50:10.259921 aiida_core-2.3.1/.github/system_tests/test_daemon.py
--rw-r--r--   0        0        0     1126 2023-05-22 21:50:10.259921 aiida_core-2.3.1/.github/system_tests/test_ipython_magics.py
--rwxr-xr-x   0        0        0      911 2023-05-22 21:50:10.263921 aiida_core-2.3.1/.github/system_tests/test_polish_workchains.sh
--rw-r--r--   0        0        0     3912 2023-05-22 21:50:10.263921 aiida_core-2.3.1/.github/system_tests/test_profile_manager.py
--rw-r--r--   0        0        0     1972 2023-05-22 21:50:10.263921 aiida_core-2.3.1/.github/system_tests/test_test_manager.py
--rwxr-xr-x   0        0        0     1611 2023-05-22 21:50:10.263921 aiida_core-2.3.1/.github/system_tests/test_verdi_load_time.sh
--rw-r--r--   0        0        0     8572 2023-05-22 21:50:10.263921 aiida_core-2.3.1/.github/system_tests/workchains.py
--rw-r--r--   0        0        0     1901 2023-05-22 21:50:10.263921 aiida_core-2.3.1/.github/workflows/benchmark-config.json
--rw-r--r--   0        0        0     2226 2023-05-22 21:50:10.263921 aiida_core-2.3.1/.github/workflows/benchmark.yml
--rw-r--r--   0        0        0     1719 2023-05-22 21:50:10.263921 aiida_core-2.3.1/.github/workflows/build_and_test_docker_on_pr.yml
--rw-r--r--   0        0        0     1327 2023-05-22 21:50:10.263921 aiida_core-2.3.1/.github/workflows/check_release_tag.py
--rw-r--r--   0        0        0     3561 2023-05-22 21:50:10.263921 aiida_core-2.3.1/.github/workflows/ci-code.yml
--rw-r--r--   0        0        0      888 2023-05-22 21:50:10.263921 aiida_core-2.3.1/.github/workflows/ci-style.yml
--rw-r--r--   0        0        0     1086 2023-05-22 21:50:10.263921 aiida_core-2.3.1/.github/workflows/docs-build.yml
--rw-r--r--   0        0        0     3477 2023-05-22 21:50:10.263921 aiida_core-2.3.1/.github/workflows/nightly.yml
--rw-r--r--   0        0        0     1803 2023-05-22 21:50:10.263921 aiida_core-2.3.1/.github/workflows/post-release.yml
--rw-r--r--   0        0        0     1377 2023-05-22 21:50:10.263921 aiida_core-2.3.1/.github/workflows/push_image_to_dockerhub.yml
--rw-r--r--   0        0        0     1696 2023-05-22 21:50:10.263921 aiida_core-2.3.1/.github/workflows/rabbitmq.yml
--rw-r--r--   0        0        0     3095 2023-05-22 21:50:10.263921 aiida_core-2.3.1/.github/workflows/release.yml
--rwxr-xr-x   0        0        0     1814 2023-05-22 21:50:10.263921 aiida_core-2.3.1/.github/workflows/setup.sh
--rw-r--r--   0        0        0    11253 2023-05-22 21:50:10.263921 aiida_core-2.3.1/.github/workflows/test-install.yml
--rwxr-xr-x   0        0        0      898 2023-05-22 21:50:10.263921 aiida_core-2.3.1/.github/workflows/tests.sh
--rwxr-xr-x   0        0        0      589 2023-05-22 21:50:10.263921 aiida_core-2.3.1/.github/workflows/tests_nightly.sh
--rwxr-xr-x   0        0        0     2135 2023-05-22 21:50:10.263921 aiida_core-2.3.1/.github/workflows/verdi.sh
--rw-r--r--   0        0        0      427 2023-05-22 21:50:10.263921 aiida_core-2.3.1/.gitignore
--rw-r--r--   0        0        0     2005 2023-05-22 21:50:10.263921 aiida_core-2.3.1/.molecule/README.md
--rw-r--r--   0        0        0      413 2023-05-22 21:50:10.263921 aiida_core-2.3.1/.molecule/default/Dockerfile
--rw-r--r--   0        0        0     1790 2023-05-22 21:50:10.263921 aiida_core-2.3.1/.molecule/default/config_local.yml
--rw-r--r--   0        0        0     6342 2023-05-22 21:50:10.263921 aiida_core-2.3.1/.molecule/default/create_docker.yml
--rw-r--r--   0        0        0      632 2023-05-22 21:50:10.263921 aiida_core-2.3.1/.molecule/default/files/polish/__init__.py
--rwxr-xr-x   0        0        0     7706 2023-05-22 21:50:10.263921 aiida_core-2.3.1/.molecule/default/files/polish/cli.py
--rw-r--r--   0        0        0      632 2023-05-22 21:50:10.263921 aiida_core-2.3.1/.molecule/default/files/polish/lib/__init__.py
--rw-r--r--   0        0        0     5384 2023-05-22 21:50:10.263921 aiida_core-2.3.1/.molecule/default/files/polish/lib/expression.py
--rw-r--r--   0        0        0     1032 2023-05-22 21:50:10.263921 aiida_core-2.3.1/.molecule/default/files/polish/lib/template/base.tpl
--rw-r--r--   0        0        0     5300 2023-05-22 21:50:10.263921 aiida_core-2.3.1/.molecule/default/files/polish/lib/template/workchain.tpl
--rw-r--r--   0        0        0     8117 2023-05-22 21:50:10.263921 aiida_core-2.3.1/.molecule/default/files/polish/lib/workchain.py
--rw-r--r--   0        0        0       46 2023-05-22 21:50:10.263921 aiida_core-2.3.1/.molecule/default/run_tests.yml
--rw-r--r--   0        0        0     2717 2023-05-22 21:50:10.263921 aiida_core-2.3.1/.molecule/default/setup_aiida.yml
--rw-r--r--   0        0        0      716 2023-05-22 21:50:10.263921 aiida_core-2.3.1/.molecule/default/setup_python.yml
--rw-r--r--   0        0        0     1650 2023-05-22 21:50:10.263921 aiida_core-2.3.1/.molecule/default/tasks/log_query_stats.yml
--rw-r--r--   0        0        0      239 2023-05-22 21:50:10.263921 aiida_core-2.3.1/.molecule/default/tasks/reset_query_stats.yml
--rw-r--r--   0        0        0     2814 2023-05-22 21:50:10.263921 aiida_core-2.3.1/.molecule/default/test_polish_workchains.yml
--rw-r--r--   0        0        0     9312 2023-05-22 21:50:10.263921 aiida_core-2.3.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      802 2023-05-22 21:50:10.263921 aiida_core-2.3.1/.readthedocs.yml
--rw-r--r--   0        0        0     1746 2023-05-22 21:50:10.263921 aiida_core-2.3.1/AUTHORS.txt
--rw-r--r--   0        0        0   201927 2023-05-22 21:50:10.263921 aiida_core-2.3.1/CHANGELOG.md
--rw-r--r--   0        0        0     3352 2023-05-22 21:50:10.263921 aiida_core-2.3.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      585 2023-05-22 21:50:10.263921 aiida_core-2.3.1/Dockerfile
--rw-r--r--   0        0        0     1312 2023-05-22 21:50:10.263921 aiida_core-2.3.1/LICENSE.txt
--rw-r--r--   0        0        0     6031 2023-05-22 21:50:10.263921 aiida_core-2.3.1/README.md
--rw-r--r--   0        0        0     3610 2023-05-22 21:50:10.263921 aiida_core-2.3.1/aiida/__init__.py
--rw-r--r--   0        0        0      807 2023-05-22 21:50:10.263921 aiida_core-2.3.1/aiida/__main__.py
--rw-r--r--   0        0        0      632 2023-05-22 21:50:10.263921 aiida_core-2.3.1/aiida/calculations/__init__.py
--rw-r--r--   0        0        0      632 2023-05-22 21:50:10.263921 aiida_core-2.3.1/aiida/calculations/arithmetic/__init__.py
--rw-r--r--   0        0        0     3907 2023-05-22 21:50:10.263921 aiida_core-2.3.1/aiida/calculations/arithmetic/add.py
--rw-r--r--   0        0        0     2547 2023-05-22 21:50:10.263921 aiida_core-2.3.1/aiida/calculations/diff_tutorial/calculations.py
--rw-r--r--   0        0        0        0 2023-05-22 21:50:10.263921 aiida_core-2.3.1/aiida/calculations/importers/__init__.py
--rw-r--r--   0        0        0        0 2023-05-22 21:50:10.263921 aiida_core-2.3.1/aiida/calculations/importers/arithmetic/__init__.py
--rw-r--r--   0        0        0     1644 2023-05-22 21:50:10.263921 aiida_core-2.3.1/aiida/calculations/importers/arithmetic/add.py
--rw-r--r--   0        0        0        0 2023-05-22 21:50:10.263921 aiida_core-2.3.1/aiida/calculations/monitors/__init__.py
--rw-r--r--   0        0        0     1161 2023-05-22 21:50:10.263921 aiida_core-2.3.1/aiida/calculations/monitors/base.py
--rw-r--r--   0        0        0     9273 2023-05-22 21:50:10.263921 aiida_core-2.3.1/aiida/calculations/templatereplacer.py
--rw-r--r--   0        0        0    10738 2023-05-22 21:50:10.263921 aiida_core-2.3.1/aiida/calculations/transfer.py
--rw-r--r--   0        0        0     1734 2023-05-22 21:50:10.263921 aiida_core-2.3.1/aiida/cmdline/__init__.py
--rw-r--r--   0        0        0     1194 2023-05-22 21:50:10.263921 aiida_core-2.3.1/aiida/cmdline/commands/__init__.py
--rw-r--r--   0        0        0    19446 2023-05-22 21:50:10.263921 aiida_core-2.3.1/aiida/cmdline/commands/cmd_archive.py
--rw-r--r--   0        0        0    14555 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/commands/cmd_calcjob.py
--rw-r--r--   0        0        0    14735 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/commands/cmd_code.py
--rw-r--r--   0        0        0    26949 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/commands/cmd_computer.py
--rw-r--r--   0        0        0     7913 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/commands/cmd_config.py
--rw-r--r--   0        0        0    10683 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/commands/cmd_daemon.py
--rw-r--r--   0        0        0      931 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/commands/cmd_data/__init__.py
--rw-r--r--   0        0        0     1337 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/commands/cmd_data/cmd_array.py
--rw-r--r--   0        0        0     4808 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/commands/cmd_data/cmd_bands.py
--rw-r--r--   0        0        0     4392 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/commands/cmd_data/cmd_cif.py
--rw-r--r--   0        0        0     1219 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/commands/cmd_data/cmd_dict.py
--rw-r--r--   0        0        0     4692 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/commands/cmd_data/cmd_export.py
--rw-r--r--   0        0        0     2889 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/commands/cmd_data/cmd_list.py
--rw-r--r--   0        0        0     3599 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/commands/cmd_data/cmd_remote.py
--rw-r--r--   0        0        0     8026 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/commands/cmd_data/cmd_show.py
--rw-r--r--   0        0        0     1341 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/commands/cmd_data/cmd_singlefile.py
--rw-r--r--   0        0        0     8890 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/commands/cmd_data/cmd_structure.py
--rw-r--r--   0        0        0     3575 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/commands/cmd_data/cmd_trajectory.py
--rw-r--r--   0        0        0     5209 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/commands/cmd_data/cmd_upf.py
--rw-r--r--   0        0        0     4761 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/commands/cmd_database.py
--rw-r--r--   0        0        0     7557 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/commands/cmd_devel.py
--rw-r--r--   0        0        0    18115 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/commands/cmd_group.py
--rw-r--r--   0        0        0     1392 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/commands/cmd_help.py
--rw-r--r--   0        0        0    20026 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/commands/cmd_node.py
--rw-r--r--   0        0        0     2950 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/commands/cmd_plugin.py
--rw-r--r--   0        0        0    12108 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/commands/cmd_process.py
--rw-r--r--   0        0        0     5739 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/commands/cmd_profile.py
--rw-r--r--   0        0        0    14051 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/commands/cmd_rabbitmq.py
--rw-r--r--   0        0        0     2530 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/commands/cmd_restapi.py
--rw-r--r--   0        0        0     4837 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/commands/cmd_run.py
--rw-r--r--   0        0        0     9391 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/commands/cmd_setup.py
--rw-r--r--   0        0        0     3439 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/commands/cmd_shell.py
--rw-r--r--   0        0        0     6934 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/commands/cmd_status.py
--rw-r--r--   0        0        0     6707 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/commands/cmd_storage.py
--rw-r--r--   0        0        0     4582 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/commands/cmd_user.py
--rw-r--r--   0        0        0     1265 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/commands/cmd_verdi.py
--rw-r--r--   0        0        0      297 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/groups/__init__.py
--rw-r--r--   0        0        0     5345 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/groups/dynamic.py
--rw-r--r--   0        0        0     6501 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/groups/verdi.py
--rw-r--r--   0        0        0     1373 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/params/__init__.py
--rw-r--r--   0        0        0     1277 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/params/arguments/__init__.py
--rw-r--r--   0        0        0     2924 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/params/arguments/main.py
--rw-r--r--   0        0        0     2374 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/params/arguments/overridable.py
--rw-r--r--   0        0        0     2652 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/params/options/__init__.py
--rw-r--r--   0        0        0      697 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/params/options/commands/__init__.py
--rw-r--r--   0        0        0     6869 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/params/options/commands/code.py
--rw-r--r--   0        0        0     6882 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/params/options/commands/computer.py
--rw-r--r--   0        0        0    13950 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/params/options/commands/setup.py
--rw-r--r--   0        0        0     2383 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/params/options/conditional.py
--rw-r--r--   0        0        0     8083 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/params/options/config.py
--rw-r--r--   0        0        0     9190 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/params/options/interactive.py
--rw-r--r--   0        0        0    21132 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/params/options/main.py
--rw-r--r--   0        0        0     3764 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/params/options/multivalue.py
--rw-r--r--   0        0        0     3918 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/params/options/overridable.py
--rw-r--r--   0        0        0     1739 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/params/types/__init__.py
--rw-r--r--   0        0        0     1348 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/params/types/calculation.py
--rw-r--r--   0        0        0     2364 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/params/types/choice.py
--rw-r--r--   0        0        0     2742 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/params/types/code.py
--rw-r--r--   0        0        0     4052 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/params/types/computer.py
--rw-r--r--   0        0        0     1714 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/params/types/config.py
--rw-r--r--   0        0        0     1311 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/params/types/data.py
--rw-r--r--   0        0        0     3901 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/params/types/group.py
--rw-r--r--   0        0        0     6199 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/params/types/identifier.py
--rw-r--r--   0        0        0     1568 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/params/types/multiple.py
--rw-r--r--   0        0        0     1317 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/params/types/node.py
--rw-r--r--   0        0        0     4488 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/params/types/path.py
--rw-r--r--   0        0        0    10750 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/params/types/plugin.py
--rw-r--r--   0        0        0     1329 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/params/types/process.py
--rw-r--r--   0        0        0     3766 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/params/types/profile.py
--rw-r--r--   0        0        0     3800 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/params/types/strings.py
--rw-r--r--   0        0        0     2058 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/params/types/user.py
--rw-r--r--   0        0        0     1335 2023-05-22 21:50:10.267921 aiida_core-2.3.1/aiida/cmdline/params/types/workflow.py
--rw-r--r--   0        0        0      177 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/cmdline/templates/deprecated.tpl
--rw-r--r--   0        0        0      218 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/cmdline/templates/multiline.tpl
--rw-r--r--   0        0        0      213 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/cmdline/templates/new_cmt.txt.tpl
--rw-r--r--   0        0        0      165 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/cmdline/templates/warning.tpl
--rw-r--r--   0        0        0     1122 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/cmdline/utils/__init__.py
--rw-r--r--   0        0        0     4001 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/cmdline/utils/ascii_vis.py
--rw-r--r--   0        0        0    17700 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/cmdline/utils/common.py
--rw-r--r--   0        0        0     9347 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/cmdline/utils/decorators.py
--rw-r--r--   0        0        0     1764 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/cmdline/utils/defaults.py
--rw-r--r--   0        0        0    10878 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/cmdline/utils/echo.py
--rw-r--r--   0        0        0     1710 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/cmdline/utils/log.py
--rw-r--r--   0        0        0     2336 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/cmdline/utils/multi_line_input.py
--rw-r--r--   0        0        0     2709 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/cmdline/utils/pluginable.py
--rw-r--r--   0        0        0      632 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/cmdline/utils/query/__init__.py
--rw-r--r--   0        0        0      981 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/cmdline/utils/query/calculation.py
--rw-r--r--   0        0        0     1026 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/cmdline/utils/query/formatting.py
--rw-r--r--   0        0        0     1007 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/cmdline/utils/query/mapping.py
--rw-r--r--   0        0        0     1393 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/cmdline/utils/repository.py
--rw-r--r--   0        0        0     5008 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/cmdline/utils/shell.py
--rw-r--r--   0        0        0      831 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/cmdline/utils/templates.py
--rw-r--r--   0        0        0     2634 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/common/__init__.py
--rw-r--r--   0        0        0    12464 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/common/constants.py
--rw-r--r--   0        0        0     8031 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/common/datastructures.py
--rw-r--r--   0        0        0     6332 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/common/escaping.py
--rw-r--r--   0        0        0     8794 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/common/exceptions.py
--rw-r--r--   0        0        0     8975 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/common/extendeddicts.py
--rw-r--r--   0        0        0     3067 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/common/files.py
--rw-r--r--   0        0        0    18668 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/common/folders.py
--rw-r--r--   0        0        0    10933 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/common/hashing.py
--rw-r--r--   0        0        0     2803 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/common/json.py
--rw-r--r--   0        0        0     3717 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/common/lang.py
--rw-r--r--   0        0        0     6586 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/common/links.py
--rw-r--r--   0        0        0     9703 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/common/log.py
--rw-r--r--   0        0        0     6909 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/common/progress_reporter.py
--rw-r--r--   0        0        0     2800 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/common/timezone.py
--rw-r--r--   0        0        0    19341 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/common/utils.py
--rw-r--r--   0        0        0     1888 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/common/warnings.py
--rw-r--r--   0        0        0     1996 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/engine/__init__.py
--rw-r--r--   0        0        0      819 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/engine/daemon/__init__.py
--rw-r--r--   0        0        0    31629 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/engine/daemon/client.py
--rw-r--r--   0        0        0    31263 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/engine/daemon/execmanager.py
--rw-r--r--   0        0        0     2295 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/engine/daemon/worker.py
--rw-r--r--   0        0        0      919 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/engine/exceptions.py
--rw-r--r--   0        0        0     5713 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/engine/launch.py
--rw-r--r--   0        0        0     6617 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/engine/persistence.py
--rw-r--r--   0        0        0     1756 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/engine/processes/__init__.py
--rw-r--r--   0        0        0    10915 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/engine/processes/builder.py
--rw-r--r--   0        0        0      937 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/engine/processes/calcjobs/__init__.py
--rw-r--r--   0        0        0    48403 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/engine/processes/calcjobs/calcjob.py
--rw-r--r--   0        0        0     1125 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/engine/processes/calcjobs/importer.py
--rw-r--r--   0        0        0    12526 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/engine/processes/calcjobs/manager.py
--rw-r--r--   0        0        0     8671 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/engine/processes/calcjobs/monitors.py
--rw-r--r--   0        0        0    32269 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/engine/processes/calcjobs/tasks.py
--rw-r--r--   0        0        0    12331 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/engine/processes/control.py
--rw-r--r--   0        0        0     3690 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/engine/processes/exit_code.py
--rw-r--r--   0        0        0    23589 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/engine/processes/functions.py
--rw-r--r--   0        0        0     3852 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/engine/processes/futures.py
--rw-r--r--   0        0        0    11954 2023-05-22 21:50:10.271921 aiida_core-2.3.1/aiida/engine/processes/ports.py
--rw-r--r--   0        0        0    43594 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/engine/processes/process.py
--rw-r--r--   0        0        0     4547 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/engine/processes/process_spec.py
--rw-r--r--   0        0        0     1018 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/engine/processes/utils.py
--rw-r--r--   0        0        0     1187 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/engine/processes/workchains/__init__.py
--rw-r--r--   0        0        0     2470 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/engine/processes/workchains/awaitable.py
--rw-r--r--   0        0        0     1968 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/engine/processes/workchains/context.py
--rw-r--r--   0        0        0    21825 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/engine/processes/workchains/restart.py
--rw-r--r--   0        0        0     7604 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/engine/processes/workchains/utils.py
--rw-r--r--   0        0        0    17279 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/engine/processes/workchains/workchain.py
--rw-r--r--   0        0        0    14996 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/engine/runners.py
--rw-r--r--   0        0        0     6129 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/engine/transports.py
--rw-r--r--   0        0        0    12275 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/engine/utils.py
--rw-r--r--   0        0        0     1845 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/manage/__init__.py
--rw-r--r--   0        0        0    11086 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/manage/caching.py
--rw-r--r--   0        0        0    11486 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/manage/configuration/__init__.py
--rw-r--r--   0        0        0    20965 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/manage/configuration/config.py
--rw-r--r--   0        0        0     1075 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/manage/configuration/migrations/__init__.py
--rw-r--r--   0        0        0    20944 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/manage/configuration/migrations/migrations.py
--rw-r--r--   0        0        0     4732 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/manage/configuration/options.py
--rw-r--r--   0        0        0    10267 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/manage/configuration/profile.py
--rw-r--r--   0        0        0      632 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/manage/configuration/schema/__init__.py
--rw-r--r--   0        0        0    15472 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/manage/configuration/schema/config-v5.schema.json
--rw-r--r--   0        0        0    12291 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/manage/configuration/schema/config-v6.schema.json
--rw-r--r--   0        0        0    12289 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/manage/configuration/schema/config-v7.schema.json
--rw-r--r--   0        0        0    12749 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/manage/configuration/schema/config-v8.schema.json
--rw-r--r--   0        0        0    13329 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/manage/configuration/schema/config-v9.schema.json
--rw-r--r--   0        0        0     5305 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/manage/configuration/settings.py
--rw-r--r--   0        0        0     1148 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/manage/external/__init__.py
--rw-r--r--   0        0        0     9955 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/manage/external/postgres.py
--rw-r--r--   0        0        0     1104 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/manage/external/rmq/__init__.py
--rw-r--r--   0        0        0     3868 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/manage/external/rmq/client.py
--rw-r--r--   0        0        0      432 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/manage/external/rmq/defaults.py
--rw-r--r--   0        0        0     7433 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/manage/external/rmq/launcher.py
--rw-r--r--   0        0        0     2743 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/manage/external/rmq/utils.py
--rw-r--r--   0        0        0    20986 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/manage/manager.py
--rw-r--r--   0        0        0    10232 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/manage/profile_access.py
--rw-r--r--   0        0        0      993 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/manage/tests/__init__.py
--rw-r--r--   0        0        0    19379 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/manage/tests/main.py
--rw-r--r--   0        0        0    34536 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/manage/tests/pytest_fixtures.py
--rw-r--r--   0        0        0     2738 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/orm/__init__.py
--rw-r--r--   0        0        0     5406 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/orm/authinfos.py
--rw-r--r--   0        0        0    12110 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/orm/autogroup.py
--rw-r--r--   0        0        0     4451 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/orm/comments.py
--rw-r--r--   0        0        0    26490 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/orm/computers.py
--rw-r--r--   0        0        0     4716 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/orm/convert.py
--rw-r--r--   0        0        0    10275 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/orm/entities.py
--rw-r--r--   0        0        0     7190 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/orm/extras.py
--rw-r--r--   0        0        0    13709 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/orm/groups.py
--rw-r--r--   0        0        0     1628 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/orm/implementation/__init__.py
--rw-r--r--   0        0        0     3059 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/orm/implementation/authinfos.py
--rw-r--r--   0        0        0     3806 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/orm/implementation/comments.py
--rw-r--r--   0        0        0     3550 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/orm/implementation/computers.py
--rw-r--r--   0        0        0     7922 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/orm/implementation/entities.py
--rw-r--r--   0        0        0     5840 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/orm/implementation/groups.py
--rw-r--r--   0        0        0     3025 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/orm/implementation/logs.py
--rw-r--r--   0        0        0    11547 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/orm/implementation/nodes.py
--rw-r--r--   0        0        0     6576 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/orm/implementation/querybuilder.py
--rw-r--r--   0        0        0    14652 2023-05-22 21:50:10.275921 aiida_core-2.3.1/aiida/orm/implementation/storage_backend.py
--rw-r--r--   0        0        0     2459 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/implementation/users.py
--rw-r--r--   0        0        0     5746 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/implementation/utils.py
--rw-r--r--   0        0        0     7505 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/logs.py
--rw-r--r--   0        0        0     1786 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/nodes/__init__.py
--rw-r--r--   0        0        0     8303 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/nodes/attributes.py
--rw-r--r--   0        0        0     7099 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/nodes/caching.py
--rw-r--r--   0        0        0     2497 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/nodes/comments.py
--rw-r--r--   0        0        0     1885 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/nodes/data/__init__.py
--rw-r--r--   0        0        0     1069 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/nodes/data/array/__init__.py
--rw-r--r--   0        0        0     9322 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/nodes/data/array/array.py
--rw-r--r--   0        0        0    73820 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/nodes/data/array/bands.py
--rw-r--r--   0        0        0    20634 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/nodes/data/array/kpoints.py
--rw-r--r--   0        0        0    13142 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/nodes/data/array/projection.py
--rw-r--r--   0        0        0    38839 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/nodes/data/array/trajectory.py
--rw-r--r--   0        0        0     6269 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/nodes/data/array/xy.py
--rw-r--r--   0        0        0     2038 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/nodes/data/base.py
--rw-r--r--   0        0        0     1828 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/nodes/data/bool.py
--rw-r--r--   0        0        0    30429 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/nodes/data/cif.py
--rw-r--r--   0        0        0      401 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/nodes/data/code/__init__.py
--rw-r--r--   0        0        0    17202 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/nodes/data/code/abstract.py
--rw-r--r--   0        0        0     5354 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/nodes/data/code/containerized.py
--rw-r--r--   0        0        0     8279 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/nodes/data/code/installed.py
--rw-r--r--   0        0        0    23043 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/nodes/data/code/legacy.py
--rw-r--r--   0        0        0     8095 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/nodes/data/code/portable.py
--rw-r--r--   0        0        0    14661 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/nodes/data/data.py
--rw-r--r--   0        0        0     5667 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/nodes/data/dict.py
--rw-r--r--   0        0        0     4588 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/nodes/data/enum.py
--rw-r--r--   0        0        0      967 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/nodes/data/float.py
--rw-r--r--   0        0        0     1690 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/nodes/data/folder.py
--rw-r--r--   0        0        0      969 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/nodes/data/int.py
--rw-r--r--   0        0        0     7427 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/nodes/data/jsonable.py
--rw-r--r--   0        0        0     4948 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/nodes/data/list.py
--rw-r--r--   0        0        0     3373 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/nodes/data/numeric.py
--rw-r--r--   0        0        0     4784 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/nodes/data/orbital.py
--rw-r--r--   0        0        0      338 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/nodes/data/remote/__init__.py
--rw-r--r--   0        0        0     8173 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/nodes/data/remote/base.py
--rw-r--r--   0        0        0      326 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/nodes/data/remote/stash/__init__.py
--rw-r--r--   0        0        0     2371 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/nodes/data/remote/stash/base.py
--rw-r--r--   0        0        0     2250 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/nodes/data/remote/stash/folder.py
--rw-r--r--   0        0        0     4935 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/nodes/data/singlefile.py
--rw-r--r--   0        0        0      910 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/nodes/data/str.py
--rw-r--r--   0        0        0    93793 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/nodes/data/structure.py
--rw-r--r--   0        0        0    19092 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/nodes/data/upf.py
--rw-r--r--   0        0        0    11454 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/nodes/links.py
--rw-r--r--   0        0        0    27920 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/nodes/node.py
--rw-r--r--   0        0        0     1009 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/nodes/process/__init__.py
--rw-r--r--   0        0        0      941 2023-05-22 21:50:10.279922 aiida_core-2.3.1/aiida/orm/nodes/process/calculation/__init__.py
--rw-r--r--   0        0        0     2605 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/orm/nodes/process/calculation/calcfunction.py
--rw-r--r--   0        0        0    21120 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/orm/nodes/process/calculation/calcjob.py
--rw-r--r--   0        0        0     2115 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/orm/nodes/process/calculation/calculation.py
--rw-r--r--   0        0        0    20753 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/orm/nodes/process/process.py
--rw-r--r--   0        0        0      936 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/orm/nodes/process/workflow/__init__.py
--rw-r--r--   0        0        0     1775 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/orm/nodes/process/workflow/workchain.py
--rw-r--r--   0        0        0     3631 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/orm/nodes/process/workflow/workflow.py
--rw-r--r--   0        0        0     2442 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/orm/nodes/process/workflow/workfunction.py
--rw-r--r--   0        0        0    15675 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/orm/nodes/repository.py
--rw-r--r--   0        0        0    61503 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/orm/querybuilder.py
--rw-r--r--   0        0        0     4785 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/orm/users.py
--rw-r--r--   0        0        0     1415 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/orm/utils/__init__.py
--rw-r--r--   0        0        0      632 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/orm/utils/builders/__init__.py
--rw-r--r--   0        0        0     8496 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/orm/utils/builders/code.py
--rw-r--r--   0        0        0     8108 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/orm/utils/builders/computer.py
--rw-r--r--   0        0        0     4952 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/orm/utils/calcjob.py
--rw-r--r--   0        0        0    17089 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/orm/utils/links.py
--rw-r--r--   0        0        0    36736 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/orm/utils/loaders.py
--rw-r--r--   0        0        0     2808 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/orm/utils/log.py
--rw-r--r--   0        0        0    10970 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/orm/utils/managers.py
--rw-r--r--   0        0        0     9786 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/orm/utils/mixins.py
--rw-r--r--   0        0        0     7008 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/orm/utils/node.py
--rw-r--r--   0        0        0     4573 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/orm/utils/remote.py
--rw-r--r--   0        0        0     9155 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/orm/utils/serialize.py
--rw-r--r--   0        0        0      847 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/parsers/__init__.py
--rw-r--r--   0        0        0     8094 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/parsers/parser.py
--rw-r--r--   0        0        0      632 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/parsers/plugins/__init__.py
--rw-r--r--   0        0        0      632 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/parsers/plugins/arithmetic/__init__.py
--rw-r--r--   0        0        0     2226 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/parsers/plugins/arithmetic/add.py
--rw-r--r--   0        0        0     1984 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/parsers/plugins/diff_tutorial/parsers.py
--rw-r--r--   0        0        0      632 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/parsers/plugins/templatereplacer/__init__.py
--rw-r--r--   0        0        0     3244 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/parsers/plugins/templatereplacer/parser.py
--rw-r--r--   0        0        0     1329 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/plugins/__init__.py
--rw-r--r--   0        0        0    17411 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/plugins/entry_point.py
--rw-r--r--   0        0        0    16492 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/plugins/factories.py
--rw-r--r--   0        0        0     4405 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/plugins/utils.py
--rw-r--r--   0        0        0       26 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/py.typed
--rw-r--r--   0        0        0     1017 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/repository/__init__.py
--rw-r--r--   0        0        0      368 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/repository/backend/__init__.py
--rw-r--r--   0        0        0     9748 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/repository/backend/abstract.py
--rw-r--r--   0        0        0     9659 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/repository/backend/disk_object_store.py
--rw-r--r--   0        0        0     4392 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/repository/backend/sandbox.py
--rw-r--r--   0        0        0     5382 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/repository/common.py
--rw-r--r--   0        0        0    24331 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/repository/repository.py
--rw-r--r--   0        0        0      823 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/restapi/__init__.py
--rw-r--r--   0        0        0     7379 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/restapi/api.py
--rw-r--r--   0        0        0      632 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/restapi/common/__init__.py
--rw-r--r--   0        0        0     1701 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/restapi/common/config.py
--rw-r--r--   0        0        0     1589 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/restapi/common/exceptions.py
--rw-r--r--   0        0        0    19441 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/restapi/common/identifiers.py
--rw-r--r--   0        0        0    34328 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/restapi/common/utils.py
--rw-r--r--   0        0        0    28984 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/restapi/resources.py
--rwxr-xr-x   0        0        0     4911 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/restapi/run_api.py
--rw-r--r--   0        0        0      632 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/restapi/translator/__init__.py
--rw-r--r--   0        0        0    18895 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/restapi/translator/base.py
--rw-r--r--   0        0        0     4211 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/restapi/translator/computer.py
--rw-r--r--   0        0        0     3321 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/restapi/translator/group.py
--rw-r--r--   0        0        0      632 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/restapi/translator/nodes/__init__.py
--rw-r--r--   0        0        0     2835 2023-05-22 21:50:10.283922 aiida_core-2.3.1/aiida/restapi/translator/nodes/data/__init__.py
--rw-r--r--   0        0        0      632 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/restapi/translator/nodes/data/array/__init__.py
--rw-r--r--   0        0        0     2051 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/restapi/translator/nodes/data/array/bands.py
--rw-r--r--   0        0        0     1478 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/restapi/translator/nodes/data/cif.py
--rw-r--r--   0        0        0     1464 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/restapi/translator/nodes/data/code.py
--rw-r--r--   0        0        0     5420 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/restapi/translator/nodes/data/kpoints.py
--rw-r--r--   0        0        0     1579 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/restapi/translator/nodes/data/structure.py
--rw-r--r--   0        0        0     1388 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/restapi/translator/nodes/data/upf.py
--rw-r--r--   0        0        0    31726 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/restapi/translator/nodes/node.py
--rw-r--r--   0        0        0      632 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/restapi/translator/nodes/process/__init__.py
--rw-r--r--   0        0        0      632 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/restapi/translator/nodes/process/calculation/__init__.py
--rw-r--r--   0        0        0     1579 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/restapi/translator/nodes/process/calculation/calcfunction.py
--rw-r--r--   0        0        0     2619 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/restapi/translator/nodes/process/calculation/calcjob.py
--rw-r--r--   0        0        0     4530 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/restapi/translator/nodes/process/process.py
--rw-r--r--   0        0        0      632 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/restapi/translator/nodes/process/workflow/__init__.py
--rw-r--r--   0        0        0     1545 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/restapi/translator/nodes/process/workflow/workchain.py
--rw-r--r--   0        0        0     1576 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/restapi/translator/nodes/process/workflow/workfunction.py
--rw-r--r--   0        0        0     2765 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/restapi/translator/user.py
--rw-r--r--   0        0        0     1074 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/schedulers/__init__.py
--rw-r--r--   0        0        0    25535 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/schedulers/datastructures.py
--rw-r--r--   0        0        0      632 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/schedulers/plugins/__init__.py
--rw-r--r--   0        0        0    15506 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/schedulers/plugins/direct.py
--rw-r--r--   0        0        0    33310 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/schedulers/plugins/lsf.py
--rw-r--r--   0        0        0    31102 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/schedulers/plugins/pbsbaseclasses.py
--rw-r--r--   0        0        0     3701 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/schedulers/plugins/pbspro.py
--rw-r--r--   0        0        0    20419 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/schedulers/plugins/sge.py
--rw-r--r--   0        0        0    35179 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/schedulers/plugins/slurm.py
--rw-r--r--   0        0        0     3799 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/schedulers/plugins/torque.py
--rw-r--r--   0        0        0    20077 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/schedulers/scheduler.py
--rw-r--r--   0        0        0     1108 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/sphinxext/__init__.py
--rw-r--r--   0        0        0     1450 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/sphinxext/calcjob.py
--rw-r--r--   0        0        0     9048 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/sphinxext/process.py
--rw-r--r--   0        0        0     1475 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/sphinxext/workchain.py
--rw-r--r--   0        0        0      810 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/storage/__init__.py
--rw-r--r--   0        0        0      815 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/storage/log.py
--rw-r--r--   0        0        0      877 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/storage/psql_dos/__init__.py
--rwxr-xr-x   0        0        0     3996 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/storage/psql_dos/alembic_cli.py
--rw-r--r--   0        0        0    18190 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/storage/psql_dos/backend.py
--rw-r--r--   0        0        0      632 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/__init__.py
--rw-r--r--   0        0        0     2198 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/env.py
--rw-r--r--   0        0        0      494 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/script.py.mako
--rw-r--r--   0        0        0      748 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/utils/__init__.py
--rw-r--r--   0        0        0     2260 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/utils/calc_state.py
--rw-r--r--   0        0        0     3916 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/utils/create_dbattribute.py
--rw-r--r--   0        0        0     8837 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/utils/dblog_update.py
--rw-r--r--   0        0        0     1563 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/utils/duplicate_uuids.py
--rw-r--r--   0        0        0    12177 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/utils/integrity.py
--rw-r--r--   0        0        0     3477 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/utils/legacy_workflows.py
--rw-r--r--   0        0        0     5991 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/utils/migrate_repository.py
--rw-r--r--   0        0        0     9306 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/utils/parity.py
--rw-r--r--   0        0        0     7520 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/utils/provenance_redesign.py
--rw-r--r--   0        0        0     5534 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/utils/reflect.py
--rw-r--r--   0        0        0    18164 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/utils/utils.py
--rw-r--r--   0        0        0     2902 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/041a79fc615f_dblog_cleaning.py
--rw-r--r--   0        0        0     1486 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/07fac78e6209_drop_computer_transport_params.py
--rw-r--r--   0        0        0     2482 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/0aebbeab274d_base_data_plugin_type_string.py
--rw-r--r--   0        0        0     1819 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/0edcdd5a30f0_dbgroup_extras.py
--rw-r--r--   0        0        0     1829 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/118349c10896_default_link_label.py
--rw-r--r--   0        0        0     2727 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/12536798d4d3_trajectory_symbols_to_attribute.py
--rw-r--r--   0        0        0     2856 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/140c971ae0a3_migrate_builtin_calculations.py
--rw-r--r--   0        0        0     1168 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/162b99bca4a2_drop_dbcalcstate.py
--rw-r--r--   0        0        0     1361 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/1830c8430131_drop_node_columns_nodeversion_public.py
--rw-r--r--   0        0        0     1872 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/1b8ed3425af9_remove_legacy_workflows.py
--rw-r--r--   0        0        0     9697 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/1de112340b16_django_parity_1.py
--rw-r--r--   0        0        0    10079 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/1de112340b17_django_parity_2.py
--rw-r--r--   0        0        0     1252 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/1de112340b18_django_parity_3.py
--rw-r--r--   0        0        0     1382 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/1feaea71bd5a_migrate_repository.py
--rw-r--r--   0        0        0     5530 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/239cea6d2452_provenance_redesign.py
--rw-r--r--   0        0        0     8062 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/26d561acd560_data_migration_legacy_job_calculations.py
--rw-r--r--   0        0        0     5861 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/34a831f4286d_entry_point_core_prefix.py
--rw-r--r--   0        0        0     2044 2023-05-22 21:50:10.287922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/35d4ee9a1b0e_code_hidden_attr_to_extra.py
--rw-r--r--   0        0        0     1309 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/375c2db70663_dblog_uuid_uniqueness_constraint.py
--rw-r--r--   0        0        0     1615 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/37f3d4882837_make_all_uuid_columns_unique.py
--rw-r--r--   0        0        0     1335 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/3d6190594e19_remove_dbcomputer_enabled.py
--rw-r--r--   0        0        0      802 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/535039300e4a_computer_name_to_label.py
--rw-r--r--   0        0        0     1892 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/59edaf8a8b79_adding_indexes_and_constraints_to_the_.py
--rw-r--r--   0        0        0     1689 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/5a49629f0d45_dblink_indices.py
--rw-r--r--   0        0        0     1742 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/5d4d844852b6_invalidating_node_hash.py
--rw-r--r--   0        0        0     1762 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/5ddd24e52864_dbnode_type_to_dbnode_node_type.py
--rw-r--r--   0        0        0     1866 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/61fc0913fae9_remove_node_prefix.py
--rw-r--r--   0        0        0     1391 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/62fe0d36de90_add_node_uuid_unique_constraint.py
--rw-r--r--   0        0        0     1621 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/6a5c2ea1439d_move_data_within_node_module.py
--rw-r--r--   0        0        0     1376 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/6c629c886f84_process_type.py
--rw-r--r--   0        0        0     1351 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/70c7d732f1b2_delete_dbpath.py
--rw-r--r--   0        0        0     1466 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/7536a82b2cc4_add_node_repository_metadata.py
--rw-r--r--   0        0        0     1360 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/7a6587e16f4c_unique_constraints_for_the_db_dbgroup_.py
--rw-r--r--   0        0        0     2610 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/7b38a9e783e7_seal_unsealed_processes.py
--rw-r--r--   0        0        0     3849 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/7ca08c391c49_calc_job_option_attribute_keys.py
--rw-r--r--   0        0        0     1311 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/89176227b25_add_indexes_to_dbworkflowdata_table.py
--rw-r--r--   0        0        0     2309 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/91b573400be5_prepare_schema_reset.py
--rw-r--r--   0        0        0      632 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/__init__.py
--rw-r--r--   0        0        0     1158 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/a514d673c163_drop_dblock.py
--rw-r--r--   0        0        0     1656 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/a603da2cc809_code_sub_class_of_data.py
--rw-r--r--   0        0        0     6613 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/a6048f0ffca8_update_linktypes.py
--rw-r--r--   0        0        0     1840 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/b8b23ddefad4_dbgroup_name_to_label_type_to_type_string.py
--rw-r--r--   0        0        0     1778 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/bf591f31dd12_dbgroup_type_string.py
--rw-r--r--   0        0        0     2269 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/ce56d84bcc35_delete_trajectory_symbols_array.py
--rw-r--r--   0        0        0     1599 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/d254fdfed416_rename_parameter_data_to_dict.py
--rw-r--r--   0        0        0     1564 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/de2eaf6978b4_simplify_user_model.py
--rw-r--r--   0        0        0    30892 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0001_initial.py
--rw-r--r--   0        0        0     1505 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0002_db_state_change.py
--rw-r--r--   0        0        0     1809 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0003_add_link_type.py
--rw-r--r--   0        0        0     1547 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0004_add_daemon_and_uuid_indices.py
--rw-r--r--   0        0        0     1246 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0005_add_cmtime_indices.py
--rw-r--r--   0        0        0     1295 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0006_delete_dbpath.py
--rw-r--r--   0        0        0     6316 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0007_update_linktypes.py
--rw-r--r--   0        0        0     2359 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0008_code_hidden_to_extra.py
--rw-r--r--   0        0        0     2275 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0009_base_data_plugin_type_string.py
--rw-r--r--   0        0        0     1474 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0010_process_type.py
--rw-r--r--   0        0        0     1712 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0011_delete_kombu_tables.py
--rw-r--r--   0        0        0     1073 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0012_drop_dblock.py
--rw-r--r--   0        0        0     1747 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0013_django_1_8.py
--rw-r--r--   0        0        0     1374 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0014_add_node_uuid_unique_constraint.py
--rw-r--r--   0        0        0     1192 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0015_invalidating_node_hash.py
--rw-r--r--   0        0        0     1171 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0016_code_sub_class_of_data.py
--rw-r--r--   0        0        0     1083 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0017_drop_dbcalcstate.py
--rw-r--r--   0        0        0     2391 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0018_django_1_11.py
--rw-r--r--   0        0        0     2558 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0019_migrate_builtin_calculations.py
--rw-r--r--   0        0        0     6233 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0020_provenance_redesign.py
--rw-r--r--   0        0        0     2439 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0021_dbgroup_name_to_label_type_to_type_string.py
--rw-r--r--   0        0        0     1539 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0022_dbgroup_type_string_change_content.py
--rw-r--r--   0        0        0     3316 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0023_calc_job_option_attribute_keys.py
--rw-r--r--   0        0        0     3663 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0024a_dblog_update.py
--rw-r--r--   0        0        0     1248 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0024b_dblog_update.py
--rw-r--r--   0        0        0     1480 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0025_move_data_within_node_module.py
--rw-r--r--   0        0        0     2250 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0026_trajectory_symbols_to_attribute.py
--rw-r--r--   0        0        0     2415 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0027_delete_trajectory_symbols_array.py
--rw-r--r--   0        0        0     1598 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0028_remove_node_prefix.py
--rw-r--r--   0        0        0     1383 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0029_rename_parameter_data_to_dict.py
--rw-r--r--   0        0        0     1267 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0030_dbnode_type_to_dbnode_node_type.py
--rw-r--r--   0        0        0     1140 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0031_remove_dbcomputer_enabled.py
--rw-r--r--   0        0        0     1552 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0032_remove_legacy_workflows.py
--rw-r--r--   0        0        0     1516 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0033_replace_text_field_with_json_field.py
--rw-r--r--   0        0        0     1203 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0034_drop_node_columns_nodeversion_public.py
--rw-r--r--   0        0        0     1550 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0035_simplify_user_model.py
--rw-r--r--   0        0        0     1156 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0036_drop_computer_transport_params.py
--rw-r--r--   0        0        0     7292 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0037_attributes_extras_settings_json.py
--rw-r--r--   0        0        0     7899 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0038_data_migration_legacy_job_calculations.py
--rw-r--r--   0        0        0     1220 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0039_reset_hash.py
--rw-r--r--   0        0        0     3186 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0040_data_migration_legacy_process_attributes.py
--rw-r--r--   0        0        0     2403 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0041_seal_unsealed_processes.py
--rw-r--r--   0        0        0     2115 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0042_prepare_schema_reset.py
--rw-r--r--   0        0        0     1612 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0043_default_link_label.py
--rw-r--r--   0        0        0     1615 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0044_dbgroup_type_string.py
--rw-r--r--   0        0        0     1673 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0045_dbgroup_extras.py
--rw-r--r--   0        0        0     1378 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0046_add_node_repository_metadata.py
--rw-r--r--   0        0        0     1297 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0047_migrate_repository.py
--rw-r--r--   0        0        0     1728 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0048_computer_name_to_label.py
--rw-r--r--   0        0        0     5770 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0049_entry_point_core_prefix.py
--rw-r--r--   0        0        0     1974 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0050_sqlalchemy_parity.py
--rw-r--r--   0        0        0    21476 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/e15ef2630a1b_initial_schema.py
--rw-r--r--   0        0        0     2135 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/e72ad251bcdb_dbgroup_class_change_type_string_values.py
--rw-r--r--   0        0        0     3393 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/e734dd5e50d7_data_migration_legacy_process_attributes.py
--rw-r--r--   0        0        0     1303 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/e797afa09270_reset_hash.py
--rw-r--r--   0        0        0     1760 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/ea2f50e7f615_dblog_create_uuid_column.py
--rw-r--r--   0        0        0     2221 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/f9a69de76a9a_delete_kombu_tables.py
--rw-r--r--   0        0        0    11820 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/main_0001_initial.py
--rw-r--r--   0        0        0    21817 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/migrator.py
--rw-r--r--   0        0        0      703 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/models/__init__.py
--rw-r--r--   0        0        0     2660 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/models/authinfo.py
--rw-r--r--   0        0        0     4494 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/models/base.py
--rw-r--r--   0        0        0     2322 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/models/comment.py
--rw-r--r--   0        0        0     2904 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/models/computer.py
--rw-r--r--   0        0        0     3635 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/models/group.py
--rw-r--r--   0        0        0     2677 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/models/log.py
--rw-r--r--   0        0        0     8274 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/models/node.py
--rw-r--r--   0        0        0     1749 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/models/settings.py
--rw-r--r--   0        0        0     1739 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/models/user.py
--rw-r--r--   0        0        0      678 2023-05-22 21:50:10.291922 aiida_core-2.3.1/aiida/storage/psql_dos/orm/__init__.py
--rw-r--r--   0        0        0     4752 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/storage/psql_dos/orm/authinfos.py
--rw-r--r--   0        0        0     6320 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/storage/psql_dos/orm/comments.py
--rw-r--r--   0        0        0     4282 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/storage/psql_dos/orm/computers.py
--rw-r--r--   0        0        0     3537 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/storage/psql_dos/orm/convert.py
--rw-r--r--   0        0        0     3451 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/storage/psql_dos/orm/entities.py
--rw-r--r--   0        0        0     3251 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/storage/psql_dos/orm/extras_mixin.py
--rw-r--r--   0        0        0    10474 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/storage/psql_dos/orm/groups.py
--rw-r--r--   0        0        0     5113 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/storage/psql_dos/orm/logs.py
--rw-r--r--   0        0        0    10981 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/storage/psql_dos/orm/nodes.py
--rw-r--r--   0        0        0      746 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/storage/psql_dos/orm/querybuilder/__init__.py
--rw-r--r--   0        0        0    23343 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/storage/psql_dos/orm/querybuilder/joiner.py
--rw-r--r--   0        0        0    45951 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/storage/psql_dos/orm/querybuilder/main.py
--rw-r--r--   0        0        0     2324 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/storage/psql_dos/orm/users.py
--rw-r--r--   0        0        0     7345 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/storage/psql_dos/orm/utils.py
--rw-r--r--   0        0        0     8962 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/storage/psql_dos/utils.py
--rw-r--r--   0        0        0     1022 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/storage/sqlite_temp/__init__.py
--rw-r--r--   0        0        0     7561 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/storage/sqlite_temp/backend.py
--rw-r--r--   0        0        0     1664 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/storage/sqlite_zip/__init__.py
--rw-r--r--   0        0        0    15085 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/storage/sqlite_zip/backend.py
--rw-r--r--   0        0        0      632 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/storage/sqlite_zip/migrations/__init__.py
--rw-r--r--   0        0        0     1999 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/storage/sqlite_zip/migrations/env.py
--rw-r--r--   0        0        0     1754 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/storage/sqlite_zip/migrations/legacy/__init__.py
--rw-r--r--   0        0        0     3332 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/storage/sqlite_zip/migrations/legacy/v04_to_v05.py
--rw-r--r--   0        0        0     7335 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/storage/sqlite_zip/migrations/legacy/v05_to_v06.py
--rw-r--r--   0        0        0     5971 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/storage/sqlite_zip/migrations/legacy/v06_to_v07.py
--rw-r--r--   0        0        0     2107 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/storage/sqlite_zip/migrations/legacy/v07_to_v08.py
--rw-r--r--   0        0        0     2361 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/storage/sqlite_zip/migrations/legacy/v08_to_v09.py
--rw-r--r--   0        0        0     1355 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/storage/sqlite_zip/migrations/legacy/v09_to_v10.py
--rw-r--r--   0        0        0     1480 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/storage/sqlite_zip/migrations/legacy/v10_to_v11.py
--rw-r--r--   0        0        0     5486 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/storage/sqlite_zip/migrations/legacy/v11_to_v12.py
--rw-r--r--   0        0        0     1698 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/storage/sqlite_zip/migrations/legacy/v12_to_v13.py
--rw-r--r--   0        0        0    12668 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/storage/sqlite_zip/migrations/legacy_to_main.py
--rw-r--r--   0        0        0      572 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/storage/sqlite_zip/migrations/script.py.mako
--rw-r--r--   0        0        0     8212 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/storage/sqlite_zip/migrations/utils.py
--rw-r--r--   0        0        0     8703 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/storage/sqlite_zip/migrations/v1_db_schema.py
--rw-r--r--   0        0        0      632 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/storage/sqlite_zip/migrations/versions/__init__.py
--rw-r--r--   0        0        0     8710 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/storage/sqlite_zip/migrations/versions/main_0000_initial.py
--rw-r--r--   0        0        0     6790 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/storage/sqlite_zip/migrations/versions/main_0000a_replace_nulls.py
--rw-r--r--   0        0        0     4413 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/storage/sqlite_zip/migrations/versions/main_0000b_non_nullable.py
--rw-r--r--   0        0        0     1044 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/storage/sqlite_zip/migrations/versions/main_0001.py
--rw-r--r--   0        0        0    17760 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/storage/sqlite_zip/migrator.py
--rw-r--r--   0        0        0     7070 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/storage/sqlite_zip/models.py
--rw-r--r--   0        0        0    15167 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/storage/sqlite_zip/orm.py
--rw-r--r--   0        0        0     4882 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/storage/sqlite_zip/utils.py
--rw-r--r--   0        0        0     1845 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/tools/__init__.py
--rw-r--r--   0        0        0     1366 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/tools/archive/__init__.py
--rw-r--r--   0        0        0     9493 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/tools/archive/abstract.py
--rw-r--r--   0        0        0     3349 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/tools/archive/common.py
--rw-r--r--   0        0        0    29933 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/tools/archive/create.py
--rw-r--r--   0        0        0     2018 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/tools/archive/exceptions.py
--rw-r--r--   0        0        0      844 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/tools/archive/implementations/__init__.py
--rw-r--r--   0        0        0      836 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/tools/archive/implementations/sqlite_zip/__init__.py
--rw-r--r--   0        0        0     3280 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/tools/archive/implementations/sqlite_zip/main.py
--rw-r--r--   0        0        0     2268 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/tools/archive/implementations/sqlite_zip/reader.py
--rw-r--r--   0        0        0    12744 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/tools/archive/implementations/sqlite_zip/writer.py
--rw-r--r--   0        0        0    50475 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/tools/archive/imports.py
--rw-r--r--   0        0        0      833 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/tools/calculations/__init__.py
--rw-r--r--   0        0        0     1053 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/tools/calculations/base.py
--rw-r--r--   0        0        0      997 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/tools/data/__init__.py
--rw-r--r--   0        0        0      862 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/tools/data/array/__init__.py
--rw-r--r--   0        0        0      952 2023-05-22 21:50:10.295922 aiida_core-2.3.1/aiida/tools/data/array/kpoints/__init__.py
--rw-r--r--   0        0        0    77224 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/tools/data/array/kpoints/legacy.py
--rw-r--r--   0        0        0    10772 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/tools/data/array/kpoints/main.py
--rw-r--r--   0        0        0     7034 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/tools/data/array/kpoints/seekpath.py
--rw-r--r--   0        0        0     1377 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/tools/data/array/trajectory.py
--rw-r--r--   0        0        0     8683 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/tools/data/cif.py
--rw-r--r--   0        0        0      899 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/tools/data/orbital/__init__.py
--rw-r--r--   0        0        0     6521 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/tools/data/orbital/orbital.py
--rw-r--r--   0        0        0    13938 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/tools/data/orbital/realhydrogen.py
--rw-r--r--   0        0        0    11892 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/tools/data/structure.py
--rw-r--r--   0        0        0      632 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/tools/dbexporters/__init__.py
--rw-r--r--   0        0        0      783 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/tools/dbimporters/__init__.py
--rw-r--r--   0        0        0    12063 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/tools/dbimporters/baseclasses.py
--rw-r--r--   0        0        0      720 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/tools/dbimporters/plugins/__init__.py
--rw-r--r--   0        0        0    12105 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/tools/dbimporters/plugins/cod.py
--rw-r--r--   0        0        0    28472 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/tools/dbimporters/plugins/icsd.py
--rw-r--r--   0        0        0     6920 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/tools/dbimporters/plugins/materialsproject.py
--rw-r--r--   0        0        0    11604 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/tools/dbimporters/plugins/mpds.py
--rw-r--r--   0        0        0     5697 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/tools/dbimporters/plugins/mpod.py
--rw-r--r--   0        0        0     5399 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/tools/dbimporters/plugins/nninc.py
--rw-r--r--   0        0        0     4692 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/tools/dbimporters/plugins/oqmd.py
--rw-r--r--   0        0        0     4463 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/tools/dbimporters/plugins/pcod.py
--rw-r--r--   0        0        0     2691 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/tools/dbimporters/plugins/tcod.py
--rw-r--r--   0        0        0      883 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/tools/graph/__init__.py
--rw-r--r--   0        0        0    17095 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/tools/graph/age_entities.py
--rw-r--r--   0        0        0    18095 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/tools/graph/age_rules.py
--rw-r--r--   0        0        0     7116 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/tools/graph/deletions.py
--rw-r--r--   0        0        0    12733 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/tools/graph/graph_traversers.py
--rw-r--r--   0        0        0     1382 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/tools/groups/__init__.py
--rw-r--r--   0        0        0    12617 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/tools/groups/paths.py
--rw-r--r--   0        0        0      632 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/tools/ipython/__init__.py
--rw-r--r--   0        0        0     1212 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/tools/ipython/aiida_magic_register.py
--rw-r--r--   0        0        0     7832 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/tools/ipython/ipython_magics.py
--rw-r--r--   0        0        0        0 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/tools/query/__init__.py
--rw-r--r--   0        0        0     6826 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/tools/query/calculation.py
--rw-r--r--   0        0        0     2963 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/tools/query/formatting.py
--rw-r--r--   0        0        0     7054 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/tools/query/mapping.py
--rw-r--r--   0        0        0      941 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/tools/visualization/__init__.py
--rw-r--r--   0        0        0    35782 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/tools/visualization/graph.py
--rw-r--r--   0        0        0      943 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/transports/__init__.py
--rw-r--r--   0        0        0     6400 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/transports/cli.py
--rw-r--r--   0        0        0      851 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/transports/plugins/__init__.py
--rw-r--r--   0        0        0    37052 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/transports/plugins/local.py
--rw-r--r--   0        0        0    62840 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/transports/plugins/ssh.py
--rw-r--r--   0        0        0    30913 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/transports/transport.py
--rw-r--r--   0        0        0     3273 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/transports/util.py
--rw-r--r--   0        0        0      632 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/workflows/__init__.py
--rw-r--r--   0        0        0      632 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/workflows/arithmetic/__init__.py
--rw-r--r--   0        0        0     1057 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/workflows/arithmetic/add_multiply.py
--rw-r--r--   0        0        0     2538 2023-05-22 21:50:10.299922 aiida_core-2.3.1/aiida/workflows/arithmetic/multiply_add.py
--rw-r--r--   0        0        0      327 2023-05-22 21:50:10.299922 aiida_core-2.3.1/codecov.yml
--rw-r--r--   0        0        0      696 2023-05-22 21:50:10.351923 aiida_core-2.3.1/environment.yml
--rw-r--r--   0        0        0    13919 2023-05-22 21:50:10.351923 aiida_core-2.3.1/open_source_licenses.txt
--rw-r--r--   0        0        0    15761 2023-05-22 21:50:10.351923 aiida_core-2.3.1/pyproject.toml
--rw-r--r--   0        0        0      510 2023-05-22 21:50:10.351923 aiida_core-2.3.1/requirements/README.md
--rw-r--r--   0        0        0     3160 2023-05-22 21:50:10.351923 aiida_core-2.3.1/requirements/requirements-py-3.10.txt
--rw-r--r--   0        0        0     3609 2023-05-22 21:50:10.351923 aiida_core-2.3.1/requirements/requirements-py-3.11.txt
--rw-r--r--   0        0        0     3234 2023-05-22 21:50:10.351923 aiida_core-2.3.1/requirements/requirements-py-3.8.txt
--rw-r--r--   0        0        0     3207 2023-05-22 21:50:10.351923 aiida_core-2.3.1/requirements/requirements-py-3.9.txt
--rw-r--r--   0        0        0      473 2023-05-22 21:50:10.407924 aiida_core-2.3.1/utils/.gource.conf
--rw-r--r--   0        0        0      697 2023-05-22 21:50:10.407924 aiida_core-2.3.1/utils/__init__.py
--rwxr-xr-x   0        0        0    16828 2023-05-22 21:50:10.407924 aiida_core-2.3.1/utils/dependency_management.py
--rw-r--r--   0        0        0     6562 2023-05-22 21:50:10.407924 aiida_core-2.3.1/utils/make_all.py
--rw-r--r--   0        0        0       73 2023-05-22 21:50:10.407924 aiida_core-2.3.1/utils/requirements.txt
--rw-r--r--   0        0        0     5871 2023-05-22 21:50:10.407924 aiida_core-2.3.1/utils/validate_consistency.py
--rw-r--r--   0        0        0    11093 1970-01-01 00:00:00.000000 aiida_core-2.3.1/PKG-INFO
+-rw-r--r--   0        0        0      539 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0      347 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1056 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.devcontainer/docker-compose.yml
+-rw-r--r--   0        0        0       56 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.devcontainer/post_create.sh
+-rw-r--r--   0        0        0      759 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.docker/docker-rabbitmq.yml
+-rwxr-xr-x   0        0        0       66 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.docker/my_init.d/configure-aiida.sh
+-rwxr-xr-x   0        0        0     3773 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.docker/opt/configure-aiida.sh
+-rw-r--r--   0        0        0      155 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.dockerignore
+-rw-r--r--   0        0        0      649 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      972 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      275 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      434 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.github/ISSUE_TEMPLATE/doc-improvements.md
+-rw-r--r--   0        0        0      754 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      181 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.github/config/README.md
+-rw-r--r--   0        0        0      307 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.github/config/add-singularity.yaml
+-rw-r--r--   0        0        0      163 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.github/config/add.yaml
+-rwxr-xr-x   0        0        0      347 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.github/config/doubler.sh
+-rw-r--r--   0        0        0      199 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.github/config/doubler.yaml
+-rw-r--r--   0        0        0       43 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.github/config/localhost-config.yaml
+-rw-r--r--   0        0        0      274 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.github/config/localhost.yaml
+-rw-r--r--   0        0        0      453 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.github/config/profile.yaml
+-rw-r--r--   0        0        0      130 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.github/config/slurm-ssh-config.yaml
+-rw-r--r--   0        0        0      275 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.github/config/slurm-ssh.yaml
+-rw-r--r--   0        0        0     1679 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.github/config/slurm_rsa
+-rw-r--r--   0        0        0      202 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.github/system_tests/README.md
+-rw-r--r--   0        0        0     3176 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.github/system_tests/pytest/test_memory_leaks.py
+-rw-r--r--   0        0        0     1387 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.github/system_tests/test_containerized_code.py
+-rw-r--r--   0        0        0    23947 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.github/system_tests/test_daemon.py
+-rw-r--r--   0        0        0     1126 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.github/system_tests/test_ipython_magics.py
+-rwxr-xr-x   0        0        0      911 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.github/system_tests/test_polish_workchains.sh
+-rw-r--r--   0        0        0     3912 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.github/system_tests/test_profile_manager.py
+-rw-r--r--   0        0        0     1972 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.github/system_tests/test_test_manager.py
+-rwxr-xr-x   0        0        0     1611 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.github/system_tests/test_verdi_load_time.sh
+-rw-r--r--   0        0        0     8560 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.github/system_tests/workchains.py
+-rw-r--r--   0        0        0     1901 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.github/workflows/benchmark-config.json
+-rw-r--r--   0        0        0     2226 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.github/workflows/benchmark.yml
+-rw-r--r--   0        0        0     1719 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.github/workflows/build_and_test_docker_on_pr.yml
+-rw-r--r--   0        0        0     1327 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.github/workflows/check_release_tag.py
+-rw-r--r--   0        0        0     3561 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.github/workflows/ci-code.yml
+-rw-r--r--   0        0        0      888 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.github/workflows/ci-style.yml
+-rw-r--r--   0        0        0     1086 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.github/workflows/docs-build.yml
+-rw-r--r--   0        0        0     3477 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.github/workflows/nightly.yml
+-rw-r--r--   0        0        0     1803 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.github/workflows/post-release.yml
+-rw-r--r--   0        0        0     1377 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.github/workflows/push_image_to_dockerhub.yml
+-rw-r--r--   0        0        0     1712 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.github/workflows/rabbitmq.yml
+-rw-r--r--   0        0        0     3095 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.github/workflows/release.yml
+-rwxr-xr-x   0        0        0     1814 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.github/workflows/setup.sh
+-rw-r--r--   0        0        0    11115 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.github/workflows/test-install.yml
+-rwxr-xr-x   0        0        0      898 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.github/workflows/tests.sh
+-rwxr-xr-x   0        0        0      589 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.github/workflows/tests_nightly.sh
+-rwxr-xr-x   0        0        0     2135 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.github/workflows/verdi.sh
+-rw-r--r--   0        0        0      427 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.gitignore
+-rw-r--r--   0        0        0     2005 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.molecule/README.md
+-rw-r--r--   0        0        0      413 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.molecule/default/Dockerfile
+-rw-r--r--   0        0        0     1790 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.molecule/default/config_local.yml
+-rw-r--r--   0        0        0     6342 2023-06-23 05:38:50.901937 aiida_core-2.4.0/.molecule/default/create_docker.yml
+-rw-r--r--   0        0        0      632 2023-06-23 05:38:50.905937 aiida_core-2.4.0/.molecule/default/files/polish/__init__.py
+-rwxr-xr-x   0        0        0     7706 2023-06-23 05:38:50.905937 aiida_core-2.4.0/.molecule/default/files/polish/cli.py
+-rw-r--r--   0        0        0      632 2023-06-23 05:38:50.905937 aiida_core-2.4.0/.molecule/default/files/polish/lib/__init__.py
+-rw-r--r--   0        0        0     5370 2023-06-23 05:38:50.905937 aiida_core-2.4.0/.molecule/default/files/polish/lib/expression.py
+-rw-r--r--   0        0        0     1032 2023-06-23 05:38:50.905937 aiida_core-2.4.0/.molecule/default/files/polish/lib/template/base.tpl
+-rw-r--r--   0        0        0     5300 2023-06-23 05:38:50.905937 aiida_core-2.4.0/.molecule/default/files/polish/lib/template/workchain.tpl
+-rw-r--r--   0        0        0     8149 2023-06-23 05:38:50.905937 aiida_core-2.4.0/.molecule/default/files/polish/lib/workchain.py
+-rw-r--r--   0        0        0       46 2023-06-23 05:38:50.905937 aiida_core-2.4.0/.molecule/default/run_tests.yml
+-rw-r--r--   0        0        0     2717 2023-06-23 05:38:50.905937 aiida_core-2.4.0/.molecule/default/setup_aiida.yml
+-rw-r--r--   0        0        0      716 2023-06-23 05:38:50.905937 aiida_core-2.4.0/.molecule/default/setup_python.yml
+-rw-r--r--   0        0        0     1650 2023-06-23 05:38:50.905937 aiida_core-2.4.0/.molecule/default/tasks/log_query_stats.yml
+-rw-r--r--   0        0        0      239 2023-06-23 05:38:50.905937 aiida_core-2.4.0/.molecule/default/tasks/reset_query_stats.yml
+-rw-r--r--   0        0        0     2814 2023-06-23 05:38:50.905937 aiida_core-2.4.0/.molecule/default/test_polish_workchains.yml
+-rw-r--r--   0        0        0     9312 2023-06-23 05:38:50.905937 aiida_core-2.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      871 2023-06-23 05:38:50.905937 aiida_core-2.4.0/.readthedocs.yml
+-rw-r--r--   0        0        0     1746 2023-06-23 05:38:50.905937 aiida_core-2.4.0/AUTHORS.txt
+-rw-r--r--   0        0        0   210156 2023-06-23 05:38:50.905937 aiida_core-2.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0     3352 2023-06-23 05:38:50.905937 aiida_core-2.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      585 2023-06-23 05:38:50.905937 aiida_core-2.4.0/Dockerfile
+-rw-r--r--   0        0        0     1312 2023-06-23 05:38:50.905937 aiida_core-2.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     6031 2023-06-23 05:38:50.905937 aiida_core-2.4.0/README.md
+-rw-r--r--   0        0        0     3610 2023-06-23 05:38:50.905937 aiida_core-2.4.0/aiida/__init__.py
+-rw-r--r--   0        0        0      807 2023-06-23 05:38:50.905937 aiida_core-2.4.0/aiida/__main__.py
+-rw-r--r--   0        0        0      632 2023-06-23 05:38:50.905937 aiida_core-2.4.0/aiida/calculations/__init__.py
+-rw-r--r--   0        0        0      632 2023-06-23 05:38:50.905937 aiida_core-2.4.0/aiida/calculations/arithmetic/__init__.py
+-rw-r--r--   0        0        0     3907 2023-06-23 05:38:50.905937 aiida_core-2.4.0/aiida/calculations/arithmetic/add.py
+-rw-r--r--   0        0        0     2547 2023-06-23 05:38:50.905937 aiida_core-2.4.0/aiida/calculations/diff_tutorial/calculations.py
+-rw-r--r--   0        0        0        0 2023-06-23 05:38:50.905937 aiida_core-2.4.0/aiida/calculations/importers/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-23 05:38:50.905937 aiida_core-2.4.0/aiida/calculations/importers/arithmetic/__init__.py
+-rw-r--r--   0        0        0     1644 2023-06-23 05:38:50.905937 aiida_core-2.4.0/aiida/calculations/importers/arithmetic/add.py
+-rw-r--r--   0        0        0        0 2023-06-23 05:38:50.905937 aiida_core-2.4.0/aiida/calculations/monitors/__init__.py
+-rw-r--r--   0        0        0     1161 2023-06-23 05:38:50.905937 aiida_core-2.4.0/aiida/calculations/monitors/base.py
+-rw-r--r--   0        0        0     9273 2023-06-23 05:38:50.905937 aiida_core-2.4.0/aiida/calculations/templatereplacer.py
+-rw-r--r--   0        0        0    10738 2023-06-23 05:38:50.905937 aiida_core-2.4.0/aiida/calculations/transfer.py
+-rw-r--r--   0        0        0     1734 2023-06-23 05:38:50.905937 aiida_core-2.4.0/aiida/cmdline/__init__.py
+-rw-r--r--   0        0        0     1194 2023-06-23 05:38:50.905937 aiida_core-2.4.0/aiida/cmdline/commands/__init__.py
+-rw-r--r--   0        0        0    19440 2023-06-23 05:38:50.905937 aiida_core-2.4.0/aiida/cmdline/commands/cmd_archive.py
+-rw-r--r--   0        0        0    14544 2023-06-23 05:38:50.905937 aiida_core-2.4.0/aiida/cmdline/commands/cmd_calcjob.py
+-rw-r--r--   0        0        0    14761 2023-06-23 05:38:50.905937 aiida_core-2.4.0/aiida/cmdline/commands/cmd_code.py
+-rw-r--r--   0        0        0    27436 2023-06-23 05:38:50.905937 aiida_core-2.4.0/aiida/cmdline/commands/cmd_computer.py
+-rw-r--r--   0        0        0     7913 2023-06-23 05:38:50.905937 aiida_core-2.4.0/aiida/cmdline/commands/cmd_config.py
+-rw-r--r--   0        0        0    10683 2023-06-23 05:38:50.905937 aiida_core-2.4.0/aiida/cmdline/commands/cmd_daemon.py
+-rw-r--r--   0        0        0      931 2023-06-23 05:38:50.905937 aiida_core-2.4.0/aiida/cmdline/commands/cmd_data/__init__.py
+-rw-r--r--   0        0        0     1342 2023-06-23 05:38:50.905937 aiida_core-2.4.0/aiida/cmdline/commands/cmd_data/cmd_array.py
+-rw-r--r--   0        0        0     4813 2023-06-23 05:38:50.905937 aiida_core-2.4.0/aiida/cmdline/commands/cmd_data/cmd_bands.py
+-rw-r--r--   0        0        0     4397 2023-06-23 05:38:50.905937 aiida_core-2.4.0/aiida/cmdline/commands/cmd_data/cmd_cif.py
+-rw-r--r--   0        0        0     1224 2023-06-23 05:38:50.905937 aiida_core-2.4.0/aiida/cmdline/commands/cmd_data/cmd_dict.py
+-rw-r--r--   0        0        0     4692 2023-06-23 05:38:50.905937 aiida_core-2.4.0/aiida/cmdline/commands/cmd_data/cmd_export.py
+-rw-r--r--   0        0        0     2889 2023-06-23 05:38:50.905937 aiida_core-2.4.0/aiida/cmdline/commands/cmd_data/cmd_list.py
+-rw-r--r--   0        0        0     3604 2023-06-23 05:38:50.905937 aiida_core-2.4.0/aiida/cmdline/commands/cmd_data/cmd_remote.py
+-rw-r--r--   0        0        0     8026 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/commands/cmd_data/cmd_show.py
+-rw-r--r--   0        0        0     1341 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/commands/cmd_data/cmd_singlefile.py
+-rw-r--r--   0        0        0     8895 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/commands/cmd_data/cmd_structure.py
+-rw-r--r--   0        0        0     3580 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/commands/cmd_data/cmd_trajectory.py
+-rw-r--r--   0        0        0     5214 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/commands/cmd_data/cmd_upf.py
+-rw-r--r--   0        0        0     4761 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/commands/cmd_database.py
+-rw-r--r--   0        0        0     7557 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/commands/cmd_devel.py
+-rw-r--r--   0        0        0    18115 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/commands/cmd_group.py
+-rw-r--r--   0        0        0     1409 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/commands/cmd_help.py
+-rw-r--r--   0        0        0    20153 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/commands/cmd_node.py
+-rw-r--r--   0        0        0     2950 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/commands/cmd_plugin.py
+-rw-r--r--   0        0        0    11938 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/commands/cmd_process.py
+-rw-r--r--   0        0        0     5837 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/commands/cmd_profile.py
+-rw-r--r--   0        0        0    14092 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/commands/cmd_rabbitmq.py
+-rw-r--r--   0        0        0     2530 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/commands/cmd_restapi.py
+-rw-r--r--   0        0        0     4845 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/commands/cmd_run.py
+-rw-r--r--   0        0        0     9391 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/commands/cmd_setup.py
+-rw-r--r--   0        0        0     3439 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/commands/cmd_shell.py
+-rw-r--r--   0        0        0     6934 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/commands/cmd_status.py
+-rw-r--r--   0        0        0     6891 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/commands/cmd_storage.py
+-rw-r--r--   0        0        0     4582 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/commands/cmd_user.py
+-rw-r--r--   0        0        0     1263 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/commands/cmd_verdi.py
+-rw-r--r--   0        0        0      297 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/groups/__init__.py
+-rw-r--r--   0        0        0     5688 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/groups/dynamic.py
+-rw-r--r--   0        0        0     6657 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/groups/verdi.py
+-rw-r--r--   0        0        0     1373 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/params/__init__.py
+-rw-r--r--   0        0        0     1277 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/params/arguments/__init__.py
+-rw-r--r--   0        0        0     2924 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/params/arguments/main.py
+-rw-r--r--   0        0        0     2374 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/params/arguments/overridable.py
+-rw-r--r--   0        0        0     2652 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/params/options/__init__.py
+-rw-r--r--   0        0        0      697 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/params/options/commands/__init__.py
+-rw-r--r--   0        0        0     6869 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/params/options/commands/code.py
+-rw-r--r--   0        0        0     6882 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/params/options/commands/computer.py
+-rw-r--r--   0        0        0    13913 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/params/options/commands/setup.py
+-rw-r--r--   0        0        0     2383 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/params/options/conditional.py
+-rw-r--r--   0        0        0     8083 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/params/options/config.py
+-rw-r--r--   0        0        0     9190 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/params/options/interactive.py
+-rw-r--r--   0        0        0    21132 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/params/options/main.py
+-rw-r--r--   0        0        0     3764 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/params/options/multivalue.py
+-rw-r--r--   0        0        0     3918 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/params/options/overridable.py
+-rw-r--r--   0        0        0     1739 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/params/types/__init__.py
+-rw-r--r--   0        0        0     1348 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/params/types/calculation.py
+-rw-r--r--   0        0        0     2404 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/params/types/choice.py
+-rw-r--r--   0        0        0     2742 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/params/types/code.py
+-rw-r--r--   0        0        0     4052 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/params/types/computer.py
+-rw-r--r--   0        0        0     1702 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/params/types/config.py
+-rw-r--r--   0        0        0     1311 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/params/types/data.py
+-rw-r--r--   0        0        0     3901 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/params/types/group.py
+-rw-r--r--   0        0        0     6199 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/params/types/identifier.py
+-rw-r--r--   0        0        0     1608 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/params/types/multiple.py
+-rw-r--r--   0        0        0     1317 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/params/types/node.py
+-rw-r--r--   0        0        0     4488 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/params/types/path.py
+-rw-r--r--   0        0        0    10756 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/params/types/plugin.py
+-rw-r--r--   0        0        0     1329 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/params/types/process.py
+-rw-r--r--   0        0        0     3754 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/params/types/profile.py
+-rw-r--r--   0        0        0     3800 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/params/types/strings.py
+-rw-r--r--   0        0        0     2046 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/params/types/user.py
+-rw-r--r--   0        0        0     1335 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/params/types/workflow.py
+-rw-r--r--   0        0        0      177 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/templates/deprecated.tpl
+-rw-r--r--   0        0        0      218 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/templates/multiline.tpl
+-rw-r--r--   0        0        0      213 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/templates/new_cmt.txt.tpl
+-rw-r--r--   0        0        0      165 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/templates/warning.tpl
+-rw-r--r--   0        0        0     1122 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/utils/__init__.py
+-rw-r--r--   0        0        0     4948 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/utils/ascii_vis.py
+-rw-r--r--   0        0        0    17700 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/utils/common.py
+-rw-r--r--   0        0        0     9331 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/utils/decorators.py
+-rw-r--r--   0        0        0     1764 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/utils/defaults.py
+-rw-r--r--   0        0        0    10918 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/utils/echo.py
+-rw-r--r--   0        0        0     1710 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/utils/log.py
+-rw-r--r--   0        0        0     2336 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/utils/multi_line_input.py
+-rw-r--r--   0        0        0     2709 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/utils/pluginable.py
+-rw-r--r--   0        0        0      632 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/utils/query/__init__.py
+-rw-r--r--   0        0        0      981 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/utils/query/calculation.py
+-rw-r--r--   0        0        0     1026 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/utils/query/formatting.py
+-rw-r--r--   0        0        0     1007 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/utils/query/mapping.py
+-rw-r--r--   0        0        0     1393 2023-06-23 05:38:50.909937 aiida_core-2.4.0/aiida/cmdline/utils/repository.py
+-rw-r--r--   0        0        0     5008 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/cmdline/utils/shell.py
+-rw-r--r--   0        0        0      831 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/cmdline/utils/templates.py
+-rw-r--r--   0        0        0     2634 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/common/__init__.py
+-rw-r--r--   0        0        0    12464 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/common/constants.py
+-rw-r--r--   0        0        0     9297 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/common/datastructures.py
+-rw-r--r--   0        0        0     6332 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/common/escaping.py
+-rw-r--r--   0        0        0     8794 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/common/exceptions.py
+-rw-r--r--   0        0        0     8975 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/common/extendeddicts.py
+-rw-r--r--   0        0        0     3067 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/common/files.py
+-rw-r--r--   0        0        0    18668 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/common/folders.py
+-rw-r--r--   0        0        0    10933 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/common/hashing.py
+-rw-r--r--   0        0        0     2803 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/common/json.py
+-rw-r--r--   0        0        0     3717 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/common/lang.py
+-rw-r--r--   0        0        0     6586 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/common/links.py
+-rw-r--r--   0        0        0     9718 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/common/log.py
+-rw-r--r--   0        0        0     6909 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/common/progress_reporter.py
+-rw-r--r--   0        0        0     2800 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/common/timezone.py
+-rw-r--r--   0        0        0    19379 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/common/utils.py
+-rw-r--r--   0        0        0     1888 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/common/warnings.py
+-rw-r--r--   0        0        0     2021 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/engine/__init__.py
+-rw-r--r--   0        0        0      844 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/engine/daemon/__init__.py
+-rw-r--r--   0        0        0    31649 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/engine/daemon/client.py
+-rw-r--r--   0        0        0    31320 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/engine/daemon/execmanager.py
+-rw-r--r--   0        0        0     2529 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/engine/daemon/worker.py
+-rw-r--r--   0        0        0      919 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/engine/exceptions.py
+-rw-r--r--   0        0        0     5713 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/engine/launch.py
+-rw-r--r--   0        0        0     6513 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/engine/persistence.py
+-rw-r--r--   0        0        0     1756 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/engine/processes/__init__.py
+-rw-r--r--   0        0        0    11001 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/engine/processes/builder.py
+-rw-r--r--   0        0        0      937 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/engine/processes/calcjobs/__init__.py
+-rw-r--r--   0        0        0    48770 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/engine/processes/calcjobs/calcjob.py
+-rw-r--r--   0        0        0     1125 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/engine/processes/calcjobs/importer.py
+-rw-r--r--   0        0        0    12526 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/engine/processes/calcjobs/manager.py
+-rw-r--r--   0        0        0     8711 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/engine/processes/calcjobs/monitors.py
+-rw-r--r--   0        0        0    32305 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/engine/processes/calcjobs/tasks.py
+-rw-r--r--   0        0        0    12377 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/engine/processes/control.py
+-rw-r--r--   0        0        0     3690 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/engine/processes/exit_code.py
+-rw-r--r--   0        0        0    25694 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/engine/processes/functions.py
+-rw-r--r--   0        0        0     3852 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/engine/processes/futures.py
+-rw-r--r--   0        0        0    11954 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/engine/processes/ports.py
+-rw-r--r--   0        0        0    43938 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/engine/processes/process.py
+-rw-r--r--   0        0        0     4547 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/engine/processes/process_spec.py
+-rw-r--r--   0        0        0     1018 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/engine/processes/utils.py
+-rw-r--r--   0        0        0     1187 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/engine/processes/workchains/__init__.py
+-rw-r--r--   0        0        0     2470 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/engine/processes/workchains/awaitable.py
+-rw-r--r--   0        0        0     1968 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/engine/processes/workchains/context.py
+-rw-r--r--   0        0        0    21741 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/engine/processes/workchains/restart.py
+-rw-r--r--   0        0        0     7604 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/engine/processes/workchains/utils.py
+-rw-r--r--   0        0        0    17320 2023-06-23 05:38:50.913937 aiida_core-2.4.0/aiida/engine/processes/workchains/workchain.py
+-rw-r--r--   0        0        0    14996 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/engine/runners.py
+-rw-r--r--   0        0        0     6072 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/engine/transports.py
+-rw-r--r--   0        0        0    12275 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/engine/utils.py
+-rw-r--r--   0        0        0     1845 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/manage/__init__.py
+-rw-r--r--   0        0        0    11086 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/manage/caching.py
+-rw-r--r--   0        0        0    11486 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/manage/configuration/__init__.py
+-rw-r--r--   0        0        0    20872 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/manage/configuration/config.py
+-rw-r--r--   0        0        0     1075 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/manage/configuration/migrations/__init__.py
+-rw-r--r--   0        0        0    20944 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/manage/configuration/migrations/migrations.py
+-rw-r--r--   0        0        0     4732 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/manage/configuration/options.py
+-rw-r--r--   0        0        0    10267 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/manage/configuration/profile.py
+-rw-r--r--   0        0        0      632 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/manage/configuration/schema/__init__.py
+-rw-r--r--   0        0        0    15472 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/manage/configuration/schema/config-v5.schema.json
+-rw-r--r--   0        0        0    12291 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/manage/configuration/schema/config-v6.schema.json
+-rw-r--r--   0        0        0    12289 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/manage/configuration/schema/config-v7.schema.json
+-rw-r--r--   0        0        0    12749 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/manage/configuration/schema/config-v8.schema.json
+-rw-r--r--   0        0        0    13559 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/manage/configuration/schema/config-v9.schema.json
+-rw-r--r--   0        0        0     5305 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/manage/configuration/settings.py
+-rw-r--r--   0        0        0     1148 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/manage/external/__init__.py
+-rw-r--r--   0        0        0     9955 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/manage/external/postgres.py
+-rw-r--r--   0        0        0     1104 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/manage/external/rmq/__init__.py
+-rw-r--r--   0        0        0     3861 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/manage/external/rmq/client.py
+-rw-r--r--   0        0        0      432 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/manage/external/rmq/defaults.py
+-rw-r--r--   0        0        0     7433 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/manage/external/rmq/launcher.py
+-rw-r--r--   0        0        0     2743 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/manage/external/rmq/utils.py
+-rw-r--r--   0        0        0    20986 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/manage/manager.py
+-rw-r--r--   0        0        0    10232 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/manage/profile_access.py
+-rw-r--r--   0        0        0      993 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/manage/tests/__init__.py
+-rw-r--r--   0        0        0    19348 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/manage/tests/main.py
+-rw-r--r--   0        0        0    35099 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/manage/tests/pytest_fixtures.py
+-rw-r--r--   0        0        0     2738 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/orm/__init__.py
+-rw-r--r--   0        0        0     5406 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/orm/authinfos.py
+-rw-r--r--   0        0        0    12110 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/orm/autogroup.py
+-rw-r--r--   0        0        0     4451 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/orm/comments.py
+-rw-r--r--   0        0        0    26490 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/orm/computers.py
+-rw-r--r--   0        0        0     4716 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/orm/convert.py
+-rw-r--r--   0        0        0    10297 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/orm/entities.py
+-rw-r--r--   0        0        0     7190 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/orm/extras.py
+-rw-r--r--   0        0        0    13653 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/orm/groups.py
+-rw-r--r--   0        0        0     1628 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/orm/implementation/__init__.py
+-rw-r--r--   0        0        0     3059 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/orm/implementation/authinfos.py
+-rw-r--r--   0        0        0     3806 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/orm/implementation/comments.py
+-rw-r--r--   0        0        0     3550 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/orm/implementation/computers.py
+-rw-r--r--   0        0        0     7922 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/orm/implementation/entities.py
+-rw-r--r--   0        0        0     5792 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/orm/implementation/groups.py
+-rw-r--r--   0        0        0     3025 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/orm/implementation/logs.py
+-rw-r--r--   0        0        0    11547 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/orm/implementation/nodes.py
+-rw-r--r--   0        0        0     6576 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/orm/implementation/querybuilder.py
+-rw-r--r--   0        0        0    14684 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/orm/implementation/storage_backend.py
+-rw-r--r--   0        0        0     2459 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/orm/implementation/users.py
+-rw-r--r--   0        0        0     5746 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/orm/implementation/utils.py
+-rw-r--r--   0        0        0     7547 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/orm/logs.py
+-rw-r--r--   0        0        0     1786 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/orm/nodes/__init__.py
+-rw-r--r--   0        0        0     8303 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/orm/nodes/attributes.py
+-rw-r--r--   0        0        0     7099 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/orm/nodes/caching.py
+-rw-r--r--   0        0        0     2466 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/orm/nodes/comments.py
+-rw-r--r--   0        0        0     1885 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/orm/nodes/data/__init__.py
+-rw-r--r--   0        0        0     1069 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/orm/nodes/data/array/__init__.py
+-rw-r--r--   0        0        0     9322 2023-06-23 05:38:50.917937 aiida_core-2.4.0/aiida/orm/nodes/data/array/array.py
+-rw-r--r--   0        0        0    73817 2023-06-23 05:38:50.921937 aiida_core-2.4.0/aiida/orm/nodes/data/array/bands.py
+-rw-r--r--   0        0        0    20634 2023-06-23 05:38:50.921937 aiida_core-2.4.0/aiida/orm/nodes/data/array/kpoints.py
+-rw-r--r--   0        0        0    13106 2023-06-23 05:38:50.921937 aiida_core-2.4.0/aiida/orm/nodes/data/array/projection.py
+-rw-r--r--   0        0        0    38822 2023-06-23 05:38:50.921937 aiida_core-2.4.0/aiida/orm/nodes/data/array/trajectory.py
+-rw-r--r--   0        0        0     6269 2023-06-23 05:38:50.921937 aiida_core-2.4.0/aiida/orm/nodes/data/array/xy.py
+-rw-r--r--   0        0        0     2038 2023-06-23 05:38:50.921937 aiida_core-2.4.0/aiida/orm/nodes/data/base.py
+-rw-r--r--   0        0        0     1828 2023-06-23 05:38:50.921937 aiida_core-2.4.0/aiida/orm/nodes/data/bool.py
+-rw-r--r--   0        0        0    30424 2023-06-23 05:38:50.921937 aiida_core-2.4.0/aiida/orm/nodes/data/cif.py
+-rw-r--r--   0        0        0      401 2023-06-23 05:38:50.921937 aiida_core-2.4.0/aiida/orm/nodes/data/code/__init__.py
+-rw-r--r--   0        0        0    17156 2023-06-23 05:38:50.921937 aiida_core-2.4.0/aiida/orm/nodes/data/code/abstract.py
+-rw-r--r--   0        0        0     5354 2023-06-23 05:38:50.921937 aiida_core-2.4.0/aiida/orm/nodes/data/code/containerized.py
+-rw-r--r--   0        0        0     8279 2023-06-23 05:38:50.921937 aiida_core-2.4.0/aiida/orm/nodes/data/code/installed.py
+-rw-r--r--   0        0        0    24081 2023-06-23 05:38:50.921937 aiida_core-2.4.0/aiida/orm/nodes/data/code/legacy.py
+-rw-r--r--   0        0        0     8095 2023-06-23 05:38:50.921937 aiida_core-2.4.0/aiida/orm/nodes/data/code/portable.py
+-rw-r--r--   0        0        0    14661 2023-06-23 05:38:50.921937 aiida_core-2.4.0/aiida/orm/nodes/data/data.py
+-rw-r--r--   0        0        0     5667 2023-06-23 05:38:50.921937 aiida_core-2.4.0/aiida/orm/nodes/data/dict.py
+-rw-r--r--   0        0        0     4588 2023-06-23 05:38:50.921937 aiida_core-2.4.0/aiida/orm/nodes/data/enum.py
+-rw-r--r--   0        0        0      967 2023-06-23 05:38:50.921937 aiida_core-2.4.0/aiida/orm/nodes/data/float.py
+-rw-r--r--   0        0        0     1690 2023-06-23 05:38:50.921937 aiida_core-2.4.0/aiida/orm/nodes/data/folder.py
+-rw-r--r--   0        0        0      969 2023-06-23 05:38:50.921937 aiida_core-2.4.0/aiida/orm/nodes/data/int.py
+-rw-r--r--   0        0        0     7427 2023-06-23 05:38:50.921937 aiida_core-2.4.0/aiida/orm/nodes/data/jsonable.py
+-rw-r--r--   0        0        0     4943 2023-06-23 05:38:50.921937 aiida_core-2.4.0/aiida/orm/nodes/data/list.py
+-rw-r--r--   0        0        0     3373 2023-06-23 05:38:50.921937 aiida_core-2.4.0/aiida/orm/nodes/data/numeric.py
+-rw-r--r--   0        0        0     4784 2023-06-23 05:38:50.921937 aiida_core-2.4.0/aiida/orm/nodes/data/orbital.py
+-rw-r--r--   0        0        0      338 2023-06-23 05:38:50.921937 aiida_core-2.4.0/aiida/orm/nodes/data/remote/__init__.py
+-rw-r--r--   0        0        0     8173 2023-06-23 05:38:50.921937 aiida_core-2.4.0/aiida/orm/nodes/data/remote/base.py
+-rw-r--r--   0        0        0      326 2023-06-23 05:38:50.921937 aiida_core-2.4.0/aiida/orm/nodes/data/remote/stash/__init__.py
+-rw-r--r--   0        0        0     2371 2023-06-23 05:38:50.921937 aiida_core-2.4.0/aiida/orm/nodes/data/remote/stash/base.py
+-rw-r--r--   0        0        0     2250 2023-06-23 05:38:50.921937 aiida_core-2.4.0/aiida/orm/nodes/data/remote/stash/folder.py
+-rw-r--r--   0        0        0     5456 2023-06-23 05:38:50.921937 aiida_core-2.4.0/aiida/orm/nodes/data/singlefile.py
+-rw-r--r--   0        0        0      910 2023-06-23 05:38:50.921937 aiida_core-2.4.0/aiida/orm/nodes/data/str.py
+-rw-r--r--   0        0        0    93752 2023-06-23 05:38:50.921937 aiida_core-2.4.0/aiida/orm/nodes/data/structure.py
+-rw-r--r--   0        0        0    19092 2023-06-23 05:38:50.921937 aiida_core-2.4.0/aiida/orm/nodes/data/upf.py
+-rw-r--r--   0        0        0    11442 2023-06-23 05:38:50.921937 aiida_core-2.4.0/aiida/orm/nodes/links.py
+-rw-r--r--   0        0        0    27864 2023-06-23 05:38:50.921937 aiida_core-2.4.0/aiida/orm/nodes/node.py
+-rw-r--r--   0        0        0     1009 2023-06-23 05:38:50.921937 aiida_core-2.4.0/aiida/orm/nodes/process/__init__.py
+-rw-r--r--   0        0        0      941 2023-06-23 05:38:50.921937 aiida_core-2.4.0/aiida/orm/nodes/process/calculation/__init__.py
+-rw-r--r--   0        0        0     2605 2023-06-23 05:38:50.921937 aiida_core-2.4.0/aiida/orm/nodes/process/calculation/calcfunction.py
+-rw-r--r--   0        0        0    21163 2023-06-23 05:38:50.921937 aiida_core-2.4.0/aiida/orm/nodes/process/calculation/calcjob.py
+-rw-r--r--   0        0        0     2115 2023-06-23 05:38:50.921937 aiida_core-2.4.0/aiida/orm/nodes/process/calculation/calculation.py
+-rw-r--r--   0        0        0    21319 2023-06-23 05:38:50.921937 aiida_core-2.4.0/aiida/orm/nodes/process/process.py
+-rw-r--r--   0        0        0      936 2023-06-23 05:38:50.921937 aiida_core-2.4.0/aiida/orm/nodes/process/workflow/__init__.py
+-rw-r--r--   0        0        0     1775 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/orm/nodes/process/workflow/workchain.py
+-rw-r--r--   0        0        0     3631 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/orm/nodes/process/workflow/workflow.py
+-rw-r--r--   0        0        0     2442 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/orm/nodes/process/workflow/workfunction.py
+-rw-r--r--   0        0        0    15675 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/orm/nodes/repository.py
+-rw-r--r--   0        0        0    62197 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/orm/querybuilder.py
+-rw-r--r--   0        0        0     4785 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/orm/users.py
+-rw-r--r--   0        0        0     1415 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/orm/utils/__init__.py
+-rw-r--r--   0        0        0      632 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/orm/utils/builders/__init__.py
+-rw-r--r--   0        0        0     8496 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/orm/utils/builders/code.py
+-rw-r--r--   0        0        0     8191 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/orm/utils/builders/computer.py
+-rw-r--r--   0        0        0     4952 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/orm/utils/calcjob.py
+-rw-r--r--   0        0        0    17089 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/orm/utils/links.py
+-rw-r--r--   0        0        0    36736 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/orm/utils/loaders.py
+-rw-r--r--   0        0        0     2808 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/orm/utils/log.py
+-rw-r--r--   0        0        0    11004 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/orm/utils/managers.py
+-rw-r--r--   0        0        0     9786 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/orm/utils/mixins.py
+-rw-r--r--   0        0        0     7008 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/orm/utils/node.py
+-rw-r--r--   0        0        0     4573 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/orm/utils/remote.py
+-rw-r--r--   0        0        0     9125 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/orm/utils/serialize.py
+-rw-r--r--   0        0        0      847 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/parsers/__init__.py
+-rw-r--r--   0        0        0     8094 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/parsers/parser.py
+-rw-r--r--   0        0        0      632 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/parsers/plugins/__init__.py
+-rw-r--r--   0        0        0      632 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/parsers/plugins/arithmetic/__init__.py
+-rw-r--r--   0        0        0     2226 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/parsers/plugins/arithmetic/add.py
+-rw-r--r--   0        0        0     1984 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/parsers/plugins/diff_tutorial/parsers.py
+-rw-r--r--   0        0        0      632 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/parsers/plugins/templatereplacer/__init__.py
+-rw-r--r--   0        0        0     3244 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/parsers/plugins/templatereplacer/parser.py
+-rw-r--r--   0        0        0     1329 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/plugins/__init__.py
+-rw-r--r--   0        0        0    17336 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/plugins/entry_point.py
+-rw-r--r--   0        0        0    16492 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/plugins/factories.py
+-rw-r--r--   0        0        0     4405 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/plugins/utils.py
+-rw-r--r--   0        0        0       26 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/py.typed
+-rw-r--r--   0        0        0     1017 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/repository/__init__.py
+-rw-r--r--   0        0        0      368 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/repository/backend/__init__.py
+-rw-r--r--   0        0        0     9748 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/repository/backend/abstract.py
+-rw-r--r--   0        0        0     9788 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/repository/backend/disk_object_store.py
+-rw-r--r--   0        0        0     4392 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/repository/backend/sandbox.py
+-rw-r--r--   0        0        0     5382 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/repository/common.py
+-rw-r--r--   0        0        0    24356 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/repository/repository.py
+-rw-r--r--   0        0        0      823 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/restapi/__init__.py
+-rw-r--r--   0        0        0     7379 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/restapi/api.py
+-rw-r--r--   0        0        0      632 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/restapi/common/__init__.py
+-rw-r--r--   0        0        0     1701 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/restapi/common/config.py
+-rw-r--r--   0        0        0     1589 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/restapi/common/exceptions.py
+-rw-r--r--   0        0        0    19441 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/restapi/common/identifiers.py
+-rw-r--r--   0        0        0    34388 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/restapi/common/utils.py
+-rw-r--r--   0        0        0    29019 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/restapi/resources.py
+-rwxr-xr-x   0        0        0     4910 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/restapi/run_api.py
+-rw-r--r--   0        0        0      632 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/restapi/translator/__init__.py
+-rw-r--r--   0        0        0    18895 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/restapi/translator/base.py
+-rw-r--r--   0        0        0     4247 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/restapi/translator/computer.py
+-rw-r--r--   0        0        0     3357 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/restapi/translator/group.py
+-rw-r--r--   0        0        0      632 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/restapi/translator/nodes/__init__.py
+-rw-r--r--   0        0        0     2835 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/restapi/translator/nodes/data/__init__.py
+-rw-r--r--   0        0        0      632 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/restapi/translator/nodes/data/array/__init__.py
+-rw-r--r--   0        0        0     2087 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/restapi/translator/nodes/data/array/bands.py
+-rw-r--r--   0        0        0     1514 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/restapi/translator/nodes/data/cif.py
+-rw-r--r--   0        0        0     1500 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/restapi/translator/nodes/data/code.py
+-rw-r--r--   0        0        0     5437 2023-06-23 05:38:50.925937 aiida_core-2.4.0/aiida/restapi/translator/nodes/data/kpoints.py
+-rw-r--r--   0        0        0     1615 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/restapi/translator/nodes/data/structure.py
+-rw-r--r--   0        0        0     1424 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/restapi/translator/nodes/data/upf.py
+-rw-r--r--   0        0        0    31797 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/restapi/translator/nodes/node.py
+-rw-r--r--   0        0        0      632 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/restapi/translator/nodes/process/__init__.py
+-rw-r--r--   0        0        0      632 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/restapi/translator/nodes/process/calculation/__init__.py
+-rw-r--r--   0        0        0     1615 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/restapi/translator/nodes/process/calculation/calcfunction.py
+-rw-r--r--   0        0        0     2655 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/restapi/translator/nodes/process/calculation/calcjob.py
+-rw-r--r--   0        0        0     4530 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/restapi/translator/nodes/process/process.py
+-rw-r--r--   0        0        0      632 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/restapi/translator/nodes/process/workflow/__init__.py
+-rw-r--r--   0        0        0     1581 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/restapi/translator/nodes/process/workflow/workchain.py
+-rw-r--r--   0        0        0     1612 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/restapi/translator/nodes/process/workflow/workfunction.py
+-rw-r--r--   0        0        0     2801 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/restapi/translator/user.py
+-rw-r--r--   0        0        0     1074 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/schedulers/__init__.py
+-rw-r--r--   0        0        0    27253 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/schedulers/datastructures.py
+-rw-r--r--   0        0        0      632 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/schedulers/plugins/__init__.py
+-rw-r--r--   0        0        0    15758 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/schedulers/plugins/direct.py
+-rw-r--r--   0        0        0    33346 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/schedulers/plugins/lsf.py
+-rw-r--r--   0        0        0    31062 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/schedulers/plugins/pbsbaseclasses.py
+-rw-r--r--   0        0        0     3701 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/schedulers/plugins/pbspro.py
+-rw-r--r--   0        0        0    20455 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/schedulers/plugins/sge.py
+-rw-r--r--   0        0        0    35173 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/schedulers/plugins/slurm.py
+-rw-r--r--   0        0        0     3799 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/schedulers/plugins/torque.py
+-rw-r--r--   0        0        0    20022 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/schedulers/scheduler.py
+-rw-r--r--   0        0        0     1108 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/sphinxext/__init__.py
+-rw-r--r--   0        0        0     1450 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/sphinxext/calcjob.py
+-rw-r--r--   0        0        0     9048 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/sphinxext/process.py
+-rw-r--r--   0        0        0     1475 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/sphinxext/workchain.py
+-rw-r--r--   0        0        0      810 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/storage/__init__.py
+-rw-r--r--   0        0        0      815 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/storage/log.py
+-rw-r--r--   0        0        0      877 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/storage/psql_dos/__init__.py
+-rwxr-xr-x   0        0        0     3996 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/storage/psql_dos/alembic_cli.py
+-rw-r--r--   0        0        0    18128 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/storage/psql_dos/backend.py
+-rw-r--r--   0        0        0      632 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/__init__.py
+-rw-r--r--   0        0        0     2204 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/env.py
+-rw-r--r--   0        0        0      494 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/script.py.mako
+-rw-r--r--   0        0        0      748 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/utils/__init__.py
+-rw-r--r--   0        0        0     2260 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/utils/calc_state.py
+-rw-r--r--   0        0        0     3916 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/utils/create_dbattribute.py
+-rw-r--r--   0        0        0     8837 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/utils/dblog_update.py
+-rw-r--r--   0        0        0     1563 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/utils/duplicate_uuids.py
+-rw-r--r--   0        0        0    13347 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/utils/integrity.py
+-rw-r--r--   0        0        0     3477 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/utils/legacy_workflows.py
+-rw-r--r--   0        0        0     5991 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/utils/migrate_repository.py
+-rw-r--r--   0        0        0     9306 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/utils/parity.py
+-rw-r--r--   0        0        0     7520 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/utils/provenance_redesign.py
+-rw-r--r--   0        0        0     5566 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/utils/reflect.py
+-rw-r--r--   0        0        0    18164 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/utils/utils.py
+-rw-r--r--   0        0        0     2902 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/041a79fc615f_dblog_cleaning.py
+-rw-r--r--   0        0        0     1486 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/07fac78e6209_drop_computer_transport_params.py
+-rw-r--r--   0        0        0     2482 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/0aebbeab274d_base_data_plugin_type_string.py
+-rw-r--r--   0        0        0     1819 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/0edcdd5a30f0_dbgroup_extras.py
+-rw-r--r--   0        0        0     1829 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/118349c10896_default_link_label.py
+-rw-r--r--   0        0        0     2600 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/12536798d4d3_trajectory_symbols_to_attribute.py
+-rw-r--r--   0        0        0     2740 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/140c971ae0a3_migrate_builtin_calculations.py
+-rw-r--r--   0        0        0     1168 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/162b99bca4a2_drop_dbcalcstate.py
+-rw-r--r--   0        0        0     1361 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/1830c8430131_drop_node_columns_nodeversion_public.py
+-rw-r--r--   0        0        0     1872 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/1b8ed3425af9_remove_legacy_workflows.py
+-rw-r--r--   0        0        0     9697 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/1de112340b16_django_parity_1.py
+-rw-r--r--   0        0        0    10079 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/1de112340b17_django_parity_2.py
+-rw-r--r--   0        0        0     1252 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/1de112340b18_django_parity_3.py
+-rw-r--r--   0        0        0     1382 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/1feaea71bd5a_migrate_repository.py
+-rw-r--r--   0        0        0     5530 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/239cea6d2452_provenance_redesign.py
+-rw-r--r--   0        0        0     8062 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/26d561acd560_data_migration_legacy_job_calculations.py
+-rw-r--r--   0        0        0     5861 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/34a831f4286d_entry_point_core_prefix.py
+-rw-r--r--   0        0        0     2044 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/35d4ee9a1b0e_code_hidden_attr_to_extra.py
+-rw-r--r--   0        0        0     1309 2023-06-23 05:38:50.929937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/375c2db70663_dblog_uuid_uniqueness_constraint.py
+-rw-r--r--   0        0        0     1488 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/37f3d4882837_make_all_uuid_columns_unique.py
+-rw-r--r--   0        0        0     1218 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/3d6190594e19_remove_dbcomputer_enabled.py
+-rw-r--r--   0        0        0      802 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/535039300e4a_computer_name_to_label.py
+-rw-r--r--   0        0        0     1892 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/59edaf8a8b79_adding_indexes_and_constraints_to_the_.py
+-rw-r--r--   0        0        0     1689 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/5a49629f0d45_dblink_indices.py
+-rw-r--r--   0        0        0     1626 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/5d4d844852b6_invalidating_node_hash.py
+-rw-r--r--   0        0        0     1645 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/5ddd24e52864_dbnode_type_to_dbnode_node_type.py
+-rw-r--r--   0        0        0     1866 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/61fc0913fae9_remove_node_prefix.py
+-rw-r--r--   0        0        0     1391 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/62fe0d36de90_add_node_uuid_unique_constraint.py
+-rw-r--r--   0        0        0     1621 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/6a5c2ea1439d_move_data_within_node_module.py
+-rw-r--r--   0        0        0     1376 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/6c629c886f84_process_type.py
+-rw-r--r--   0        0        0     1351 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/70c7d732f1b2_delete_dbpath.py
+-rw-r--r--   0        0        0     1466 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/7536a82b2cc4_add_node_repository_metadata.py
+-rw-r--r--   0        0        0     1360 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/7a6587e16f4c_unique_constraints_for_the_db_dbgroup_.py
+-rw-r--r--   0        0        0     2493 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/7b38a9e783e7_seal_unsealed_processes.py
+-rw-r--r--   0        0        0     3732 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/7ca08c391c49_calc_job_option_attribute_keys.py
+-rw-r--r--   0        0        0     1311 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/89176227b25_add_indexes_to_dbworkflowdata_table.py
+-rw-r--r--   0        0        0     2192 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/91b573400be5_prepare_schema_reset.py
+-rw-r--r--   0        0        0      632 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/__init__.py
+-rw-r--r--   0        0        0     1158 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/a514d673c163_drop_dblock.py
+-rw-r--r--   0        0        0     1656 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/a603da2cc809_code_sub_class_of_data.py
+-rw-r--r--   0        0        0     6613 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/a6048f0ffca8_update_linktypes.py
+-rw-r--r--   0        0        0     1840 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/b8b23ddefad4_dbgroup_name_to_label_type_to_type_string.py
+-rw-r--r--   0        0        0     1778 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/bf591f31dd12_dbgroup_type_string.py
+-rw-r--r--   0        0        0     2269 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/ce56d84bcc35_delete_trajectory_symbols_array.py
+-rw-r--r--   0        0        0     1599 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/d254fdfed416_rename_parameter_data_to_dict.py
+-rw-r--r--   0        0        0     1564 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/de2eaf6978b4_simplify_user_model.py
+-rw-r--r--   0        0        0    30892 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0001_initial.py
+-rw-r--r--   0        0        0     1505 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0002_db_state_change.py
+-rw-r--r--   0        0        0     1809 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0003_add_link_type.py
+-rw-r--r--   0        0        0     1547 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0004_add_daemon_and_uuid_indices.py
+-rw-r--r--   0        0        0     1246 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0005_add_cmtime_indices.py
+-rw-r--r--   0        0        0     1295 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0006_delete_dbpath.py
+-rw-r--r--   0        0        0     6316 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0007_update_linktypes.py
+-rw-r--r--   0        0        0     2359 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0008_code_hidden_to_extra.py
+-rw-r--r--   0        0        0     2275 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0009_base_data_plugin_type_string.py
+-rw-r--r--   0        0        0     1474 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0010_process_type.py
+-rw-r--r--   0        0        0     1712 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0011_delete_kombu_tables.py
+-rw-r--r--   0        0        0     1073 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0012_drop_dblock.py
+-rw-r--r--   0        0        0     1747 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0013_django_1_8.py
+-rw-r--r--   0        0        0     1374 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0014_add_node_uuid_unique_constraint.py
+-rw-r--r--   0        0        0     1192 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0015_invalidating_node_hash.py
+-rw-r--r--   0        0        0     1171 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0016_code_sub_class_of_data.py
+-rw-r--r--   0        0        0     1083 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0017_drop_dbcalcstate.py
+-rw-r--r--   0        0        0     2391 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0018_django_1_11.py
+-rw-r--r--   0        0        0     2558 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0019_migrate_builtin_calculations.py
+-rw-r--r--   0        0        0     6233 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0020_provenance_redesign.py
+-rw-r--r--   0        0        0     2439 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0021_dbgroup_name_to_label_type_to_type_string.py
+-rw-r--r--   0        0        0     1539 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0022_dbgroup_type_string_change_content.py
+-rw-r--r--   0        0        0     3316 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0023_calc_job_option_attribute_keys.py
+-rw-r--r--   0        0        0     3663 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0024a_dblog_update.py
+-rw-r--r--   0        0        0     1248 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0024b_dblog_update.py
+-rw-r--r--   0        0        0     1480 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0025_move_data_within_node_module.py
+-rw-r--r--   0        0        0     2250 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0026_trajectory_symbols_to_attribute.py
+-rw-r--r--   0        0        0     2415 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0027_delete_trajectory_symbols_array.py
+-rw-r--r--   0        0        0     1598 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0028_remove_node_prefix.py
+-rw-r--r--   0        0        0     1383 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0029_rename_parameter_data_to_dict.py
+-rw-r--r--   0        0        0     1267 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0030_dbnode_type_to_dbnode_node_type.py
+-rw-r--r--   0        0        0     1140 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0031_remove_dbcomputer_enabled.py
+-rw-r--r--   0        0        0     1552 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0032_remove_legacy_workflows.py
+-rw-r--r--   0        0        0     1516 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0033_replace_text_field_with_json_field.py
+-rw-r--r--   0        0        0     1203 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0034_drop_node_columns_nodeversion_public.py
+-rw-r--r--   0        0        0     1550 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0035_simplify_user_model.py
+-rw-r--r--   0        0        0     1156 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0036_drop_computer_transport_params.py
+-rw-r--r--   0        0        0     7292 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0037_attributes_extras_settings_json.py
+-rw-r--r--   0        0        0     7899 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0038_data_migration_legacy_job_calculations.py
+-rw-r--r--   0        0        0     1280 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0039_reset_hash.py
+-rw-r--r--   0        0        0     3186 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0040_data_migration_legacy_process_attributes.py
+-rw-r--r--   0        0        0     2403 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0041_seal_unsealed_processes.py
+-rw-r--r--   0        0        0     2115 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0042_prepare_schema_reset.py
+-rw-r--r--   0        0        0     1612 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0043_default_link_label.py
+-rw-r--r--   0        0        0     1615 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0044_dbgroup_type_string.py
+-rw-r--r--   0        0        0     1673 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0045_dbgroup_extras.py
+-rw-r--r--   0        0        0     1378 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0046_add_node_repository_metadata.py
+-rw-r--r--   0        0        0     1297 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0047_migrate_repository.py
+-rw-r--r--   0        0        0     1728 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0048_computer_name_to_label.py
+-rw-r--r--   0        0        0     5770 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0049_entry_point_core_prefix.py
+-rw-r--r--   0        0        0     1974 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0050_sqlalchemy_parity.py
+-rw-r--r--   0        0        0    21476 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/e15ef2630a1b_initial_schema.py
+-rw-r--r--   0        0        0     2135 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/e72ad251bcdb_dbgroup_class_change_type_string_values.py
+-rw-r--r--   0        0        0     3276 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/e734dd5e50d7_data_migration_legacy_process_attributes.py
+-rw-r--r--   0        0        0     1363 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/e797afa09270_reset_hash.py
+-rw-r--r--   0        0        0     1760 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/ea2f50e7f615_dblog_create_uuid_column.py
+-rw-r--r--   0        0        0     2221 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/f9a69de76a9a_delete_kombu_tables.py
+-rw-r--r--   0        0        0    11820 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/main_0001_initial.py
+-rw-r--r--   0        0        0     1553 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/main_0002_recompute_hash_calc_job_node.py
+-rw-r--r--   0        0        0    21850 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/migrator.py
+-rw-r--r--   0        0        0      703 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/models/__init__.py
+-rw-r--r--   0        0        0     2660 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/models/authinfo.py
+-rw-r--r--   0        0        0     4494 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/models/base.py
+-rw-r--r--   0        0        0     2322 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/models/comment.py
+-rw-r--r--   0        0        0     2904 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/models/computer.py
+-rw-r--r--   0        0        0     3635 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/models/group.py
+-rw-r--r--   0        0        0     2677 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/models/log.py
+-rw-r--r--   0        0        0     8274 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/models/node.py
+-rw-r--r--   0        0        0     1749 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/models/settings.py
+-rw-r--r--   0        0        0     1739 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/models/user.py
+-rw-r--r--   0        0        0      678 2023-06-23 05:38:50.933937 aiida_core-2.4.0/aiida/storage/psql_dos/orm/__init__.py
+-rw-r--r--   0        0        0     4752 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/storage/psql_dos/orm/authinfos.py
+-rw-r--r--   0        0        0     6320 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/storage/psql_dos/orm/comments.py
+-rw-r--r--   0        0        0     4282 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/storage/psql_dos/orm/computers.py
+-rw-r--r--   0        0        0     3537 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/storage/psql_dos/orm/convert.py
+-rw-r--r--   0        0        0     3483 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/storage/psql_dos/orm/entities.py
+-rw-r--r--   0        0        0     3251 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/storage/psql_dos/orm/extras_mixin.py
+-rw-r--r--   0        0        0    10474 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/storage/psql_dos/orm/groups.py
+-rw-r--r--   0        0        0     5113 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/storage/psql_dos/orm/logs.py
+-rw-r--r--   0        0        0    10981 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/storage/psql_dos/orm/nodes.py
+-rw-r--r--   0        0        0      746 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/storage/psql_dos/orm/querybuilder/__init__.py
+-rw-r--r--   0        0        0    23391 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/storage/psql_dos/orm/querybuilder/joiner.py
+-rw-r--r--   0        0        0    45959 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/storage/psql_dos/orm/querybuilder/main.py
+-rw-r--r--   0        0        0     2324 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/storage/psql_dos/orm/users.py
+-rw-r--r--   0        0        0     7345 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/storage/psql_dos/orm/utils.py
+-rw-r--r--   0        0        0     8962 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/storage/psql_dos/utils.py
+-rw-r--r--   0        0        0     1022 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/storage/sqlite_temp/__init__.py
+-rw-r--r--   0        0        0     7561 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/storage/sqlite_temp/backend.py
+-rw-r--r--   0        0        0     1664 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/storage/sqlite_zip/__init__.py
+-rw-r--r--   0        0        0    15054 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/storage/sqlite_zip/backend.py
+-rw-r--r--   0        0        0      632 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/storage/sqlite_zip/migrations/__init__.py
+-rw-r--r--   0        0        0     2005 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/storage/sqlite_zip/migrations/env.py
+-rw-r--r--   0        0        0     1754 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/storage/sqlite_zip/migrations/legacy/__init__.py
+-rw-r--r--   0        0        0     3332 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/storage/sqlite_zip/migrations/legacy/v04_to_v05.py
+-rw-r--r--   0        0        0     7335 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/storage/sqlite_zip/migrations/legacy/v05_to_v06.py
+-rw-r--r--   0        0        0     5971 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/storage/sqlite_zip/migrations/legacy/v06_to_v07.py
+-rw-r--r--   0        0        0     2107 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/storage/sqlite_zip/migrations/legacy/v07_to_v08.py
+-rw-r--r--   0        0        0     2361 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/storage/sqlite_zip/migrations/legacy/v08_to_v09.py
+-rw-r--r--   0        0        0     1355 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/storage/sqlite_zip/migrations/legacy/v09_to_v10.py
+-rw-r--r--   0        0        0     1480 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/storage/sqlite_zip/migrations/legacy/v10_to_v11.py
+-rw-r--r--   0        0        0     5486 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/storage/sqlite_zip/migrations/legacy/v11_to_v12.py
+-rw-r--r--   0        0        0     1698 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/storage/sqlite_zip/migrations/legacy/v12_to_v13.py
+-rw-r--r--   0        0        0    12706 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/storage/sqlite_zip/migrations/legacy_to_main.py
+-rw-r--r--   0        0        0      572 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/storage/sqlite_zip/migrations/script.py.mako
+-rw-r--r--   0        0        0     8160 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/storage/sqlite_zip/migrations/utils.py
+-rw-r--r--   0        0        0     8703 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/storage/sqlite_zip/migrations/v1_db_schema.py
+-rw-r--r--   0        0        0      632 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/storage/sqlite_zip/migrations/versions/__init__.py
+-rw-r--r--   0        0        0     8710 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/storage/sqlite_zip/migrations/versions/main_0000_initial.py
+-rw-r--r--   0        0        0     6790 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/storage/sqlite_zip/migrations/versions/main_0000a_replace_nulls.py
+-rw-r--r--   0        0        0     4413 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/storage/sqlite_zip/migrations/versions/main_0000b_non_nullable.py
+-rw-r--r--   0        0        0     1044 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/storage/sqlite_zip/migrations/versions/main_0001.py
+-rw-r--r--   0        0        0    17760 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/storage/sqlite_zip/migrator.py
+-rw-r--r--   0        0        0     7070 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/storage/sqlite_zip/models.py
+-rw-r--r--   0        0        0    15167 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/storage/sqlite_zip/orm.py
+-rw-r--r--   0        0        0     4882 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/storage/sqlite_zip/utils.py
+-rw-r--r--   0        0        0     1845 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/tools/__init__.py
+-rw-r--r--   0        0        0     1366 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/tools/archive/__init__.py
+-rw-r--r--   0        0        0     9493 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/tools/archive/abstract.py
+-rw-r--r--   0        0        0     3349 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/tools/archive/common.py
+-rw-r--r--   0        0        0    29963 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/tools/archive/create.py
+-rw-r--r--   0        0        0     2018 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/tools/archive/exceptions.py
+-rw-r--r--   0        0        0      844 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/tools/archive/implementations/__init__.py
+-rw-r--r--   0        0        0      836 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/tools/archive/implementations/sqlite_zip/__init__.py
+-rw-r--r--   0        0        0     3280 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/tools/archive/implementations/sqlite_zip/main.py
+-rw-r--r--   0        0        0     2268 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/tools/archive/implementations/sqlite_zip/reader.py
+-rw-r--r--   0        0        0    12718 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/tools/archive/implementations/sqlite_zip/writer.py
+-rw-r--r--   0        0        0    50561 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/tools/archive/imports.py
+-rw-r--r--   0        0        0      833 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/tools/calculations/__init__.py
+-rw-r--r--   0        0        0     1053 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/tools/calculations/base.py
+-rw-r--r--   0        0        0      997 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/tools/data/__init__.py
+-rw-r--r--   0        0        0      862 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/tools/data/array/__init__.py
+-rw-r--r--   0        0        0      952 2023-06-23 05:38:50.937937 aiida_core-2.4.0/aiida/tools/data/array/kpoints/__init__.py
+-rw-r--r--   0        0        0    77224 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/tools/data/array/kpoints/legacy.py
+-rw-r--r--   0        0        0    10748 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/tools/data/array/kpoints/main.py
+-rw-r--r--   0        0        0     7024 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/tools/data/array/kpoints/seekpath.py
+-rw-r--r--   0        0        0     1377 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/tools/data/array/trajectory.py
+-rw-r--r--   0        0        0     8683 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/tools/data/cif.py
+-rw-r--r--   0        0        0      899 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/tools/data/orbital/__init__.py
+-rw-r--r--   0        0        0     6521 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/tools/data/orbital/orbital.py
+-rw-r--r--   0        0        0    13938 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/tools/data/orbital/realhydrogen.py
+-rw-r--r--   0        0        0    11904 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/tools/data/structure.py
+-rw-r--r--   0        0        0      632 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/tools/dbexporters/__init__.py
+-rw-r--r--   0        0        0      783 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/tools/dbimporters/__init__.py
+-rw-r--r--   0        0        0    12076 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/tools/dbimporters/baseclasses.py
+-rw-r--r--   0        0        0      720 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/tools/dbimporters/plugins/__init__.py
+-rw-r--r--   0        0        0    12075 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/tools/dbimporters/plugins/cod.py
+-rw-r--r--   0        0        0    28481 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/tools/dbimporters/plugins/icsd.py
+-rw-r--r--   0        0        0     6960 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/tools/dbimporters/plugins/materialsproject.py
+-rw-r--r--   0        0        0    11616 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/tools/dbimporters/plugins/mpds.py
+-rw-r--r--   0        0        0     5667 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/tools/dbimporters/plugins/mpod.py
+-rw-r--r--   0        0        0     5369 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/tools/dbimporters/plugins/nninc.py
+-rw-r--r--   0        0        0     4662 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/tools/dbimporters/plugins/oqmd.py
+-rw-r--r--   0        0        0     4463 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/tools/dbimporters/plugins/pcod.py
+-rw-r--r--   0        0        0     2691 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/tools/dbimporters/plugins/tcod.py
+-rw-r--r--   0        0        0      883 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/tools/graph/__init__.py
+-rw-r--r--   0        0        0    17137 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/tools/graph/age_entities.py
+-rw-r--r--   0        0        0    18098 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/tools/graph/age_rules.py
+-rw-r--r--   0        0        0     7116 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/tools/graph/deletions.py
+-rw-r--r--   0        0        0    12733 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/tools/graph/graph_traversers.py
+-rw-r--r--   0        0        0     1382 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/tools/groups/__init__.py
+-rw-r--r--   0        0        0    12617 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/tools/groups/paths.py
+-rw-r--r--   0        0        0      632 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/tools/ipython/__init__.py
+-rw-r--r--   0        0        0     1212 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/tools/ipython/aiida_magic_register.py
+-rw-r--r--   0        0        0     7920 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/tools/ipython/ipython_magics.py
+-rw-r--r--   0        0        0        0 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/tools/query/__init__.py
+-rw-r--r--   0        0        0     6826 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/tools/query/calculation.py
+-rw-r--r--   0        0        0     2963 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/tools/query/formatting.py
+-rw-r--r--   0        0        0     7054 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/tools/query/mapping.py
+-rw-r--r--   0        0        0      941 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/tools/visualization/__init__.py
+-rw-r--r--   0        0        0    35782 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/tools/visualization/graph.py
+-rw-r--r--   0        0        0      943 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/transports/__init__.py
+-rw-r--r--   0        0        0     6400 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/transports/cli.py
+-rw-r--r--   0        0        0      851 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/transports/plugins/__init__.py
+-rw-r--r--   0        0        0    37031 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/transports/plugins/local.py
+-rw-r--r--   0        0        0    62951 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/transports/plugins/ssh.py
+-rw-r--r--   0        0        0    30913 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/transports/transport.py
+-rw-r--r--   0        0        0     3273 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/transports/util.py
+-rw-r--r--   0        0        0      632 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/workflows/__init__.py
+-rw-r--r--   0        0        0      632 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/workflows/arithmetic/__init__.py
+-rw-r--r--   0        0        0     1057 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/workflows/arithmetic/add_multiply.py
+-rw-r--r--   0        0        0     2538 2023-06-23 05:38:50.941937 aiida_core-2.4.0/aiida/workflows/arithmetic/multiply_add.py
+-rw-r--r--   0        0        0      327 2023-06-23 05:38:50.941937 aiida_core-2.4.0/codecov.yml
+-rw-r--r--   0        0        0      666 2023-06-23 05:38:50.997937 aiida_core-2.4.0/environment.yml
+-rw-r--r--   0        0        0    13919 2023-06-23 05:38:50.997937 aiida_core-2.4.0/open_source_licenses.txt
+-rw-r--r--   0        0        0    15885 2023-06-23 05:38:50.997937 aiida_core-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0      510 2023-06-23 05:38:50.997937 aiida_core-2.4.0/requirements/README.md
+-rw-r--r--   0        0        0     4229 2023-06-23 05:38:50.997937 aiida_core-2.4.0/requirements/requirements-py-3.10.txt
+-rw-r--r--   0        0        0     4194 2023-06-23 05:38:50.997937 aiida_core-2.4.0/requirements/requirements-py-3.11.txt
+-rw-r--r--   0        0        0     4304 2023-06-23 05:38:50.997937 aiida_core-2.4.0/requirements/requirements-py-3.9.txt
+-rw-r--r--   0        0        0      473 2023-06-23 05:38:51.053937 aiida_core-2.4.0/utils/.gource.conf
+-rw-r--r--   0        0        0      697 2023-06-23 05:38:51.053937 aiida_core-2.4.0/utils/__init__.py
+-rwxr-xr-x   0        0        0    16839 2023-06-23 05:38:51.057937 aiida_core-2.4.0/utils/dependency_management.py
+-rw-r--r--   0        0        0     6562 2023-06-23 05:38:51.057937 aiida_core-2.4.0/utils/make_all.py
+-rw-r--r--   0        0        0       73 2023-06-23 05:38:51.057937 aiida_core-2.4.0/utils/requirements.txt
+-rw-r--r--   0        0        0     5871 2023-06-23 05:38:51.057937 aiida_core-2.4.0/utils/validate_consistency.py
+-rw-r--r--   0        0        0    10971 1970-01-01 00:00:00.000000 aiida_core-2.4.0/PKG-INFO
```

### Comparing `aiida_core-2.3.1/.devcontainer/Dockerfile` & `aiida_core-2.4.0/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/.devcontainer/docker-compose.yml` & `aiida_core-2.4.0/.devcontainer/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/.docker/docker-rabbitmq.yml` & `aiida_core-2.4.0/.docker/docker-rabbitmq.yml`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/.docker/opt/configure-aiida.sh` & `aiida_core-2.4.0/.docker/opt/configure-aiida.sh`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/.github/CODEOWNERS` & `aiida_core-2.4.0/.github/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/.github/ISSUE_TEMPLATE/bug_report.md` & `aiida_core-2.4.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/.github/ISSUE_TEMPLATE/feature_request.md` & `aiida_core-2.4.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/.github/config/slurm_rsa` & `aiida_core-2.4.0/.github/config/slurm_rsa`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/.github/system_tests/pytest/test_memory_leaks.py` & `aiida_core-2.4.0/.github/system_tests/pytest/test_memory_leaks.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/.github/system_tests/test_containerized_code.py` & `aiida_core-2.4.0/.github/system_tests/test_containerized_code.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/.github/system_tests/test_daemon.py` & `aiida_core-2.4.0/.github/system_tests/test_daemon.py`

 * *Files 0% similar despite different names*

```diff
@@ -289,30 +289,28 @@
 
 
 def create_calculation_process(code, inputval):
     """
     Create the process and inputs for a submitting / running a calculation.
     """
     TemplatereplacerCalculation = CalculationFactory('core.templatereplacer')
-    parameters = Dict(dict={'value': inputval})
-    template = Dict(
-        dict={
-            # The following line adds a significant sleep time.
-            # I set it to 1 second to speed up tests
-            # I keep it to a non-zero value because I want
-            # To test the case when AiiDA finds some calcs
-            # in a queued state
-            # 'cmdline_params': ["{}".format(counter % 3)], # Sleep time
-            'cmdline_params': ['1'],
-            'input_file_template': '{value}',  # File just contains the value to double
-            'input_file_name': 'value_to_double.txt',
-            'output_file_name': 'output.txt',
-            'retrieve_temporary_files': ['triple_value.tmp']
-        }
-    )
+    parameters = Dict({'value': inputval})
+    template = Dict({
+        # The following line adds a significant sleep time.
+        # I set it to 1 second to speed up tests
+        # I keep it to a non-zero value because I want
+        # To test the case when AiiDA finds some calcs
+        # in a queued state
+        # 'cmdline_params': ["{}".format(counter % 3)], # Sleep time
+        'cmdline_params': ['1'],
+        'input_file_template': '{value}',  # File just contains the value to double
+        'input_file_name': 'value_to_double.txt',
+        'output_file_name': 'output.txt',
+        'retrieve_temporary_files': ['triple_value.tmp']
+    })
     options = {
         'resources': {
             'num_machines': 1
         },
         'max_wallclock_seconds': 5 * 60,
         'withmpi': False,
         'parser_name': 'core.templatereplacer',
@@ -380,15 +378,15 @@
     results, node = run.get_node(ArithmeticAddBaseWorkChain, **inputs)
     assert not node.is_finished_ok, node.process_state
     assert node.exit_status == ArithmeticAddBaseWorkChain.exit_codes.ERROR_TOO_BIG.status, node.exit_status  # pylint: disable=no-member
     assert len(node.called) == 1
 
     # Check that overriding default handler enabled status works
     inputs['add']['y'] = Int(1)
-    inputs['handler_overrides'] = Dict(dict={'disabled_handler': True})
+    inputs['handler_overrides'] = Dict({'disabled_handler': True})
     results, node = run.get_node(ArithmeticAddBaseWorkChain, **inputs)
     assert not node.is_finished_ok, node.process_state
     assert node.exit_status == ArithmeticAddBaseWorkChain.exit_codes.ERROR_ENABLED_DOOM.status, node.exit_status  # pylint: disable=no-member
     assert len(node.called) == 1
 
 
 def run_multiply_add_workchain():
```

### Comparing `aiida_core-2.3.1/.github/system_tests/test_ipython_magics.py` & `aiida_core-2.4.0/.github/system_tests/test_ipython_magics.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/.github/system_tests/test_polish_workchains.sh` & `aiida_core-2.4.0/.github/system_tests/test_polish_workchains.sh`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/.github/system_tests/test_profile_manager.py` & `aiida_core-2.4.0/.github/system_tests/test_profile_manager.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/.github/system_tests/test_test_manager.py` & `aiida_core-2.4.0/.github/system_tests/test_test_manager.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/.github/system_tests/test_verdi_load_time.sh` & `aiida_core-2.4.0/.github/system_tests/test_verdi_load_time.sh`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/.github/system_tests/workchains.py` & `aiida_core-2.4.0/.github/system_tests/workchains.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
     @process_handler(priority=460, enabled=False)
     def disabled_handler(self, node):  # pylint: disable=unused-argument
         """By default this is not enabled and so should never be called, irrespective of exit codes of sub process."""
         return ProcessHandlerReport(True, self.exit_codes.ERROR_ENABLED_DOOM)  # pylint: disable=no-member
 
     @process_handler(priority=450, exit_codes=ExitCode(1000, 'Unicorn encountered'))
-    def a_magic_unicorn_appeared(self, node):  # pylint: disable=no-self-argument,no-self-use
+    def a_magic_unicorn_appeared(self, node):  # pylint: disable=no-self-argument
         """As we all know unicorns do not exist so we should never have to deal with it."""
         raise RuntimeError('this handler should never even have been called')
 
     @process_handler(priority=400, exit_codes=ArithmeticAddCalculation.exit_codes.ERROR_NEGATIVE_NUMBER)
     def error_negative_sum(self, node):
         """What even is a negative number, how can I have minus three melons?!."""
         self.ctx.inputs.x = Int(abs(node.inputs.x.value))
```

### Comparing `aiida_core-2.3.1/.github/workflows/benchmark-config.json` & `aiida_core-2.4.0/.github/workflows/benchmark-config.json`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/.github/workflows/benchmark.yml` & `aiida_core-2.4.0/.github/workflows/benchmark.yml`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/.github/workflows/build_and_test_docker_on_pr.yml` & `aiida_core-2.4.0/.github/workflows/build_and_test_docker_on_pr.yml`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/.github/workflows/check_release_tag.py` & `aiida_core-2.4.0/.github/workflows/check_release_tag.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/.github/workflows/ci-code.yml` & `aiida_core-2.4.0/.github/workflows/ci-code.yml`

 * *Files 5% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 
     runs-on: ubuntu-latest
     timeout-minutes: 5
 
     steps:
     - uses: actions/checkout@v2
 
-    - name: Set up Python 3.8
+    - name: Set up Python 3.9
       uses: actions/setup-python@v2
       with:
-        python-version: '3.8'
+        python-version: '3.9'
 
     - name: Install utils/ dependencies
       run: pip install -r utils/requirements.txt
 
     - name: Check requirements files
       id: check_reqs
       run: python ./utils/dependency_management.py check-requirements DEFAULT
@@ -45,15 +45,15 @@
 
     runs-on: ubuntu-latest
     timeout-minutes: 45
 
     strategy:
       fail-fast: false
       matrix:
-        python-version: ['3.8', '3.11']
+        python-version: ['3.9', '3.11']
 
     services:
       postgres:
         image: postgres:10
         env:
           POSTGRES_DB: test_aiida
           POSTGRES_PASSWORD: ''
@@ -107,30 +107,30 @@
       env:
         AIIDA_WARN_v3: 1
         SQLALCHEMY_WARN_20: 1
       run:
         .github/workflows/tests.sh
 
     - name: Upload coverage report
-      if: matrix.python-version == 3.8 && github.repository == 'aiidateam/aiida-core'
+      if: matrix.python-version == 3.9 && github.repository == 'aiidateam/aiida-core'
       uses: codecov/codecov-action@v1
       with:
-        name: aiida-pytests-py3.8
+        name: aiida-pytests-py3.9
         file: ./coverage.xml
         fail_ci_if_error: false  # don't fail job, if coverage upload fails
 
   verdi:
 
     runs-on: ubuntu-latest
     timeout-minutes: 15
 
     strategy:
       fail-fast: false
       matrix:
-        python-version: ['3.8', '3.11']
+        python-version: ['3.9', '3.11']
 
     steps:
     - uses: actions/checkout@v2
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
```

### Comparing `aiida_core-2.3.1/.github/workflows/ci-style.yml` & `aiida_core-2.4.0/.github/workflows/ci-style.yml`

 * *Files 18% similar despite different names*

```diff
@@ -12,28 +12,28 @@
 
     runs-on: ubuntu-latest
     timeout-minutes: 30
 
     steps:
     - uses: actions/checkout@v2
 
-    - name: Set up Python 3.8
+    - name: Set up Python 3.9
       uses: actions/setup-python@v2
       with:
-        python-version: '3.8'
+        python-version: '3.9'
 
     - name: Install system dependencies
       # note libkrb5-dev is required as a dependency for the gssapi pip install
       run: |
         sudo apt update
         sudo apt install libkrb5-dev ruby ruby-dev
 
     - name: Install python dependencies
       run: |
         pip install --upgrade pip
-        pip install -r requirements/requirements-py-3.8.txt
+        pip install -r requirements/requirements-py-3.9.txt
         pip install -e .[pre-commit]
         pip freeze
 
     - name: Run pre-commit
       run:
         pre-commit run --all-files || ( git status --short ; git diff ; exit 1 )
```

### Comparing `aiida_core-2.3.1/.github/workflows/docs-build.yml` & `aiida_core-2.4.0/.github/workflows/docs-build.yml`

 * *Files 11% similar despite different names*

```diff
@@ -12,18 +12,18 @@
   docs-linkcheck:
 
     runs-on: ubuntu-latest
     timeout-minutes: 30
 
     steps:
     - uses: actions/checkout@v2
-    - name: Set up Python 3.8
+    - name: Set up Python 3.9
       uses: actions/setup-python@v2
       with:
-        python-version: '3.8'
+        python-version: '3.9'
     - name: Install python dependencies
       run: |
         pip install --upgrade pip
         pip install -e .[docs,tests,rest,atomic_tools]
     - name: Build HTML docs
       id: linkcheck
       run: |
```

### Comparing `aiida_core-2.3.1/.github/workflows/nightly.yml` & `aiida_core-2.4.0/.github/workflows/nightly.yml`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/.github/workflows/post-release.yml` & `aiida_core-2.4.0/.github/workflows/post-release.yml`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/.github/workflows/push_image_to_dockerhub.yml` & `aiida_core-2.4.0/.github/workflows/push_image_to_dockerhub.yml`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/.github/workflows/rabbitmq.yml` & `aiida_core-2.4.0/.github/workflows/rabbitmq.yml`

 * *Files 15% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
         runs-on: ubuntu-latest
         timeout-minutes: 30
 
         strategy:
             fail-fast: false
             matrix:
-                rabbitmq: ['3.6', '3.7', '3.8']
+                rabbitmq-version: ['3.6', '3.7', '3.8']
 
         services:
             postgres:
                 image: postgres:10
                 env:
                     POSTGRES_DB: test_aiida
                     POSTGRES_PASSWORD: ''
@@ -30,36 +30,36 @@
                     --health-cmd pg_isready
                     --health-interval 10s
                     --health-timeout 5s
                     --health-retries 5
                 ports:
                 -   5432:5432
             rabbitmq:
-                image: rabbitmq:${{ matrix.rabbitmq }}-management
+                image: rabbitmq:${{ matrix.rabbitmq-version }}-management
                 ports:
                 -   5672:5672
                 -   15672:15672
 
         steps:
         -   uses: actions/checkout@v2
 
-        -   name: Set up Python 3.8
+        -   name: Set up Python 3.9
             uses: actions/setup-python@v2
             with:
-                python-version: '3.8'
+                python-version: '3.9'
 
         -   name: Install system dependencies
             run: sudo apt update && sudo apt install postgresql
 
         -   name: Upgrade pip
             run: |
                 pip install --upgrade pip
                 pip --version
 
         -   name: Install aiida-core
             run: |
-                pip install -r requirements/requirements-py-3.8.txt
+                pip install -r requirements/requirements-py-3.9.txt
                 pip install --no-deps -e .
                 pip freeze
 
         -   name: Run tests
             run: pytest -sv -k 'requires_rmq'
```

### Comparing `aiida_core-2.3.1/.github/workflows/release.yml` & `aiida_core-2.4.0/.github/workflows/release.yml`

 * *Files 4% similar despite different names*

```diff
@@ -15,41 +15,41 @@
 
     # Only run this job on the main repository and not on forks
     if: github.repository == 'aiidateam/aiida-core'
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v2
-    - name: Set up Python 3.8
+    - name: Set up Python 3.9
       uses: actions/setup-python@v2
       with:
-        python-version: '3.8'
+        python-version: '3.9'
     - run: python .github/workflows/check_release_tag.py $GITHUB_REF
 
   pre-commit:
 
     needs: [check-release-tag]
     runs-on: ubuntu-latest
     timeout-minutes: 30
 
     steps:
     - uses: actions/checkout@v2
-    - name: Set up Python 3.8
+    - name: Set up Python 3.9
       uses: actions/setup-python@v2
       with:
-        python-version: '3.8'
+        python-version: '3.9'
     - name: Install system dependencies
       # note libkrb5-dev is required as a dependency for the gssapi pip install
       run: |
         sudo apt update
         sudo apt install libkrb5-dev ruby ruby-dev
     - name: Install python dependencies
       run: |
         pip install --upgrade pip
-        pip install -r requirements/requirements-py-3.8.txt
+        pip install -r requirements/requirements-py-3.9.txt
         pip install -e .[pre-commit]
         pip freeze
     - name: Run pre-commit
       run: pre-commit run --all-files || ( git status --short ; git diff ; exit 1 )
 
   tests:
 
@@ -75,31 +75,31 @@
         image: rabbitmq:3.8.14-management
         ports:
           - 5672:5672
           - 15672:15672
 
     steps:
     - uses: actions/checkout@v2
-    - name: Set up Python 3.8
+    - name: Set up Python 3.9
       uses: actions/setup-python@v2
       with:
-        python-version: '3.8'
+        python-version: '3.9'
     - name: Install system dependencies
       run: |
         sudo apt update
         sudo apt install postgresql graphviz
 
     - name: Upgrade pip
       run: |
         pip install --upgrade pip
         pip --version
 
     - name: Install aiida-core
       run: |
-        pip install -r requirements/requirements-py-3.8.txt
+        pip install -r requirements/requirements-py-3.9.txt
         pip install --no-deps -e .
     - name: Run sub-set of test suite
       run: pytest -sv -k 'requires_rmq'
 
   publish:
 
     name: Publish to PyPI
@@ -107,18 +107,18 @@
     needs: [check-release-tag, pre-commit, tests]
 
     runs-on: ubuntu-latest
 
     steps:
     - name: Checkout source
       uses: actions/checkout@v2
-    - name: Set up Python 3.8
+    - name: Set up Python 3.9
       uses: actions/setup-python@v2
       with:
-        python-version: '3.8'
+        python-version: '3.9'
     - name: install flit
       run: |
         pip install flit~=3.4
     - name: Build and publish
       run: |
         flit publish
       env:
```

### Comparing `aiida_core-2.3.1/.github/workflows/setup.sh` & `aiida_core-2.4.0/.github/workflows/setup.sh`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/.github/workflows/test-install.yml` & `aiida_core-2.4.0/.github/workflows/test-install.yml`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     if: github.repository == 'aiidateam/aiida-core'
     runs-on: ubuntu-latest
     timeout-minutes: 5
 
     strategy:
       fail-fast: false
       matrix:
-        python-version: ['3.8', '3.9', '3.10', '3.11']
+        python-version: ['3.9', '3.10', '3.11']
 
     steps:
     - uses: actions/checkout@v2
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
@@ -106,20 +106,18 @@
       fail-fast: false
       matrix:
         extras: [ '', '[atomic_tools,docs,notebook,rest,tests]' ]
 
     steps:
     - uses: actions/checkout@v2
 
-      # Set to Python version 3.8, as the installation with 3.9 still takes
-      # significantly longer to install.
-    - name: Set up Python 3.8
+    - name: Set up Python 3.9
       uses: actions/setup-python@v2
       with:
-        python-version: '3.8'
+        python-version: '3.9'
 
     - name: Pip install
       id: pip_install
       run: |
         python -m pip --version
         python -m pip install -e .${{ matrix.extras }}
         python -m pip freeze
@@ -136,15 +134,15 @@
     runs-on: ubuntu-latest
     timeout-minutes: 25
 
     strategy:
       fail-fast: false
       matrix:
 
-        python-version: ['3.8', '3.9', '3.10', '3.11']
+        python-version: ['3.9', '3.10', '3.11']
 
         # Not being able to install with conda on a specific Python version is
         # not sufficient to fail the run, but something we want to be aware of.
         optional: [true]
 
         include:
           # Installing with conda without specyfing the Python version should
@@ -187,15 +185,15 @@
     needs: [install-with-pip]
     runs-on: ubuntu-latest
     timeout-minutes: 35
 
     strategy:
       fail-fast: false
       matrix:
-        python-version: ['3.8', '3.9', '3.10', '3.11']
+        python-version: ['3.9', '3.10', '3.11']
 
     services:
       postgres:
         image: postgres:10
         env:
           POSTGRES_DB: test_aiida
           POSTGRES_PASSWORD: ''
```

### Comparing `aiida_core-2.3.1/.github/workflows/tests.sh` & `aiida_core-2.4.0/.github/workflows/tests.sh`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/.github/workflows/tests_nightly.sh` & `aiida_core-2.4.0/.github/workflows/tests_nightly.sh`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/.github/workflows/verdi.sh` & `aiida_core-2.4.0/.github/workflows/verdi.sh`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/.molecule/README.md` & `aiida_core-2.4.0/.molecule/README.md`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/.molecule/default/config_local.yml` & `aiida_core-2.4.0/.molecule/default/config_local.yml`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/.molecule/default/create_docker.yml` & `aiida_core-2.4.0/.molecule/default/create_docker.yml`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/.molecule/default/files/polish/__init__.py` & `aiida_core-2.4.0/.molecule/default/files/polish/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/.molecule/default/files/polish/cli.py` & `aiida_core-2.4.0/.molecule/default/files/polish/cli.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/.molecule/default/files/polish/lib/__init__.py` & `aiida_core-2.4.0/.molecule/default/files/polish/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/.molecule/default/files/polish/lib/expression.py` & `aiida_core-2.4.0/.molecule/default/files/polish/lib/expression.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             return False, 'expression contains incongruent number of symbols'
 
         try:
             operand = int(operand)
         except ValueError:
             return False, f'the operand {operand} is not a valid integer'
 
-        if operator not in OPERATORS.keys():
+        if operator not in OPERATORS:
             return False, f'the operator {operator} is not supported'
 
         if OPERATORS[operator] is operators.pow and operand < 0:
             return False, f'a negative operand {operand} was found for the ^ operator, which is not allowed'
 
     # At this point the symbols list should only contain the initial operand
     try:
@@ -115,15 +115,15 @@
     :param expression: the expression in Reverse Polish Notation
     :return: the result of the evaluted expression
     """
     stack = collections.deque()
     result = 0
 
     for part in expression.split():
-        if part not in OPERATORS.keys():
+        if part not in OPERATORS:
             stack.appendleft(part)
         else:
             operator = OPERATORS[part]
 
             left_hand = int(stack.popleft())
             right_hand = int(stack.popleft())
             result = operator(left_hand, right_hand)
```

### Comparing `aiida_core-2.3.1/.molecule/default/files/polish/lib/template/base.tpl` & `aiida_core-2.4.0/.molecule/default/files/polish/lib/template/base.tpl`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/.molecule/default/files/polish/lib/template/workchain.tpl` & `aiida_core-2.4.0/.molecule/default/files/polish/lib/template/workchain.tpl`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/.molecule/default/files/polish/lib/workchain.py` & `aiida_core-2.4.0/.molecule/default/files/polish/lib/workchain.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     """
     stack = collections.deque()
     values = []
     outline = [['add']]
 
     for part in expression.split():
 
-        if part not in OPERATORS.keys():
+        if part not in OPERATORS:
             stack.appendleft(part)
             values.append(part)
         else:
             stack.popleft()
 
             sub_outline = outline[-1]
 
@@ -218,15 +218,15 @@
     code_strings.append('\n')
 
     counter = len(outlines) - 1
     for outline in outlines:
 
         outline_string = ''
         for subline in outline.split('\n'):
-            outline_string += f'\t\t\t{subline}\n'
+            outline_string += f'\t\t\t{subline}\n'  # pylint: disable=consider-using-join
 
         if counter == len(outlines) - 1:
             child_class = None
         else:
             child_class = f'Polish{counter + 1:02d}WorkChain'
 
         subs = {
```

### Comparing `aiida_core-2.3.1/.molecule/default/setup_aiida.yml` & `aiida_core-2.4.0/.molecule/default/setup_aiida.yml`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/.molecule/default/setup_python.yml` & `aiida_core-2.4.0/.molecule/default/setup_python.yml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
   tasks:
 
   - name: pip install aiida-core requirements
     pip:
       chdir: "{{ aiida_core_dir }}"
       # TODO dynamically change for python version
-      requirements: requirements/requirements-py-3.8.txt
+      requirements: requirements/requirements-py-3.9.txt
       executable: "{{ venv_bin }}/pip"
       extra_args: --cache-dir {{ aiida_pip_cache }}
     register: pip_install_deps
 
   - name: pip install aiida-core
     pip:
       chdir: "{{ aiida_core_dir }}"
```

### Comparing `aiida_core-2.3.1/.molecule/default/tasks/log_query_stats.yml` & `aiida_core-2.4.0/.molecule/default/tasks/log_query_stats.yml`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/.molecule/default/test_polish_workchains.yml` & `aiida_core-2.4.0/.molecule/default/test_polish_workchains.yml`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/.pre-commit-config.yaml` & `aiida_core-2.4.0/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -24,24 +24,24 @@
 
 -   repo: https://github.com/pycqa/isort
     rev: 5.12.0
     hooks:
     - id: isort
 
 -   repo: https://github.com/ikamensh/flynt/
-    rev: '0.77'
+    rev: '0.78'
     hooks:
     -   id: flynt
         args: [
             '--line-length=120',
             '--fail-on-change',
         ]
 
 -   repo: https://github.com/google/yapf
-    rev: v0.32.0
+    rev: v0.33.0
     hooks:
     -   id: yapf
         name: yapf
         types: [python]
         exclude: &exclude_files >
             (?x)^(
                 docs/.*|
```

### Comparing `aiida_core-2.3.1/.readthedocs.yml` & `aiida_core-2.4.0/.readthedocs.yml`

 * *Files 20% similar despite different names*

```diff
@@ -2,17 +2,23 @@
 
 # Important: we need to disable all unneeded formats.
 # Note that HTML and JSON are always built: https://docs.readthedocs.io/en/latest/yaml-config.html#formats
 # Especially, the 'htmlzip' format takes a LOT of memory and causes the build to fail - see our issue #1472:
 # https://github.com/aiidateam/aiida-core/issues/1472
 formats: []
 
+build:
+  apt_packages:
+    - graphviz
+  os: ubuntu-22.04
+  tools:
+    python: "3.10"
+
 # Need to install the package itself such that the entry points are installed and the API doc can build properly
 python:
-    version: 3.8
     install:
         - method: pip
           path: .
           extra_requirements:
             - docs
             - tests
             - rest
```

### Comparing `aiida_core-2.3.1/AUTHORS.txt` & `aiida_core-2.4.0/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/CHANGELOG.md` & `aiida_core-2.4.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,77 @@
 # Changelog
 
+## v2.4.0 - 2023-06-22
+
+This minor release comes with a number of new features and improvements as well as a significant amount of bug fixes.
+Support for Python 3.8 has been officially dropped in accordance with [AEP 003](https://github.com/aiidateam/AEP/blob/master/003_adopt_nep_29/readme.md).
+
+As a result of one of the bug fixes, related to the [caching of `CalcJob` nodes](https://github.com/aiidateam/aiida-core/commit/685e0f87d7c571df24aea8f0ce21c6c45dfbd8a0), a database migration had to be added, the first since the release of v2.0.
+After ugrading to v2.4.0, you will be prompted to migrate your database.
+The automated migration drops the hashes of existing `CalcJobNode`s and provides you with the optional command to recompute them.
+Execute the command if existing `CalcJobNode`s need to be usable as valid cache sources.
+
+### Features
+- Config: Add option to change recursion limit in daemon workers [[226159fd9]](https://github.com/aiidateam/aiida-core/commit/226159fd96c01782f4e1b4b52db945e3aef76285)
+- CLI: Added `compress` option to `verdi storage maintain` [[add474cbb]](https://github.com/aiidateam/aiida-core/commit/add474cbb0d67e278803e9340e521ea1046ef35c)
+- Expose `get_daemon_client` so it can be imported from `aiida.engine` [[1a0c1ee93]](https://github.com/aiidateam/aiida-core/commit/1a0c1ee932f24a6b191dc2e4d770973b8b32d66e)
+- `verdi computer test`: Improve messaging of login shell check [[062a58260]](https://github.com/aiidateam/aiida-core/commit/062a5826077907f43165084d4dc02db3f71bfb73)
+- `verdi node rehash`: Add `aiida.node` as group for `--entry-point` [[2fd07514d]](https://github.com/aiidateam/aiida-core/commit/2fd07514d9a76ceb5576dd23c02596794dea0666)
+- `verdi process status`: Add `call_link_label` to stack entries [[bd9372a5f]](https://github.com/aiidateam/aiida-core/commit/bd9372a5f4ce6681b16ef806338512c0fb02e25e)
+- `SinglefileData`: Add the `from_string` classmethod [[c25de615e]](https://github.com/aiidateam/aiida-core/commit/c25de615e4680b809f5d65d42031afdf95bd6923)
+- `DynamicEntryPointCommandGroup`: Add support for shared options [[220a65c76]](https://github.com/aiidateam/aiida-core/commit/220a65c76d9fcf3144ef77925caff8f5c653b2c9)
+- `DynamicEntryPointCommandGroup`: Pass ctx to `command` callable [[7de711be4]](https://github.com/aiidateam/aiida-core/commit/7de711be468f91e09baf6def3e319d85288e3be1)
+- `ProcessNode`: Add the `exit_code` property [[ad8a539ee]](https://github.com/aiidateam/aiida-core/commit/ad8a539ee2b481d526607b5924789fbbd1e14102)
+
+### Fixes
+- Engine: Dynamically update maximum stack size close to overflow to address `RecursionError` under heavy load [[f797b4766]](https://github.com/aiidateam/aiida-core/commit/f797b476622d9b2724d1460bbe55ef989166f57d)
+- `CalcJobNode`: Fix the computation of the hash [[685e0f87d]](https://github.com/aiidateam/aiida-core/commit/685e0f87d7c571df24aea8f0ce21c6c45dfbd8a0)
+- `CalcJob`: Ignore file in `remote_copy_list` not existing [[101a8d61b]](https://github.com/aiidateam/aiida-core/commit/101a8d61ba1c9f50a0231cd249c5a7f7ff1d77a4)
+- `CalcJob`: Assign outputs from node in case of cache hit [[777b97601]](https://github.com/aiidateam/aiida-core/commit/777b976013d0041e059f86c1ac0d2f43b52884df)
+- Fix log messages being logged twice to the daemon log file [[bfd63c790]](https://github.com/aiidateam/aiida-core/commit/bfd63c790a6bd5fdcb60a2d1b840c7b285c53334)
+- Process control: Change language when not waiting for response [[68cb4579d]](https://github.com/aiidateam/aiida-core/commit/68cb4579d9e77b32dc6182dc704e6079b6f9c0c2)
+- Do not assume `pgtest` cluster started in `postgres_cluster` fixture [[1de2ca576]](https://github.com/aiidateam/aiida-core/commit/1de2ca576c7fbe5c6586f53160304b46c99a3a10)
+- Process control: Warn instead of except when daemon is not running [[ad4fbcccb]](https://github.com/aiidateam/aiida-core/commit/ad4fbcccb14ac68653a941bf17be2e532ca162bc)
+- `DirectScheduler`: Add `?` as `JobState.UNDETERMINED` [[ffc869d8f]](https://github.com/aiidateam/aiida-core/commit/ffc869d8f91a860055b12f0d3803615895fa464f)
+- CLI: Correct `verdi devel rabbitmq tasks revive` docstring [[13cadd05f]](https://github.com/aiidateam/aiida-core/commit/13cadd05f2463b0fd240dde2f979801fbac122f9)
+- `SinglefileData`: Fix bug when `filename` is `pathlib.Path` [[f36bf583c]](https://github.com/aiidateam/aiida-core/commit/f36bf583c2bb4ac532d97f843141c907ee350f69)
+- Improve clarity of various deprecation warnings [[c72a252ed]](https://github.com/aiidateam/aiida-core/commit/c72a252ed563c7f0a7604d15632331c094973b5f)
+- `CalcJob`: Remove default of `withmpi` input and make it optional [[6a88cb315]](https://github.com/aiidateam/aiida-core/commit/6a88cb3158c0b84b601a289f50f51cfe6ae42687)
+- `Process`: Have `inputs` property always return `AttributesFrozenDict` [[60756fe30]](https://github.com/aiidateam/aiida-core/commit/60756fe30dfaff443ab434d92196249eea47f166)
+- `PsqlDos`: Add migration to remove hashes for all `CalcJobNodes` [[7ad916836]](https://github.com/aiidateam/aiida-core/commit/7ad91683643a5d9134c2a9532901e00b903996b4)
+- `PsqlDosMigrator`: Commit changes when migrating existing schema [[f84fe5b60]](https://github.com/aiidateam/aiida-core/commit/f84fe5b608d0656c82a38edbcbcb7bf48b399562)
+- `PsqlDos`: Add `entry_point_string` argument to `drop_hashes` [[c7a36fa3d]](https://github.com/aiidateam/aiida-core/commit/c7a36fa3d1fcd59e5ff31348c9f64619a7835b75)
+- `PsqlDos`: Make hash reset migrations more explicit [[c447a1af3]](https://github.com/aiidateam/aiida-core/commit/c447a1af39f99f2b53cffef36828d2523ab720a5)
+- `verdi process list`: Fix double percent sign in daemon usage [[68be866e6]](https://github.com/aiidateam/aiida-core/commit/68be866e653c610e9b957a3fdedc1b77e6e41a05)
+- Fix the `daemon_client` fixture [[9e5f5eefd]](https://github.com/aiidateam/aiida-core/commit/9e5f5eefd0cd6be44f0be76efae157dcf6e160ed)
+- Transports: Raise `FileNotFoundError` in `copy` if source doesn't exist [[d82069441]](https://github.com/aiidateam/aiida-core/commit/d82069441ce4bb002c8c9b5a419a9d8a8c4446b7)
+
+### Devops
+- Add `graphviz` to system requirements of RTD build runner [[3df02550e]](https://github.com/aiidateam/aiida-core/commit/3df02550eff02cd625d0e14eb35e6d6b01b4b12d)
+- Add types for `DefaultFieldsAttributeDict` subclasses [[afed5dc46]](https://github.com/aiidateam/aiida-core/commit/afed5dc4630b25b72b2c5a27d542222c086067a7)
+- Bump Python version for RTD build [[5df446cd3]](https://github.com/aiidateam/aiida-core/commit/5df446cd3558b1b7ee11d9b60d75287d6395a693)
+- Pre-commit: Fix `mypy` warning in `aiida.orm.utils.serialize` [[c25922484]](https://github.com/aiidateam/aiida-core/commit/c2592248482c087807d550c8304fa3703744cdf2)
+- Update Docker base image `aiida-prerequisites==0.7.0` [[ac755afae]](https://github.com/aiidateam/aiida-core/commit/ac755afaec836ffc9bc05e0617065eade5ef9ca7)
+- Use f-strings in `aiida/engine/daemon/execmanager.py` [[49cffff21]](https://github.com/aiidateam/aiida-core/commit/49cffff21e9fedac517e0e3659eaf1aacb61e448)
+
+### Dependencies
+- Drop support for Python 3.8 [[3defb8bb7]](https://github.com/aiidateam/aiida-core/commit/3defb8bb70fab87c5a4375e34dc07144077036fd)
+- Update requirement `pylint~=2.17.4` [[397634444]](https://github.com/aiidateam/aiida-core/commit/39763444499eac6fbe76e337fe7e7ca21d675a07)
+- Update requirement `flask~=2.2` [[a2a05a69f]](https://github.com/aiidateam/aiida-core/commit/a2a05a69fb2fa6aae9a96d49d543e72008d2888f)
+
+### Deprecations
+- `QueryBuilder`: Deprecate `debug` argument and use logger [[603ff37a0]](https://github.com/aiidateam/aiida-core/commit/603ff37a0b6ecd3f5309c8148054b2ac5d022833)
+
+### Documentation
+- Add missing `core.` prefix to all `verdi data` subcommands [[99319b3c1]](https://github.com/aiidateam/aiida-core/commit/99319b3c175b260ebc813cbec78208deefcdb562)
+- Clarify negation operator in `QueryBuilder` filters [[2c828811f]](https://github.com/aiidateam/aiida-core/commit/2c828811fbdf7e80358ae3cb223aca1dd67e9bb8)
+- Correct "variable" to "variadic" arguments [[978217693]](https://github.com/aiidateam/aiida-core/commit/978217693af987f015b51dc1c422a2e71bd39f4f)
+- Fix reference target warnings related to `flask_restful` [[4f76e0bd7]](https://github.com/aiidateam/aiida-core/commit/4f76e0bd75bdaf1bab1cae521c52c4a983708544)
+
+
 ## v2.3.1 - 2023-05-22
 
 ### Fixes
 - `DaemonClient`: Clean stale PID file in `stop_daemon` [[#6007]](https://github.com/aiidateam/aiida-core/pull/6007)
 
 
 ## v2.3.0 - 2023-04-17
@@ -28,16 +96,16 @@
 - [New contributors](#new-contributors)
 
 
 ### Process function improvements
 A number of improvements in the usage of process functions, i.e., `calcfunction` and `workfunction`, have been added.
 Each subsection title is a link to the documentation for more details.
 
-#### [Variable arguments](https://aiida.readthedocs.io/projects/aiida-core/en/latest/topics/processes/functions.html#variable-and-keyword-arguments)
-Variable arguments can be used in case the function should accept a list of inputs of unknown length.
+#### [Variadic arguments](https://aiida.readthedocs.io/projects/aiida-core/en/latest/topics/processes/functions.html#variadic-and-keyword-arguments)
+Variadic arguments can be used in case the function should accept a list of inputs of unknown length.
 Consider the example of a calculation function that computes the average of a number of `Int` nodes:
 ```python
 @calcfunction
 def average(*args):
     return sum(args) / len(args)
 
 result = average(*(1, 2, 3))
@@ -401,40 +469,40 @@
 - `BaseRestartWorkChain`: Fix bug in `_wrap_bare_dict_inputs` introduced in `v2.1.0` [[#5757]](https://github.com/aiidateam/aiida-core/pull/5757)
 
 
 ## v2.1.1 - 2022-11-10
 
 ### Fixes
 
-- Engine: Remove `*args` from the `Process.submit` method. [[#5753]](https://github.com/aiidateam/aiida-core/pull/5753)  
+- Engine: Remove `*args` from the `Process.submit` method. [[#5753]](https://github.com/aiidateam/aiida-core/pull/5753)
   Positional arguments were silently ignored leading to a misleading error message.
   For example, if a user called
   ```python
   inputs = {}
   self.submit(cls, inputs)
   ```
   instead of the intended
   ```python
   inputs = {}
   self.submit(cls, **inputs)
   ```
   The returned error message was that one of the required inputs was not defined.
   Now it will correctly raise a `TypeError` saying that positional arguments are not supported.
-- Process functions: Add serialization for Python base type defaults [[#5744]](https://github.com/aiidateam/aiida-core/pull/5744)  
+- Process functions: Add serialization for Python base type defaults [[#5744]](https://github.com/aiidateam/aiida-core/pull/5744)
   Defining Python base types as defaults, such as:
   ```python
   @calcfunction
   def function(a, b = 5):
       return a + b
   ```
   would raise an exception.
   The default is now automatically serialized, just as an input argument would be upon function call.
-- Process control: Reinstate process status for paused/killed processes [[#5754]](https://github.com/aiidateam/aiida-core/pull/5754)  
+- Process control: Reinstate process status for paused/killed processes [[#5754]](https://github.com/aiidateam/aiida-core/pull/5754)
   Regression introduced in `aiida-core==2.1.0` caused the message `Killed through 'verdi process list'` to no longer be set on the `process_status` of the node.
-- `QueryBuilder`: use a nested session in `iterall` and `iterdict` [[#5736]](https://github.com/aiidateam/aiida-core/pull/5736)  
+- `QueryBuilder`: use a nested session in `iterall` and `iterdict` [[#5736]](https://github.com/aiidateam/aiida-core/pull/5736)
   Modifying entities yielded by `QueryBuilder.iterall` and `QueryBuilder.iterdict` would raise an exception, for example:
   ```python
   for [node] in QueryBuilder().append(Node).iterall():
       node.base.extras.set('some', 'extra')
   ```
```

### Comparing `aiida_core-2.3.1/CODE_OF_CONDUCT.md` & `aiida_core-2.4.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/Dockerfile` & `aiida_core-2.4.0/Dockerfile`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-FROM aiidateam/aiida-prerequisites:0.6.0
+FROM aiidateam/aiida-prerequisites:0.7.0
 
 USER root
 
 ENV SETUP_DEFAULT_PROFILE true
 
 ENV PROFILE_NAME default
 ENV USER_EMAIL aiida@localhost
```

### Comparing `aiida_core-2.3.1/LICENSE.txt` & `aiida_core-2.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/README.md` & `aiida_core-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/__init__.py` & `aiida_core-2.4.0/aiida/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from aiida.manage.configuration import get_config_option, get_profile, load_profile, profile_context
 
 __copyright__ = (
     'Copyright (c), This file is part of the AiiDA platform. '
     'For further information please visit http://www.aiida.net/. All rights reserved.'
 )
 __license__ = 'MIT license, see LICENSE.txt file.'
-__version__ = '2.3.1'
+__version__ = '2.4.0'
 __authors__ = 'The AiiDA team.'
 __paper__ = (
     'S. P. Huber et al., "AiiDA 1.0, a scalable computational infrastructure for automated reproducible workflows and '
     'data provenance", Scientific Data 7, 300 (2020); https://doi.org/10.1038/s41597-020-00638-4'
 )
 __paper_short__ = 'S. P. Huber et al., Scientific Data 7, 300 (2020).'
```

### Comparing `aiida_core-2.3.1/aiida/__main__.py` & `aiida_core-2.4.0/aiida/__main__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/calculations/__init__.py` & `aiida_core-2.4.0/aiida/calculations/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/calculations/arithmetic/__init__.py` & `aiida_core-2.4.0/aiida/calculations/arithmetic/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/calculations/arithmetic/add.py` & `aiida_core-2.4.0/aiida/calculations/arithmetic/add.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/calculations/diff_tutorial/calculations.py` & `aiida_core-2.4.0/aiida/calculations/diff_tutorial/calculations.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/calculations/importers/arithmetic/add.py` & `aiida_core-2.4.0/aiida/calculations/importers/arithmetic/add.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/calculations/monitors/base.py` & `aiida_core-2.4.0/aiida/calculations/monitors/base.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/calculations/templatereplacer.py` & `aiida_core-2.4.0/aiida/calculations/templatereplacer.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/calculations/transfer.py` & `aiida_core-2.4.0/aiida/calculations/transfer.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/__init__.py` & `aiida_core-2.4.0/aiida/cmdline/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/commands/__init__.py` & `aiida_core-2.4.0/aiida/cmdline/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/commands/cmd_archive.py` & `aiida_core-2.4.0/aiida/cmdline/commands/cmd_archive.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,15 +185,15 @@
         'overwrite': force,
         'compression': compress,
         'batch_size': batch_size,
         'test_run': test_run
     }
 
     if AIIDA_LOGGER.level <= logging.REPORT:  # pylint: disable=no-member
-        set_progress_bar_tqdm(leave=(AIIDA_LOGGER.level <= logging.INFO))
+        set_progress_bar_tqdm(leave=AIIDA_LOGGER.level <= logging.INFO)
     else:
         set_progress_reporter(None)
 
     try:
         create_archive(entities, filename=output_file, archive_format=archive_format, **kwargs)
     except ArchiveExportError as exception:
         echo.echo_critical(f'failed to write the archive file. Exception: {exception}')
@@ -228,15 +228,15 @@
         force = True
     elif not output_file:
         echo.echo_critical(
             'no output file specified. Please add --in-place flag if you would like to migrate in place.'
         )
 
     if AIIDA_LOGGER.level <= logging.REPORT:  # pylint: disable=no-member
-        set_progress_bar_tqdm(leave=(AIIDA_LOGGER.level <= logging.INFO))
+        set_progress_bar_tqdm(leave=AIIDA_LOGGER.level <= logging.INFO)
     else:
         set_progress_reporter(None)
 
     archive_format = get_format()
 
     if version is None:
         version = archive_format.latest_version
@@ -340,15 +340,15 @@
 
     The archive can be specified by its relative or absolute file path, or its HTTP URL.
     """
     # pylint: disable=unused-argument
     from aiida.common.progress_reporter import set_progress_bar_tqdm, set_progress_reporter
 
     if AIIDA_LOGGER.level <= logging.REPORT:  # pylint: disable=no-member
-        set_progress_bar_tqdm(leave=(AIIDA_LOGGER.level <= logging.INFO))
+        set_progress_bar_tqdm(leave=AIIDA_LOGGER.level <= logging.INFO)
     else:
         set_progress_reporter(None)
 
     all_archives = _gather_imports(archives, webpages)
 
     # Preliminary sanity check
     if not all_archives:
```

### Comparing `aiida_core-2.3.1/aiida/cmdline/commands/cmd_calcjob.py` & `aiida_core-2.4.0/aiida/cmdline/commands/cmd_calcjob.py`

 * *Files 0% similar despite different names*

```diff
@@ -282,15 +282,15 @@
         only_not_cleaned=True,
     )
 
     if path_mapping is None:
         echo.echo_critical('no calcjobs found with the given criteria')
 
     if not force:
-        path_count = sum([len(paths) for computer, paths in path_mapping.items()])
+        path_count = sum(len(paths) for paths in path_mapping.values())
         warning = f'Are you sure you want to clean the work directory of {path_count} calcjobs?'
         click.confirm(warning, abort=True)
 
     user = orm.User.collection.get_default()
 
     for computer_uuid, paths in path_mapping.items():
```

### Comparing `aiida_core-2.3.1/aiida/cmdline/commands/cmd_code.py` & `aiida_core-2.4.0/aiida/cmdline/commands/cmd_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 
 @verdi.group('code')
 def verdi_code():
     """Setup and manage codes."""
 
 
-def create_code(cls, non_interactive, **kwargs):  # pylint: disable=unused-argument
+def create_code(ctx: click.Context, cls, non_interactive: bool, **kwargs):  # pylint: disable=unused-argument
     """Create a new `Code` instance."""
     try:
         instance = cls(**kwargs)
     except (TypeError, ValueError) as exception:
         echo.echo_critical(f'Failed to create instance `{cls}`: {exception}')
 
     try:
```

### Comparing `aiida_core-2.3.1/aiida/cmdline/commands/cmd_computer.py` & `aiida_core-2.4.0/aiida/cmdline/commands/cmd_computer.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # For further information on the license, see the LICENSE.txt file        #
 # For further information please visit http://www.aiida.net               #
 ###########################################################################
 # pylint: disable=invalid-name,too-many-statements,too-many-branches
 """`verdi computer` command."""
 from copy import deepcopy
 from functools import partial
+from math import isclose
 
 import click
 import tabulate
 
 from aiida.cmdline.commands.cmd_verdi import VerdiCommandGroup, verdi
 from aiida.cmdline.params import arguments, options
 from aiida.cmdline.params.options.commands import computer as options_computer
@@ -42,27 +43,27 @@
     return []
 
 
 def prompt_for_computer_configuration(computer):  # pylint: disable=unused-argument
     pass
 
 
-def _computer_test_get_jobs(transport, scheduler, authinfo):  # pylint: disable=unused-argument
+def _computer_test_get_jobs(transport, scheduler, authinfo, computer):  # pylint: disable=unused-argument
     """Internal test to check if it is possible to check the queue state.
 
     :param transport: an open transport
     :param scheduler: the corresponding scheduler class
     :param authinfo: the AuthInfo object (from which one can get computer and aiidauser)
     :return: tuple of boolean indicating success or failure and an optional string message
     """
     found_jobs = scheduler.get_jobs(as_dict=True)
     return True, f'{len(found_jobs)} jobs found in the queue'
 
 
-def _computer_test_no_unexpected_output(transport, scheduler, authinfo):  # pylint: disable=unused-argument
+def _computer_test_no_unexpected_output(transport, scheduler, authinfo, computer):  # pylint: disable=unused-argument
     """Test that there is no unexpected output from the connection.
 
     This can happen if e.g. there is some spurious command in the
     .bashrc or .bash_profile that is not guarded in case of non-interactive
     shells.
 
     :param transport: an open transport
@@ -89,27 +90,27 @@
 
     if stderr:
         return False, template.format('stderr', stderr)
 
     return True, None
 
 
-def _computer_get_remote_username(transport, scheduler, authinfo):  # pylint: disable=unused-argument
+def _computer_get_remote_username(transport, scheduler, authinfo, computer):  # pylint: disable=unused-argument
     """Internal test to check if it is possible to determine the username on the remote.
 
     :param transport: an open transport
     :param scheduler: the corresponding scheduler class
     :param authinfo: the AuthInfo object
     :return: tuple of boolean indicating success or failure and an optional string message
     """
     remote_user = transport.whoami()
     return True, remote_user
 
 
-def _computer_create_temp_file(transport, scheduler, authinfo):  # pylint: disable=unused-argument
+def _computer_create_temp_file(transport, scheduler, authinfo, computer):  # pylint: disable=unused-argument
     """
     Internal test to check if it is possible to create a temporary file
     and then delete it in the work directory
 
     :note: exceptions could be raised
 
     :param transport: an open transport
@@ -183,25 +184,26 @@
         with authinfo.get_transport() as transport:
             transport.whoami()
         timings.append(time.time() - time_start)
 
     return sum(timings) / iterations
 
 
-def _computer_use_login_shell_performance(transport, scheduler, authinfo):  # pylint: disable=unused-argument
+def _computer_use_login_shell_performance(transport, scheduler, authinfo, computer):  # pylint: disable=unused-argument
     """Execute a command over the transport with and without the ``use_login_shell`` option enabled.
 
     By default, AiiDA uses a login shell when connecting to a computer in order to operate in the same environment as a
     user connecting to the computer. However, loading the login scripts of the shell can take time, which can
     significantly slow down all commands executed by AiiDA and impact the throughput of calculation jobs. This test
     executes a simple command both with and without using a login shell and emits a warning if the login shell is slower
     by at least 100 ms. If the computer is already configured to avoid using a login shell, the test is skipped and the
     function returns a successful test result.
     """
-    tolerance = 0.1  # 100 ms
+    rel_tol = 0.5  # Factor of two
+    abs_tol = 0.1  # 100 ms
     iterations = 3
 
     auth_params = authinfo.get_auth_params()
 
     # If ``use_login_shell=False`` we don't need to test for it being slower.
     if not auth_params.get('use_login_shell', True):
         return True, None
@@ -212,21 +214,24 @@
         timing_false = time_use_login_shell(authinfo, auth_params_clone, False, iterations)
         timing_true = time_use_login_shell(authinfo, auth_params_clone, True, iterations)
     finally:
         authinfo.set_auth_params(auth_params)
 
     echo.echo_debug(f'Execution time: {timing_true} vs {timing_false} for login shell and normal, respectively')
 
-    if timing_true - timing_false > tolerance:
-        message = (
-            'computer is configured to use a login shell, which is slower compared to a normal shell (Command execution'
-            f' time of {timing_true} s versus {timing_false}, respectively).\nUnless this setting is really necessary, '
-            'consider disabling it with: verdi computer configure core.local COMPUTER_NAME -n --no-use-login-shell'
+    if not isclose(timing_true, timing_false, rel_tol=rel_tol, abs_tol=abs_tol):
+        return True, (
+            f"\n\n{click.style('Warning:', fg='yellow', bold=True)} "
+            'The computer is configured to use a login shell, which is slower compared to a normal shell.\n'
+            f'Command execution time of {timing_true:.3f} versus {timing_false:.3f} seconds, respectively).\n'
+            'Unless this setting is really necessary, consider disabling it with:\n'
+            f'\n    verdi computer configure {computer.transport_type} {computer.label} -n --no-use-login-shell\n\n'
+            'For details, please refer to the documentation: '
+            'https://aiida.readthedocs.io/projects/aiida-core/en/latest/topics/transport.html#login-shells\n'
         )
-        return False, message
 
     return True, None
 
 
 def get_parameter_default(parameter, ctx):
     """
     Get the value for a specific parameter from the computer_builder or the default value of that option
@@ -547,15 +552,17 @@
             scheduler.set_transport(transport)
 
             for test, test_label in tests.items():
 
                 echo.echo(f'* {test_label}... ', nl=False)
                 num_tests += 1
                 try:
-                    success, message = test(transport=transport, scheduler=scheduler, authinfo=authinfo)
+                    success, message = test(
+                        transport=transport, scheduler=scheduler, authinfo=authinfo, computer=computer
+                    )
                 except Exception as exception:  # pylint:disable=broad-except
                     success = False
                     message = f'{exception.__class__.__name__}: {str(exception)}'
 
                     if print_traceback:
                         message += '\n  Full traceback:\n'
                         message += '\n'.join([f'  {l}' for l in traceback.format_exc().splitlines()])
```

### Comparing `aiida_core-2.3.1/aiida/cmdline/commands/cmd_config.py` & `aiida_core-2.4.0/aiida/cmdline/commands/cmd_config.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/commands/cmd_daemon.py` & `aiida_core-2.4.0/aiida/cmdline/commands/cmd_daemon.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/commands/cmd_data/__init__.py` & `aiida_core-2.4.0/aiida/cmdline/commands/cmd_data/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/commands/cmd_data/cmd_array.py` & `aiida_core-2.4.0/aiida/cmdline/commands/cmd_data/cmd_array.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright (c), The AiiDA team. All rights reserved.                     #
 # This file is part of the AiiDA code.                                    #
 #                                                                         #
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-core #
 # For further information on the license, see the LICENSE.txt file        #
 # For further information please visit http://www.aiida.net               #
 ###########################################################################
-"""`verdi data array` command."""
+"""`verdi data core.array` command."""
 
 from aiida.cmdline.commands.cmd_data import verdi_data
 from aiida.cmdline.params import arguments, options, types
 
 
 @verdi_data.group('core.array')
 def array():
```

### Comparing `aiida_core-2.3.1/aiida/cmdline/commands/cmd_data/cmd_bands.py` & `aiida_core-2.4.0/aiida/cmdline/commands/cmd_data/cmd_bands.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright (c), The AiiDA team. All rights reserved.                     #
 # This file is part of the AiiDA code.                                    #
 #                                                                         #
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-core #
 # For further information on the license, see the LICENSE.txt file        #
 # For further information please visit http://www.aiida.net               #
 ###########################################################################
-"""`verdi data bands` command."""
+"""`verdi data core.bands` command."""
 
 import click
 
 from aiida.cmdline.commands.cmd_data import cmd_show, verdi_data
 from aiida.cmdline.commands.cmd_data.cmd_export import data_export
 from aiida.cmdline.commands.cmd_data.cmd_list import list_options
 from aiida.cmdline.params import arguments, options, types
```

### Comparing `aiida_core-2.3.1/aiida/cmdline/commands/cmd_data/cmd_cif.py` & `aiida_core-2.4.0/aiida/cmdline/commands/cmd_data/cmd_cif.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright (c), The AiiDA team. All rights reserved.                     #
 # This file is part of the AiiDA code.                                    #
 #                                                                         #
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-core #
 # For further information on the license, see the LICENSE.txt file        #
 # For further information please visit http://www.aiida.net               #
 ###########################################################################
-"""`verdi data cif` command."""
+"""`verdi data core.cif` command."""
 
 import click
 
 from aiida.cmdline.commands.cmd_data import cmd_show, verdi_data
 from aiida.cmdline.commands.cmd_data.cmd_export import data_export, export_options
 from aiida.cmdline.commands.cmd_data.cmd_list import data_list, list_options
 from aiida.cmdline.params import arguments, options, types
```

### Comparing `aiida_core-2.3.1/aiida/cmdline/commands/cmd_data/cmd_dict.py` & `aiida_core-2.4.0/aiida/cmdline/commands/cmd_data/cmd_dict.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright (c), The AiiDA team. All rights reserved.                     #
 # This file is part of the AiiDA code.                                    #
 #                                                                         #
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-core #
 # For further information on the license, see the LICENSE.txt file        #
 # For further information please visit http://www.aiida.net               #
 ###########################################################################
-"""`verdi data dict` command."""
+"""`verdi data core.dict` command."""
 
 from aiida.cmdline.commands.cmd_data import verdi_data
 from aiida.cmdline.params import arguments, options, types
 
 
 @verdi_data.group('core.dict')
 def dictionary():
```

### Comparing `aiida_core-2.3.1/aiida/cmdline/commands/cmd_data/cmd_export.py` & `aiida_core-2.4.0/aiida/cmdline/commands/cmd_data/cmd_export.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/commands/cmd_data/cmd_list.py` & `aiida_core-2.4.0/aiida/cmdline/commands/cmd_data/cmd_list.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/commands/cmd_data/cmd_remote.py` & `aiida_core-2.4.0/aiida/cmdline/commands/cmd_data/cmd_remote.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright (c), The AiiDA team. All rights reserved.                     #
 # This file is part of the AiiDA code.                                    #
 #                                                                         #
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-core #
 # For further information on the license, see the LICENSE.txt file        #
 # For further information please visit http://www.aiida.net               #
 ###########################################################################
-"""`verdi data remote` command."""
+"""`verdi data core.remote` command."""
 import stat
 
 import click
 
 from aiida.cmdline.commands.cmd_data import verdi_data
 from aiida.cmdline.params import arguments, types
 from aiida.cmdline.utils import echo
```

### Comparing `aiida_core-2.3.1/aiida/cmdline/commands/cmd_data/cmd_show.py` & `aiida_core-2.4.0/aiida/cmdline/commands/cmd_data/cmd_show.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/commands/cmd_data/cmd_singlefile.py` & `aiida_core-2.4.0/aiida/cmdline/commands/cmd_data/cmd_singlefile.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/commands/cmd_data/cmd_structure.py` & `aiida_core-2.4.0/aiida/cmdline/commands/cmd_data/cmd_structure.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright (c), The AiiDA team. All rights reserved.                     #
 # This file is part of the AiiDA code.                                    #
 #                                                                         #
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-core #
 # For further information on the license, see the LICENSE.txt file        #
 # For further information please visit http://www.aiida.net               #
 ###########################################################################
-"""`verdi data structure` command."""
+"""`verdi data core.structure` command."""
 
 import click
 
 from aiida.cmdline.commands.cmd_data import cmd_show, verdi_data
 from aiida.cmdline.commands.cmd_data.cmd_export import data_export, export_options
 from aiida.cmdline.commands.cmd_data.cmd_list import data_list, list_options
 from aiida.cmdline.params import arguments, options, types
```

### Comparing `aiida_core-2.3.1/aiida/cmdline/commands/cmd_data/cmd_trajectory.py` & `aiida_core-2.4.0/aiida/cmdline/commands/cmd_data/cmd_trajectory.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright (c), The AiiDA team. All rights reserved.                     #
 # This file is part of the AiiDA code.                                    #
 #                                                                         #
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-core #
 # For further information on the license, see the LICENSE.txt file        #
 # For further information please visit http://www.aiida.net               #
 ###########################################################################
-"""`verdi data trajectory` command."""
+"""`verdi data core.trajectory` command."""
 
 import click
 
 from aiida.cmdline.commands.cmd_data import cmd_show, verdi_data
 from aiida.cmdline.commands.cmd_data.cmd_export import data_export, export_options
 from aiida.cmdline.commands.cmd_data.cmd_list import data_list, list_options
 from aiida.cmdline.commands.cmd_data.cmd_show import show_options
```

### Comparing `aiida_core-2.3.1/aiida/cmdline/commands/cmd_data/cmd_upf.py` & `aiida_core-2.4.0/aiida/cmdline/commands/cmd_data/cmd_upf.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright (c), The AiiDA team. All rights reserved.                     #
 # This file is part of the AiiDA code.                                    #
 #                                                                         #
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-core #
 # For further information on the license, see the LICENSE.txt file        #
 # For further information please visit http://www.aiida.net               #
 ###########################################################################
-"""`verdi data upf` command."""
+"""`verdi data core.upf` command."""
 
 import os
 
 import click
 
 from aiida.cmdline.commands.cmd_data import verdi_data
 from aiida.cmdline.commands.cmd_data.cmd_export import data_export, export_options
```

### Comparing `aiida_core-2.3.1/aiida/cmdline/commands/cmd_database.py` & `aiida_core-2.4.0/aiida/cmdline/commands/cmd_database.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/commands/cmd_devel.py` & `aiida_core-2.4.0/aiida/cmdline/commands/cmd_devel.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/commands/cmd_group.py` & `aiida_core-2.4.0/aiida/cmdline/commands/cmd_group.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/commands/cmd_help.py` & `aiida_core-2.4.0/aiida/cmdline/commands/cmd_help.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,11 +26,11 @@
     if command:
         cmd = verdi.get_command(ctx.parent, command)
 
         if not cmd:
             # we should never end up here since verdi.get_command(...) gives
             # suggestions if the command could not be found and calls click.fail
             echo.echo_critical(f"command '{command}' not found")
-
-        cmdctx = click.Context(cmd, info_name=cmd.name, parent=ctx.parent)
+        else:
+            cmdctx = click.Context(cmd, info_name=cmd.name, parent=ctx.parent)
 
     echo.echo(cmdctx.get_help())
```

### Comparing `aiida_core-2.3.1/aiida/cmdline/commands/cmd_node.py` & `aiida_core-2.4.0/aiida/cmdline/commands/cmd_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -325,51 +325,54 @@
 
 
 @verdi_node.command('rehash')
 @arguments.NODES()
 @click.option(
     '-e',
     '--entry-point',
-    type=PluginParamType(group=('aiida.calculations', 'aiida.data', 'aiida.workflows'), load=True),
+    type=PluginParamType(group=('aiida.calculations', 'aiida.data', 'aiida.node', 'aiida.workflows'), load=True),
     default=None,
     help='Only include nodes that are class or sub class of the class identified by this entry point.'
 )
 @options.FORCE()
 @with_dbenv()
 def rehash(nodes, entry_point, force):
     """Recompute the hash for nodes in the database.
 
     The set of nodes that will be rehashed can be filtered by their identifier and/or based on their class.
     """
     from aiida.orm import Data, ProcessNode, QueryBuilder
 
+    # If no explicit entry point is defined, rehash all nodes, which are either Data nodes or ProcessNodes
+    if entry_point is None:
+        classes = (Data, ProcessNode)
+    else:
+        classes = (entry_point,)
+
     if not force:
-        echo.echo_warning('This command will recompute and overwrite the hashes of all nodes.')
+        class_names = ', '.join([cls.__name__ for cls in classes])
+        echo.echo_warning(f'This command will recompute and overwrite the hashes of all {class_names} nodes.')
         echo.echo_warning('Note that this can take a lot of time for big databases.')
         echo.echo_warning('')
         echo.echo_warning('', nl=False)
 
         confirm_message = 'Do you want to continue?'
 
         try:
             click.confirm(text=confirm_message, abort=True)
         except click.Abort:
             echo.echo('\n')
             echo.echo_critical('Migration aborted, the data has not been affected.')
 
-    # If no explicit entry point is defined, rehash all nodes, which are either Data nodes or ProcessNodes
-    if entry_point is None:
-        entry_point = (Data, ProcessNode)
-
     if nodes:
-        to_hash = [(node,) for node in nodes if isinstance(node, entry_point)]
+        to_hash = [(node,) for node in nodes if isinstance(node, classes)]
         num_nodes = len(to_hash)
     else:
         builder = QueryBuilder()
-        builder.append(entry_point, tag='node')
+        builder.append(classes, tag='node')
         to_hash = builder.all()
         num_nodes = builder.count()
 
     if not to_hash:
         echo.echo_critical('no matching nodes found')
 
     with click.progressbar(to_hash, label='Rehashing Nodes:') as iter_hash:
```

### Comparing `aiida_core-2.3.1/aiida/cmdline/commands/cmd_plugin.py` & `aiida_core-2.4.0/aiida/cmdline/commands/cmd_plugin.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/commands/cmd_process.py` & `aiida_core-2.4.0/aiida/cmdline/commands/cmd_process.py`

 * *Files 6% similar despite different names*

```diff
@@ -122,18 +122,18 @@
                     'in': ('created', 'waiting', 'running')
                 }
             }
         ).count()
         available_slots = active_workers * slots_per_worker
         percent_load = active_processes / available_slots
         if percent_load > 0.9:  # 90%
-            echo.echo_warning(f'{percent_load * 100:.0f}%% of the available daemon worker slots have been used!')
+            echo.echo_warning(f'{percent_load * 100:.0f}% of the available daemon worker slots have been used!')
             echo.echo_warning('Increase the number of workers with `verdi daemon incr`.')
         else:
-            echo.echo_report(f'Using {percent_load * 100:.0f}%% of the available daemon worker slots.')
+            echo.echo_report(f'Using {percent_load * 100:.0f}% of the available daemon worker slots.')
 
 
 @verdi_process.command('show')
 @arguments.PROCESSES()
 @decorators.with_dbenv()
 def process_show(processes):
     """Show details for one or multiple processes."""
@@ -194,33 +194,33 @@
         elif isinstance(process, (CalcFunctionNode, WorkFunctionNode)):
             echo.echo(get_process_function_report(process))
         else:
             echo.echo(f'Nothing to show for node type {process.__class__}')
 
 
 @verdi_process.command('status')
+@click.option('-c', '--call-link-label', 'call_link_label', is_flag=True, help='Include the call link label if set.')
 @click.option(
     '-m', '--max-depth', 'max_depth', type=int, default=None, help='Limit the number of levels to be printed.'
 )
 @arguments.PROCESSES()
-def process_status(max_depth, processes):
+def process_status(call_link_label, max_depth, processes):
     """Print the status of one or multiple processes."""
     from aiida.cmdline.utils.ascii_vis import format_call_graph
 
     for process in processes:
-        graph = format_call_graph(process, max_depth=max_depth)
+        graph = format_call_graph(process, max_depth=max_depth, call_link_label=call_link_label)
         echo.echo(graph)
 
 
 @verdi_process.command('kill')
 @arguments.PROCESSES()
 @options.TIMEOUT()
 @options.WAIT()
 @decorators.with_dbenv()
-@decorators.only_if_daemon_running(echo.echo_warning, 'daemon is not running, so process may not be reachable')
 def process_kill(processes, timeout, wait):
     """Kill running processes."""
     from aiida.engine.processes import control
 
     try:
         message = 'Killed through `verdi process kill`'
         control.kill_processes(processes, timeout=timeout, wait=wait, message=message)
@@ -230,15 +230,14 @@
 
 @verdi_process.command('pause')
 @arguments.PROCESSES()
 @options.ALL(help='Pause all active processes if no specific processes are specified.')
 @options.TIMEOUT()
 @options.WAIT()
 @decorators.with_dbenv()
-@decorators.only_if_daemon_running(echo.echo_warning, 'daemon is not running, so process may not be reachable')
 def process_pause(processes, all_entries, timeout, wait):
     """Pause running processes."""
     from aiida.engine.processes import control
 
     if processes and all_entries:
         raise click.BadOptionUsage('all', 'cannot specify individual processes and the `--all` flag at the same time.')
 
@@ -251,15 +250,14 @@
 
 @verdi_process.command('play')
 @arguments.PROCESSES()
 @options.ALL(help='Play all paused processes if no specific processes are specified.')
 @options.TIMEOUT()
 @options.WAIT()
 @decorators.with_dbenv()
-@decorators.only_if_daemon_running(echo.echo_warning, 'daemon is not running, so process may not be reachable')
 def process_play(processes, all_entries, timeout, wait):
     """Play (unpause) paused processes."""
     from aiida.engine.processes import control
 
     if processes and all_entries:
         raise click.BadOptionUsage('all', 'cannot specify individual processes and the `--all` flag at the same time.')
```

### Comparing `aiida_core-2.3.1/aiida/cmdline/commands/cmd_profile.py` & `aiida_core-2.4.0/aiida/cmdline/commands/cmd_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,16 @@
         echo.echo_critical(str(exception))
     else:
         echo.echo_report(f'configuration folder: {config.dirpath}')
 
     if not config.profiles:
         echo.echo_warning('no profiles configured: run `verdi setup` to create one')
     else:
-        sort = lambda profile: profile.name
-        highlight = lambda profile: profile.name == config.default_profile_name
+        sort = lambda profile: profile.name  # pylint: disable=unnecessary-lambda-assignment
+        highlight = lambda profile: profile.name == config.default_profile_name  # pylint: disable=unnecessary-lambda-assignment
         echo.echo_formatted_list(config.profiles, ['name'], sort=sort, highlight=highlight)
 
 
 def _strip_private_keys(dct: dict):
     """Remove private keys (starting `_`) from the dictionary."""
     return {
         key: _strip_private_keys(value) if isinstance(value, dict) else value
```

### Comparing `aiida_core-2.3.1/aiida/cmdline/commands/cmd_rabbitmq.py` & `aiida_core-2.4.0/aiida/cmdline/commands/cmd_rabbitmq.py`

 * *Files 2% similar despite different names*

```diff
@@ -368,19 +368,20 @@
 
     Warning: Use only as a last resort after you've gone through the checklist below.
 
     \b
         1. Does ``verdi status`` indicate that both daemon and RabbitMQ are running properly?
            If not, restart the daemon with ``verdi daemon restart --reset`` and restart RabbitMQ.
         2. Try ``verdi process play <PID>``.
-           If you receive a message that the process is no longer reachable, use ``verdi devel revive <PID>``.
+           If you receive a message that the process is no longer reachable,
+           use ``verdi devel rabbitmq tasks revive <PID>``.
 
     Details: When RabbitMQ loses the process task before the process has completed, the process is never picked up by
-    the daemon and will remain "stuck". ``verdi devel revive`` recreates the task, which can lead to multiple instances
-    of the task being executed and should thus be used with caution.
+    the daemon and will remain "stuck". ``verdi devel rabbitmq tasks revive`` recreates the task, which can lead to
+    multiple instances of the task being executed and should thus be used with caution.
     """
     from aiida.engine.processes.control import revive_processes
 
     if not force:
         echo.echo_warning('This command should only be used if you are absolutely sure the process task was lost.')
         click.confirm(text='Do you want to continue?', abort=True)
```

### Comparing `aiida_core-2.3.1/aiida/cmdline/commands/cmd_restapi.py` & `aiida_core-2.4.0/aiida/cmdline/commands/cmd_restapi.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/commands/cmd_run.py` & `aiida_core-2.4.0/aiida/cmdline/commands/cmd_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,27 +18,27 @@
 from aiida.cmdline.params.options.multivalue import MultipleValueOption
 from aiida.cmdline.utils import decorators
 
 
 @contextlib.contextmanager
 def update_environment(argv):
     """Context manager that temporarily replaces `sys.argv` with `argv` and adds current working dir to the path."""
-    try:
-        # Store a copy of the current path and argv as a backup variable so it can be restored later
-        _path = sys.path[:]
-        _argv = sys.argv[:]
+    # Store a copy of the current path and argv as a backup variable so it can be restored later
+    _path = sys.path[:]
+    _argv = sys.argv[:]
 
+    try:
         # Add the current working directory to the path, such that local modules can be imported
         sys.path.append(str(pathlib.Path.cwd().resolve()))
         sys.argv = argv[:]
         yield
     finally:
         # Restore old parameters when exiting from the context manager
-        sys.argv = _argv
-        sys.path = _path
+        sys.argv = _argv  # pylint
+        sys.path = _path  # pylint
 
 
 def validate_entry_point_strings(_, __, value):
     """Validate that `value` is a valid entrypoint string."""
     from aiida.orm import autogroup
 
     try:
```

### Comparing `aiida_core-2.3.1/aiida/cmdline/commands/cmd_setup.py` & `aiida_core-2.4.0/aiida/cmdline/commands/cmd_setup.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/commands/cmd_shell.py` & `aiida_core-2.4.0/aiida/cmdline/commands/cmd_shell.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/commands/cmd_status.py` & `aiida_core-2.4.0/aiida/cmdline/commands/cmd_status.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/commands/cmd_storage.py` & `aiida_core-2.4.0/aiida/cmdline/commands/cmd_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,17 +115,20 @@
 @options.FORCE()
 @click.option(
     '--dry-run',
     is_flag=True,
     help=
     'Run the maintenance in dry-run mode which will print actions that would be taken without actually executing them.'
 )
+@click.option(
+    '--compress', is_flag=True, default=False, help='Use compression if possible when carrying out maintenance tasks.'
+)
 @decorators.with_dbenv()
 @click.pass_context
-def storage_maintain(ctx, full, no_repack, force, dry_run):
+def storage_maintain(ctx, full, no_repack, force, dry_run, compress):
     """Performs maintenance tasks on the repository."""
     from aiida.common.exceptions import LockingProfileError
     from aiida.manage.manager import get_manager
 
     manager = get_manager()
     profile = ctx.obj.profile
     storage = manager.get_profile_storage()
@@ -153,13 +156,13 @@
         )
 
     if not dry_run and not force and not click.confirm('Are you sure you want continue in this mode?'):
         return
 
     try:
         if full and no_repack:
-            storage.maintain(full=full, dry_run=dry_run, do_repack=False)
+            storage.maintain(full=full, dry_run=dry_run, do_repack=False, compress=compress)
         else:
-            storage.maintain(full=full, dry_run=dry_run)
+            storage.maintain(full=full, dry_run=dry_run, compress=compress)
     except LockingProfileError as exception:
         echo.echo_critical(str(exception))
     echo.echo_success('Requested maintenance procedures finished.')
```

### Comparing `aiida_core-2.3.1/aiida/cmdline/commands/cmd_user.py` & `aiida_core-2.4.0/aiida/cmdline/commands/cmd_user.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/commands/cmd_verdi.py` & `aiida_core-2.4.0/aiida/cmdline/commands/cmd_verdi.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,13 +13,13 @@
 from aiida import __version__
 
 from ..groups import VerdiCommandGroup
 from ..params import options, types
 
 
 # Pass the version explicitly to ``version_option`` otherwise editable installs can show the wrong version number
-@click.command(cls=VerdiCommandGroup, context_settings={'help_option_names': ['--help', '-h']})
+@click.group(cls=VerdiCommandGroup, context_settings={'help_option_names': ['--help', '-h']})
 @options.PROFILE(type=types.ProfileParamType(load_profile=True), expose_value=False)
 @options.VERBOSITY()
 @click.version_option(__version__, package_name='aiida_core', message='AiiDA version %(version)s')
 def verdi():
     """The command line interface of AiiDA."""
```

### Comparing `aiida_core-2.3.1/aiida/cmdline/groups/dynamic.py` & `aiida_core-2.4.0/aiida/cmdline/groups/dynamic.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,20 +37,28 @@
 
         @click.group('create', cls=DynamicEntryPointCommandGroup, command=create_instance,)
         def cmd_create():
             pass
 
     """
 
-    def __init__(self, command, entry_point_group: str, entry_point_name_filter=r'.*', **kwargs):
+    def __init__(
+        self,
+        command,
+        entry_point_group: str,
+        entry_point_name_filter: str = r'.*',
+        shared_options: list[click.Option] | None = None,
+        **kwargs
+    ):
         super().__init__(**kwargs)
         self.command = command
         self.entry_point_group = entry_point_group
         self.entry_point_name_filter = entry_point_name_filter
         self.factory = ENTRY_POINT_GROUP_FACTORY_MAPPING[entry_point_group]
+        self.shared_options = shared_options
 
     def list_commands(self, ctx) -> list[str]:
         """Return the sorted list of subcommands for this group.
 
         :param ctx: The :class:`click.Context`.
         """
         commands = super().list_commands(ctx)
@@ -64,23 +72,23 @@
         """Return the command with the given name.
 
         :param ctx: The :class:`click.Context`.
         :param cmd_name: The name of the command.
         :returns: The :class:`click.Command`.
         """
         try:
-            command = self.create_command(cmd_name)
+            command = self.create_command(ctx, cmd_name)
         except exceptions.EntryPointError:
             command = super().get_command(ctx, cmd_name)
         return command
 
-    def create_command(self, entry_point):
+    def create_command(self, ctx, entry_point):
         """Create a subcommand for the given ``entry_point``."""
         cls = self.factory(entry_point)
-        command = functools.partial(self.command, cls)
+        command = functools.partial(self.command, ctx, cls)
         command.__doc__ = cls.__doc__
         return click.command(entry_point)(self.create_options(entry_point)(command))
 
     def create_options(self, entry_point):
         """Create the option decorators for the command function for the given entry point.
 
         :param entry_point: The entry point.
@@ -93,14 +101,20 @@
 
             options_list = self.list_options(entry_point)
             options_list.reverse()
 
             for option in options_list:
                 func = option(func)
 
+            shared_options = self.shared_options or []
+            shared_options.reverse()
+
+            for option in shared_options:
+                func = option(func)
+
             return func
 
         return apply_options
 
     def list_options(self, entry_point):
         """Return the list of options that should be applied to the command for the given entry point.
```

### Comparing `aiida_core-2.3.1/aiida/cmdline/groups/verdi.py` & `aiida_core-2.4.0/aiida/cmdline/groups/verdi.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # -*- coding: utf-8 -*-
 """Subclass of :class:`click.Group` for the ``verdi`` CLI."""
+from __future__ import annotations
+
 import base64
 import difflib
 import gzip
 
 import click
 
 from aiida.common.exceptions import ConfigurationError
@@ -53,23 +55,23 @@
     The class automatically adds the verbosity option to all commands in the interface. It also adds some functionality
     to provide suggestions of commands in case the user provided command name does not exist.
     """
 
     context_class = VerdiContext
 
     @staticmethod
-    def add_verbosity_option(cmd):
+    def add_verbosity_option(cmd: click.Command):
         """Apply the ``verbosity`` option to the command, which is common to all ``verdi`` commands."""
         # Only apply the option if it hasn't been already added in a previous call.
         if cmd is not None and 'verbosity' not in [param.name for param in cmd.params]:
             cmd = options.VERBOSITY()(cmd)
 
         return cmd
 
-    def fail_with_suggestions(self, ctx, cmd_name):
+    def fail_with_suggestions(self, ctx: click.Context, cmd_name: str):
         """Fail the command while trying to suggest commands to resemble the requested ``cmd_name``."""
         # We might get better results with the Levenshtein distance or more advanced methods implemented in FuzzyWuzzy
         # or similar libs, but this is an easy win for now.
         matches = difflib.get_close_matches(cmd_name, self.list_commands(ctx), cutoff=0.5)
 
         if not matches:
             # Single letters are sometimes not matched so also try with a simple startswith
@@ -77,15 +79,15 @@
 
         if matches:
             formatted = '\n'.join(f'\t{m}' for m in sorted(matches))
             ctx.fail(f'`{cmd_name}` is not a {self.name} command.\n\nThe most similar commands are:\n{formatted}')
         else:
             ctx.fail(f'`{cmd_name}` is not a {self.name} command.\n\nNo similar commands found.')
 
-    def get_command(self, ctx, cmd_name):
+    def get_command(self, ctx: click.Context, cmd_name: str) -> click.Command | None:
         """Return the command that corresponds to the requested ``cmd_name``.
 
         This method is overridden from the base class in order to two functionalities:
 
             * If the command is found, automatically add the verbosity option.
             * If the command is not found, attempt to provide a list of suggestions with existing commands that resemble
               the requested command name.
@@ -107,15 +109,17 @@
         # execute the rest of this method to try and match commands that are similar in order to provide the user with
         # some hints. The problem is that there is no one canonical way to determine whether the invocation is due to a
         # normal command execution or a tab-complete operation. The `resilient_parsing` attribute of the `Context` is
         # designed to allow things like tab-completion, however, it is not the only purpose. For now this is our best
         # bet though to detect a tab-complete event. When `resilient_parsing` is switched on, we assume a tab-complete
         # and do nothing in case the command name does not match an actual command.
         if ctx.resilient_parsing:
-            return
+            return None
 
         self.fail_with_suggestions(ctx, cmd_name)
 
-    def group(self, *args, **kwargs):
+        return None
+
+    def group(self, *args, **kwargs) -> click.Group:
         """Ensure that sub command groups use the same class but do not override an explicitly set value."""
         kwargs.setdefault('cls', self.__class__)
         return super().group(*args, **kwargs)
```

### Comparing `aiida_core-2.3.1/aiida/cmdline/params/__init__.py` & `aiida_core-2.4.0/aiida/cmdline/params/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/params/arguments/__init__.py` & `aiida_core-2.4.0/aiida/cmdline/params/arguments/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/params/arguments/main.py` & `aiida_core-2.4.0/aiida/cmdline/params/arguments/main.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/params/arguments/overridable.py` & `aiida_core-2.4.0/aiida/cmdline/params/arguments/overridable.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/params/options/__init__.py` & `aiida_core-2.4.0/aiida/cmdline/params/options/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/params/options/commands/__init__.py` & `aiida_core-2.4.0/aiida/cmdline/params/options/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/params/options/commands/code.py` & `aiida_core-2.4.0/aiida/cmdline/params/options/commands/code.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/params/options/commands/computer.py` & `aiida_core-2.4.0/aiida/cmdline/params/options/commands/computer.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/params/options/commands/setup.py` & `aiida_core-2.4.0/aiida/cmdline/params/options/commands/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,22 +43,22 @@
     attribute, default = attribute_tuple
     parts = attribute.split('.')
 
     try:
         validate_profile_parameter(ctx)
     except click.BadParameter:
         return default
-    else:
-        try:
-            data = ctx.params['profile'].dictionary
-            for part in parts:
-                data = data[part]
-            return data
-        except KeyError:
-            return default
+
+    try:
+        data = ctx.params['profile'].dictionary
+        for part in parts:
+            data = data[part]
+        return data
+    except KeyError:
+        return default
 
 
 def get_repository_uri_default(ctx):
     """Return the default value for the repository URI for the current profile in the click context.
 
     :param ctx: click context which should contain the selected profile
     :return: default repository URI
```

### Comparing `aiida_core-2.3.1/aiida/cmdline/params/options/conditional.py` & `aiida_core-2.4.0/aiida/cmdline/params/options/conditional.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/params/options/config.py` & `aiida_core-2.4.0/aiida/cmdline/params/options/config.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/params/options/interactive.py` & `aiida_core-2.4.0/aiida/cmdline/params/options/interactive.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/params/options/main.py` & `aiida_core-2.4.0/aiida/cmdline/params/options/main.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/params/options/multivalue.py` & `aiida_core-2.4.0/aiida/cmdline/params/options/multivalue.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/params/options/overridable.py` & `aiida_core-2.4.0/aiida/cmdline/params/options/overridable.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/params/types/__init__.py` & `aiida_core-2.4.0/aiida/cmdline/params/types/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/params/types/calculation.py` & `aiida_core-2.4.0/aiida/cmdline/params/types/calculation.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/params/types/choice.py` & `aiida_core-2.4.0/aiida/cmdline/params/types/choice.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     its autocomplete. This type will generate the choices set lazily through the
     choices property
     """
 
     name = 'choice'
 
     def __init__(self, get_choices):
+        """Construct a new instance."""
         if not callable(get_choices):
             raise TypeError(f"Must pass a callable, got '{get_choices}'")
 
         super().__init__()
         self._get_choices = get_choices
         self.__click_choice = None
```

### Comparing `aiida_core-2.3.1/aiida/cmdline/params/types/code.py` & `aiida_core-2.4.0/aiida/cmdline/params/types/code.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/params/types/computer.py` & `aiida_core-2.4.0/aiida/cmdline/params/types/computer.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/params/types/config.py` & `aiida_core-2.4.0/aiida/cmdline/params/types/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         from aiida.manage.configuration.options import get_option, get_option_names
 
         if value not in get_option_names():
             raise click.BadParameter(f'{value} is not a valid configuration option')
 
         return get_option(value)
 
-    def shell_complete(self, ctx, param, incomplete):  # pylint: disable=unused-argument,no-self-use
+    def shell_complete(self, ctx, param, incomplete):  # pylint: disable=unused-argument
         """
         Return possible completions based on an incomplete value
 
         :returns: list of tuples of valid entry points (matching incomplete) and a description
         """
         from aiida.manage.configuration.options import get_option_names
```

### Comparing `aiida_core-2.3.1/aiida/cmdline/params/types/data.py` & `aiida_core-2.4.0/aiida/cmdline/params/types/data.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/params/types/group.py` & `aiida_core-2.4.0/aiida/cmdline/params/types/group.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/params/types/identifier.py` & `aiida_core-2.4.0/aiida/cmdline/params/types/identifier.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/params/types/multiple.py` & `aiida_core-2.4.0/aiida/cmdline/params/types/multiple.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 class MultipleValueParamType(click.ParamType):
     """
     An extension of click.ParamType that can parse multiple values for a given ParamType
     """
 
     def __init__(self, param_type):
+        """Construct a new instance."""
         super().__init__()
         self._param_type = param_type
 
         if hasattr(param_type, 'name'):
             self.name = f'{param_type.name}...'
         else:
             self.name = f'{param_type.__name__.upper()}...'
```

### Comparing `aiida_core-2.3.1/aiida/cmdline/params/types/node.py` & `aiida_core-2.4.0/aiida/cmdline/params/types/node.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/params/types/path.py` & `aiida_core-2.4.0/aiida/cmdline/params/types/path.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/params/types/plugin.py` & `aiida_core-2.4.0/aiida/cmdline/params/types/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,15 +210,15 @@
                     "entry point '{}' is not valid for any of the allowed "
                     'entry point groups: {}'.format(name, ' '.join(self.groups))
                 )
 
             group = matching_groups.pop()
 
         else:
-            ValueError(f'invalid entry point string format: {entry_point_string}')
+            raise ValueError(f'invalid entry point string format: {entry_point_string}')
 
         # If there is a factory for the entry point group, use that, otherwise use ``get_entry_point``
         try:
             get_entry_point_partial = functools.partial(self._factory_mapping[group], load=False)
         except KeyError:
             get_entry_point_partial = functools.partial(get_entry_point, group)
```

### Comparing `aiida_core-2.3.1/aiida/cmdline/params/types/process.py` & `aiida_core-2.4.0/aiida/cmdline/params/types/process.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/params/types/profile.py` & `aiida_core-2.4.0/aiida/cmdline/params/types/profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         if self._load_profile:
             load_profile(profile.name)
 
         ctx.obj.profile = profile
 
         return profile
 
-    def shell_complete(self, ctx, param, incomplete):  # pylint: disable=unused-argument,no-self-use
+    def shell_complete(self, ctx, param, incomplete):  # pylint: disable=unused-argument
         """Return possible completions based on an incomplete value
 
         :returns: list of tuples of valid entry points (matching incomplete) and a description
         """
         from aiida.common.exceptions import MissingConfigurationError
         from aiida.manage.configuration import get_config
```

### Comparing `aiida_core-2.3.1/aiida/cmdline/params/types/strings.py` & `aiida_core-2.4.0/aiida/cmdline/params/types/strings.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/params/types/user.py` & `aiida_core-2.4.0/aiida/cmdline/params/types/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
         if len(results) > 1:
             self.fail(f"Multiple users found with email '{value}': {results}")
 
         return results[0]
 
     @with_dbenv()
-    def shell_complete(self, ctx, param, incomplete):  # pylint: disable=unused-argument,no-self-use
+    def shell_complete(self, ctx, param, incomplete):  # pylint: disable=unused-argument
         """
         Return possible completions based on an incomplete value
 
         :returns: list of tuples of valid entry points (matching incomplete) and a description
         """
         from aiida import orm
```

### Comparing `aiida_core-2.3.1/aiida/cmdline/params/types/workflow.py` & `aiida_core-2.4.0/aiida/cmdline/params/types/workflow.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/utils/__init__.py` & `aiida_core-2.4.0/aiida/cmdline/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/utils/ascii_vis.py` & `aiida_core-2.4.0/aiida/cmdline/utils/ascii_vis.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,70 +11,90 @@
 __all__ = ('format_call_graph',)
 
 TREE_LAST_ENTRY = '\u2514\u2500\u2500 '
 TREE_MIDDLE_ENTRY = '\u251C\u2500\u2500 '
 TREE_FIRST_ENTRY = TREE_MIDDLE_ENTRY
 
 
-def calc_info(node) -> str:
-    """Return a string with the summary of the state of a CalculationNode."""
+def calc_info(node, call_link_label: bool = False) -> str:
+    """Return a string with the summary of the state of a CalculationNode.
+
+    :param calc_node: The calculation node
+    :param call_link_label: Include the call link label if other from the default ``CALL``.
+    """
     from aiida.orm import ProcessNode, WorkChainNode
 
     if not isinstance(node, ProcessNode):
         raise TypeError(f'Unknown type: {type(node)}')
 
     process_label = node.process_label
     process_state = node.process_state.value.capitalize()
     exit_status = node.exit_status
 
-    if exit_status is not None:
-        string = f'{process_label}<{node.pk}> {process_state} [{exit_status}]'
+    if call_link_label and (caller := node.caller):
+        from aiida.common.links import LinkType
+        call_link = [
+            triple.link_label
+            for triple in caller.base.links.get_outgoing(link_type=(LinkType.CALL_CALC, LinkType.CALL_WORK)).all()
+            if triple.node.pk == node.pk
+        ][0]
+    else:
+        call_link = None
+
+    if call_link and call_link != 'CALL':
+        string = f'{process_label}<{node.pk} | {call_link}> {process_state}'
     else:
         string = f'{process_label}<{node.pk}> {process_state}'
 
+    if exit_status is not None:
+        string += f' [{exit_status}]'
+
     if isinstance(node, WorkChainNode) and node.stepper_state_info:
         string += f' [{node.stepper_state_info}]'
 
     return string
 
 
-def format_call_graph(calc_node, max_depth: int = None, info_fn=calc_info):
-    """
-    Print a tree like the POSIX tree command for the calculation call graph
+def format_call_graph(calc_node, max_depth: int = None, call_link_label: bool = False, info_fn=calc_info):
+    """Print a tree like the POSIX tree command for the calculation call graph.
 
     :param calc_node: The calculation node
     :param max_depth: Maximum depth of the call graph to print
-    :param info_fn: An optional function that takes the node and returns a string
-        of information to be displayed for each node.
+    :param call_link_label: Include the call link label if other from the default ``CALL``.
+    :param info_fn: An optional function that takes the node and returns a string of information to be displayed for
+        each node.
     """
-    call_tree = build_call_graph(calc_node, max_depth=max_depth, info_fn=info_fn)
+    call_tree = build_call_graph(calc_node, max_depth=max_depth, call_link_label=call_link_label, info_fn=info_fn)
     return format_tree_descending(call_tree)
 
 
-def build_call_graph(calc_node, max_depth: int = None, info_fn=calc_info) -> str:
+def build_call_graph(calc_node, max_depth: int = None, call_link_label: bool = False, info_fn=calc_info) -> str:
     """Build the call graph of a given node.
 
     :param calc_node: The calculation node
     :param max_depth: Maximum depth of the call graph to build. Use `None` for unlimited.
-    :param info_fn: An optional function that takes the node and returns a string
-        of information to be displayed for each node.
+    :param call_link_label: Include the call link label if other from the default ``CALL``.
+    :param info_fn: An optional function that takes the node and returns a string of information to be displayed for
+        each node.
     """
     if max_depth is not None:
         if max_depth < 0:
             raise ValueError('max_depth must be >= 0')
         if max_depth == 0:
             return ''
 
-    info_string = info_fn(calc_node)
+    info_string = info_fn(calc_node, call_link_label)
     called = calc_node.called
     called.sort(key=lambda x: x.ctime)
     if called and max_depth != 1:
         if max_depth is not None:
             max_depth -= 1
-        return info_string, [build_call_graph(child, max_depth=max_depth, info_fn=info_fn) for child in called]
+        return info_string, [
+            build_call_graph(c, max_depth=max_depth, call_link_label=call_link_label, info_fn=info_fn) for c in called
+        ]
 
     return info_string
 
 
 def format_tree_descending(tree, prefix='', pos=-1):
     """Format a descending tree."""
     # pylint: disable=too-many-branches
```

### Comparing `aiida_core-2.3.1/aiida/cmdline/utils/common.py` & `aiida_core-2.4.0/aiida/cmdline/utils/common.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/utils/decorators.py` & `aiida_core-2.4.0/aiida/cmdline/utils/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,15 +195,15 @@
         @click.command()
         @check_circus_zmq_version
         def do_circus_stuff():
             pass
     """
     import zmq
     try:
-        zmq_version = [int(part) for part in zmq.__version__.split('.')[:2]]  # type: ignore
+        zmq_version = [int(part) for part in zmq.__version__.split('.')[:2]]
         if len(zmq_version) < 2:
             raise ValueError()
     except (AttributeError, ValueError):
         echo.echo_critical('Unknown PyZQM version - aborting...')
 
     if zmq_version[0] < 13 or (zmq_version[0] == 13 and zmq_version[1] < 1):
         echo.echo_critical('AiiDA daemon needs PyZMQ >= 13.1.0 to run - aborting...')
```

### Comparing `aiida_core-2.3.1/aiida/cmdline/utils/defaults.py` & `aiida_core-2.4.0/aiida/cmdline/utils/defaults.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/utils/echo.py` & `aiida_core-2.4.0/aiida/cmdline/utils/echo.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,54 +52,54 @@
     :param message: the message to log.
     :param fg: if provided this will become the foreground color.
     :param bold: whether to print the messaformat bold.
     :param nl: whether to print a newlineaddhe end of the message.
     :param err: whether to log to stderr.
     """
     message = click.style(message, fg=fg, bold=bold)
-    CMDLINE_LOGGER.report(message, extra=dict(nl=nl, err=err, prefix=False))
+    CMDLINE_LOGGER.report(message, extra={'nl': nl, 'err': err, 'prefix': False})
 
 
 def echo_debug(message: str, bold: bool = False, nl: bool = True, err: bool = False, prefix: bool = True) -> None:
     """Log a debug message to the cmdline logger.
 
     :param message: the message to log.
     :param bold: whether to format the message in bold.
     :param nl: whether to add a newline at the end of the message.
     :param err: whether to log to stderr.
     :param prefix: whether the message should be prefixed with a colored version of the log level.
     """
     message = click.style(message, bold=bold)
-    CMDLINE_LOGGER.debug(message, extra=dict(nl=nl, err=err, prefix=prefix))
+    CMDLINE_LOGGER.debug(message, extra={'nl': nl, 'err': err, 'prefix': prefix})
 
 
 def echo_info(message: str, bold: bool = False, nl: bool = True, err: bool = False, prefix: bool = True) -> None:
     """Log an info message to the cmdline logger.
 
     :param message: the message to log.
     :param bold: whether to format the message in bold.
     :param nl: whether to add a newline at the end of the message.
     :param err: whether to log to stderr.
     :param prefix: whether the message should be prefixed with a colored version of the log level.
     """
     message = click.style(message, bold=bold)
-    CMDLINE_LOGGER.info(message, extra=dict(nl=nl, err=err, prefix=prefix))
+    CMDLINE_LOGGER.info(message, extra={'nl': nl, 'err': err, 'prefix': prefix})
 
 
 def echo_report(message: str, bold: bool = False, nl: bool = True, err: bool = False, prefix: bool = True) -> None:
     """Log an report message to the cmdline logger.
 
     :param message: the message to log.
     :param bold: whether to format the message in bold.
     :param nl: whether to add a newline at the end of the message.
     :param err: whether to log to stderr.
     :param prefix: whether the message should be prefixed with a colored version of the log level.
     """
     message = click.style(message, bold=bold)
-    CMDLINE_LOGGER.report(message, extra=dict(nl=nl, err=err, prefix=prefix))
+    CMDLINE_LOGGER.report(message, extra={'nl': nl, 'err': err, 'prefix': prefix})
 
 
 def echo_success(message: str, bold: bool = False, nl: bool = True, err: bool = False, prefix: bool = True) -> None:
     """Log a success message to the cmdline logger.
 
     .. note:: The message will be logged at the ``REPORT`` level and always with the ``Success:`` prefix.
 
@@ -110,41 +110,41 @@
     :param prefix: whether the message should be prefixed with a colored version of the log level.
     """
     message = click.style(message, bold=bold)
 
     if prefix:
         message = click.style('Success: ', bold=True, fg=COLORS['success']) + message
 
-    CMDLINE_LOGGER.report(message, extra=dict(nl=nl, err=err, prefix=False))
+    CMDLINE_LOGGER.report(message, extra={'nl': nl, 'err': err, 'prefix': False})
 
 
 def echo_warning(message: str, bold: bool = False, nl: bool = True, err: bool = False, prefix: bool = True) -> None:
     """Log a warning message to the cmdline logger.
 
     :param message: the message to log.
     :param bold: whether to format the message in bold.
     :param nl: whether to add a newline at the end of the message.
     :param err: whether to log to stderr.
     :param prefix: whether the message should be prefixed with a colored version of the log level.
     """
     message = click.style(message, bold=bold)
-    CMDLINE_LOGGER.warning(message, extra=dict(nl=nl, err=err, prefix=prefix))
+    CMDLINE_LOGGER.warning(message, extra={'nl': nl, 'err': err, 'prefix': prefix})
 
 
 def echo_error(message: str, bold: bool = False, nl: bool = True, err: bool = True, prefix: bool = True) -> None:
     """Log an error message to the cmdline logger.
 
     :param message: the message to log.
     :param bold: whether to format the message in bold.
     :param nl: whether to add a newline at the end of the message.
     :param err: whether to log to stderr.
     :param prefix: whether the message should be prefixed with a colored version of the log level.
     """
     message = click.style(message, bold=bold)
-    CMDLINE_LOGGER.error(message, extra=dict(nl=nl, err=err, prefix=prefix))
+    CMDLINE_LOGGER.error(message, extra={'nl': nl, 'err': err, 'prefix': prefix})
 
 
 def echo_critical(message: str, bold: bool = False, nl: bool = True, err: bool = True, prefix: bool = True) -> None:
     """Log a critical error message to the cmdline logger and exit with ``exit_status``.
 
     This should be used to print messages for errors that cannot be recovered from and so the script should be directly
     terminated with a non-zero exit status to indicate that the command failed.
@@ -152,15 +152,15 @@
     :param message: the message to log.
     :param bold: whether to format the message in bold.
     :param nl: whether to add a newline at the end of the message.
     :param err: whether to log to stderr.
     :param prefix: whether the message should be prefixed with a colored version of the log level.
     """
     message = click.style(message, bold=bold)
-    CMDLINE_LOGGER.critical(message, extra=dict(nl=nl, err=err, prefix=prefix))
+    CMDLINE_LOGGER.critical(message, extra={'nl': nl, 'err': err, 'prefix': prefix})
     sys.exit(ExitCode.CRITICAL)
 
 
 def echo_deprecated(message: str, bold: bool = False, nl: bool = True, err: bool = True, exit: bool = False) -> None:
     """Log an error message to the cmdline logger, prefixed with 'Deprecated:' exiting with the given ``exit_status``.
 
     This should be used to indicate deprecated commands.
```

### Comparing `aiida_core-2.3.1/aiida/cmdline/utils/log.py` & `aiida_core-2.4.0/aiida/cmdline/utils/log.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/utils/multi_line_input.py` & `aiida_core-2.4.0/aiida/cmdline/utils/multi_line_input.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/utils/pluginable.py` & `aiida_core-2.4.0/aiida/cmdline/utils/pluginable.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/utils/query/__init__.py` & `aiida_core-2.4.0/aiida/cmdline/utils/query/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/utils/query/calculation.py` & `aiida_core-2.4.0/aiida/cmdline/utils/query/calculation.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/utils/query/formatting.py` & `aiida_core-2.4.0/aiida/cmdline/utils/query/formatting.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/utils/query/mapping.py` & `aiida_core-2.4.0/aiida/cmdline/utils/query/mapping.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/utils/repository.py` & `aiida_core-2.4.0/aiida/cmdline/utils/repository.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/utils/shell.py` & `aiida_core-2.4.0/aiida/cmdline/utils/shell.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/cmdline/utils/templates.py` & `aiida_core-2.4.0/aiida/cmdline/utils/templates.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/common/__init__.py` & `aiida_core-2.4.0/aiida/common/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/common/constants.py` & `aiida_core-2.4.0/aiida/common/constants.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/common/datastructures.py` & `aiida_core-2.4.0/aiida/common/datastructures.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,18 @@
 # This file is part of the AiiDA code.                                    #
 #                                                                         #
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-core #
 # For further information on the license, see the LICENSE.txt file        #
 # For further information please visit http://www.aiida.net               #
 ###########################################################################
 """Module to define commonly used data structures."""
+from __future__ import annotations
+
 from enum import Enum, IntEnum
+from typing import TYPE_CHECKING
 
 from .extendeddicts import DefaultFieldsAttributeDict
 
 __all__ = ('StashMode', 'CalcJobState', 'CalcInfo', 'CodeInfo', 'CodeRunMode')
 
 
 class StashMode(Enum):
@@ -89,14 +92,39 @@
     _default_fields = (
         'job_environment', 'email', 'email_on_started', 'email_on_terminated', 'uuid', 'prepend_text', 'append_text',
         'num_machines', 'num_mpiprocs_per_machine', 'priority', 'max_wallclock_seconds', 'max_memory_kb', 'rerunnable',
         'retrieve_list', 'retrieve_temporary_list', 'local_copy_list', 'remote_copy_list', 'remote_symlink_list',
         'provenance_exclude_list', 'codes_info', 'codes_run_mode', 'skip_submit'
     )
 
+    if TYPE_CHECKING:
+
+        job_environment: None | dict[str, str]
+        email: None | str
+        email_on_started: bool
+        email_on_terminated: bool
+        uuid: None | str
+        prepend_text: None | str
+        append_text: None | str
+        num_machines: None | int
+        num_mpiprocs_per_machine: None | int
+        priority: None | int
+        max_wallclock_seconds: None | int
+        max_memory_kb: None | int
+        rerunnable: bool
+        retrieve_list: None | list[str | tuple[str, str, str]]
+        retrieve_temporary_list: None | list[str | tuple[str, str, str]]
+        local_copy_list: None | list[tuple[str, str, str]]
+        remote_copy_list: None | list[tuple[str, str, str]]
+        remote_symlink_list: None | list[tuple[str, str, str]]
+        provenance_exclude_list: None | list[str]
+        codes_info: None | list[CodeInfo]
+        codes_run_mode: None | CodeRunMode
+        skip_submit: None | bool
+
 
 class CodeInfo(DefaultFieldsAttributeDict):
     """
     This attribute-dictionary contains the information needed to execute a code.
     Possible attributes are:
 
     * ``cmdline_params``: a list of strings, containing parameters to be written on
@@ -144,14 +172,24 @@
         'stdout_name',
         'stderr_name',
         'join_files',
         'withmpi',
         'code_uuid'
     )
 
+    if TYPE_CHECKING:
+
+        cmdline_params: None | list[str]
+        stdin_name: None | str
+        stdout_name: None | str
+        stderr_name: None | str
+        join_files: None | bool
+        withmpi: None | bool
+        code_uuid: None | str
+
 
 class CodeRunMode(IntEnum):
     """Enum to indicate the way the codes of a calculation should be run.
 
     For PARALLEL, the codes for a given calculation will be run in parallel by running them in the background::
 
         code1.x &
```

### Comparing `aiida_core-2.3.1/aiida/common/escaping.py` & `aiida_core-2.4.0/aiida/common/escaping.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/common/exceptions.py` & `aiida_core-2.4.0/aiida/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/common/extendeddicts.py` & `aiida_core-2.4.0/aiida/common/extendeddicts.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/common/files.py` & `aiida_core-2.4.0/aiida/common/files.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/common/folders.py` & `aiida_core-2.4.0/aiida/common/folders.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/common/hashing.py` & `aiida_core-2.4.0/aiida/common/hashing.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/common/json.py` & `aiida_core-2.4.0/aiida/common/json.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/common/lang.py` & `aiida_core-2.4.0/aiida/common/lang.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/common/links.py` & `aiida_core-2.4.0/aiida/common/links.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/common/log.py` & `aiida_core-2.4.0/aiida/common/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,15 +208,15 @@
                 # Remove the `console` stdout stream handler to prevent messages being duplicated in the daemon log file
                 logger['handlers'].remove('console')
             except ValueError:
                 pass
 
     # If the ``CLI_ACTIVE`` is set, a ``verdi`` command is being executed, so we replace the ``console`` handler with
     # the ``cli`` one for all loggers.
-    if CLI_ACTIVE is True:
+    if CLI_ACTIVE is True and not daemon:
         for logger in config['loggers'].values():
             handlers = logger['handlers']
             if 'console' in handlers:
                 handlers.remove('console')
             handlers.append('cli')
 
     # If ``CLI_LOG_LEVEL`` is set, a ``verdi`` command is being executed with the ``--verbosity`` option. In this case
```

### Comparing `aiida_core-2.3.1/aiida/common/progress_reporter.py` & `aiida_core-2.4.0/aiida/common/progress_reporter.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/common/timezone.py` & `aiida_core-2.4.0/aiida/common/timezone.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/common/utils.py` & `aiida_core-2.4.0/aiida/common/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
     # wrong results in these cases, see
     # http://docs.python.org/2/library/datetime.html
     s_tot = int(s_tot)
 
     if negative_to_zero:
         s_tot = max(s_tot, 0)
 
-    negative = (s_tot < 0)
+    negative = s_tot < 0
     s_tot = abs(s_tot)
 
     negative_string = ' in the future' if negative else ' ago'
 
     # For the moment stay away from months and years, difficult to get
     days, remainder = divmod(s_tot, 3600 * 24)
     hours, remainder = divmod(remainder, 3600)
@@ -515,14 +515,15 @@
     :param capture_stderr: if True, also captures sys.stderr. To access the
         lines, use obj.stderr_lines. If False, obj.stderr_lines is None.
     """
 
     # pylint: disable=attribute-defined-outside-init
 
     def __init__(self, capture_stderr=False):
+        """Construct a new instance."""
         self.stdout_lines = []
         super().__init__()
 
         self._capture_stderr = capture_stderr
         if self._capture_stderr:
             self.stderr_lines = []
         else:
```

### Comparing `aiida_core-2.3.1/aiida/common/warnings.py` & `aiida_core-2.4.0/aiida/common/warnings.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/engine/__init__.py` & `aiida_core-2.4.0/aiida/engine/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     'WithNonDb',
     'WithSerialize',
     'WorkChain',
     'append_',
     'assign_',
     'calcfunction',
     'construct_awaitable',
+    'get_daemon_client',
     'get_object_loader',
     'if_',
     'interruptable_task',
     'is_process_function',
     'process_handler',
     'return_',
     'run',
```

### Comparing `aiida_core-2.3.1/aiida/engine/daemon/__init__.py` & `aiida_core-2.4.0/aiida/engine/daemon/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,10 +14,11 @@
 # yapf: disable
 # pylint: disable=wildcard-import
 
 from .client import *
 
 __all__ = (
     'DaemonClient',
+    'get_daemon_client',
 )
 
 # yapf: enable
```

### Comparing `aiida_core-2.3.1/aiida/engine/daemon/client.py` & `aiida_core-2.4.0/aiida/engine/daemon/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 LOGGER = AIIDA_LOGGER.getChild('engine.daemon.client')
 
 VERDI_BIN = shutil.which('verdi')
 # Recent versions of virtualenv create the environment variable VIRTUAL_ENV
 VIRTUALENV = os.environ.get('VIRTUAL_ENV', None)
 
-__all__ = ('DaemonClient',)
+__all__ = ('DaemonClient', 'get_daemon_client')
 
 
 class ControllerProtocol(enum.Enum):
     """The protocol to use for the controller of the Circus daemon."""
 
     IPC = 0
     TCP = 1
```

### Comparing `aiida_core-2.3.1/aiida/engine/daemon/execmanager.py` & `aiida_core-2.4.0/aiida/engine/daemon/execmanager.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,36 +106,34 @@
     if dry_run:
         workdir = transport.getcwd()
     else:
         remote_user = transport.whoami()
         remote_working_directory = computer.get_workdir().format(username=remote_user)
         if not remote_working_directory.strip():
             raise exceptions.ConfigurationError(
-                "[submission of calculation {}] No remote_working_directory configured for computer '{}'".format(
-                    node.pk, computer.label
-                )
+                f'[submission of calculation {node.pk}] No remote_working_directory '
+                f"configured for computer '{computer.label}'"
             )
 
         # If it already exists, no exception is raised
         try:
             transport.chdir(remote_working_directory)
         except IOError:
             logger.debug(
-                '[submission of calculation {}] Unable to chdir in {}, trying to create it'.format(
-                    node.pk, remote_working_directory
-                )
+                f'[submission of calculation {node.pk}] Unable to '
+                f'chdir in {remote_working_directory}, trying to create it'
             )
             try:
                 transport.makedirs(remote_working_directory)
                 transport.chdir(remote_working_directory)
             except EnvironmentError as exc:
                 raise exceptions.ConfigurationError(
-                    '[submission of calculation {}] '
-                    'Unable to create the remote directory {} on '
-                    "computer '{}': {}".format(node.pk, remote_working_directory, computer.label, exc)
+                    f'[submission of calculation {node.pk}] '
+                    f'Unable to create the remote directory {remote_working_directory} on '
+                    f"computer '{computer.label}': {exc}"
                 )
         # Store remotely with sharding (here is where we choose
         # the folder structure of remote jobs; then I store this
         # in the calculation properties using _set_remote_dir
         # and I do not have to know the logic, but I just need to
         # read the absolute path from the calculation properties.
         transport.mkdir(calc_info.uuid[:2], ignore_existing=True)
@@ -245,71 +243,72 @@
         for filename in folder.get_content_list():
             logger.debug(f'[submission of calculation {node.pk}] copying file/folder {filename}...')
             transport.put(folder.get_abs_path(filename), filename)
 
         for (remote_computer_uuid, remote_abs_path, dest_rel_path) in remote_copy_list:
             if remote_computer_uuid == computer.uuid:
                 logger.debug(
-                    '[submission of calculation {}] copying {} remotely, directly on the machine {}'.format(
-                        node.pk, dest_rel_path, computer.label
-                    )
+                    f'[submission of calculation {node.pk}] copying {dest_rel_path} '
+                    f'remotely, directly on the machine {computer.label}'
                 )
                 try:
                     transport.copy(remote_abs_path, dest_rel_path)
+                except FileNotFoundError:
+                    logger.warning(
+                        f'[submission of calculation {node.pk}] Unable to copy remote '
+                        f'resource from {remote_abs_path} to {dest_rel_path}! NOT Stopping but just ignoring!.'
+                    )
                 except (IOError, OSError):
                     logger.warning(
-                        '[submission of calculation {}] Unable to copy remote resource from {} to {}! '
-                        'Stopping.'.format(node.pk, remote_abs_path, dest_rel_path)
+                        f'[submission of calculation {node.pk}] Unable to copy remote '
+                        f'resource from {remote_abs_path} to {dest_rel_path}! Stopping.'
                     )
                     raise
             else:
                 raise NotImplementedError(
-                    '[submission of calculation {}] Remote copy between two different machines is '
-                    'not implemented yet'.format(node.pk)
+                    f'[submission of calculation {node.pk}] Remote copy between two different machines is '
+                    'not implemented yet'
                 )
 
         for (remote_computer_uuid, remote_abs_path, dest_rel_path) in remote_symlink_list:
             if remote_computer_uuid == computer.uuid:
                 logger.debug(
-                    '[submission of calculation {}] copying {} remotely, directly on the machine {}'.format(
-                        node.pk, dest_rel_path, computer.label
-                    )
+                    f'[submission of calculation {node.pk}] copying {dest_rel_path} remotely, '
+                    f'directly on the machine {computer.label}'
                 )
                 try:
                     transport.symlink(remote_abs_path, dest_rel_path)
                 except (IOError, OSError):
                     logger.warning(
-                        '[submission of calculation {}] Unable to create remote symlink from {} to {}! '
-                        'Stopping.'.format(node.pk, remote_abs_path, dest_rel_path)
+                        f'[submission of calculation {node.pk}] Unable to create remote symlink '
+                        f'from {remote_abs_path} to {dest_rel_path}! Stopping.'
                     )
                     raise
             else:
                 raise IOError(
                     f'It is not possible to create a symlink between two different machines for calculation {node.pk}'
                 )
     else:
 
         if remote_copy_list:
             filepath = os.path.join(workdir, '_aiida_remote_copy_list.txt')
             with open(filepath, 'w', encoding='utf-8') as handle:  # type: ignore[assignment]
                 for remote_computer_uuid, remote_abs_path, dest_rel_path in remote_copy_list:
                     handle.write(
-                        'would have copied {} to {} in working directory on remote {}'.format(
-                            remote_abs_path, dest_rel_path, computer.label
-                        )
+                        f'would have copied {remote_abs_path} to {dest_rel_path} in working '
+                        f'directory on remote {computer.label}'
                     )
 
         if remote_symlink_list:
             filepath = os.path.join(workdir, '_aiida_remote_symlink_list.txt')
             with open(filepath, 'w', encoding='utf-8') as handle:  # type: ignore[assignment]
                 for remote_computer_uuid, remote_abs_path, dest_rel_path in remote_symlink_list:
                     handle.write(
-                        'would have created symlinks from {} to {} in working directory on remote {}'.format(
-                            remote_abs_path, dest_rel_path, computer.label
-                        )
+                        f'would have created symlinks from {remote_abs_path} to {dest_rel_path} in working'
+                        f'directory on remote {computer.label}'
                     )
 
     # Loop recursively over content of the sandbox folder copying all that are not in `provenance_exclude_list`. Note
     # that directories are not created explicitly. The `node.put_object_from_filelike` call will create intermediate
     # directories for nested files automatically when needed. This means though that empty folders in the sandbox or
     # folders that would be empty when considering the `provenance_exclude_list` will *not* be copied to the repo. The
     # advantage of this explicit copying instead of deleting the files from `provenance_exclude_list` from the sandbox
```

### Comparing `aiida_core-2.3.1/aiida/engine/daemon/worker.py` & `aiida_core-2.4.0/aiida/engine/daemon/worker.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,19 +7,20 @@
 # For further information on the license, see the LICENSE.txt file        #
 # For further information please visit http://www.aiida.net               #
 ###########################################################################
 """Function that starts a daemon worker."""
 import asyncio
 import logging
 import signal
+import sys
 
 from aiida.common.log import configure_logging
 from aiida.engine.daemon.client import get_daemon_client
 from aiida.engine.runners import Runner
-from aiida.manage import get_manager
+from aiida.manage import get_config_option, get_manager
 
 LOGGER = logging.getLogger(__name__)
 
 
 async def shutdown_worker(runner: Runner) -> None:
     """Cleanup tasks tied to the service's shutdown."""
     from asyncio import all_tasks, current_task
@@ -45,14 +46,18 @@
         manager = get_manager()
         runner = manager.create_daemon_runner()
         manager.set_runner(runner)
     except Exception:
         LOGGER.exception('daemon worker failed to start')
         raise
 
+    if isinstance(rlimit := get_config_option('daemon.recursion_limit'), int):
+        LOGGER.info('Setting maximum recursion limit of daemon worker to %s', rlimit)
+        sys.setrecursionlimit(rlimit)
+
     signals = (signal.SIGTERM, signal.SIGINT)
     for s in signals:  # pylint: disable=invalid-name
         runner.loop.add_signal_handler(s, lambda s=s: asyncio.create_task(shutdown_worker(runner)))
 
     try:
         LOGGER.info('Starting a daemon worker')
         runner.start()
```

### Comparing `aiida_core-2.3.1/aiida/engine/exceptions.py` & `aiida_core-2.4.0/aiida/engine/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/engine/launch.py` & `aiida_core-2.4.0/aiida/engine/launch.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/engine/persistence.py` & `aiida_core-2.4.0/aiida/engine/persistence.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 LOGGER = logging.getLogger(__name__)
 OBJECT_LOADER = None
 
 
 class ObjectLoader(plumpy.loaders.DefaultObjectLoader):
     """Custom object loader for `aiida-core`."""
 
-    def load_object(self, identifier: str) -> Any:  # pylint: disable=no-self-use
+    def load_object(self, identifier: str) -> Any:
         """Attempt to load the object identified by the given `identifier`.
 
         .. note:: We override the `plumpy.DefaultObjectLoader` to be able to throw an `ImportError` instead of a
             `ValueError` which in the context of `aiida-core` is not as apt, since we are loading classes.
 
         :param identifier: concatenation of module and resource name
         :return: loaded object
@@ -66,15 +66,15 @@
         OBJECT_LOADER = ObjectLoader()
     return OBJECT_LOADER
 
 
 class AiiDAPersister(plumpy.persistence.Persister):
     """Persister to take saved process instance states and persisting them to the database."""
 
-    def save_checkpoint(self, process: 'Process', tag: Optional[str] = None):  # type: ignore[override] # pylint: disable=no-self-use
+    def save_checkpoint(self, process: 'Process', tag: Optional[str] = None):  # type: ignore[override]
         """Persist a Process instance.
 
         :param process: :class:`aiida.engine.Process`
         :param tag: optional checkpoint identifier to allow distinguishing multiple checkpoints for the same process
         :raises: :class:`PersistenceError` Raised if there was a problem saving the checkpoint
         """
         LOGGER.debug('Persisting process<%d>', process.pid)
@@ -91,15 +91,15 @@
         try:
             process.node.set_checkpoint(serialize.serialize(bundle))
         except Exception:
             raise PersistenceError(f"Failed to store a checkpoint for '{process}': {traceback.format_exc()}")
 
         return bundle
 
-    def load_checkpoint(self, pid: Hashable, tag: Optional[str] = None) -> plumpy.persistence.Bundle:  # pylint: disable=no-self-use
+    def load_checkpoint(self, pid: Hashable, tag: Optional[str] = None) -> plumpy.persistence.Bundle:
         """Load a process from a persisted checkpoint by its process id.
 
         :param pid: the process id of the :class:`plumpy.Process`
         :param tag: optional checkpoint identifier to allow retrieving a specific sub checkpoint
         :return: a bundle with the process state
         :rtype: :class:`plumpy.Bundle`
         :raises: :class:`PersistenceError` Raised if there was a problem loading the checkpoint
@@ -136,15 +136,15 @@
     def get_process_checkpoints(self, pid: Hashable):
         """Return a list of all the current persisted process checkpoints for the specified process.
 
         :param pid: the process pid
         :return: list of PersistedCheckpoint tuples with element containing the process id and optional checkpoint tag.
         """
 
-    def delete_checkpoint(self, pid: Hashable, tag: Optional[str] = None) -> None:  # pylint: disable=no-self-use,unused-argument
+    def delete_checkpoint(self, pid: Hashable, tag: Optional[str] = None) -> None:  # pylint: disable=unused-argument
         """Delete a persisted process checkpoint, where no error will be raised if the checkpoint does not exist.
 
         :param pid: the process id of the :class:`plumpy.Process`
         :param tag: optional checkpoint identifier to allow retrieving a specific sub checkpoint
         """
         from aiida.orm import load_node
```

### Comparing `aiida_core-2.3.1/aiida/engine/processes/__init__.py` & `aiida_core-2.4.0/aiida/engine/processes/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/engine/processes/builder.py` & `aiida_core-2.4.0/aiida/engine/processes/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,21 +202,21 @@
         :param kwds: keyword value pairs that should be mapped onto the ports.
         """
         if args:
             for key, value in args[0].items():
                 if isinstance(value, Mapping):
                     self[key].update(value)
                 else:
-                    self.__setattr__(key, value)
+                    self.__setattr__(key, value)  # pylint: disable=unnecessary-dunder-call
 
         for key, value in kwds.items():
             if isinstance(value, Mapping):
                 self[key].update(value)
             else:
-                self.__setattr__(key, value)
+                self.__setattr__(key, value)  # pylint: disable=unnecessary-dunder-call
 
     def _inputs(self, prune: bool = False) -> dict:
         """Return the entire mapping of inputs specified for this builder.
 
         :param prune: boolean, when True, will prune nested namespaces that contain no actual values whatsoever
         :return: mapping of inputs ports and their input values.
         """
```

### Comparing `aiida_core-2.3.1/aiida/engine/processes/calcjobs/__init__.py` & `aiida_core-2.4.0/aiida/engine/processes/calcjobs/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/engine/processes/calcjobs/calcjob.py` & `aiida_core-2.4.0/aiida/engine/processes/calcjobs/calcjob.py`

 * *Files 2% similar despite different names*

```diff
@@ -321,15 +321,15 @@
             valid_type=str,
             required=False,
             help='Set the quality of service to use in for the queue on the remote computer'
         )
         spec.input(
             'metadata.options.withmpi',
             valid_type=bool,
-            default=False,
+            required=False,
             help='Set the calculation to use mpi',
         )
         spec.input(
             'metadata.options.mpirun_extra_params',
             valid_type=(list, tuple),
             default=lambda: [],
             help='Set the extra params to pass to the mpirun (or equivalent) command after the one provided in '
@@ -535,27 +535,32 @@
         This means invoking the `presubmit` and storing the temporary folder in the node's repository. Then we move the
         process in the `Wait` state, waiting for the `UPLOAD` transport task to be started.
 
         :returns: the `Stop` command if a dry run, int if the process has an exit status,
             `Wait` command if the calcjob is to be uploaded
 
         """
-        if self.inputs.metadata.dry_run:  # type: ignore[union-attr]
+        if self.inputs.metadata.dry_run:
             self._perform_dry_run()
             return plumpy.process_states.Stop(None, True)
 
-        if 'remote_folder' in self.inputs:  # type: ignore[operator]
+        if 'remote_folder' in self.inputs:
             exit_code = self._perform_import()
             return exit_code
 
         # The following conditional is required for the caching to properly work. Even if the source node has a process
         # state of `Finished` the cached process will still enter the running state. The process state will have then
         # been overridden by the engine to `Running` so we cannot check that, but if the `exit_status` is anything other
         # than `None`, it should mean this node was taken from the cache, so the process should not be rerun.
         if self.node.exit_status is not None:
+            # Normally the outputs will be attached to the process by a ``Parser``, if defined in the inputs. But in
+            # this case, the parser will not be called. The outputs will already have been added to the process node
+            # though, so all that needs to be done here is just also assign them to the process instance. This such that
+            # when the process returns its results, it returns the actual outputs and not an empty dictionary.
+            self._outputs = self.node.get_outgoing(link_type=LinkType.CREATE).nested()  # pylint: disable=attribute-defined-outside-init
             return self.node.exit_status
 
         # Launch the upload operation
         return plumpy.process_states.Wait(msg='Waiting to upload', data=UPLOAD_COMMAND)
 
     def prepare_for_submission(self, folder: Folder) -> CalcInfo:
         """Prepare the calculation for submission.
@@ -587,15 +592,15 @@
         super()._setup_inputs()
 
         # If a computer has not yet been set, which should have been done in ``_setup_metadata`` if it was specified
         # in the ``metadata`` inputs, set the computer associated with the ``code`` input. Note that not all ``code``s
         # will have an associated computer, but in that case the ``computer`` property should return ``None`` and
         # nothing would change anyway.
         if not self.node.computer:
-            self.node.computer = self.inputs.code.computer  # type: ignore[union-attr]
+            self.node.computer = self.inputs.code.computer
 
     def _perform_dry_run(self):
         """Perform a dry run.
 
         Instead of performing the normal sequence of steps, just the `presubmit` is called, which will call the method
         `prepare_for_submission` of the plugin to generate the input files based on the inputs. Then the upload action
         is called, but using a normal local transport that will copy the files to a local sandbox folder. The generated
@@ -631,17 +636,15 @@
 
         filepath_sandbox = get_config_option('storage.sandbox') or None
 
         with LocalTransport() as transport:
             with SandboxFolder(filepath_sandbox) as folder:
                 with SandboxFolder(filepath_sandbox) as retrieved_temporary_folder:
                     self.presubmit(folder)
-                    self.node.set_remote_workdir(
-                        self.inputs.remote_folder.get_remote_path()  # type: ignore[union-attr]
-                    )
+                    self.node.set_remote_workdir(self.inputs.remote_folder.get_remote_path())
                     retrieve_calculation(self.node, transport, retrieved_temporary_folder.abspath)
                     self.node.set_state(CalcJobState.PARSING)
                     self.node.base.attributes.set(orm.CalcJobNode.IMMIGRATED_KEY, True)
                     return self.parse(retrieved_temporary_folder.abspath)
 
     def parse(
         self, retrieved_temporary_folder: Optional[str] = None, existing_exit_code: ExitCode | None = None
@@ -812,15 +815,15 @@
         from aiida.common.exceptions import InputValidationError, InvalidOperation, PluginInternalError, ValidationError
         from aiida.common.utils import validate_list_of_string_tuples
         from aiida.orm import AbstractCode, Computer, load_code
         from aiida.schedulers.datastructures import JobTemplate, JobTemplateCodeInfo
 
         inputs = self.node.base.links.get_incoming(link_type=LinkType.INPUT_CALC)
 
-        if not self.inputs.metadata.dry_run and not self.node.is_stored:  # type: ignore[union-attr]
+        if not self.inputs.metadata.dry_run and not self.node.is_stored:
             raise InvalidOperation('calculation node is not stored.')
 
         computer = self.node.computer
         assert computer is not None
         codes = [_ for _ in inputs.all_nodes() if isinstance(_, AbstractCode)]
 
         for code in codes:
@@ -939,16 +942,16 @@
                     error += f'\nThe code `{code}` required `{with_mpi_code}`.'
                 raise RuntimeError(error)
 
             # At this point we know that the three explicit values agree if they are defined, so we simply set the value
             if with_mpi_values_set:
                 with_mpi = with_mpi_values_set.pop()
             else:
-                # Fall back to the default of the ``metadata.options.withmpi`` of the ``Calcjob`` class
-                with_mpi = self.node.get_option('withmpi')
+                # Fall back to the default, which is to not use MPI
+                with_mpi = False
 
             if with_mpi:
                 prepend_cmdline_params = code.get_prepend_cmdline_params(mpi_args, extra_mpirun_params)
             else:
                 prepend_cmdline_params = code.get_prepend_cmdline_params()
 
             cmdline_params = code.get_executable_cmdline_params(code_info.cmdline_params)
@@ -957,15 +960,15 @@
             tmpl_code_info.prepend_cmdline_params = prepend_cmdline_params
             tmpl_code_info.cmdline_params = cmdline_params
             tmpl_code_info.use_double_quotes = [computer.get_use_double_quotes(), code.use_double_quotes]
             tmpl_code_info.wrap_cmdline_params = code.wrap_cmdline_params
             tmpl_code_info.stdin_name = code_info.stdin_name
             tmpl_code_info.stdout_name = code_info.stdout_name
             tmpl_code_info.stderr_name = code_info.stderr_name
-            tmpl_code_info.join_files = code_info.join_files
+            tmpl_code_info.join_files = code_info.join_files or False
 
             tmpl_codes_info.append(tmpl_code_info)
         job_tmpl.codes_info = tmpl_codes_info
 
         # set the codes execution mode, default set to `SERIAL`
         codes_run_mode = CodeRunMode.SERIAL
         if calc_info.codes_run_mode:
```

### Comparing `aiida_core-2.3.1/aiida/engine/processes/calcjobs/importer.py` & `aiida_core-2.4.0/aiida/engine/processes/calcjobs/importer.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/engine/processes/calcjobs/manager.py` & `aiida_core-2.4.0/aiida/engine/processes/calcjobs/manager.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/engine/processes/calcjobs/monitors.py` & `aiida_core-2.4.0/aiida/engine/processes/calcjobs/monitors.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,14 +145,15 @@
 
     The :meth:`~aiida.engine.processes.calcjobs.monitors.CalcJobMonitors.process` method can be called providing an
     instance of a ``CalcJobNode`` and a ``Transport`` and it will iterate over the collection of monitors, executing
     each monitor in order, and stopping on the first to return a ``CalcJobMonitorResult`` to pass it up to its caller.
     """
 
     def __init__(self, monitors: dict[str, Dict]):
+        """Construct a new instance."""
         type_check(monitors, dict)
 
         if any(not isinstance(monitor, Dict) for monitor in monitors.values()):
             raise TypeError('at least one value of `monitors` is not a `Dict` node.')
 
         monitors = {key: CalcJobMonitor(**node.get_dict()) for key, node in monitors.items()}
         self._monitors = collections.OrderedDict(sorted(monitors.items(), key=lambda x: (-x[1].priority, x[0])))
```

### Comparing `aiida_core-2.3.1/aiida/engine/processes/calcjobs/tasks.py` & `aiida_core-2.4.0/aiida/engine/processes/calcjobs/tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         logger.info(f'scheduled request to upload CalcJob<{node.pk}>')
         ignore_exceptions = (plumpy.futures.CancelledError, PreSubmitException, plumpy.process_states.Interruption)
         skip_submit = await exponential_backoff_retry(
             do_upload, initial_interval, max_attempts, logger=node.logger, ignore_exceptions=ignore_exceptions
         )
     except PreSubmitException:
         raise
-    except (plumpy.futures.CancelledError, plumpy.process_states.Interruption):
+    except (plumpy.futures.CancelledError, plumpy.process_states.Interruption):  # pylint: disable=try-except-raise
         raise
     except Exception as exception:
         logger.warning(f'uploading CalcJob<{node.pk}> failed')
         raise TransportTaskException(f'upload_calculation failed {max_attempts} times consecutively') from exception
     else:
         logger.info(f'uploading CalcJob<{node.pk}> successful')
         node.set_state(CalcJobState.SUBMITTING)
```

### Comparing `aiida_core-2.3.1/aiida/engine/processes/control.py` & `aiida_core-2.4.0/aiida/engine/processes/control.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,28 +89,28 @@
     :param processes: List of processes to play.
     :param all_entries: Play all paused processes.
     :param timeout: Raise a ``ProcessTimeoutException`` if the process does not respond within this amount of seconds.
     :param wait: Set to ``True`` to wait for process response, for ``False`` the action is fire-and-forget.
     :raises ``ProcessTimeoutException``: If the processes do not respond within the timeout.
     """
     if not get_daemon_client().is_daemon_running:
-        raise DaemonException('The daemon is not running.')
+        LOGGER.warning('The daemon is not running, so processes submitted to the daemon are not reachable.')
 
     if processes and all_entries:
         raise ValueError('cannot specify processes when `all_entries = True`.')
 
     if not processes and all_entries:
         processes = get_active_processes(paused=True)
 
     if not processes:
         LOGGER.report('no active processes selected.')
         return
 
     controller = get_manager().get_process_controller()
-    _perform_actions(processes, controller.play_process, 'play', 'playing', 'played', timeout, wait)
+    _perform_actions(processes, controller.play_process, 'play', 'playing', timeout, wait)
 
 
 def pause_processes(
     processes: list[ProcessNode] | None = None,
     *,
     message: str = 'Paused through `aiida.engine.processes.control.pause_processes`',
     all_entries: bool = False,
@@ -124,28 +124,28 @@
     :param processes: List of processes to play.
     :param all_entries: Pause all playing processes.
     :param timeout: Raise a ``ProcessTimeoutException`` if the process does not respond within this amount of seconds.
     :param wait: Set to ``True`` to wait for process response, for ``False`` the action is fire-and-forget.
     :raises ``ProcessTimeoutException``: If the processes do not respond within the timeout.
     """
     if not get_daemon_client().is_daemon_running:
-        raise DaemonException('The daemon is not running.')
+        LOGGER.warning('The daemon is not running, so processes submitted to the daemon are not reachable.')
 
     if processes and all_entries:
         raise ValueError('cannot specify processes when `all_entries = True`.')
 
     if not processes and all_entries:
         processes = get_active_processes()
 
     if not processes:
         LOGGER.report('no active processes selected.')
         return
 
     controller = get_manager().get_process_controller()
-    _perform_actions(processes, controller.pause_process, 'pause', 'pausing', 'paused', timeout, wait, msg=message)
+    _perform_actions(processes, controller.pause_process, 'pause', 'pausing', timeout, wait, msg=message)
 
 
 def kill_processes(
     processes: list[ProcessNode] | None = None,
     *,
     message: str = 'Killed through `aiida.engine.processes.control.kill_processes`',
     all_entries: bool = False,
@@ -159,36 +159,35 @@
     :param processes: List of processes to play.
     :param all_entries: Kill all active processes.
     :param timeout: Raise a ``ProcessTimeoutException`` if the process does not respond within this amount of seconds.
     :param wait: Set to ``True`` to wait for process response, for ``False`` the action is fire-and-forget.
     :raises ``ProcessTimeoutException``: If the processes do not respond within the timeout.
     """
     if not get_daemon_client().is_daemon_running:
-        raise DaemonException('The daemon is not running.')
+        LOGGER.warning('The daemon is not running, so processes submitted to the daemon are not reachable.')
 
     if processes and all_entries:
         raise ValueError('cannot specify processes when `all_entries = True`.')
 
     if not processes and all_entries:
         processes = get_active_processes()
 
     if not processes:
         LOGGER.report('no active processes selected.')
         return
 
     controller = get_manager().get_process_controller()
-    _perform_actions(processes, controller.kill_process, 'kill', 'killing', 'killed', timeout, wait, msg=message)
+    _perform_actions(processes, controller.kill_process, 'kill', 'killing', timeout, wait, msg=message)
 
 
 def _perform_actions(
     processes: list[ProcessNode],
     action: t.Callable,
     infinitive: str,
     present: str,
-    past: str,
     timeout: float = None,
     wait: bool = False,
     **kwargs: t.Any
 ) -> None:
     """Perform an action on a list of processes.
 
     :param processes: The list of processes to perform the action on.
@@ -212,43 +211,41 @@
         try:
             future = action(process.pk, **kwargs)
         except communications.UnroutableError:
             LOGGER.error(f'Process<{process.pk}> is unreachable.')
         else:
             futures[future] = process
 
-    _resolve_futures(futures, infinitive, present, past, wait, timeout)
+    _resolve_futures(futures, infinitive, present, wait, timeout)
 
 
 def _resolve_futures(
     futures: dict[concurrent.futures.Future, ProcessNode],
     infinitive: str,
     present: str,
-    past: str,
     wait: bool = False,
     timeout: float = None
 ) -> None:
     """Process a mapping of futures representing an action on an active process.
 
     This function will echo the correct information strings based on the outcomes of the futures and the given verb
     conjugations. You can optionally wait for any pending actions to be completed before the functions returns and use a
     timeout to put a maximum wait time on the actions.
 
     :param futures: The map of action futures and the corresponding processes.
     :param infinitive: The infinitive form of the action verb.
     :param present: The present tense form of the action verb.
-    :param past: The past tense form of the action verb.
     :param wait: Set to ``True`` to wait for process response, for ``False`` the action is fire-and-forget.
     :param timeout: Raise a ``ProcessTimeoutException`` if the process does not respond within this amount of seconds.
     """
     scheduled = {}
 
     def handle_result(result):
         if result is True:
-            LOGGER.report(f'{past} Process<{process.pk}>')
+            LOGGER.report(f'request to {infinitive} Process<{process.pk}> sent')
         elif result is False:
             LOGGER.error(f'problem {present} Process<{process.pk}>')
         elif isinstance(result, kiwipy.Future):
             LOGGER.report(f'scheduled {infinitive} Process<{process.pk}>')
             scheduled[result] = process
         else:
             LOGGER.error(f'got unexpected response when {present} Process<{process.pk}>: {result}')
```

### Comparing `aiida_core-2.3.1/aiida/engine/processes/exit_code.py` & `aiida_core-2.4.0/aiida/engine/processes/exit_code.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/engine/processes/functions.py` & `aiida_core-2.4.0/aiida/engine/processes/functions.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,16 +9,18 @@
 ###########################################################################
 """Class and decorators to generate processes out of simple python functions."""
 from __future__ import annotations
 
 import collections
 import functools
 import inspect
+import itertools
 import logging
 import signal
+import sys
 import types
 import typing as t
 from typing import TYPE_CHECKING
 
 import docstring_parser
 
 from aiida.common.lang import override
@@ -55,15 +57,38 @@
 if TYPE_CHECKING:
     from .exit_code import ExitCode
 
 __all__ = ('calcfunction', 'workfunction', 'FunctionProcess')
 
 LOGGER = logging.getLogger(__name__)
 
-FunctionType = t.TypeVar('FunctionType', bound=t.Callable[..., t.Any])
+FunctionType = t.TypeVar('FunctionType', bound=t.Callable[..., t.Any])  # pylint: disable=invalid-name
+
+
+def get_stack_size(size: int = 2) -> int:  # type: ignore[return]
+    """Return the stack size for the caller's frame.
+
+    This solution is taken from https://stackoverflow.com/questions/34115298/ as a more performant alternative to the
+    naive ``len(inspect.stack())` solution. This implementation is about three orders of magnitude faster compared to
+    the naive solution and it scales especially well for larger stacks, which will be usually the case for the usage
+    of ``aiida-core``. However, it does use the internal ``_getframe`` of the ``sys`` standard library. It this ever
+    were to stop working, simply switch to using ``len(inspect.stack())``.
+
+    :param size: Hint for the expected stack size.
+    :returns: The stack size for caller's frame.
+    """
+    frame = sys._getframe(size)  # pylint: disable=protected-access
+    try:
+        for size in itertools.count(size, 8):  # pylint: disable=redefined-argument-from-local
+            frame = frame.f_back.f_back.f_back.f_back.f_back.f_back.f_back.f_back  # type: ignore[assignment,union-attr]
+    except AttributeError:
+        while frame:
+            frame = frame.f_back  # type: ignore[assignment]
+            size += 1
+        return size - 1
 
 
 def calcfunction(function: FunctionType) -> FunctionType:
     """
     A decorator to turn a standard python function into a calcfunction.
     Example usage:
 
@@ -135,16 +160,29 @@
         def run_get_node(*args, **kwargs) -> tuple[dict[str, t.Any] | None, 'ProcessNode']:
             """
             Run the FunctionProcess with the supplied inputs in a local runner.
 
             :param args: input arguments to construct the FunctionProcess
             :param kwargs: input keyword arguments to construct the FunctionProcess
             :return: tuple of the outputs of the process and the process node
-
             """
+            frame_delta = 1000
+            frame_count = get_stack_size()
+            stack_limit = sys.getrecursionlimit()
+            LOGGER.info('Executing process function, current stack status: %d frames of %d', frame_count, stack_limit)
+
+            # If the current frame count is more than 80% of the stack limit, or comes within 200 frames, increase the
+            # stack limit by ``frame_delta``.
+            if frame_count > min(0.8 * stack_limit, stack_limit - 200):
+                LOGGER.warning(
+                    'Current stack contains %d frames which is close to the limit of %d. Increasing the limit by %d',
+                    frame_count, stack_limit, frame_delta
+                )
+                sys.setrecursionlimit(stack_limit + frame_delta)
+
             manager = get_manager()
             runner = manager.get_runner()
             inputs = process_class.create_inputs(*args, **kwargs)
 
             # Remove all the known inputs from the kwargs
             for port in process_class.spec().inputs:
                 kwargs.pop(port, None)
@@ -356,15 +394,15 @@
                 # If a default is defined and it is not a ``Data`` instance it should be serialized, but this should be
                 # done lazily using a lambda, just as any port defaults should not define node instances directly as is
                 # also checked by the ``spec.input`` call.
                 if (
                     default is not None and default != UNSPECIFIED and not isinstance(default, Data) and
                     not callable(default)
                 ):
-                    indirect_default = lambda value=default: to_aiida_type(value)
+                    indirect_default = lambda value=default: to_aiida_type(value)  # pylint: disable=unnecessary-lambda-assignment
                 else:
                     indirect_default = default
 
                 spec.input(
                     parameter.name,
                     valid_type=valid_type,
                     default=indirect_default,
```

### Comparing `aiida_core-2.3.1/aiida/engine/processes/futures.py` & `aiida_core-2.4.0/aiida/engine/processes/futures.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/engine/processes/ports.py` & `aiida_core-2.4.0/aiida/engine/processes/ports.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/engine/processes/process.py` & `aiida_core-2.4.0/aiida/engine/processes/process.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 from aio_pika.exceptions import ConnectionClosed
 from kiwipy.communications import UnroutableError
 import plumpy.exceptions
 import plumpy.futures
 import plumpy.persistence
 from plumpy.process_states import Finished, ProcessState
 import plumpy.processes
+from plumpy.utils import AttributesFrozendict
 
 from aiida import orm
 from aiida.common import exceptions
 from aiida.common.extendeddicts import AttributeDict
 from aiida.common.lang import classproperty, override
 from aiida.common.links import LinkType
 from aiida.common.log import LOG_LEVEL_REPORT
@@ -230,14 +231,23 @@
         """Return the UUID of the process which corresponds to the UUID of its associated `ProcessNode`.
 
         :return: the UUID associated to this process instance
         """
         return self.node.uuid
 
     @property
+    def inputs(self) -> AttributesFrozendict:
+        """Return the inputs attribute dictionary or an empty one.
+
+        This overrides the property of the base class because that can also return ``None``. This override ensures
+        calling functions that they will always get an instance of ``AttributesFrozenDict``.
+        """
+        return super().inputs or AttributesFrozendict()
+
+    @property
     def metadata(self) -> AttributeDict:
         """Return the metadata that were specified when this process instance was launched.
 
         :return: metadata dictionary
 
         """
         try:
@@ -621,25 +631,25 @@
 
         if self.node.pk is not None:
             return self.node.pk
 
         return UUID(self.node.uuid)
 
     @override
-    def encode_input_args(self, inputs: Dict[str, Any]) -> str:  # pylint: disable=no-self-use
+    def encode_input_args(self, inputs: Dict[str, Any]) -> str:
         """
         Encode input arguments such that they may be saved in a Bundle
 
         :param inputs: A mapping of the inputs as passed to the process
         :return: The encoded (serialized) inputs
         """
         return serialize.serialize(inputs)
 
     @override
-    def decode_input_args(self, encoded: str) -> Dict[str, Any]:  # pylint: disable=no-self-use
+    def decode_input_args(self, encoded: str) -> Dict[str, Any]:
         """
         Decode saved input arguments as they came from the saved instance state Bundle
 
         :param encoded: encoded (serialized) inputs
         :return: The decoded input args
         """
         return serialize.deserialize_unsafe(encoded)
@@ -795,16 +805,15 @@
             if not port.is_metadata:
                 return None
 
             try:
                 clean_value(port_value)
             except exceptions.ValidationError:
                 return None
-            else:
-                return port_value
+            return port_value
 
         result = {}
 
         for key, value in port_value.items():
             if key not in port:
                 continue
 
@@ -949,15 +958,15 @@
             # The sub_namespace None indicates the base level sub_namespace
             if sub_namespace is None:
                 inputs = self.inputs
                 port_namespace = self.spec().inputs
             else:
                 inputs = self.inputs
                 for part in sub_namespace.split('.'):
-                    inputs = inputs[part]  # type: ignore[index]
+                    inputs = inputs[part]
                 try:
                     port_namespace = self.spec().inputs.get_port(sub_namespace)  # type: ignore[assignment]
                 except KeyError:
                     raise ValueError(f'this process does not contain the "{sub_namespace}" input namespace')
 
             # Get the list of ports that were exposed for the given Process class in the current sub_namespace
             exposed_inputs_list = self.spec()._exposed_inputs[sub_namespace][process_class]  # pylint: disable=protected-access
```

### Comparing `aiida_core-2.3.1/aiida/engine/processes/process_spec.py` & `aiida_core-2.4.0/aiida/engine/processes/process_spec.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/engine/processes/utils.py` & `aiida_core-2.4.0/aiida/engine/processes/utils.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/engine/processes/workchains/__init__.py` & `aiida_core-2.4.0/aiida/engine/processes/workchains/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/engine/processes/workchains/awaitable.py` & `aiida_core-2.4.0/aiida/engine/processes/workchains/awaitable.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/engine/processes/workchains/context.py` & `aiida_core-2.4.0/aiida/engine/processes/workchains/context.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/engine/processes/workchains/restart.py` & `aiida_core-2.4.0/aiida/engine/processes/workchains/restart.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,15 +174,15 @@
 
     def should_run_process(self) -> bool:
         """Return whether a new process should be run.
 
         This is the case as long as the last process has not finished successfully and the maximum number of restarts
         has not yet been exceeded.
         """
-        max_iterations = self.inputs.max_iterations.value  # type: ignore[union-attr]
+        max_iterations = self.inputs.max_iterations.value
         return not self.ctx.is_finished and self.ctx.iteration < max_iterations
 
     def run_process(self) -> ToContext:
         """Run the next process, taking the input dictionary from the context at `self.ctx.inputs`."""
         self.ctx.iteration += 1
 
         try:
@@ -307,15 +307,15 @@
     def results(self) -> Optional['ExitCode']:
         """Attach the outputs specified in the output specification from the last completed process."""
         node = self.ctx.children[self.ctx.iteration - 1]
 
         # We check the `is_finished` attribute of the work chain and not the successfulness of the last process
         # because the error handlers in the last iteration can have qualified a "failed" process as satisfactory
         # for the outcome of the work chain and so have marked it as `is_finished=True`.
-        max_iterations = self.inputs.max_iterations.value  # type: ignore[union-attr]
+        max_iterations = self.inputs.max_iterations.value
         if not self.ctx.is_finished and self.ctx.iteration >= max_iterations:
             self.report(
                 f'reached the maximum number of iterations {max_iterations}: '
                 f'last ran {self.ctx.process_name}<{node.pk}>'
             )
             return self.exit_codes.ERROR_MAXIMUM_ITERATIONS_EXCEEDED  # pylint: disable=no-member
 
@@ -388,15 +388,15 @@
 
         return handlers
 
     def on_terminated(self):
         """Clean the working directories of all child calculation jobs if `clean_workdir=True` in the inputs."""
         super().on_terminated()
 
-        if self.inputs.clean_workdir.value is False:  # type: ignore[union-attr]
+        if self.inputs.clean_workdir.value is False:
             self.report('remote folders will not be cleaned')
             return
 
         cleaned_calcs = []
 
         for called_descendant in self.node.called_descendants:
             if isinstance(called_descendant, orm.CalcJobNode):
```

### Comparing `aiida_core-2.3.1/aiida/engine/processes/workchains/utils.py` & `aiida_core-2.4.0/aiida/engine/processes/workchains/utils.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/engine/processes/workchains/workchain.py` & `aiida_core-2.4.0/aiida/engine/processes/workchains/workchain.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,47 +55,47 @@
                 "This method cannot be overridden by a subclass."
 
     If a subclass is imported that overrides the subclass, a ``RuntimeError`` is raised.
     """
 
     __SENTINEL = object()
 
-    def __new__(cls, name, bases, namespace, **kwargs):
+    def __new__(mcs, name, bases, namespace, **kwargs):
         """Collect all methods that were marked as protected and raise if the subclass defines it.
 
         :raises RuntimeError: If the new class defines (i.e. overrides) a method that was decorated with ``final``.
         """
         private = {
-            key for base in bases for key, value in vars(base).items() if callable(value) and cls.__is_final(value)
+            key for base in bases for key, value in vars(base).items() if callable(value) and mcs.__is_final(value)
         }
         for key in namespace:
             if key in private:
                 raise RuntimeError(f'the method `{key}` is protected cannot be overridden.')
-        return super().__new__(cls, name, bases, namespace, **kwargs)
+        return super().__new__(mcs, name, bases, namespace, **kwargs)
 
     @classmethod
-    def __is_final(cls, method) -> bool:
+    def __is_final(mcs, method) -> bool:  # pylint: disable=unused-private-member
         """Return whether the method has been decorated by the ``final`` classmethod.
 
         :return: Boolean, ``True`` if the method is marked as final, ``False`` otherwise.
         """
         try:
-            return method.__final is cls.__SENTINEL  # pylint: disable=protected-access
+            return method.__final is mcs.__SENTINEL  # pylint: disable=protected-access
         except AttributeError:
             return False
 
     @classmethod
-    def final(cls, method: t.Any):
+    def final(mcs, method: t.Any):
         """Decorate a method with this method to protect it from being overridden.
 
         Adds the ``__SENTINEL`` object as the ``__final`` private attribute to the given ``method`` and wraps it in
         the ``typing.final`` decorator. The latter indicates to typing systems that it cannot be overridden in
         subclasses.
         """
-        method.__final = cls.__SENTINEL  # pylint: disable=protected-access,unused-private-member
+        method.__final = mcs.__SENTINEL  # pylint: disable=protected-access,unused-private-member
         return t.final(method)
 
 
 @auto_persist('_awaitables')
 class WorkChain(Process, metaclass=Protect):
     """The `WorkChain` class is the principle component to implement workflows in AiiDA."""
```

### Comparing `aiida_core-2.3.1/aiida/engine/runners.py` & `aiida_core-2.4.0/aiida/engine/runners.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/engine/transports.py` & `aiida_core-2.4.0/aiida/engine/transports.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,17 +97,15 @@
                         transport_request.future.set_result(transport)
 
             # Save the handle so that we can cancel the callback if the user no longer wants it
             # Note: Don't pass the Process context, since (a) it is not needed by `do_open` and (b) the transport is
             # passed around to many places, including outside aiida-core (e.g. paramiko). Anyone keeping a reference
             # to this handle would otherwise keep the Process context (and thus the process itself) in memory.
             # See https://github.com/aiidateam/aiida-core/issues/4698
-            open_callback_handle = self._loop.call_later(
-                safe_open_interval, do_open, context=contextvars.Context()
-            )  #  type: ignore[call-arg]
+            open_callback_handle = self._loop.call_later(safe_open_interval, do_open, context=contextvars.Context())
 
         try:
             transport_request.count += 1
             yield transport_request.future
         except asyncio.CancelledError:  # pylint: disable=try-except-raise
             # note this is only required in python<=3.7,
             # where asyncio.CancelledError inherits from Exception
```

### Comparing `aiida_core-2.3.1/aiida/engine/utils.py` & `aiida_core-2.4.0/aiida/engine/utils.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/manage/__init__.py` & `aiida_core-2.4.0/aiida/manage/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/manage/caching.py` & `aiida_core-2.4.0/aiida/manage/caching.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/manage/configuration/__init__.py` & `aiida_core-2.4.0/aiida/manage/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/manage/configuration/config.py` & `aiida_core-2.4.0/aiida/manage/configuration/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,21 +6,15 @@
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-core #
 # For further information on the license, see the LICENSE.txt file        #
 # For further information please visit http://www.aiida.net               #
 ###########################################################################
 """Module that defines the configuration file of an AiiDA instance and functions to create and load it."""
 import codecs
 from functools import lru_cache
-
-try:
-    # Python <= 3.8
-    from importlib_resources import files
-except ImportError:
-    from importlib.resources import files
-
+from importlib.resources import files
 import json
 import os
 import shutil
 import tempfile
 from typing import Any, Dict, Optional, Sequence, Tuple
 
 import jsonschema
```

### Comparing `aiida_core-2.3.1/aiida/manage/configuration/migrations/__init__.py` & `aiida_core-2.4.0/aiida/manage/configuration/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/manage/configuration/migrations/migrations.py` & `aiida_core-2.4.0/aiida/manage/configuration/migrations/migrations.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/manage/configuration/options.py` & `aiida_core-2.4.0/aiida/manage/configuration/options.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/manage/configuration/profile.py` & `aiida_core-2.4.0/aiida/manage/configuration/profile.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/manage/configuration/schema/__init__.py` & `aiida_core-2.4.0/aiida/manage/configuration/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/manage/configuration/schema/config-v5.schema.json` & `aiida_core-2.4.0/aiida/manage/configuration/schema/config-v5.schema.json`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/manage/configuration/schema/config-v6.schema.json` & `aiida_core-2.4.0/aiida/manage/configuration/schema/config-v6.schema.json`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/manage/configuration/schema/config-v7.schema.json` & `aiida_core-2.4.0/aiida/manage/configuration/schema/config-v7.schema.json`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/manage/configuration/schema/config-v8.schema.json` & `aiida_core-2.4.0/aiida/manage/configuration/schema/config-v8.schema.json`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/manage/configuration/schema/config-v9.schema.json` & `aiida_core-2.4.0/aiida/manage/configuration/schema/config-v9.schema.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998372395833334%*

 * *Differences: {"'definitions'": "{'options': {'properties': {'daemon.recursion_limit': OrderedDict([('type', "*

 * *                  "'integer'), ('default', 3000), ('maximum', 100000), ('minimum', 1), "*

 * *                  "('description', 'Maximum recursion depth for the daemon workers')])}}}"}*

```diff
@@ -46,14 +46,21 @@
                 },
                 "daemon.default_workers": {
                     "default": 1,
                     "description": "Default number of workers to be launched by `verdi daemon start`",
                     "minimum": 1,
                     "type": "integer"
                 },
+                "daemon.recursion_limit": {
+                    "default": 3000,
+                    "description": "Maximum recursion depth for the daemon workers",
+                    "maximum": 100000,
+                    "minimum": 1,
+                    "type": "integer"
+                },
                 "daemon.timeout": {
                     "default": 2,
                     "description": "Used to set default timeout in the :class:`aiida.engine.daemon.client.DaemonClient` for calls to the daemon",
                     "minimum": 0,
                     "type": "integer"
                 },
                 "daemon.worker_process_slots": {
```

### Comparing `aiida_core-2.3.1/aiida/manage/configuration/settings.py` & `aiida_core-2.4.0/aiida/manage/configuration/settings.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/manage/external/__init__.py` & `aiida_core-2.4.0/aiida/manage/external/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/manage/external/postgres.py` & `aiida_core-2.4.0/aiida/manage/external/postgres.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/manage/external/rmq/__init__.py` & `aiida_core-2.4.0/aiida/manage/external/rmq/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/manage/external/rmq/client.py` & `aiida_core-2.4.0/aiida/manage/external/rmq/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         :param method: The HTTP method.
         :param params: Query parameters to add to the URL.
         :returns: The response of the request.
         :raises `ManagementApiConnectionError`: If connection to the API cannot be made.
         """
         url = self.format_url(url, url_params)
         try:
-            return requests.request(method, url, auth=self._authentication, params=params or {})
+            return requests.request(method, url, auth=self._authentication, params=params or {}, timeout=5)
         except requests.exceptions.ConnectionError as exception:
             raise ManagementApiConnectionError(
                 'Could not connect to the management API. Make sure RabbitMQ is running and the management plugin is '
                 'installed using `sudo rabbitmq-plugins enable rabbitmq_management`.'
             ) from exception
 
     @property
@@ -86,9 +86,8 @@
 
         :returns: ``True`` if the server can be reached, ``False`` otherwise.
         """
         try:
             self.request('cluster-name')
         except ManagementApiConnectionError:
             return False
-        else:
-            return True
+        return True
```

### Comparing `aiida_core-2.3.1/aiida/manage/external/rmq/launcher.py` & `aiida_core-2.4.0/aiida/manage/external/rmq/launcher.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/manage/external/rmq/utils.py` & `aiida_core-2.4.0/aiida/manage/external/rmq/utils.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/manage/manager.py` & `aiida_core-2.4.0/aiida/manage/manager.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/manage/profile_access.py` & `aiida_core-2.4.0/aiida/manage/profile_access.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/manage/tests/__init__.py` & `aiida_core-2.4.0/aiida/manage/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/manage/tests/main.py` & `aiida_core-2.4.0/aiida/manage/tests/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,15 @@
         manager.reset_runner()
 
         self.ensure_default_user()
 
     def has_profile_open(self):
         return self._profile is not None
 
-    def destroy_all(self):  # pylint: disable=no-self-use
+    def destroy_all(self):
         manager = get_manager()
         manager.reset_profile()
 
 
 class TemporaryProfileManager(ProfileManager):
     """
     Manage the life cycle of a completely separated and temporary AiiDA environment.
```

### Comparing `aiida_core-2.3.1/aiida/manage/tests/pytest_fixtures.py` & `aiida_core-2.4.0/aiida/manage/tests/pytest_fixtures.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,27 +91,29 @@
     postgres_config = {
         'database_engine': 'postgresql_psycopg2',
         'database_name': database_name or str(uuid.uuid4()),
         'database_username': database_username or 'guest',
         'database_password': database_password or 'guest',
     }
 
+    cluster = None
     try:
         cluster = PGTest()
 
         postgres = Postgres(interactive=False, quiet=True, dbinfo=cluster.dsn)
         postgres.create_dbuser(postgres_config['database_username'], postgres_config['database_password'], 'CREATEDB')
         postgres.create_db(postgres_config['database_username'], postgres_config['database_name'])
 
         postgres_config['database_hostname'] = postgres.host_for_psycopg2
         postgres_config['database_port'] = postgres.port_for_psycopg2
 
         yield postgres_config
     finally:
-        cluster.close()
+        if cluster is not None:
+            cluster.close()
 
 
 @pytest.fixture(scope='session')
 def aiida_test_profile() -> str | None:
     """Return the name of the AiiDA test profile if defined.
 
     The name is taken from the ``AIIDA_TEST_PROFILE`` environment variable.
@@ -128,15 +130,15 @@
     :returns: The global manager instance.
     """
     return get_manager()
 
 
 @pytest.fixture(scope='session')
 def aiida_instance(
-    tmp_path_factory: pytest.TempPathFactory,
+    tmp_path_factory: pytest.tmpdir.TempPathFactory,
     aiida_manager: Manager,
     aiida_test_profile: str | None,
 ) -> t.Generator[Config, None, None]:
     """Return the :class:`~aiida.manage.configuration.config.Config` instance that is used for the test session.
 
     If an existing test profile is defined through the ``aiida_test_profile`` fixture, the configuration of the actual
     AiiDA instance is loaded and returned. If no test profile is defined, a completely independent and temporary AiiDA
@@ -181,15 +183,15 @@
                 configuration.CONFIG = current_config
                 if current_profile:
                     aiida_manager.load_profile(current_profile.name, allow_switch=True)
 
 
 @pytest.fixture(scope='session')
 def config_psql_dos(
-    tmp_path_factory: pytest.TempPathFactory,
+    tmp_path_factory: pytest.tmpdir.TempPathFactory,
     postgres_cluster: dict[str, str],
 ) -> t.Callable[[dict[str, t.Any] | None], dict[str, t.Any]]:
     """Return a profile configuration for the :class:`~aiida.storage.psql_dos.backend.PsqlDosBackend`."""
 
     def factory(custom_configuration: dict[str, t.Any] | None = None) -> dict[str, t.Any]:
         """Return a profile configuration for the :class:`~aiida.storage.psql_dos.backend.PsqlDosBackend`.
 
@@ -658,15 +660,21 @@
     try:
         yield daemon_client
     finally:
         try:
             daemon_client.stop_daemon(wait=True)
         except DaemonNotRunningException:
             pass
-        assert not daemon_client.is_daemon_running
+        # Give an additional grace period by manually waiting for the daemon to be stopped. In certain unit test
+        # scenarios, the built in wait time in ``daemon_client.stop_daemon`` is not sufficient and even though the
+        # daemon is stopped, ``daemon_client.is_daemon_running`` will return false for a little bit longer.
+        daemon_client._await_condition(  # pylint: disable=protected-access
+            lambda: not daemon_client.is_daemon_running,
+            DaemonTimeoutException('The daemon failed to stop.'),
+        )
 
 
 @pytest.fixture()
 def started_daemon_client(daemon_client):
     """Ensure that the daemon is running for the test profile and return the associated client."""
     if not daemon_client.is_daemon_running:
         daemon_client.start_daemon()
```

### Comparing `aiida_core-2.3.1/aiida/orm/__init__.py` & `aiida_core-2.4.0/aiida/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/authinfos.py` & `aiida_core-2.4.0/aiida/orm/authinfos.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/autogroup.py` & `aiida_core-2.4.0/aiida/orm/autogroup.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/comments.py` & `aiida_core-2.4.0/aiida/orm/comments.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/computers.py` & `aiida_core-2.4.0/aiida/orm/computers.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/convert.py` & `aiida_core-2.4.0/aiida/orm/convert.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/entities.py` & `aiida_core-2.4.0/aiida/orm/entities.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,41 +161,43 @@
 
 class Entity(abc.ABC, Generic[BackendEntityType, CollectionType]):
     """An AiiDA entity"""
 
     _CLS_COLLECTION: Type[CollectionType] = Collection  # type: ignore
 
     @classproperty
-    def objects(cls: EntityType) -> CollectionType:  # pylint: disable=no-self-argument,no-self-use
+    def objects(cls: EntityType) -> CollectionType:  # pylint: disable=no-self-argument
         """Get a collection for objects of this type, with the default backend.
 
         .. deprecated:: This will be removed in v3, use ``collection`` instead.
 
         :return: an object that can be used to access entities of this type
         """
-        warn_deprecation('This property is deprecated, use `.collection` instead.', version=3, stacklevel=2)
+        warn_deprecation('`objects` property is deprecated, use `collection` instead.', version=3, stacklevel=4)
         return cls.collection
 
     @classproperty
-    def collection(cls) -> CollectionType:  # pylint: disable=no-self-argument,no-self-use
+    def collection(cls) -> CollectionType:  # pylint: disable=no-self-argument
         """Get a collection for objects of this type, with the default backend.
 
         :return: an object that can be used to access entities of this type
         """
         return cls._CLS_COLLECTION.get_cached(cls, get_manager().get_profile_storage())
 
     @classmethod
     def get(cls, **kwargs):
         """Get an entity of the collection matching the given filters.
 
         .. deprecated: Will be removed in v3, use `Entity.collection.get` instead.
 
         """
         warn_deprecation(
-            f'This method is deprecated, use `{cls.__name__}.collection.get` instead.', version=3, stacklevel=2
+            f'`{cls.__name__}.get` method is deprecated, use `{cls.__name__}.collection.get` instead.',
+            version=3,
+            stacklevel=2
         )
         return cls.collection.get(**kwargs)  # pylint: disable=no-member
 
     def __init__(self, backend_entity: BackendEntityType) -> None:
         """
         :param backend_entity: the backend model supporting this entity
         """
@@ -219,15 +221,15 @@
 
         This identifier is guaranteed to be unique amongst entities of the same type for a single backend instance.
 
         .. deprecated: Will be removed in v3, use `pk` instead.
 
         :return: the entity's id
         """
-        warn_deprecation('This method is deprecated, use `pk` instead.', version=3, stacklevel=2)
+        warn_deprecation('`id` property is deprecated, use `pk` instead.', version=3, stacklevel=2)
         return self._backend_entity.id
 
     @property
     def pk(self) -> int:
         """Return the primary key for this entity.
 
         This identifier is guaranteed to be unique amongst entities of the same type for a single backend instance.
```

### Comparing `aiida_core-2.3.1/aiida/orm/extras.py` & `aiida_core-2.4.0/aiida/orm/extras.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/groups.py` & `aiida_core-2.4.0/aiida/orm/groups.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,18 +50,18 @@
 
     return group_class
 
 
 class GroupMeta(ABCMeta):
     """Meta class for `aiida.orm.groups.Group` to automatically set the `type_string` attribute."""
 
-    def __new__(cls, name, bases, namespace, **kwargs):
+    def __new__(mcs, name, bases, namespace, **kwargs):
         from aiida.plugins.entry_point import get_entry_point_from_class
 
-        newcls = ABCMeta.__new__(cls, name, bases, namespace, **kwargs)  # pylint: disable=too-many-function-args
+        newcls = ABCMeta.__new__(mcs, name, bases, namespace, **kwargs)  # pylint: disable=too-many-function-args
 
         mod = namespace['__module__']
         entry_point_group, entry_point = get_entry_point_from_class(mod, name)
 
         if entry_point_group is None or entry_point_group != 'aiida.groups':
             newcls._type_string = None  # type: ignore[attr-defined]
             message = f'no registered entry point for `{mod}:{name}` so its instances will not be storable.'
@@ -188,15 +188,14 @@
 
     @classproperty
     def entry_point(cls) -> Optional['EntryPoint']:
         """Return the entry point associated this group type.
 
         :return: the associated entry point or ``None`` if it isn't known.
         """
-        # pylint: disable=no-self-use
         from aiida.plugins.entry_point import get_entry_point_from_class
         return get_entry_point_from_class(cls.__module__, cls.__name__)[1]
 
     @property
     def uuid(self) -> str:
         """Return the UUID for this group.
 
@@ -286,16 +285,15 @@
 
         :return: True if it contains no nodes, False otherwise
         """
         try:
             self.nodes[0]
         except IndexError:
             return True
-        else:
-            return False
+        return False
 
     def clear(self) -> None:
         """Remove all the nodes from this group."""
         return self._backend_entity.clear()
 
     def add_nodes(self, nodes: Union['Node', Sequence['Node']]) -> None:
         """Add a node or a set of nodes to the group.
```

### Comparing `aiida_core-2.3.1/aiida/orm/implementation/__init__.py` & `aiida_core-2.4.0/aiida/orm/implementation/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/implementation/authinfos.py` & `aiida_core-2.4.0/aiida/orm/implementation/authinfos.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/implementation/comments.py` & `aiida_core-2.4.0/aiida/orm/implementation/comments.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/implementation/computers.py` & `aiida_core-2.4.0/aiida/orm/implementation/computers.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/implementation/entities.py` & `aiida_core-2.4.0/aiida/orm/implementation/entities.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/implementation/groups.py` & `aiida_core-2.4.0/aiida/orm/implementation/groups.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,27 +21,23 @@
 
 
 class NodeIterator(Protocol):
     """Protocol for iterating over nodes in a group"""
 
     def __iter__(self) -> 'NodeIterator':  # pylint: disable=non-iterator-returned
         """Return an iterator over the nodes in the group."""
-        ...
 
     def __next__(self) -> BackendNode:
         """Return the next node in the group."""
-        ...
 
     def __getitem__(self, value: Union[int, slice]) -> Union[BackendNode, List[BackendNode]]:
         """Index node(s) from the group."""
-        ...
 
     def __len__(self) -> int:  # pylint: disable=invalid-length-returned
         """Return the number of nodes in the group."""
-        ...
 
 
 class BackendGroup(BackendEntity, BackendEntityExtrasMixin):
     """Backend implementation for the `Group` ORM class.
 
     A group is a collection of nodes.
     """
```

### Comparing `aiida_core-2.3.1/aiida/orm/implementation/logs.py` & `aiida_core-2.4.0/aiida/orm/implementation/logs.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/implementation/nodes.py` & `aiida_core-2.4.0/aiida/orm/implementation/nodes.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/implementation/querybuilder.py` & `aiida_core-2.4.0/aiida/orm/implementation/querybuilder.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/implementation/storage_backend.py` & `aiida_core-2.4.0/aiida/orm/implementation/storage_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         BackendUserCollection,
     )
     from aiida.orm.users import User
     from aiida.repository.backend.abstract import AbstractRepositoryBackend
 
 __all__ = ('StorageBackend',)
 
-TransactionType = TypeVar('TransactionType')
+TransactionType = TypeVar('TransactionType')  # pylint: disable=invalid-name
 
 
 class StorageBackend(abc.ABC):  # pylint: disable=too-many-public-methods
     """Abstraction for a backend to read/write persistent data for a profile's provenance graph.
 
     AiiDA splits data storage into two sources:
```

### Comparing `aiida_core-2.3.1/aiida/orm/implementation/users.py` & `aiida_core-2.4.0/aiida/orm/implementation/users.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/implementation/utils.py` & `aiida_core-2.4.0/aiida/orm/implementation/utils.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/logs.py` & `aiida_core-2.4.0/aiida/orm/logs.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         :param order_by: a list of (key, direction) pairs specifying the sort order
 
         :return: the list of log entries
         """
         from . import nodes
 
         if not isinstance(entity, nodes.Node):
-            raise Exception('Only node logs are stored')
+            raise Exception('Only node logs are stored')  # pylint: disable=broad-exception-raised
 
         return self.find({'dbnode_id': entity.pk}, order_by=order_by)
 
     def delete(self, pk: int) -> None:
         """Remove a Log entry from the collection with the given id
 
         :param pk: id of the Log to delete
```

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/__init__.py` & `aiida_core-2.4.0/aiida/orm/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/attributes.py` & `aiida_core-2.4.0/aiida/orm/nodes/attributes.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/caching.py` & `aiida_core-2.4.0/aiida/orm/nodes/caching.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/comments.py` & `aiida_core-2.4.0/aiida/orm/nodes/comments.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,13 +52,13 @@
         :param content: the new comment content
         :raise aiida.common.NotExistent: if the comment with the given id does not exist
         :raise aiida.common.MultipleObjectsError: if the id cannot be uniquely resolved to a comment
         """
         comment = Comment.collection(self._node.backend).get(dbnode_id=self._node.pk, id=identifier)
         comment.set_content(content)
 
-    def remove(self, identifier: int) -> None:  # pylint: disable=no-self-use
+    def remove(self, identifier: int) -> None:
         """Delete an existing comment.
 
         :param identifier: the comment pk
         """
         Comment.collection(self._node.backend).delete(identifier)
```

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/data/__init__.py` & `aiida_core-2.4.0/aiida/orm/nodes/data/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/data/array/__init__.py` & `aiida_core-2.4.0/aiida/orm/nodes/data/array/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/data/array/array.py` & `aiida_core-2.4.0/aiida/orm/nodes/data/array/array.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/data/array/bands.py` & `aiida_core-2.4.0/aiida/orm/nodes/data/array/bands.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
                         list(zip(*j)) for j in [
                             sorted(zip(i[0].tolist(), i[1].tolist()), key=lambda x: x[0])
                             for i in zip(bands, occupations)
                         ]
                     ]
                 )
             ]
-            number_electrons = int(round(sum([sum(i) for i in occupations]) / num_kpoints))
+            number_electrons = int(round(sum(sum(i) for i in occupations) / num_kpoints))
 
             homo_indexes = [numpy.where(numpy.array([nint(_) for _ in x]) > 0)[0][-1] for x in occupations]
             if len(set(homo_indexes)) > 1:  # there must be intersections of valence and conduction bands
                 return False, None
 
             homo = [_[0][_[1]] for _ in zip(bands, homo_indexes)]
             try:
@@ -203,20 +203,20 @@
 
         # case of semimetals, fermi energy at the crossing of two bands
         # this will only work if the dirac point is computed!
         if (any(i[0] == fermi_energy for i in max_mins) and any(i[1] == fermi_energy for i in max_mins)):
             return False, 0.
 
         # insulating case, take the max of the band maxima below the fermi energy
-        homo = max([i[0] for i in max_mins if i[0] < fermi_energy])
+        homo = max(i[0] for i in max_mins if i[0] < fermi_energy)
         # take the min of the band minima above the fermi energy
-        lumo = min([i[1] for i in max_mins if i[1] > fermi_energy])
+        lumo = min(i[1] for i in max_mins if i[1] > fermi_energy)
         gap = lumo - homo
         if gap <= 0.:
-            raise Exception('Something wrong has been implemented. Revise the code!')
+            raise RuntimeError('Something wrong has been implemented. Revise the code!')
         return True, gap
 
 
 class BandsData(KpointsData):
     """
     Class to handle bands data
     """
```

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/data/array/kpoints.py` & `aiida_core-2.4.0/aiida/orm/nodes/data/array/kpoints.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/data/array/projection.py` & `aiida_core-2.4.0/aiida/orm/nodes/data/array/projection.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,16 +234,15 @@
         if bool(list_of_energy) != bool(list_of_pdos):
             raise exceptions.ValidationError('list_of_pdos and list_of_energy must always be set together')
 
         orb_length = len(list_of_orbitals)
 
         # verifies and sets the orbital dicts
         list_of_orbital_dicts = []
-        for i, _ in enumerate(list_of_orbitals):
-            this_orbital = list_of_orbitals[i]
+        for i, this_orbital in enumerate(list_of_orbitals):
             orbital_dict = this_orbital.get_orbital_dict()
             try:
                 orbital_type = orbital_dict.pop('_orbital_type')
             except KeyError:
                 raise exceptions.ValidationError(f'No _orbital_type key found in dictionary: {orbital_dict}')
             cls = OrbitalFactory(orbital_type)
             test_orbital = cls(**orbital_dict)
```

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/data/array/trajectory.py` & `aiida_core-2.4.0/aiida/orm/nodes/data/array/trajectory.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     """
 
     def __init__(self, structurelist=None, **kwargs):
         super().__init__(**kwargs)
         if structurelist is not None:
             self.set_structurelist(structurelist)
 
-    def _internal_validate(self, stepids, cells, symbols, positions, times, velocities):  # pylint: disable=too-many-arguments,too-many-locals,no-self-use,too-many-branches
+    def _internal_validate(self, stepids, cells, symbols, positions, times, velocities):  # pylint: disable=too-many-arguments,too-many-locals,too-many-branches
         """
         Internal function to validate the type and shape of the arrays. See
         the documentation of py:meth:`.set_trajectory` for a description of the
         valid shape and type of the parameters.
         """
         import numpy
 
@@ -498,15 +498,15 @@
           :py:class:`aiida.orm.nodes.data.structure.StructureData` will be used.
 
         :return: :py:class:`aiida.orm.nodes.data.structure.StructureData` node.
         """
         from aiida.orm.nodes.data.dict import Dict
         from aiida.tools.data.array.trajectory import _get_aiida_structure_inline
 
-        param = Dict(dict=kwargs)
+        param = Dict(kwargs)
 
         ret_dict = _get_aiida_structure_inline(trajectory=self, parameters=param, metadata={'store_provenance': store})  # pylint: disable=unexpected-keyword-arg
         return ret_dict['structure']
 
     def get_cif(self, index=None, **kwargs):
         """
         Creates :py:class:`aiida.orm.nodes.data.cif.CifData`
```

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/data/array/xy.py` & `aiida_core-2.4.0/aiida/orm/nodes/data/array/xy.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/data/base.py` & `aiida_core-2.4.0/aiida/orm/nodes/data/base.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/data/bool.py` & `aiida_core-2.4.0/aiida/orm/nodes/data/bool.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/data/cif.py` & `aiida_core-2.4.0/aiida/orm/nodes/data/cif.py`

 * *Files 0% similar despite different names*

```diff
@@ -750,15 +750,15 @@
         :param site_tolerance: This tolerance is used to determine if two sites are sitting in the same position,
             in which case they will be combined to a single disordered site. Defaults to 1e-4. (pymatgen only)
         :return: :py:class:`aiida.orm.nodes.data.structure.StructureData` node.
         """
         from aiida.orm import Dict
         from aiida.tools.data import cif as cif_tools
 
-        parameters = Dict(dict=kwargs)
+        parameters = Dict(kwargs)
 
         try:
             convert_function = getattr(cif_tools, f'_get_aiida_structure_{converter}_inline')
         except AttributeError:
             raise ValueError(f"No such converter '{converter}' available")
 
         result = convert_function(cif=self, parameters=parameters, metadata={'store_provenance': store})
```

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/data/code/abstract.py` & `aiida_core-2.4.0/aiida/orm/nodes/data/code/abstract.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,18 +94,16 @@
         """Return the list of executable with its command line parameters.
 
         :param cmdline_params: List of command line parameters provided by the ``CalcJob`` plugin.
         :return: List of the executable followed by its command line parameters.
         """
         return [str(self.get_executable())] + (cmdline_params or [])
 
-    def get_prepend_cmdline_params( # pylint: disable=no-self-use
-        self,
-        mpi_args: list[str] | None = None,
-        extra_mpirun_params: list[str] | None = None
+    def get_prepend_cmdline_params(
+        self, mpi_args: list[str] | None = None, extra_mpirun_params: list[str] | None = None
     ) -> list[str]:
         """Return List of command line parameters to be prepended to the executable in submission line.
         These command line parameters are typically parameters related to MPI invocations.
 
         :param mpi_args: List of MPI parameters provided by the ``Computer.get_mpirun_command`` method.
         :param extra_mpiruns_params: List of MPI parameters provided by the ``metadata.options.extra_mpirun_params``
             input of the ``CalcJob``.
```

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/data/code/containerized.py` & `aiida_core-2.4.0/aiida/orm/nodes/data/code/containerized.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/data/code/installed.py` & `aiida_core-2.4.0/aiida/orm/nodes/data/code/installed.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/data/code/legacy.py` & `aiida_core-2.4.0/aiida/orm/nodes/data/code/legacy.py`

 * *Files 7% similar despite different names*

```diff
@@ -98,31 +98,31 @@
 
         return pathlib.PurePosixPath(exec_path)
 
     def hide(self):
         """
         Hide the code (prevents from showing it in the verdi code list)
         """
-        warn_deprecation('This property is deprecated, use the `Code.is_hidden` property instead.', version=3)
+        warn_deprecation('`Code.hide` property is deprecated, use the `Code.is_hidden` property instead.', version=3)
         self.is_hidden = True
 
     def reveal(self):
         """
         Reveal the code (allows to show it in the verdi code list)
         By default, it is revealed
         """
-        warn_deprecation('This property is deprecated, use the `Code.is_hidden` property instead.', version=3)
+        warn_deprecation('`Code.reveal` property is deprecated, use the `Code.is_hidden` property instead.', version=3)
         self.is_hidden = False
 
     @property
     def hidden(self):
         """
         Determines whether the Code is hidden or not
         """
-        warn_deprecation('This property is deprecated, use the `Code.is_hidden` property instead.', version=3)
+        warn_deprecation('`Code.hidden` property is deprecated, use the `Code.is_hidden` property instead.', version=3)
         return self.is_hidden
 
     def set_files(self, files):
         """
         Given a list of filenames (or a single filename string),
         add it to the path (all at level zero, i.e. without folders).
         Therefore, be careful for files with the same name!
@@ -144,15 +144,16 @@
             return f"Local code '{self.label}' pk: {self.pk}, uuid: {self.uuid}"
 
         return f"Remote code '{self.label}' on {self.computer.label} pk: {self.pk}, uuid: {self.uuid}"
 
     def get_computer_label(self):
         """Get label of this code's computer."""
         warn_deprecation(
-            'This method is deprecated, use the `InstalledCode.computer.label` property instead.', version=3
+            '`Code.get_computer_label` method is deprecated, use the `InstalledCode.computer.label` property instead.',
+            version=3
         )
         return 'repository' if self.computer is None else self.computer.label
 
     @property
     def full_label(self):
         """Get full label of this code.
 
@@ -161,28 +162,30 @@
         return f'{self.label}@{"repository" if self.computer is None else self.computer.label}'
 
     def relabel(self, new_label):
         """Relabel this code.
 
         :param new_label: new code label
         """
-        warn_deprecation('This method is deprecated, use the `label` property instead.', version=3)
+        warn_deprecation('`Code.relabel` method is deprecated, use the `label` property instead.', version=3)
         if self.computer is not None:
             suffix = f'@{self.computer.label}'
             if new_label.endswith(suffix):
                 new_label = new_label[:-len(suffix)]
 
         self.label = new_label
 
     def get_description(self):
         """Return a string description of this Code instance.
 
         :return: string description of this Code instance
         """
-        warn_deprecation('This method is deprecated, use the `description` property instead.', version=3)
+        warn_deprecation(
+            '`Code.get_description` method is deprecated, use the `description` property instead.', version=3
+        )
         return f'{self.description}'
 
     @classmethod
     def get_code_helper(cls, label, machinename=None, backend=None):
         """
         :param label: the code label identifying the code to load
         :param machinename: the machine name where code is setup
@@ -190,15 +193,17 @@
         :raise aiida.common.NotExistent: if no code identified by the given string is found
         :raise aiida.common.MultipleObjectsError: if the string cannot identify uniquely
             a code
         """
         from aiida.common.exceptions import MultipleObjectsError, NotExistent
         from aiida.orm.querybuilder import QueryBuilder
 
-        warn_deprecation('This method is deprecated, use `aiida.orm.load_code` instead.', version=3)
+        warn_deprecation(
+            '`Code.get_code_helper` classmethod is deprecated, use `aiida.orm.load_code` instead.', version=3
+        )
 
         query = QueryBuilder(backend=backend)
         query.append(cls, filters={'label': label}, project='*', tag='code')
         if machinename:
             query.append(Computer, filters={'label': machinename}, with_node='code')
 
         if query.count() == 0:
@@ -229,15 +234,15 @@
         :raise aiida.common.NotExistent: if no code identified by the given string is found
         :raise aiida.common.MultipleObjectsError: if the string cannot identify uniquely a code
         :raise ValueError: if neither a pk nor a label was passed in
         """
         # pylint: disable=arguments-differ
         from aiida.orm.utils import load_code
 
-        warn_deprecation('This method is deprecated, use `aiida.orm.load_code` instead.', version=3)
+        warn_deprecation('`Code.get` classmethod is deprecated, use `aiida.orm.load_code` instead.', version=3)
 
         # first check if code pk is provided
         if pk:
             code_int = int(pk)
             try:
                 return load_code(pk=code_int)
             except exceptions.NotExistent:
@@ -270,15 +275,17 @@
         :raise aiida.common.MultipleObjectsError: if the string cannot identify uniquely
             a code
         :raise TypeError: if code_string is not of string type
 
         """
         from aiida.common.exceptions import MultipleObjectsError, NotExistent
 
-        warn_deprecation('This method is deprecated, use `aiida.orm.load_code` instead.', version=3)
+        warn_deprecation(
+            '`Code.get_from_string` classmethod is deprecated, use `aiida.orm.load_code` instead.', version=3
+        )
 
         try:
             label, _, machinename = code_string.partition('@')
         except AttributeError:
             raise TypeError('the provided code_string is not of valid string type')
 
         try:
@@ -297,15 +304,15 @@
         :param labels: if True, return a list of code names, otherwise
           return the code PKs (integers).
         :return: a list of string, with the code names if labels is True,
           otherwise a list of integers with the code PKs.
         """
         from aiida.orm.querybuilder import QueryBuilder
 
-        warn_deprecation('This method has been deprecated, there is no replacement.', version=3)
+        warn_deprecation('`Code.list_for_plugin` classmethod has been deprecated, there is no replacement.', version=3)
 
         query = QueryBuilder(backend=backend)
         query.append(cls, filters={'attributes.input_plugin': {'==': plugin}})
         valid_codes = query.all(flat=True)
 
         if labels:
             return [c.label for c in valid_codes]  # type: ignore[union-attr]
@@ -343,15 +350,16 @@
         is intentionally not called in ``_validate`` as to allow the creation of ``Code`` instances whose computers can
         not yet be connected to and as to not require the overhead of opening transports in storing a new code.
 
         :raises `~aiida.common.exceptions.ValidationError`: if no transport could be opened or if the defined executable
             does not exist on the remote computer.
         """
         warn_deprecation(
-            'This method is deprecated, use the `InstalledCode.validate_filepath_executable` property instead.',
+            '`Code.validate_remote_exec_path` method is deprecated, use the '
+            '`InstalledCode.validate_filepath_executable` property instead.',
             version=3
         )
         filepath = self.get_remote_exec_path()
 
         if self.computer is None:
             raise exceptions.ValidationError('checking the remote exec path is not available for a local code.')
 
@@ -370,98 +378,122 @@
             )
 
     def set_prepend_text(self, code):
         """
         Pass a string of code that will be put in the scheduler script before the
         execution of the code.
         """
-        warn_deprecation('This method is deprecated, use the `prepend_text` property instead.', version=3)
+        warn_deprecation(
+            '`Code.set_prepend_text` method is deprecated, use the `prepend_text` property instead.', version=3
+        )
         self.prepend_text = code
 
     def get_prepend_text(self):
         """
         Return the code that will be put in the scheduler script before the
         execution, or an empty string if no pre-exec code was defined.
         """
-        warn_deprecation('This method is deprecated, use the `prepend_text` property instead.', version=3)
+        warn_deprecation(
+            '`Code.get_prepend_text` method is deprecated, use the `prepend_text` property instead.', version=3
+        )
         return self.prepend_text
 
     def set_input_plugin_name(self, input_plugin):
         """
         Set the name of the default input plugin, to be used for the automatic
         generation of a new calculation.
         """
-        warn_deprecation('This method is deprecated, use the `default_calc_job_plugin` property instead.', version=3)
+        warn_deprecation(
+            '`Code.set_input_plugin_name` method is deprecated, use the `default_calc_job_plugin` property instead.',
+            version=3
+        )
         self.default_calc_job_plugin = input_plugin
 
     def get_input_plugin_name(self):
         """
         Return the name of the default input plugin (or None if no input plugin
         was set.
         """
-        warn_deprecation('This method is deprecated, use the `default_calc_job_plugin` property instead.', version=3)
+        warn_deprecation(
+            '`Code.get_input_plugin_name` method is deprecated, use the `default_calc_job_plugin` property instead.',
+            version=3
+        )
         return self.default_calc_job_plugin
 
     def set_use_double_quotes(self, use_double_quotes: bool):
         """Set whether the command line invocation of this code should be escaped with double quotes.
 
         :param use_double_quotes: True if to escape with double quotes, False otherwise.
         """
-        warn_deprecation('This method is deprecated, use the `use_double_quotes` property instead.', version=3)
+        warn_deprecation(
+            '`Code.set_use_double_quotes` method is deprecated, use the `use_double_quotes` property instead.',
+            version=3
+        )
         self.use_double_quotes = use_double_quotes
 
     def get_use_double_quotes(self) -> bool:
         """Return whether the command line invocation of this code should be escaped with double quotes.
 
         :returns: True if to escape with double quotes, False otherwise which is also the default.
         """
-        warn_deprecation('This method is deprecated, use the `use_double_quotes` property instead.', version=3)
+        warn_deprecation(
+            '`Code.get_use_double_quotes` method is deprecated, use the `use_double_quotes` property instead.',
+            version=3
+        )
         return self.use_double_quotes
 
     def set_append_text(self, code):
         """
         Pass a string of code that will be put in the scheduler script after the
         execution of the code.
         """
-        warn_deprecation('This method is deprecated, use the `append_text` property instead.', version=3)
+        warn_deprecation(
+            '`Code.set_append_text` method is deprecated, use the `append_text` property instead.', version=3
+        )
         self.append_text = code
 
     def get_append_text(self):
         """
         Return the postexec_code, or an empty string if no post-exec code was defined.
         """
-        warn_deprecation('This method is deprecated, use the `append_text` property instead.', version=3)
+        warn_deprecation(
+            '`Code.get_append_text` method is deprecated, use the `append_text` property instead.', version=3
+        )
         return self.append_text
 
     def set_local_executable(self, exec_name):
         """
         Set the filename of the local executable.
         Implicitly set the code as local.
         """
-        warn_deprecation('This method is deprecated, use `PortableCode`.', version=3)
+        warn_deprecation('`Code.set_local_executable` method is deprecated, use `PortableCode`.', version=3)
 
         self._set_local()
         self.filepath_executable = exec_name
 
     def get_local_executable(self):
-        warn_deprecation('This method is deprecated, use `PortableCode.filepath_executable` instead.', version=3)
+        """Return the local executable."""
+        warn_deprecation(
+            '`Code.get_local_executable` method is deprecated, use `PortableCode.filepath_executable` instead.',
+            version=3
+        )
         return self.filepath_executable
 
     def set_remote_computer_exec(self, remote_computer_exec):
         """
         Set the code as remote, and pass the computer on which it resides
         and the absolute path on that computer.
 
         :param remote_computer_exec: a tuple (computer, remote_exec_path), where computer is a aiida.orm.Computer and
             remote_exec_path is the absolute path of the main executable on remote computer.
         """
         from aiida import orm
         from aiida.common.lang import type_check
 
-        warn_deprecation('This method is deprecated, use `InstalledCode`.', version=3)
+        warn_deprecation('`Code.set_remote_computer_exec` method is deprecated, use `InstalledCode`.', version=3)
 
         if (not isinstance(remote_computer_exec, (list, tuple)) or len(remote_computer_exec) != 2):
             raise ValueError(
                 'remote_computer_exec must be a list or tuple of length 2, with machine and executable name'
             )
 
         computer, remote_exec_path = tuple(remote_computer_exec)
@@ -472,22 +504,28 @@
         type_check(computer, orm.Computer)
 
         self._set_remote()
         self.computer = computer
         self.base.attributes.set('remote_exec_path', remote_exec_path)
 
     def get_remote_exec_path(self):
-        warn_deprecation('This method is deprecated, use `InstalledCode.filepath_executable` instead.', version=3)
+        """Return the ``remote_exec_path`` attribute."""
+        warn_deprecation(
+            '`Code.get_remote_exec_path` method is deprecated, use `InstalledCode.filepath_executable` instead.',
+            version=3
+        )
         if self.is_local():
             raise ValueError('The code is local')
         return self.base.attributes.get('remote_exec_path', '')
 
     def get_remote_computer(self):
         """Return the remote computer associated with this code."""
-        warn_deprecation('This method is deprecated, use the `computer` attribute instead.', version=3)
+        warn_deprecation(
+            '`Code.get_remote_computer` method is deprecated, use the `computer` attribute instead.', version=3
+        )
         if self.is_local():
             raise ValueError('The code is local')
 
         return self.computer
 
     def _set_local(self):
         """
@@ -519,38 +557,40 @@
             pass
 
     def is_local(self):
         """
         Return True if the code is 'local', False if it is 'remote' (see also documentation
         of the set_local and set_remote functions).
         """
-        warn_deprecation('This method is deprecated, use a `PortableCode` instance and check the type.', version=3)
+        warn_deprecation(
+            '`Code.is_local` method is deprecated, use a `PortableCode` instance and check the type.', version=3
+        )
         return self.base.attributes.get('is_local', None)
 
     def can_run_on(self, computer):
         """
         Return True if this code can run on the given computer, False otherwise.
 
         Local codes can run on any machine; remote codes can run only on the machine
         on which they reside.
 
         TODO: add filters to mask the remote machines on which a local code can run.
         """
         from aiida import orm
         from aiida.common.lang import type_check
 
-        warn_deprecation('This method is deprecated, use `can_run_on_computer` instead.', version=3)
+        warn_deprecation('`Code.can_run_on` method is deprecated, use `can_run_on_computer` instead.', version=3)
 
         if self.is_local():
             return True
 
         type_check(computer, orm.Computer)
         return computer.pk == self.get_remote_computer().pk
 
     def get_execname(self):
         """
         Return the executable string to be put in the script.
         For local codes, it is ./LOCAL_EXECUTABLE_NAME
         For remote codes, it is the absolute path to the executable.
         """
-        warn_deprecation('This method is deprecated, use `get_executable` instead.', version=3)
+        warn_deprecation('`Code.get_execname` method is deprecated, use `get_executable` instead.', version=3)
         return str(self.get_executable())
```

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/data/code/portable.py` & `aiida_core-2.4.0/aiida/orm/nodes/data/code/portable.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/data/data.py` & `aiida_core-2.4.0/aiida/orm/nodes/data/data.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/data/dict.py` & `aiida_core-2.4.0/aiida/orm/nodes/data/dict.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/data/enum.py` & `aiida_core-2.4.0/aiida/orm/nodes/data/enum.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/data/float.py` & `aiida_core-2.4.0/aiida/orm/nodes/data/float.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/data/folder.py` & `aiida_core-2.4.0/aiida/orm/nodes/data/folder.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/data/int.py` & `aiida_core-2.4.0/aiida/orm/nodes/data/int.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/data/jsonable.py` & `aiida_core-2.4.0/aiida/orm/nodes/data/jsonable.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/data/list.py` & `aiida_core-2.4.0/aiida/orm/nodes/data/list.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,8 +144,8 @@
         :rtype: bool
         """
         return not self.is_stored
 
 
 @to_aiida_type.register(list)
 def _(value):
-    return List(list=value)
+    return List(value)
```

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/data/numeric.py` & `aiida_core-2.4.0/aiida/orm/nodes/data/numeric.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/data/orbital.py` & `aiida_core-2.4.0/aiida/orm/nodes/data/orbital.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/data/remote/base.py` & `aiida_core-2.4.0/aiida/orm/nodes/data/remote/base.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/data/remote/stash/base.py` & `aiida_core-2.4.0/aiida/orm/nodes/data/remote/stash/base.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/data/remote/stash/folder.py` & `aiida_core-2.4.0/aiida/orm/nodes/data/remote/stash/folder.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/data/singlefile.py` & `aiida_core-2.4.0/aiida/orm/nodes/data/singlefile.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,18 @@
 # This file is part of the AiiDA code.                                    #
 #                                                                         #
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-core #
 # For further information on the license, see the LICENSE.txt file        #
 # For further information please visit http://www.aiida.net               #
 ###########################################################################
 """Data class that can be used to store a single file in its repository."""
+from __future__ import annotations
+
 import contextlib
+import io
 import os
 import pathlib
 
 from aiida.common import exceptions
 
 from .data import Data
 
@@ -20,15 +23,24 @@
 
 
 class SinglefileData(Data):
     """Data class that can be used to store a single file in its repository."""
 
     DEFAULT_FILENAME = 'file.txt'
 
-    def __init__(self, file, filename=None, **kwargs):
+    @classmethod
+    def from_string(cls, content: str, filename: str | pathlib.Path | None = None, **kwargs):
+        """Construct a new instance and set ``content`` as its contents.
+
+        :param content: The content as a string.
+        :param filename: Specify filename to use (defaults to ``file.txt``).
+        """
+        return cls(io.StringIO(content), filename, **kwargs)
+
+    def __init__(self, file, filename: str | pathlib.Path | None = None, **kwargs):
         """Construct a new instance and set the contents to that of the file.
 
         :param file: an absolute filepath or filelike object whose contents to copy.
             Hint: Pass io.BytesIO(b"my string") to construct the SinglefileData directly from a string.
         :param filename: specify filename to use (defaults to name of provided file).
         """
         # pylint: disable=redefined-builtin
@@ -63,15 +75,15 @@
         """Return the content of the single file stored for this data node.
 
         :return: the content of the file as a string
         """
         with self.open() as handle:
             return handle.read()
 
-    def set_file(self, file, filename=None):
+    def set_file(self, file, filename: str | pathlib.Path | None = None):
         """Store the content of the file in the node's repository, deleting any other existing objects.
 
         :param file: an absolute filepath or filelike object whose contents to copy
             Hint: Pass io.BytesIO(b"my string") to construct the file directly from a string.
         :param filename: specify filename to use (defaults to name of provided file).
         """
         # pylint: disable=redefined-builtin
@@ -88,16 +100,15 @@
         else:
             is_filelike = True
             try:
                 key = os.path.basename(file.name)
             except AttributeError:
                 key = self.DEFAULT_FILENAME
 
-        key = filename or key
-
+        key = str(filename) if filename is not None else key
         existing_object_names = self.base.repository.list_object_names()
 
         try:
             # Remove the 'key' from the list of currently existing objects such that it is not deleted after storing
             existing_object_names.remove(key)
         except ValueError:
             pass
@@ -122,9 +133,9 @@
         except AttributeError:
             raise exceptions.ValidationError('the `filename` attribute is not set.')
 
         objects = self.base.repository.list_object_names()
 
         if [filename] != objects:
             raise exceptions.ValidationError(
-                f'respository files {objects} do not match the `filename` attribute {filename}.'
+                f'respository files {objects} do not match the `filename` attribute `{filename}`.'
             )
```

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/data/str.py` & `aiida_core-2.4.0/aiida/orm/nodes/data/str.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/data/structure.py` & `aiida_core-2.4.0/aiida/orm/nodes/data/structure.py`

 * *Files 1% similar despite different names*

```diff
@@ -799,19 +799,17 @@
         :param margin: the margin to be added in all directions of the
             bounding box of the molecule.
 
         .. note:: Requires the pymatgen module (version >= 3.0.13, usage
             of earlier versions may cause errors).
         """
         box = [
-            max([x.coords.tolist()[0] for x in mol.sites]) - min([x.coords.tolist()[0] for x in mol.sites]) +
-            2 * margin,
-            max([x.coords.tolist()[1] for x in mol.sites]) - min([x.coords.tolist()[1] for x in mol.sites]) +
-            2 * margin,
-            max([x.coords.tolist()[2] for x in mol.sites]) - min([x.coords.tolist()[2] for x in mol.sites]) + 2 * margin
+            max(x.coords.tolist()[0] for x in mol.sites) - min(x.coords.tolist()[0] for x in mol.sites) + 2 * margin,
+            max(x.coords.tolist()[1] for x in mol.sites) - min(x.coords.tolist()[1] for x in mol.sites) + 2 * margin,
+            max(x.coords.tolist()[2] for x in mol.sites) - min(x.coords.tolist()[2] for x in mol.sites) + 2 * margin
         ]
         self.set_pymatgen_structure(mol.get_boxed_structure(*box))
         self.pbc = [False, False, False]
 
     def set_pymatgen_structure(self, struct):
         """
         Load the structure from a pymatgen Structure object.
@@ -1747,15 +1745,15 @@
             AiiDA database for record. Default False.
         :return: :py:class:`aiida.orm.nodes.data.cif.CifData` node.
         """
         from aiida.tools.data import structure as structure_tools
 
         from .dict import Dict
 
-        param = Dict(dict=kwargs)
+        param = Dict(kwargs)
         try:
             conv_f = getattr(structure_tools, f'_get_cif_{converter}_inline')
         except AttributeError:
             raise ValueError(f"No such converter '{converter}' available")
         ret_dict = conv_f(struct=self, parameters=param, metadata={'store_provenance': store})
         return ret_dict['cif']
```

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/data/upf.py` & `aiida_core-2.4.0/aiida/orm/nodes/data/upf.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/links.py` & `aiida_core-2.4.0/aiida/orm/nodes/links.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         if link_type in [LinkType.CREATE, LinkType.INPUT_CALC, LinkType.INPUT_WORK]:
             builder = QueryBuilder(backend=self._node.backend).append(
                 Node, filters={'id': self._node.pk}, tag='parent').append(
                 Node, filters={'id': source.pk}, tag='child', with_ancestors='parent')  # yapf:disable
             if builder.count() > 0:
                 raise ValueError('the link you are attempting to create would generate a cycle in the graph')
 
-    def validate_outgoing(self, target: 'Node', link_type: LinkType, link_label: str) -> None:  # pylint: disable=unused-argument,no-self-use
+    def validate_outgoing(self, target: 'Node', link_type: LinkType, link_label: str) -> None:  # pylint: disable=unused-argument
         """Validate adding a link of the given type from ourself to a given node.
 
         The validity of the triple (source, link, target) should be validated in the `validate_incoming` call.
         This method will be called afterwards and can be overriden by subclasses to add additional checks that are
         specific to that subclass.
 
         :param target: the node to which the link is going
```

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/node.py` & `aiida_core-2.4.0/aiida/orm/nodes/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 if TYPE_CHECKING:
     from aiida.plugins.entry_point import EntryPoint  # type: ignore
 
     from ..implementation import BackendNode, StorageBackend
 
 __all__ = ('Node',)
 
-NodeType = TypeVar('NodeType', bound='Node')
+NodeType = TypeVar('NodeType', bound='Node')  # pylint: disable=invalid-name
 
 
 class NodeCollection(EntityCollection[NodeType], Generic[NodeType]):
     """The collection of nodes."""
 
     @staticmethod
     def _entity_base_cls() -> Type['Node']:  # type: ignore
@@ -242,15 +242,14 @@
         Subclasses can override this method to perform additional checks
         and should usually call ``super()._validate()`` first!
 
         This method is called automatically before storing the node in the DB.
         Therefore, use :py:meth:`~aiida.orm.nodes.attributes.NodeAttributes.get()` and similar methods that
         automatically read either from the DB or from the internal attribute cache.
         """
-        # pylint: disable=no-self-use
         return True
 
     def _validate_storability(self) -> None:
         """Verify that the current node is allowed to be stored.
 
         :raises `aiida.common.exceptions.StoringNotAllowed`: if the node does not match all requirements for storing
         """
@@ -538,15 +537,14 @@
             new_node.store()
 
     def get_description(self) -> str:
         """Return a string with a description of the node.
 
         :return: a description string
         """
-        # pylint: disable=no-self-use
         return ''
 
     @property
     def is_valid_cache(self) -> bool:
         """Hook to exclude certain ``Node`` classes from being considered a valid cache.
 
         The base class assumes that all node instances are valid to cache from, unless the ``_VALID_CACHE_KEY`` extra
@@ -649,15 +647,15 @@
         'validate_outgoing': 'validate_outgoing',
         'get_stored_link_triples': 'get_stored_link_triples',
         'get_incoming': 'get_incoming',
         'get_outgoing': 'get_outgoing',
     }
 
     @classproperty
-    def Collection(cls):  # pylint: disable=invalid-name,no-self-use
+    def Collection(cls):  # pylint: disable=invalid-name
         """Return the collection type for this class.
 
         This used to be a class argument with the value ``NodeCollection``. The argument is deprecated and this property
         is here for backwards compatibility to print the deprecation warning.
         """
         warn_deprecation(
             'This attribute is deprecated, use `aiida.orm.nodes.node.NodeCollection` instead.', version=3, stacklevel=2
```

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/process/__init__.py` & `aiida_core-2.4.0/aiida/orm/nodes/process/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/process/calculation/__init__.py` & `aiida_core-2.4.0/aiida/orm/nodes/process/calculation/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/process/calculation/calcfunction.py` & `aiida_core-2.4.0/aiida/orm/nodes/process/calculation/calcfunction.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/process/calculation/calcjob.py` & `aiida_core-2.4.0/aiida/orm/nodes/process/calculation/calcjob.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,14 +62,15 @@
         return objects
 
 
 class CalcJobNode(CalculationNode):
     """ORM class for all nodes representing the execution of a CalcJob."""
 
     # pylint: disable=too-many-public-methods
+    _CLS_NODE_CACHING = CalcJobNodeCaching
 
     CALC_JOB_STATE_KEY = 'state'
     IMMIGRATED_KEY = 'imported'
     REMOTE_WORKDIR_KEY = 'remote_workdir'
     RETRIEVE_LIST_KEY = 'retrieve_list'
     RETRIEVE_TEMPORARY_LIST_KEY = 'retrieve_temporary_list'
     SCHEDULER_JOB_ID_KEY = 'job_id'
```

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/process/calculation/calculation.py` & `aiida_core-2.4.0/aiida/orm/nodes/process/calculation/calculation.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/process/process.py` & `aiida_core-2.4.0/aiida/orm/nodes/process/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from aiida.common.links import LinkType
 from aiida.orm.utils.mixins import Sealable
 
 from ..caching import NodeCaching
 from ..node import Node, NodeLinks
 
 if TYPE_CHECKING:
-    from aiida.engine.processes import Process
+    from aiida.engine.processes import ExitCode, Process
     from aiida.engine.processes.builder import ProcessBuilder
 
 __all__ = ('ProcessNode',)
 
 
 class ProcessNodeCaching(NodeCaching):
     """Interface to control caching of a node instance."""
@@ -395,14 +395,32 @@
 
         :return: True if the process has failed, False otherwise
         :rtype: bool
         """
         return self.is_finished and self.exit_status != 0
 
     @property
+    def exit_code(self) -> Optional['ExitCode']:
+        """Return the exit code of the process.
+
+        It is reconstituted from the ``exit_status`` and ``exit_message`` attributes if both of those are defined.
+
+        :returns: The exit code if defined, or ``None``.
+        """
+        from aiida.engine.processes.exit_code import ExitCode
+
+        exit_status = self.exit_status
+        exit_message = self.exit_message
+
+        if exit_status is None or exit_message is None:
+            return None
+
+        return ExitCode(exit_status, exit_message)
+
+    @property
     def exit_status(self) -> Optional[int]:
         """
         Return the exit status of the process
 
         :returns: the exit status, an integer exit code or None
         """
         return self.base.attributes.get(self.EXIT_STATUS_KEY, None)
@@ -559,9 +577,8 @@
 
         :returns: process node that called this process node instance or None
         """
         try:
             caller = self.base.links.get_incoming(link_type=(LinkType.CALL_CALC, LinkType.CALL_WORK)).one().node
         except ValueError:
             return None
-        else:
-            return caller
+        return caller
```

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/process/workflow/__init__.py` & `aiida_core-2.4.0/aiida/orm/nodes/process/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/process/workflow/workchain.py` & `aiida_core-2.4.0/aiida/orm/nodes/process/workflow/workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/process/workflow/workflow.py` & `aiida_core-2.4.0/aiida/orm/nodes/process/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/process/workflow/workfunction.py` & `aiida_core-2.4.0/aiida/orm/nodes/process/workflow/workfunction.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/nodes/repository.py` & `aiida_core-2.4.0/aiida/orm/nodes/repository.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/querybuilder.py` & `aiida_core-2.4.0/aiida/orm/querybuilder.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,16 @@
     Type,
     Union,
     cast,
     overload,
 )
 import warnings
 
+from aiida.common.log import AIIDA_LOGGER
+from aiida.common.warnings import warn_deprecation
 from aiida.manage import get_manager
 from aiida.orm.entities import EntityTypes
 from aiida.orm.implementation.querybuilder import (
     GROUP_ENTITY_TYPE_PREFIX,
     BackendQueryBuilder,
     EntityRelationships,
     PathItemType,
@@ -63,14 +65,16 @@
 
 # re-usable type annotations
 EntityClsType = Type[Union[entities.Entity, 'Process']]  # pylint: disable=invalid-name
 ProjectType = Union[str, dict, Sequence[Union[str, dict]]]  # pylint: disable=invalid-name
 FilterType = Dict[str, Any]  # pylint: disable=invalid-name
 OrderByType = Union[dict, List[dict], Tuple[dict, ...]]
 
+LOGGER = AIIDA_LOGGER.getChild('querybuilder')
+
 
 class Classifier(NamedTuple):
     """A classifier for an entity."""
     ormclass_type_string: str
     process_type_string: Optional[str] = None
 
 
@@ -96,15 +100,15 @@
     _EDGE_TAG_DELIM = '--'
     _VALID_PROJECTION_KEYS = ('func', 'cast')
 
     def __init__(
         self,
         backend: Optional['StorageBackend'] = None,
         *,
-        debug: bool = False,
+        debug: bool | None = None,
         path: Optional[Sequence[Union[str, Dict[str, Any], EntityClsType]]] = (),
         filters: Optional[Dict[str, FilterType]] = None,
         project: Optional[Dict[str, ProjectType]] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         order_by: Optional[OrderByType] = None,
         distinct: bool = False,
@@ -156,15 +160,24 @@
         self._offset: Optional[int] = None
         self._distinct: bool = distinct
 
         # cache of tag mappings, populated during appends
         self._tags = _QueryTagMap()
 
         # Set the debug level
-        self.set_debug(debug)
+        if debug is not None:
+            warn_deprecation(
+                'The `debug` argument is deprecated. Configure the log level of the AiiDA logger instead.', version=3
+            )
+        else:
+            debug = False
+
+        with warnings.catch_warnings():
+            warnings.simplefilter('ignore')
+            self.set_debug(debug)
 
         # Validate & add the query path
         if not isinstance(path, (list, tuple)):
             raise TypeError('Path needs to be a tuple or a list')
         for path_spec in path:
             if isinstance(path_spec, dict):
                 self.append(**path_spec)
@@ -212,15 +225,14 @@
         if copy:
             return deepcopy(data)
         return data
 
     @property
     def queryhelp(self) -> 'QueryDictType':
         """"Legacy name for ``as_dict`` method."""
-        from aiida.common.warnings import warn_deprecation
         warn_deprecation('`QueryBuilder.queryhelp` is deprecated, use `QueryBuilder.as_dict()` instead', version=3)
         return self.as_dict()
 
     @classmethod
     def from_dict(cls, dct: Dict[str, Any]) -> 'QueryBuilder':
         """Create an instance from a dictionary representation of the query."""
         return cls(**dct)
@@ -402,15 +414,15 @@
         # Now, several things can go wrong along the way, so I need to split into
         # atomic blocks that I can reverse if something goes wrong.
 
         # TAG ALIASING ##############################
         try:
             self._tags.add(tag, ormclass, cls)
         except Exception as exception:
-            self.debug('Exception caught in append, cleaning up: %s', exception)
+            LOGGER.debug('Exception caught in append, cleaning up: %s', exception)
             self._tags.remove(tag)
             raise
 
         # FILTERS ######################################
         try:
             self._filters[tag] = {}
             # Subclassing is currently only implemented for the `Node` and `Group` classes.
@@ -425,26 +437,26 @@
 
             # The order has to be first _add_node_type_filter and then add_filter.
             # If the user adds a query on the type column, it overwrites what I did
             # if the user specified a filter, add it:
             if filters is not None:
                 self.add_filter(tag, filters)
         except Exception as exception:
-            self.debug('Exception caught in append, cleaning up: %s', exception)
+            LOGGER.debug('Exception caught in append, cleaning up: %s', exception)
             self._tags.remove(tag)
             self._filters.pop(tag)
             raise
 
         # PROJECTIONS ##############################
         try:
             self._projections[tag] = []
             if project is not None:
                 self.add_projection(tag, project)
         except Exception as exception:
-            self.debug('Exception caught in append, cleaning up: %s', exception)
+            LOGGER.debug('Exception caught in append, cleaning up: %s', exception)
             self._tags.remove(tag)
             self._filters.pop(tag)
             self._projections.pop(tag)
             raise exception
 
         # JOINING #####################################
         # pylint: disable=too-many-nested-blocks
@@ -491,15 +503,15 @@
                 if ormclass == EntityTypes.NODE:
                     joining_keyword = 'with_incoming'
                 else:
                     joining_keyword = 'with_node'
                 joining_value = self._path[-1]['tag']
 
         except Exception as exception:
-            self.debug('Exception caught in append (part filters), cleaning up: %s', exception)
+            LOGGER.debug('Exception caught in append (part filters), cleaning up: %s', exception)
             self._tags.remove(tag)
             self._filters.pop(tag)
             self._projections.pop(tag)
             # There's not more to clean up here!
             raise exception
 
         # EDGES #################################
@@ -508,15 +520,15 @@
             try:
                 if edge_tag is None:
                     edge_destination_tag = self._tags.get(joining_value)
                     edge_tag = edge_destination_tag + self._EDGE_TAG_DELIM + tag
                 else:
                     if edge_tag in self._tags:
                         raise ValueError(f'The tag {edge_tag} is already in use')
-                self.debug('edge_tag chosen: %s', edge_tag)
+                LOGGER.debug('edge_tag chosen: %s', edge_tag)
 
                 # edge tags do not have an ormclass
                 self._tags.add(edge_tag)
 
                 # Filters on links:
                 # Beware, I alway add this entry now, but filtering here might be
                 # non-sensical, since this ONLY works for m2m relationship where
@@ -525,15 +537,15 @@
                 if edge_filters is not None:
                     self.add_filter(edge_tag, edge_filters)
                 # Projections on links
                 self._projections[edge_tag] = []
                 if edge_project is not None:
                     self.add_projection(edge_tag, edge_project)
             except Exception as exception:
-                self.debug('Exception caught in append (part joining), cleaning up %s', exception)
+                LOGGER.debug('Exception caught in append (part joining), cleaning up %s', exception)
                 self._tags.remove(tag)
                 self._filters.pop(tag)
                 self._projections.pop(tag)
                 if edge_tag is not None:
                     self._tags.remove(edge_tag)
                     self._filters.pop(edge_tag, None)
                     self._projections.pop(edge_tag, None)
@@ -812,15 +824,15 @@
             # >>> 'user_id, description, ctime, label, extras, mtime, id, attributes, dbcomputer_id, type, uuid'
 
         Be aware that the result of ``**`` depends on the backend implementation.
 
         """
         tag = self._tags.get(tag_spec)
         _projections = []
-        self.debug('Adding projection of %s: %s', tag_spec, projection_spec)
+        LOGGER.debug('Adding projection of %s: %s', tag_spec, projection_spec)
         if not isinstance(projection_spec, (list, tuple)):
             projection_spec = [projection_spec]  # type: ignore
         for projection in projection_spec:
             if isinstance(projection, dict):
                 _thisprojection = projection
             elif isinstance(projection, str):
                 _thisprojection = {projection: {}}
@@ -834,35 +846,39 @@
 
                 for key, val in spec.items():
                     if key not in self._VALID_PROJECTION_KEYS:
                         raise ValueError(f'{key} is not a valid key {self._VALID_PROJECTION_KEYS}')
                     if not isinstance(val, str):
                         raise TypeError(f'{val} has to be a string')
             _projections.append(_thisprojection)
-        self.debug('projections have become: %s', _projections)
+        LOGGER.debug('projections have become: %s', _projections)
         self._projections[tag] = _projections
 
     def set_debug(self, debug: bool) -> 'QueryBuilder':
         """
         Run in debug mode. This does not affect functionality, but prints intermediate stages
         when creating a query on screen.
 
         :param debug: Turn debug on or off
         """
+        warn_deprecation(
+            '`QueryBuilder.set_debug` is deprecated. Configure the log level of the AiiDA logger instead.', version=3
+        )
         if not isinstance(debug, bool):
             return TypeError('I expect a boolean')
         self._debug = debug
 
         return self
 
     def debug(self, msg: str, *objects: Any) -> None:
         """Log debug message.
 
         objects will passed to the format string, e.g. ``msg % objects``
         """
+        warn_deprecation('`QueryBuilder.debug` is deprecated.', version=3)
         if self._debug:
             print(f'DEBUG: {msg}' % objects)
 
     def limit(self, limit: Optional[int]) -> 'QueryBuilder':
         """
         Set the limit (nr of rows to return)
 
@@ -1385,14 +1401,15 @@
     return filters
 
 
 class _QueryTagMap:
     """Cache of tag mappings for a query."""
 
     def __init__(self):
+        """Construct a new instance."""
         self._tag_to_type: Dict[str, Union[None, EntityTypes]] = {}
         # A dictionary for classes passed to the tag given to them
         # Everything is specified with unique tags, which are strings.
         # But somebody might not care about giving tags, so to do
         # everything with classes one needs a map, that also defines classes
         # as tags, to allow the following example:
```

### Comparing `aiida_core-2.3.1/aiida/orm/users.py` & `aiida_core-2.4.0/aiida/orm/users.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/utils/__init__.py` & `aiida_core-2.4.0/aiida/orm/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/utils/builders/__init__.py` & `aiida_core-2.4.0/aiida/orm/utils/builders/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/utils/builders/code.py` & `aiida_core-2.4.0/aiida/orm/utils/builders/code.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/utils/builders/computer.py` & `aiida_core-2.4.0/aiida/orm/utils/builders/computer.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         spec['mpirun_command'] = ' '.join(computer.get_mpirun_command())
         spec['mpiprocs_per_machine'] = computer.get_default_mpiprocs_per_machine()
         spec['default_memory_per_machine'] = computer.get_default_memory_per_machine()
 
         return spec
 
     def __init__(self, **kwargs):
+        """Construct a new instance."""
         self._computer_spec = {}
         self._err_acc = ErrorAccumulator(self.ComputerValidationError)
 
         for key, value in kwargs.items():
             self.__setattr__(key, value)
 
     def validate(self, raise_error=True):
@@ -150,15 +151,15 @@
         Return a spec, or raise if not defined.
         Moreover, add the key to the 'used' dict.
 
         :param key: name of a computer spec
         :param used: should be a set of keys that you want to track.
            ``key`` will be added to this set if the value exists in the spec and can be retrieved.
         """
-        retval = self.__getattr__(key)
+        retval = self.__getattr__(key)  # pylint: disable=unnecessary-dunder-call
         # I first get a retval, so if I get an exception, I don't add it to the 'used' set
         used.add(key)
         return retval
 
     def __setattr__(self, key, value):
         if not key.startswith('_'):
             self._set_computer_attr(key, value)
```

### Comparing `aiida_core-2.3.1/aiida/orm/utils/calcjob.py` & `aiida_core-2.4.0/aiida/orm/utils/calcjob.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/utils/links.py` & `aiida_core-2.4.0/aiida/orm/utils/links.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/utils/loaders.py` & `aiida_core-2.4.0/aiida/orm/utils/loaders.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/utils/log.py` & `aiida_core-2.4.0/aiida/orm/utils/log.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/utils/managers.py` & `aiida_core-2.4.0/aiida/orm/utils/managers.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,16 @@
                 self._namespace_separator in label and
                 not (label.startswith(self._namespace_separator) and label.endswith(self._namespace_separator))
             ):
                 import functools
                 warn_deprecation(
                     'dereferencing nodes with links containing double underscores is deprecated, simply replace '
                     'the double underscores with a single dot instead. For example: \n'
-                    '`self.inputs.some__label` can be written as `self.inputs.some.label` instead.\n',
+                    '`node.inputs.some__label` can be written as `node.inputs.some.label` instead.\n',
+                    stacklevel=4,
                     version=3
                 )  # pylint: disable=no-member
                 namespaces = label.split(self._namespace_separator)
                 try:
                     return functools.reduce(lambda d, namespace: d.get(namespace), namespaces, attribute_dict)
                 except TypeError as exc:
                     # This can be raised if part of the `namespaces` correspond to an actual leaf node, but is treated
```

### Comparing `aiida_core-2.3.1/aiida/orm/utils/mixins.py` & `aiida_core-2.4.0/aiida/orm/utils/mixins.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/utils/node.py` & `aiida_core-2.4.0/aiida/orm/utils/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,16 +153,16 @@
 
     return type_string
 
 
 class AbstractNodeMeta(ABCMeta):
     """Some python black magic to set correctly the logger also in subclasses."""
 
-    def __new__(cls, name, bases, namespace, **kwargs):
-        newcls = ABCMeta.__new__(cls, name, bases, namespace, **kwargs)  # pylint: disable=too-many-function-args
+    def __new__(mcs, name, bases, namespace, **kwargs):
+        newcls = ABCMeta.__new__(mcs, name, bases, namespace, **kwargs)  # pylint: disable=too-many-function-args
         newcls._logger = logging.getLogger(f"{namespace['__module__']}.{name}")
 
         # Set the plugin type string and query type string based on the plugin type string
         newcls._plugin_type_string = get_type_string_from_class(namespace['__module__'], name)  # pylint: disable=protected-access
         newcls._query_type_string = get_query_type_from_type_string(newcls._plugin_type_string)  # pylint: disable=protected-access
 
         return newcls
```

### Comparing `aiida_core-2.3.1/aiida/orm/utils/remote.py` & `aiida_core-2.4.0/aiida/orm/utils/remote.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/orm/utils/serialize.py` & `aiida_core-2.4.0/aiida/orm/utils/serialize.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from dataclasses import asdict, is_dataclass
 from enum import Enum
 from functools import partial
 import inspect
 from typing import Any, Protocol, Type, overload
 
-from plumpy import Bundle, get_object_loader  # type: ignore[attr-defined]
+from plumpy import Bundle, get_object_loader
 from plumpy.utils import AttributesFrozendict
 import yaml
 
 from aiida import orm
 from aiida.common import AttributeDict
 
 _ENUM_TAG = '!enum'
```

### Comparing `aiida_core-2.3.1/aiida/parsers/__init__.py` & `aiida_core-2.4.0/aiida/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/parsers/parser.py` & `aiida_core-2.4.0/aiida/parsers/parser.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/parsers/plugins/__init__.py` & `aiida_core-2.4.0/aiida/parsers/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/parsers/plugins/arithmetic/__init__.py` & `aiida_core-2.4.0/aiida/parsers/plugins/arithmetic/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/parsers/plugins/arithmetic/add.py` & `aiida_core-2.4.0/aiida/parsers/plugins/arithmetic/add.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/parsers/plugins/diff_tutorial/parsers.py` & `aiida_core-2.4.0/aiida/parsers/plugins/diff_tutorial/parsers.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/parsers/plugins/templatereplacer/__init__.py` & `aiida_core-2.4.0/aiida/parsers/plugins/templatereplacer/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/parsers/plugins/templatereplacer/parser.py` & `aiida_core-2.4.0/aiida/parsers/plugins/templatereplacer/parser.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/plugins/__init__.py` & `aiida_core-2.4.0/aiida/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/plugins/entry_point.py` & `aiida_core-2.4.0/aiida/plugins/entry_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,18 +176,19 @@
     :param entry_point_string: the entry point string
     :returns: the entry point type
     """
     try:
         group, _ = entry_point_string.split(ENTRY_POINT_STRING_SEPARATOR)
     except ValueError:
         return EntryPointFormat.MINIMAL
-    else:
-        if group.startswith(ENTRY_POINT_GROUP_PREFIX):
-            return EntryPointFormat.FULL
-        return EntryPointFormat.PARTIAL
+
+    if group.startswith(ENTRY_POINT_GROUP_PREFIX):
+        return EntryPointFormat.FULL
+
+    return EntryPointFormat.PARTIAL
 
 
 def get_entry_point_from_string(entry_point_string: str) -> EntryPoint:
     """
     Return an entry point for the given entry point string
 
     :param entry_point_string: the entry point string
@@ -302,22 +303,20 @@
 
     This method should be removed in ``aiida-core==3.0``.
     """
     try:
         deprecated_entry_points = DEPRECATED_ENTRY_POINTS_MAPPING[group]
     except KeyError:
         return name
-    else:
-        if name in deprecated_entry_points:
-            warn_deprecation(
-                f'The entry point `{name}` is deprecated. Please replace it with `core.{name}`.', version=3
-            )
-            name = f'core.{name}'
 
-        return name
+    if name in deprecated_entry_points:
+        warn_deprecation(f'The entry point `{name}` is deprecated. Please replace it with `core.{name}`.', version=3)
+        name = f'core.{name}'
+
+    return name
 
 
 @functools.lru_cache(maxsize=100)
 def get_entry_point_from_class(class_module: str, class_name: str) -> Tuple[Optional[str], Optional[EntryPoint]]:
     """
     Given the module and name of a class, attempt to obtain the corresponding entry point if it exists
```

### Comparing `aiida_core-2.3.1/aiida/plugins/factories.py` & `aiida_core-2.4.0/aiida/plugins/factories.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/plugins/utils.py` & `aiida_core-2.4.0/aiida/plugins/utils.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/repository/__init__.py` & `aiida_core-2.4.0/aiida/repository/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/repository/backend/abstract.py` & `aiida_core-2.4.0/aiida/repository/backend/abstract.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/repository/backend/disk_object_store.py` & `aiida_core-2.4.0/aiida/repository/backend/disk_object_store.py`

 * *Files 3% similar despite different names*

```diff
@@ -145,22 +145,24 @@
         self,
         dry_run: bool = False,
         live: bool = True,
         pack_loose: bool = None,
         do_repack: bool = None,
         clean_storage: bool = None,
         do_vacuum: bool = None,
+        compress: bool = False,
     ) -> dict:
         """Performs maintenance operations.
 
         :param live:if True, will only perform operations that are safe to do while the repository is in use.
         :param pack_loose:flag for forcing the packing of loose files.
         :param do_repack:flag for forcing the re-packing of already packed files.
         :param clean_storage:flag for forcing the cleaning of soft-deleted files from the repository.
         :param do_vacuum:flag for forcing the vacuuming of the internal database when cleaning the repository.
+        :param compress:flag for compressing the data when packing loose files.
         :return:a dictionary with information on the operations performed.
         """
         if live and (do_repack or clean_storage or do_vacuum):
             overrides = {'do_repack': do_repack, 'clean_storage': clean_storage, 'do_vacuum': do_vacuum}
             keys = ', '.join([key for key, override in overrides.items() if override is True])  # type: ignore
             raise ValueError(f'The following overrides were enabled but cannot be if `live=True`: {keys}')
 
@@ -177,15 +179,15 @@
 
         with self._container as container:
             if pack_loose:
                 files_numb = container.count_objects()['loose']
                 files_size = container.get_total_size()['total_size_loose'] * BYTES_TO_MB
                 logger.report(f'Packing all loose files ({files_numb} files occupying {files_size} MB) ...')
                 if not dry_run:
-                    container.pack_all_loose()
+                    container.pack_all_loose(compress=compress)
 
             if do_repack:
                 files_numb = container.count_objects()['packed']
                 files_size = container.get_total_size()['total_size_packfiles_on_disk'] * BYTES_TO_MB
                 logger.report(f'Re-packing all pack files ({files_numb} files in packs, occupying {files_size} MB) ...')
                 if not dry_run:
                     container.repack()
```

### Comparing `aiida_core-2.3.1/aiida/repository/backend/sandbox.py` & `aiida_core-2.4.0/aiida/repository/backend/sandbox.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/repository/common.py` & `aiida_core-2.4.0/aiida/repository/common.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/repository/repository.py` & `aiida_core-2.4.0/aiida/repository/repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     @classmethod
     def from_serialized(cls, backend: AbstractRepositoryBackend, serialized: Dict[str, Any]) -> 'Repository':
         """Construct an instance where the metadata is initialized from the serialized content.
 
         :param backend: instance of repository backend to use to actually store the file objects.
         """
         instance = cls.__new__(cls)
-        instance.__init__(backend)  # type: ignore[misc]
+        instance.__init__(backend)  # type: ignore[misc]  # pylint: disable=unnecessary-dunder-call
 
         if serialized:
             for name, obj in serialized['o'].items():
                 instance.get_directory().objects[name] = cls._file_cls.from_serialized(obj, name)
 
         return instance
 
@@ -372,16 +372,15 @@
         :return: True if the object exists, False otherwise.
         :raises TypeError: if the path is not a string or ``Path``, or is an absolute path.
         """
         try:
             self.get_object(path)
         except FileNotFoundError:
             return False
-        else:
-            return True
+        return True
 
     @contextlib.contextmanager
     def open(self, path: FilePath) -> Iterator[BinaryIO]:
         """Open a file handle to an object stored under the given path.
 
         .. note:: this should only be used to open a handle to read an existing file. To write a new file use the method
             ``put_object_from_filelike`` instead.
```

### Comparing `aiida_core-2.3.1/aiida/restapi/__init__.py` & `aiida_core-2.4.0/aiida/restapi/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/restapi/api.py` & `aiida_core-2.4.0/aiida/restapi/api.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/restapi/common/__init__.py` & `aiida_core-2.4.0/aiida/restapi/common/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/restapi/common/config.py` & `aiida_core-2.4.0/aiida/restapi/common/config.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/restapi/common/exceptions.py` & `aiida_core-2.4.0/aiida/restapi/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/restapi/common/identifiers.py` & `aiida_core-2.4.0/aiida/restapi/common/identifiers.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/restapi/common/utils.py` & `aiida_core-2.4.0/aiida/restapi/common/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,66 +8,66 @@
 # For further information please visit http://www.aiida.net               #
 ###########################################################################
 """ Util methods """
 from datetime import datetime, timedelta
 import urllib.parse
 
 from flask import jsonify
-from flask.json import JSONEncoder
+from flask.json.provider import DefaultJSONProvider
 from wrapt import decorator
 
 from aiida.common.exceptions import InputValidationError, ValidationError
 from aiida.common.utils import DatetimePrecision
 from aiida.manage import get_manager
 from aiida.restapi.common.exceptions import RestInputValidationError, RestValidationError
 
 # Important to match querybuilder keys
 PK_DBSYNONYM = 'id'
 # Example uuid (version 4)
 UUID_REF = 'd55082b6-76dc-426b-af89-0e08b59524d2'
 
 
 ########################## Classes #####################
-class CustomJSONEncoder(JSONEncoder):
+class CustomJSONProvider(DefaultJSONProvider):
     """
     Custom json encoder for serialization.
     This has to be provided to the Flask app in order to replace the default
     encoder.
     """
 
-    def default(self, o):
-        # pylint: disable=method-hidden
+    def default(self, obj, **kwargs):
         """
-        Override default method from JSONEncoder to change serializer
-        :param o: Object e.g. dict, list that will be serialized
-        :return: serialized object
+        Override serialization of ``DefaultJSONProvider`` for ``datetime`` and ``bytes`` objects.
+
+        :param obj: Object e.g. dict, list that will be serialized.
+        :return: Serialized object as a string.
         """
 
         from aiida.restapi.common.config import SERIALIZER_CONFIG
 
         # Treat the datetime objects
-        if isinstance(o, datetime):
+        if isinstance(obj, datetime):
             if 'datetime_format' in SERIALIZER_CONFIG and SERIALIZER_CONFIG['datetime_format'] != 'default':
                 if SERIALIZER_CONFIG['datetime_format'] == 'asinput':
-                    if o.utcoffset() is not None:
-                        o = o - o.utcoffset()
-                        return '-'.join([str(o.year), str(o.month).zfill(2),
-                                         str(o.day).zfill(2)]) + 'T' + \
+                    if obj.utcoffset() is not None:
+                        obj = obj - obj.utcoffset()
+                        return '-'.join([str(obj.year), str(obj.month).zfill(2),
+                                         str(obj.day).zfill(2)]) + 'T' + \
                                ':'.join([str(
-                                   o.hour).zfill(2), str(o.minute).zfill(2),
-                                         str(o.second).zfill(2)])
+                                   obj.hour).zfill(2), str(obj.minute).zfill(2),
+                                         str(obj.second).zfill(2)])
 
         # To support bytes objects, try to decode to a string
         try:
-            return o.decode('utf-8')
+            return obj.decode('utf-8')
         except (UnicodeDecodeError, AttributeError):
             pass
 
         # If not returned yet, do it in the default way
-        return JSONEncoder.default(self, o)
+        return super().default(obj, **kwargs)
 
 
 class Utils:
     """
     A class that gathers all the utility functions for parsing URI,
     validating request, pass it to the translator, and building HTTP response
 
@@ -215,15 +215,15 @@
             raise RestInputValidationError('The requested URL is not found on the server.')
 
         return (resource_type, page, node_id, query_type)
 
     def validate_request(
         self, limit=None, offset=None, perpage=None, page=None, query_type=None, is_querystring_defined=False
     ):
-        # pylint: disable=fixme,no-self-use,too-many-arguments,too-many-branches
+        # pylint: disable=fixme,too-many-arguments,too-many-branches
         """
         Performs various checks on the consistency of the request.
         Add here all the checks that you want to do, except validity of the page
         number that is done in paginate().
         Future additional checks must be added here
         """
 
@@ -302,15 +302,15 @@
         if page > 1:
             prev_page = page - 1
 
         next_page = None
         if page < last_page:
             next_page = page + 1
 
-        rel_pages = dict(prev=prev_page, next=next_page, first=first_page, last=last_page)
+        rel_pages = {'prev': prev_page, 'next': next_page, 'first': first_page, 'last': last_page}
 
         return (limit, offset, rel_pages)
 
     def build_headers(self, rel_pages=None, url=None, total_count=None):
         """
         Construct the header dictionary for an HTTP response. It includes related
         pages, total count of results (before pagination).
@@ -438,15 +438,15 @@
         by a "tolerant" operator which checks whether the datetime is in an
         interval.
 
         :return: a suitable entry of the filter dictionary
         """
 
         if not isinstance(dtobj, DatetimePrecision):
-            TypeError('dtobj argument has to be a DatetimePrecision object')
+            raise TypeError('dtobj argument has to be a DatetimePrecision object')
 
         reference_datetime = dtobj.dtobj
         precision = dtobj.precision
 
         ## Define interval according to the precision
         if precision == 1:
             delta_time = timedelta(days=1)
@@ -649,15 +649,15 @@
                     filter_value = self.build_datetime_filter(field_value)
                 else:
                     filter_value = {self.op_conv_map[field[1]]: field_value}
 
                 # Here I treat the AND clause
                 if field_counts[field_key] > 1:
 
-                    if field_key not in filters.keys():
+                    if field_key not in filters:
                         filters.update({field_key: {'and': [filter_value]}})
                     else:
                         filters[field_key]['and'].append(filter_value)
                 else:
                     filters.update({field_key: filter_value})
 
         # #Impose defaults if needed
@@ -766,24 +766,24 @@
 
         ########################################################################
 
         # Convert datetime value to datetime object
         value_datetime.setParseAction(validate_time)
 
         # More General types
-        value = (value_string | value_bool | value_datetime | value_num | value_orderby)
+        value = value_string | value_bool | value_datetime | value_num | value_orderby
         # List of values (I do not check the homogeneity of the types of values,
         # query builder will do it somehow)
         value_list = Group(value + OneOrMore(Suppress(',') + value) + Optional(Suppress(',')))
 
         # Fields
         single_field = Group(key + operator + value)
         list_field = Group(key + (Literal('=in=') | Literal('=notin=')) + value_list)
         orderby_field = Group(key + Literal('=') + value_list)
-        field = (list_field | orderby_field | single_field)
+        field = list_field | orderby_field | single_field
 
         # Fields separator
         separator = Suppress(Literal('&'))
 
         # General query string
         general_grammar = SS() + Optional(field) + ZeroOrMore(
             separator + field) + \
```

### Comparing `aiida_core-2.3.1/aiida/restapi/resources.py` & `aiida_core-2.4.0/aiida/restapi/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # Copyright (c), The AiiDA team. All rights reserved.                     #
 # This file is part of the AiiDA code.                                    #
 #                                                                         #
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-core #
 # For further information on the license, see the LICENSE.txt file        #
 # For further information please visit http://www.aiida.net               #
 ###########################################################################
+# pylint: disable=use-dict-literal
 """ Resources for REST API """
 from urllib.parse import unquote
 
 from flask import make_response, request
 from flask_restful import Resource
 
 from aiida.common.lang import classproperty
```

### Comparing `aiida_core-2.3.1/aiida/restapi/run_api.py` & `aiida_core-2.4.0/aiida/restapi/run_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,16 +91,16 @@
 
     # Allow cross-origin resource sharing
     cors_prefix = r'{}/*'.format(config_module.API_CONFIG['PREFIX'])
     CORS(app, resources={cors_prefix: {'origins': '*'}})
 
     # Configure the serializer
     if config_module.SERIALIZER_CONFIG:
-        from aiida.restapi.common.utils import CustomJSONEncoder
-        app.json_encoder = CustomJSONEncoder
+        from aiida.restapi.common.utils import CustomJSONProvider
+        app.json = CustomJSONProvider(app)
 
     # Set up WSGI profiler if requested
     if wsgi_profile:
         from werkzeug.middleware.profiler import ProfilerMiddleware
 
         app.config['PROFILE'] = True
         app.wsgi_app = ProfilerMiddleware(app.wsgi_app, restrictions=[30])
```

### Comparing `aiida_core-2.3.1/aiida/restapi/translator/__init__.py` & `aiida_core-2.4.0/aiida/restapi/translator/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/restapi/translator/base.py` & `aiida_core-2.4.0/aiida/restapi/translator/base.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/restapi/translator/computer.py` & `aiida_core-2.4.0/aiida/restapi/translator/computer.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     _aiida_type = 'Computer'
 
     # If True (False) the corresponding AiiDA class has (no) uuid property
     _has_uuid = True
 
     _result_type = __label__
 
-    def get_projectable_properties(self):
+    def get_projectable_properties(self):  # pylint: disable=arguments-differ
         """
         Get projectable properties specific for Computer
         :return: dict of projectable properties and column_order list
         """
         from aiida.common.exceptions import EntryPointError
         from aiida.plugins.entry_point import get_entry_points
```

### Comparing `aiida_core-2.3.1/aiida/restapi/translator/group.py` & `aiida_core-2.4.0/aiida/restapi/translator/group.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     _aiida_type = 'groups.Group'
 
     # If True (False) the corresponding AiiDA class has (no) uuid property
     _has_uuid = True
 
     _result_type = __label__
 
-    def get_projectable_properties(self):
+    def get_projectable_properties(self):  # pylint: disable=arguments-differ
         """
         Get projectable properties specific for Group
         :return: dict of projectable properties and column_order list
         """
         projectable_properties = {
             'description': {
                 'display_name': 'Description',
```

### Comparing `aiida_core-2.3.1/aiida/restapi/translator/nodes/__init__.py` & `aiida_core-2.4.0/aiida/restapi/translator/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/restapi/translator/nodes/data/__init__.py` & `aiida_core-2.4.0/aiida/restapi/translator/nodes/data/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/restapi/translator/nodes/data/array/__init__.py` & `aiida_core-2.4.0/aiida/restapi/translator/nodes/data/array/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/restapi/translator/nodes/data/array/bands.py` & `aiida_core-2.4.0/aiida/restapi/translator/nodes/data/array/bands.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     _aiida_class = BandsData
     # The string name of the AiiDA class
     _aiida_type = 'data.core.array.bands.BandsData'
 
     _result_type = __label__
 
     @staticmethod
-    def get_derived_properties(node):
+    def get_derived_properties(node):  # pylint: disable=arguments-differ
         """
         Returns: data in a format required by dr.js to visualize a 2D plot
         with multiple data series.
 
         Strategy: I take advantage of the export functionality of BandsData
         objects. The raw export has to be filtered for string escape characters.
         this is done by decoding the string returned by node._exportcontent.
```

### Comparing `aiida_core-2.3.1/aiida/restapi/translator/nodes/data/cif.py` & `aiida_core-2.4.0/aiida/restapi/translator/nodes/data/cif.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     _aiida_class = CifData
     # The string name of the AiiDA class
     _aiida_type = 'data.core.cif.CifData'
 
     _result_type = __label__
 
     @staticmethod
-    def get_derived_properties(node):
+    def get_derived_properties(node):  # pylint: disable=arguments-differ
         """
         Generic function extended for cif. Currently
         it is not implemented.
 
         :param node: node object
         :returns: empty dict
         """
```

### Comparing `aiida_core-2.3.1/aiida/restapi/translator/nodes/data/code.py` & `aiida_core-2.4.0/aiida/restapi/translator/nodes/process/calculation/calcfunction.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,39 +4,39 @@
 # This file is part of the AiiDA code.                                    #
 #                                                                         #
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-core #
 # For further information on the license, see the LICENSE.txt file        #
 # For further information please visit http://www.aiida.net               #
 ###########################################################################
 """
-Translator for code
+Translator for calcfunction node
 """
 
-from aiida.restapi.translator.nodes.data import DataTranslator
+from aiida.restapi.translator.nodes.process.process import ProcessTranslator
 
 
-class CodeTranslator(DataTranslator):
+class CalcFunctionTranslator(ProcessTranslator):
     """
-    Translator relative to resource 'codes' and aiida class Code
+    Translator relative to resource 'calcfunction' and aiida class Calculation
     """
 
     # A label associated to the present class (coincides with the resource name)
-    __label__ = 'codes'
+    __label__ = 'calcfunction'
     # The AiiDA class one-to-one associated to the present class
-    from aiida.orm import Code
-    _aiida_class = Code
+    from aiida.orm import CalcFunctionNode
+    _aiida_class = CalcFunctionNode
     # The string name of the AiiDA class
-    _aiida_type = 'data.core.code.Code'
+    _aiida_type = 'process.calculation.calcfunction.CalcFunctionNode'
 
     _result_type = __label__
 
     @staticmethod
-    def get_derived_properties(node):
+    def get_derived_properties(node):  # pylint: disable=arguments-differ
         """
-        Generic function extended for codes data. Currently
+        Generic function extended for calcfunction. Currently
         it is not implemented.
 
         :param node: node object
         :returns: empty dict
         """
         response = {}
```

### Comparing `aiida_core-2.3.1/aiida/restapi/translator/nodes/data/kpoints.py` & `aiida_core-2.4.0/aiida/restapi/translator/nodes/data/kpoints.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     # The string name of the AiiDA class
     _aiida_type = 'data.core.array.kpoints.KpointsData'
 
     _result_type = __label__
 
     @staticmethod
     def get_derived_properties(node):
-        # pylint: disable=too-many-locals,too-many-statements,too-many-branches
+        # pylint: disable=too-many-locals,too-many-statements,too-many-branches,arguments-differ
         """
 
         Returns: data in a format required by dr.js to visualize a 2D plot
         with multiple data series.
 
         Strategy: For the time being rely on the function implemented in
         seekpath to calculate brillouin zone faces, and triangulate them. The
```

### Comparing `aiida_core-2.3.1/aiida/restapi/translator/nodes/data/structure.py` & `aiida_core-2.4.0/aiida/restapi/translator/nodes/data/structure.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     _aiida_class = StructureData
     # The string name of the AiiDA class
     _aiida_type = 'data.core.structure.StructureData'
 
     _result_type = __label__
 
     @staticmethod
-    def get_derived_properties(node):
+    def get_derived_properties(node):  # pylint: disable=arguments-differ
         """
         Returns: derived properties of the structure.
         """
         response = {}
 
         # Add extra information
         response['dimensionality'] = node.get_dimensionality()
```

### Comparing `aiida_core-2.3.1/aiida/restapi/translator/nodes/data/upf.py` & `aiida_core-2.4.0/aiida/restapi/translator/nodes/data/upf.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     _aiida_class = UpfData
     # The string name of the AiiDA class
     _aiida_type = 'data.core.upf.UpfData'
 
     _result_type = __label__
 
     @staticmethod
-    def get_derived_properties(node):
+    def get_derived_properties(node):  # pylint: disable=arguments-differ
         """
         :param node: node object
         :returns: empty dict
         """
         response = {}
 
         return response
```

### Comparing `aiida_core-2.3.1/aiida/restapi/translator/nodes/node.py` & `aiida_core-2.4.0/aiida/restapi/translator/nodes/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
                 'cls': self._aiida_class,
                 'tag': self._result_type,
                 'edge_tag': edge_tag,
                 self._result_type: self.__label__
             })
             self._query_help['project'][edge_tag] = [{'label': {}}, {'type': {}}]
 
-    def set_query(
+    def set_query(  # pylint: disable=arguments-renamed
         self,
         filters=None,
         orders=None,
         projections=None,
         query_type=None,
         node_id=None,
         download_format=None,
@@ -355,15 +355,15 @@
             # N.B. pkgutil.walk_packages requires a LIST of paths
 
             full_path_base = os.path.join(package_path, name)
             if is_pkg:
                 # re-implementation of deprecated `imp.load_package`
                 if os.path.isdir(full_path_base):
                     #Adds an extension to check for __init__ file in the package directory
-                    extensions = (importlib.machinery.SOURCE_SUFFIXES[:] + importlib.machinery.BYTECODE_SUFFIXES[:])
+                    extensions = importlib.machinery.SOURCE_SUFFIXES[:] + importlib.machinery.BYTECODE_SUFFIXES[:]
                     for extension in extensions:
                         init_path = os.path.join(full_path_base, '__init__' + extension)
                         if os.path.exists(init_path):
                             path = init_path
                             break
                     else:
                         raise ValueError(f'{full_path_base!r} is not a package')
@@ -758,15 +758,15 @@
             'total_no_of_outgoings': total_no_of_outgoings,
             'sent_no_of_incomings': sent_no_of_incomings,
             'sent_no_of_outgoings': sent_no_of_outgoings
         }]
 
         return {'nodes': nodes, 'metadata': metadata}
 
-    def get_projectable_properties(self):
+    def get_projectable_properties(self):  # pylint: disable=arguments-differ
         """
         Get projectable properties specific for Node
         :return: dict of projectable properties and column_order list
         """
         projectable_properties = {
             'creator': {
                 'display_name': 'Creator',
```

### Comparing `aiida_core-2.3.1/aiida/restapi/translator/nodes/process/__init__.py` & `aiida_core-2.4.0/aiida/restapi/translator/nodes/process/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/restapi/translator/nodes/process/calculation/__init__.py` & `aiida_core-2.4.0/aiida/restapi/translator/nodes/process/calculation/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/restapi/translator/nodes/process/calculation/calcfunction.py` & `aiida_core-2.4.0/aiida/restapi/translator/nodes/process/workflow/workfunction.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,39 +4,39 @@
 # This file is part of the AiiDA code.                                    #
 #                                                                         #
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-core #
 # For further information on the license, see the LICENSE.txt file        #
 # For further information please visit http://www.aiida.net               #
 ###########################################################################
 """
-Translator for calcfunction node
+Translator for workfunction node
 """
 
 from aiida.restapi.translator.nodes.process.process import ProcessTranslator
 
 
-class CalcFunctionTranslator(ProcessTranslator):
+class WorkFunctionTranslator(ProcessTranslator):
     """
     Translator relative to resource 'calcfunction' and aiida class Calculation
     """
 
     # A label associated to the present class (coincides with the resource name)
-    __label__ = 'calcfunction'
+    __label__ = 'workfunction'
     # The AiiDA class one-to-one associated to the present class
-    from aiida.orm import CalcFunctionNode
-    _aiida_class = CalcFunctionNode
+    from aiida.orm import WorkFunctionNode
+    _aiida_class = WorkFunctionNode
     # The string name of the AiiDA class
-    _aiida_type = 'process.calculation.calcfunction.CalcFunctionNode'
+    _aiida_type = 'process.workflow.workfunction.WorkFunctionNode'
 
     _result_type = __label__
 
     @staticmethod
-    def get_derived_properties(node):
+    def get_derived_properties(node):  # pylint: disable=arguments-differ
         """
-        Generic function extended for calcfunction. Currently
+        Generic function extended for workfunction. Currently
         it is not implemented.
 
         :param node: node object
         :returns: empty dict
         """
         response = {}
```

### Comparing `aiida_core-2.3.1/aiida/restapi/translator/nodes/process/calculation/calcjob.py` & `aiida_core-2.4.0/aiida/restapi/translator/nodes/process/calculation/calcjob.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,15 +56,15 @@
             response['status'] = 200
             response['data'] = 'This node does not have retrieved folder'
             return response
 
         return NodeTranslator.get_repo_list(retrieved_folder_node, filename)
 
     @staticmethod
-    def get_derived_properties(node):
+    def get_derived_properties(node):  # pylint: disable=arguments-differ
         """
         Generic function extended for calcjob. Currently
         it is not implemented.
 
         :param node: node object
         :returns: empty dict
         """
```

### Comparing `aiida_core-2.3.1/aiida/restapi/translator/nodes/process/process.py` & `aiida_core-2.4.0/aiida/restapi/translator/nodes/process/process.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/restapi/translator/nodes/process/workflow/__init__.py` & `aiida_core-2.4.0/aiida/restapi/translator/nodes/process/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/restapi/translator/nodes/process/workflow/workchain.py` & `aiida_core-2.4.0/aiida/restapi/translator/nodes/process/workflow/workchain.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     _aiida_class = WorkChainNode
     # The string name of the AiiDA class
     _aiida_type = 'process.workflow.workchain.WorkChainNode'
 
     _result_type = __label__
 
     @staticmethod
-    def get_derived_properties(node):
+    def get_derived_properties(node):  # pylint: disable=arguments-differ
         """
         Generic function extended for workchain. Currently
         it is not implemented.
 
         :param node: node object
         :returns: empty dict
         """
```

### Comparing `aiida_core-2.3.1/aiida/restapi/translator/nodes/process/workflow/workfunction.py` & `aiida_core-2.4.0/aiida/restapi/translator/nodes/data/code.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,39 +4,39 @@
 # This file is part of the AiiDA code.                                    #
 #                                                                         #
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-core #
 # For further information on the license, see the LICENSE.txt file        #
 # For further information please visit http://www.aiida.net               #
 ###########################################################################
 """
-Translator for workfunction node
+Translator for code
 """
 
-from aiida.restapi.translator.nodes.process.process import ProcessTranslator
+from aiida.restapi.translator.nodes.data import DataTranslator
 
 
-class WorkFunctionTranslator(ProcessTranslator):
+class CodeTranslator(DataTranslator):
     """
-    Translator relative to resource 'calcfunction' and aiida class Calculation
+    Translator relative to resource 'codes' and aiida class Code
     """
 
     # A label associated to the present class (coincides with the resource name)
-    __label__ = 'workfunction'
+    __label__ = 'codes'
     # The AiiDA class one-to-one associated to the present class
-    from aiida.orm import WorkFunctionNode
-    _aiida_class = WorkFunctionNode
+    from aiida.orm import Code
+    _aiida_class = Code
     # The string name of the AiiDA class
-    _aiida_type = 'process.workflow.workfunction.WorkFunctionNode'
+    _aiida_type = 'data.core.code.Code'
 
     _result_type = __label__
 
     @staticmethod
-    def get_derived_properties(node):
+    def get_derived_properties(node):  # pylint: disable=arguments-differ
         """
-        Generic function extended for workfunction. Currently
+        Generic function extended for codes data. Currently
         it is not implemented.
 
         :param node: node object
         :returns: empty dict
         """
         response = {}
```

### Comparing `aiida_core-2.3.1/aiida/restapi/translator/user.py` & `aiida_core-2.4.0/aiida/restapi/translator/user.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     # If True (False) the corresponding AiiDA class has (no) uuid property
     _has_uuid = False
 
     _result_type = __label__
 
     _default_projections = ['id', 'first_name', 'last_name', 'institution']
 
-    def get_projectable_properties(self):
+    def get_projectable_properties(self):  # pylint: disable=arguments-differ
         """
         Get projectable properties specific for User
         :return: dict of projectable properties and column_order list
         """
         projectable_properties = {
             'id': {
                 'display_name': 'Id',
```

### Comparing `aiida_core-2.3.1/aiida/schedulers/__init__.py` & `aiida_core-2.4.0/aiida/schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/schedulers/datastructures.py` & `aiida_core-2.4.0/aiida/schedulers/datastructures.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,16 +17,17 @@
 from __future__ import annotations
 
 import abc
 from dataclasses import dataclass, field
 from datetime import datetime, timezone
 import enum
 import json
+from typing import TYPE_CHECKING
 
-from aiida.common import AIIDA_LOGGER
+from aiida.common import AIIDA_LOGGER, CodeRunMode
 from aiida.common.extendeddicts import AttributeDict, DefaultFieldsAttributeDict
 from aiida.common.timezone import make_aware, timezone_from_name
 
 SCHEDULER_LOGGER = AIIDA_LOGGER.getChild('scheduler')
 
 __all__ = (
     'JobState', 'JobResource', 'JobTemplate', 'JobInfo', 'NodeNumberJobResource', 'ParEnvJobResource', 'MachineInfo'
@@ -104,14 +105,20 @@
     _default_fields = (
         'num_machines',
         'num_mpiprocs_per_machine',
         'num_cores_per_machine',
         'num_cores_per_mpiproc',
     )
 
+    if TYPE_CHECKING:
+        num_machines: int
+        num_mpiprocs_per_machine: int
+        num_cores_per_machine: int
+        num_cores_per_mpiproc: int
+
     @classmethod
     def validate_resources(cls, **kwargs):
         """Validate the resources against the job resource class of this scheduler.
 
         :param kwargs: dictionary of values to define the job resources
         :return: attribute dictionary with the parsed parameters populated
         :raises ValueError: if the resources are invalid or incomplete
@@ -189,14 +196,18 @@
     """`JobResource` for schedulers that support the specification of a parallel environment and number of MPI procs."""
 
     _default_fields = (
         'parallel_env',
         'tot_num_mpiprocs',
     )
 
+    if TYPE_CHECKING:
+        parallel_env: str
+        tot_num_mpiprocs: int
+
     @classmethod
     def validate_resources(cls, **kwargs):
         """Validate the resources against the job resource class of this scheduler.
 
         :param kwargs: dictionary of values to define the job resources
         :return: attribute dictionary with the parsed parameters populated
         :raises ValueError: if the resources are invalid or incomplete
@@ -362,14 +373,42 @@
         'prepend_text',
         'append_text',
         'import_sys_environment',
         'codes_run_mode',
         'codes_info',
     )
 
+    if TYPE_CHECKING:
+        shebang: str
+        submit_as_hold: bool
+        rerunnable: bool
+        job_environment: dict[str, str] | None
+        environment_variables_double_quotes: bool | None
+        working_directory: str
+        email: str
+        email_on_started: bool
+        email_on_terminated: bool
+        job_name: str
+        sched_output_path: str
+        sched_error_path: str
+        sched_join_files: bool
+        queue_name: str
+        account: str
+        qos: str
+        job_resource: JobResource
+        priority: str
+        max_memory_kb: int | None
+        max_wallclock_seconds: int
+        custom_scheduler_commands: str
+        prepend_text: str
+        append_text: str
+        import_sys_environment: bool | None
+        codes_run_mode: CodeRunMode
+        codes_info: list[JobTemplateCodeInfo]
+
 
 @dataclass
 class JobTemplateCodeInfo:
     """
     Data structure to communicate to a `Scheduler` how a code should be run in submit script.
 
     `Scheduler.get_submit_script` will pass a list of these objects to `Scheduler._get_run_line` which
@@ -470,14 +509,37 @@
     _default_fields = (
         'job_id', 'title', 'exit_status', 'terminating_signal', 'annotation', 'job_state', 'job_substate',
         'allocated_machines', 'job_owner', 'num_mpiprocs', 'num_cpus', 'num_machines', 'queue_name', 'account', 'qos',
         'wallclock_time_seconds', 'requested_wallclock_time_seconds', 'cpu_time', 'submission_time', 'dispatch_time',
         'finish_time'
     )
 
+    if TYPE_CHECKING:
+        job_id: str
+        title: str
+        exit_status: int
+        terminating_signal: int
+        annotation: str
+        job_state: JobState
+        job_substate: str
+        allocated_machines: list[MachineInfo]
+        job_owner: str
+        num_mpiprocs: int
+        num_cpus: int
+        num_machines: int
+        queue_name: str
+        account: str
+        qos: str
+        wallclock_time_seconds: int
+        requested_wallclock_time_seconds: int
+        cpu_time: int
+        submission_time: datetime
+        dispatch_time: datetime
+        finish_time: datetime
+
     # If some fields require special serializers, specify them here.
     # You then need to define also the respective _serialize_FIELDTYPE and
     # _deserialize_FIELDTYPE methods
     _special_serializers = {
         'submission_time': 'date',
         'dispatch_time': 'date',
         'finish_time': 'date',
```

### Comparing `aiida_core-2.3.1/aiida/schedulers/plugins/__init__.py` & `aiida_core-2.4.0/aiida/schedulers/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/schedulers/plugins/direct.py` & `aiida_core-2.4.0/aiida/schedulers/plugins/direct.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,19 @@
     'R': JobState.RUNNING,
     'S': JobState.RUNNING,
     'T': JobState.SUSPENDED,
     'U': JobState.RUNNING,
     'W': JobState.RUNNING,
     'X': JobState.DONE,
     'Z': JobState.DONE,
+    '?': JobState.UNDETERMINED,
+    # `ps` can sometimes return `?` for the state of a process on macOS. This corresponds to an "unknown" state, see:
+    #
+    # https://apple.stackexchange.com/q/460394/497071
+    #
     # Not sure about these three, I comment them out (they used to be in
     # here, but they don't appear neither on ubuntu nor on Mac)
     #    'F': JobState.DONE,
     #    'H': JobState.QUEUED_HELD,
     #    'Q': JobState.QUEUED,
 }
 
@@ -74,15 +79,15 @@
         return False
 
 
 class DirectScheduler(aiida.schedulers.Scheduler):
     """
     Support for the direct execution bypassing schedulers.
     """
-    _logger = aiida.schedulers.Scheduler._logger.getChild('direct')
+    _logger = aiida.schedulers.Scheduler._logger.getChild('direct')  # pylint: disable=protected-access
 
     # Query only by list of jobs and not by user
     _features = {
         'can_query_by_user': True,
     }
 
     # The class to be used for the job resource.
```

### Comparing `aiida_core-2.3.1/aiida/schedulers/plugins/lsf.py` & `aiida_core-2.4.0/aiida/schedulers/plugins/lsf.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,15 +174,15 @@
 
 
 class LsfScheduler(aiida.schedulers.Scheduler):
     """
     Support for the IBM LSF scheduler
     'https://www-01.ibm.com/support/knowledgecenter/SSETD4_9.1.2/lsf_welcome.html'
     """
-    _logger = aiida.schedulers.Scheduler._logger.getChild('lsf')
+    _logger = aiida.schedulers.Scheduler._logger.getChild('lsf')  # pylint: disable=protected-access
 
     # Query only by list of jobs and not by user
     _features = {
         'can_query_by_user': False,
     }
 
     # The class to be used for the job resource.
```

### Comparing `aiida_core-2.3.1/aiida/schedulers/plugins/pbsbaseclasses.py` & `aiida_core-2.4.0/aiida/schedulers/plugins/pbsbaseclasses.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
                 )
 
         elif resources.num_cores_per_mpiproc is not None:
             if resources.num_cores_per_mpiproc < 1:
                 raise ValueError('num_cores_per_mpiproc must be greater than or equal to one.')
 
             # In this plugin we never used num_cores_per_mpiproc so if it is not defined it is OK.
-            resources.num_cores_per_machine = (resources.num_cores_per_mpiproc * resources.num_mpiprocs_per_machine)
+            resources.num_cores_per_machine = resources.num_cores_per_mpiproc * resources.num_mpiprocs_per_machine
 
         return resources
 
 
 class PbsBaseClass(Scheduler):
     """
     Base class with support for the PBSPro scheduler
@@ -559,30 +559,30 @@
 
             try:
                 this_job.queue_name = raw_data['queue']
             except KeyError:
                 _LOGGER.debug(f"No 'queue' field for job id {this_job.job_id}")
 
             try:
-                this_job.requested_wallclock_time = (self._convert_time(raw_data['resource_list.walltime']))  # pylint: disable=invalid-name
+                this_job.requested_wallclock_time = self._convert_time(raw_data['resource_list.walltime'])
             except KeyError:
                 _LOGGER.debug(f"No 'resource_list.walltime' field for job id {this_job.job_id}")
             except ValueError:
                 _LOGGER.warning(f"Error parsing 'resource_list.walltime' for job id {this_job.job_id}")
 
             try:
-                this_job.wallclock_time_seconds = (self._convert_time(raw_data['resources_used.walltime']))
+                this_job.wallclock_time_seconds = self._convert_time(raw_data['resources_used.walltime'])
             except KeyError:
                 # May not have started yet
                 pass
             except ValueError:
                 _LOGGER.warning(f"Error parsing 'resources_used.walltime' for job id {this_job.job_id}")
 
             try:
-                this_job.cpu_time = (self._convert_time(raw_data['resources_used.cput']))
+                this_job.cpu_time = self._convert_time(raw_data['resources_used.cput'])
             except KeyError:
                 # May not have started yet
                 pass
             except ValueError:
                 _LOGGER.warning(f"Error parsing 'resources_used.cput' for job id {this_job.job_id}")
 
             #
```

### Comparing `aiida_core-2.3.1/aiida/schedulers/plugins/pbspro.py` & `aiida_core-2.4.0/aiida/schedulers/plugins/pbspro.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/schedulers/plugins/sge.py` & `aiida_core-2.4.0/aiida/schedulers/plugins/sge.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     pass
 
 
 class SgeScheduler(aiida.schedulers.Scheduler):
     """
     Support for the Sun Grid Engine scheduler and its variants/forks (Son of Grid Engine, Oracle Grid Engine, ...)
     """
-    _logger = aiida.schedulers.Scheduler._logger.getChild('sge')
+    _logger = aiida.schedulers.Scheduler._logger.getChild('sge')  # pylint: disable=protected-access
 
     # For SGE, we can have a good qstat xml output by querying by
     # user, but not by job id
     _features = {
         'can_query_by_user': True,
     }
```

### Comparing `aiida_core-2.3.1/aiida/schedulers/plugins/slurm.py` & `aiida_core-2.4.0/aiida/schedulers/plugins/slurm.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
                     ' particular it should be a multiple of `num_cores_per_mpiproc` and/or `num_mpiprocs_per_machine`'
                 )
 
         elif resources.num_cores_per_machine is not None:
             if resources.num_cores_per_machine < 1:
                 raise ValueError('num_cores_per_machine must be greater than or equal to one.')
 
-            resources.num_cores_per_mpiproc = (resources.num_cores_per_machine / resources.num_mpiprocs_per_machine)
+            resources.num_cores_per_mpiproc = resources.num_cores_per_machine / resources.num_mpiprocs_per_machine
             if int(resources.num_cores_per_mpiproc) != resources.num_cores_per_mpiproc:
                 raise ValueError(
                     '`num_cores_per_machine` must be equal to `num_cores_per_mpiproc * num_mpiprocs_per_machine` and in'
                     ' particular it should be a multiple of `num_cores_per_mpiproc` and/or `num_mpiprocs_per_machine`'
                 )
             resources.num_cores_per_mpiproc = int(resources.num_cores_per_mpiproc)
 
@@ -581,24 +581,24 @@
             # this_job.allocated_machines undefined
             if this_job.job_state == JobState.RUNNING:
                 this_job.allocated_machines_raw = thisjob_dict['allocated_machines']
 
             this_job.queue_name = thisjob_dict['partition']
 
             try:
-                walltime = (self._convert_time(thisjob_dict['time_limit']))
+                walltime = self._convert_time(thisjob_dict['time_limit'])
                 this_job.requested_wallclock_time_seconds = walltime  # pylint: disable=invalid-name
             except ValueError:
                 self.logger.warning(f'Error parsing the time limit for job id {this_job.job_id}')
 
             # Only if it is RUNNING; otherwise it is not meaningful,
             # and may be not set (in my test, it is set to zero)
             if this_job.job_state == JobState.RUNNING:
                 try:
-                    this_job.wallclock_time_seconds = (self._convert_time(thisjob_dict['time_used']))
+                    this_job.wallclock_time_seconds = self._convert_time(thisjob_dict['time_used'])
                 except ValueError:
                     self.logger.warning(f'Error parsing time_used for job id {this_job.job_id}')
 
                 try:
                     this_job.dispatch_time = self._parse_time_string(thisjob_dict['dispatch_time'])
                 except ValueError:
                     self.logger.warning(f'Error parsing dispatch_time for job id {this_job.job_id}')
```

### Comparing `aiida_core-2.3.1/aiida/schedulers/plugins/torque.py` & `aiida_core-2.4.0/aiida/schedulers/plugins/torque.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/schedulers/scheduler.py` & `aiida_core-2.4.0/aiida/schedulers/scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,15 +185,15 @@
         footer = self._get_submit_script_footer(job_tmpl)
         if footer:
             script_lines.append(footer)
             script_lines.append(empty_line)
 
         return '\n'.join(script_lines)
 
-    def _get_submit_script_environment_variables(self, template: JobTemplate) -> str:  # pylint: disable=no-self-use
+    def _get_submit_script_environment_variables(self, template: JobTemplate) -> str:
         """Return the part of the submit script header that defines environment variables.
 
         :parameter template: a `aiida.schedulers.datastrutures.JobTemplate` instance.
         :return: string containing environment variable declarations.
         """
         if not isinstance(template.job_environment, dict):
             raise ValueError('If you provide job_environment, it must be a dictionary')
@@ -217,15 +217,15 @@
 
     def _get_submit_script_footer(self, job_tmpl: JobTemplate) -> str:
         """Return the submit script final part, using the parameters from the job template.
 
         :param job_tmpl: a `JobTemplate` instance with relevant parameters set.
         :return: string with the submission script footer.
         """
-        # pylint: disable=no-self-use,unused-argument
+        # pylint: disable=unused-argument
         return ''
 
     def _get_run_line(self, codes_info: list[JobTemplateCodeInfo], codes_run_mode: CodeRunMode) -> str:
         """Return a string with the line to execute a specific code with specific arguments.
 
         :parameter codes_info: a list of `aiida.scheduler.datastructures.JobTemplateCodeInfo` objects.
             Each contains the information needed to run the code. I.e. `cmdline_params`, `stdin_name`,
@@ -304,15 +304,15 @@
 
         This is typically called after the job has finished, to retrieve the most detailed information possible about
         the job. This is done because most schedulers just make finished jobs disappear from the `qstat` command, and
         instead sometimes it is useful to know some more detailed information about the job exit status, etc.
 
         :raises: :class:`aiida.common.exceptions.FeatureNotAvailable`
         """
-        # pylint: disable=no-self-use,not-callable,unused-argument
+        # pylint: disable=not-callable,unused-argument
         raise exceptions.FeatureNotAvailable('Cannot get detailed job info')
 
     def get_detailed_job_info(self, job_id: str) -> dict[str, str | int]:
         """Return the detailed job info.
 
         This will be a dictionary with the return value, stderr and stdout content returned by calling the command that
         is returned by `_get_detailed_job_info_command`.
```

### Comparing `aiida_core-2.3.1/aiida/sphinxext/__init__.py` & `aiida_core-2.4.0/aiida/sphinxext/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/sphinxext/calcjob.py` & `aiida_core-2.4.0/aiida/sphinxext/calcjob.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/sphinxext/process.py` & `aiida_core-2.4.0/aiida/sphinxext/process.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/sphinxext/workchain.py` & `aiida_core-2.4.0/aiida/sphinxext/workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/__init__.py` & `aiida_core-2.4.0/aiida/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/log.py` & `aiida_core-2.4.0/aiida/storage/log.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/__init__.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/alembic_cli.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/alembic_cli.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/backend.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -301,28 +301,28 @@
         # https://docs.sqlalchemy.org/en/14/changelog/migration_14.html#orm-batch-inserts-with-psycopg2-now-batch-statements-with-returning-in-most-cases
         # by contrast, in sqlite, bulk_insert is faster: https://docs.sqlalchemy.org/en/14/faq/performance.html
         session = self.get_session()
         with (nullcontext() if self.in_transaction else self.transaction()):
             session.bulk_insert_mappings(mapper, rows, render_nulls=True, return_defaults=True)
         return [row['id'] for row in rows]
 
-    def bulk_update(self, entity_type: EntityTypes, rows: List[dict]) -> None:  # pylint: disable=no-self-use
+    def bulk_update(self, entity_type: EntityTypes, rows: List[dict]) -> None:
         mapper, keys = self._get_mapper_from_entity(entity_type, True)
         if not rows:
             return None
         for row in rows:
             if 'id' not in row:
                 raise IntegrityError(f"'id' field not given for {entity_type}: {set(row)}")
             if not keys.issuperset(row):
                 raise IntegrityError(f'Incorrect fields given for {entity_type}: {set(row)} not subset of {keys}')
         session = self.get_session()
         with (nullcontext() if self.in_transaction else self.transaction()):
             session.bulk_update_mappings(mapper, rows)
 
-    def delete_nodes_and_connections(self, pks_to_delete: Sequence[int]) -> None:  # pylint: disable=no-self-use
+    def delete_nodes_and_connections(self, pks_to_delete: Sequence[int]) -> None:
         # pylint: disable=no-value-for-parameter
         from aiida.storage.psql_dos.models.group import DbGroupNode
         from aiida.storage.psql_dos.models.node import DbLink, DbNode
 
         if not self.in_transaction:
             raise AssertionError('Cannot delete nodes and links outside a transaction')
```

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/__init__.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/env.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/env.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,13 +40,13 @@
     )
 
     context.run_migrations()  # pylint: disable=no-member
 
 
 try:
     if context.is_offline_mode():  # pylint: disable=no-member
-        NotImplementedError('This feature is not currently supported.')
+        raise NotImplementedError('This feature is not currently supported.')
 
     run_migrations_online()
 except NameError:
     # This will occur in an environment that is just compiling the documentation
     pass
```

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/utils/__init__.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/utils/calc_state.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/utils/calc_state.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/utils/create_dbattribute.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/utils/create_dbattribute.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/utils/dblog_update.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/utils/dblog_update.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/utils/duplicate_uuids.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/utils/duplicate_uuids.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/utils/integrity.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/utils/integrity.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,20 @@
 #                                                                         #
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-core #
 # For further information on the license, see the LICENSE.txt file        #
 # For further information please visit http://www.aiida.net               #
 ###########################################################################
 # pylint: disable=invalid-name
 """Methods to validate the database integrity and fix violations."""
+from __future__ import annotations
+
+from aiida.common.log import AIIDA_LOGGER
+
+LOGGER = AIIDA_LOGGER.getChild(__file__)
+
 WARNING_BORDER = '*' * 120
 
 # These are all the entry points from the `aiida.calculations` category as registered with the AiiDA registry
 # on Tuesday December 4 at 13:00:00 UTC
 registered_calculation_entry_points = [
     'ase.ase = aiida_ase.calculations.ase:AseCalculation',
     'castep.bs = aiida_castep.calculations.castep:CastepBSCalculation',
@@ -156,53 +162,71 @@
     """
     # pylint: disable=duplicate-string-formatting-argument
     from datetime import datetime
     from tempfile import NamedTemporaryFile
 
     from tabulate import tabulate
 
-    from aiida.cmdline.utils import echo
     from aiida.manage import configuration
 
     global_profile = configuration.get_profile()
     if global_profile and global_profile.is_test_profile:
         return
 
     if action_message is None:
         action_message = 'nothing'
 
     with NamedTemporaryFile(prefix='migration-', suffix='.log', dir='.', delete=False, mode='w+') as handle:
-        echo.echo('')
-        echo.echo_warning(
+        LOGGER.warning(
             '\n{}\nFound one or multiple records that violate the integrity of the database\nViolation reason: {}\n'
             'Performed action: {}\nViolators written to: {}\n{}\n'.format(
                 WARNING_BORDER, reason_message, action_message, handle.name, WARNING_BORDER
             )
         )
 
         handle.write(f'# {datetime.utcnow().isoformat()}\n')
         handle.write(f'# Violation reason: {reason_message}\n')
         handle.write(f'# Performed action: {action_message}\n')
         handle.write('\n')
         handle.write(tabulate(results, headers))
 
 
-# Currently valid hash key
-_HASH_EXTRA_KEY = '_aiida_hash'
-
-
-def drop_hashes(conn):
+def drop_hashes(conn, hash_extra_key: str, entry_point_string: str | None = None) -> None:
     """Drop hashes of nodes.
 
     Print warning only if the DB actually contains nodes.
+
+    :param hash_extra_key: The key in the extras used to store the hash at the time of this migration.
+    :param entry_point_string: Optional entry point string of a node type to narrow the subset of nodes to reset. The
+        value should be a complete entry point string, e.g., ``aiida.node:process.calculation.calcjob`` to drop the hash
+        of all ``CalcJobNode`` rows.
     """
-    # Remove when https://github.com/PyCQA/pylint/issues/1931 is fixed
-    # pylint: disable=no-name-in-module,import-error
     from sqlalchemy.sql import text
 
-    from aiida.cmdline.utils import echo
-    n_nodes = conn.execute(text("""SELECT count(*) FROM db_dbnode;""")).fetchall()[0][0]
-    if n_nodes > 0:
-        echo.echo_warning('Invalidating the hashes of all nodes. Please run "verdi rehash".', bold=True)
+    from aiida.orm.utils.node import get_type_string_from_class
+    from aiida.plugins import load_entry_point_from_string
+
+    if entry_point_string is not None:
+        entry_point = load_entry_point_from_string(entry_point_string)
+        node_type = get_type_string_from_class(entry_point.__module__, entry_point.__name__)
+    else:
+        node_type = None
+
+    if node_type:
+        statement_count = text(f"SELECT count(*) FROM db_dbnode WHERE node_type = '{node_type}';")
+        statement_update = text(
+            f"UPDATE db_dbnode SET extras = extras #- '{{{hash_extra_key}}}'::text[]  WHERE node_type = '{node_type}';"
+        )
+    else:
+        statement_count = text('SELECT count(*) FROM db_dbnode;')
+        statement_update = text(f"UPDATE db_dbnode SET extras = extras #- '{{{hash_extra_key}}}'::text[];")
+
+    node_count = conn.execute(statement_count).fetchall()[0][0]
+
+    if node_count > 0:
+        if entry_point_string:
+            msg = f'Invalidating the hashes of certain nodes. Please run `verdi node rehash -e {entry_point_string}`.'
+        else:
+            msg = 'Invalidating the hashes of all nodes. Please run `verdi node rehash`.'
+        LOGGER.warning(msg)
 
-    statement = text(f"UPDATE db_dbnode SET extras = extras #- '{{{_HASH_EXTRA_KEY}}}'::text[];")
-    conn.execute(statement)
+    conn.execute(statement_update)
```

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/utils/legacy_workflows.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/utils/legacy_workflows.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/utils/migrate_repository.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/utils/migrate_repository.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/utils/parity.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/utils/parity.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/utils/provenance_redesign.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/utils/provenance_redesign.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/utils/reflect.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/utils/reflect.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     however, over time it has changed.
     So is not possible to know declaratively exactly what constraints/indexes are present on a users database,
     withtout knowing the exact django version that created it (and run migrations).
     Therefore, we need to reflect the database's schema, to determine what is present on the database,
     to know what to drop.
     """
 
-    def __init__(self, op: alembic.op) -> None:
+    def __init__(self, op: alembic.op) -> None:  # pylint: disable=invalid-name
         self.op = op  # pylint: disable=invalid-name
         # note, we only want to instatiate the inspector once, since it caches reflection calls to the database
         self.inspector = inspect(op.get_bind())
 
     def reset_cache(self) -> None:
         """Reset the inspector cache."""
         self.inspector = inspect(self.op.get_bind())
```

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/utils/utils.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/utils/utils.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/041a79fc615f_dblog_cleaning.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/041a79fc615f_dblog_cleaning.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/07fac78e6209_drop_computer_transport_params.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/07fac78e6209_drop_computer_transport_params.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/0aebbeab274d_base_data_plugin_type_string.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/0aebbeab274d_base_data_plugin_type_string.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/0edcdd5a30f0_dbgroup_extras.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/0edcdd5a30f0_dbgroup_extras.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/118349c10896_default_link_label.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/118349c10896_default_link_label.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/12536798d4d3_trajectory_symbols_to_attribute.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/12536798d4d3_trajectory_symbols_to_attribute.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,17 +15,14 @@
 Revision ID: 12536798d4d3
 Revises: 37f3d4882837
 Create Date: 2019-01-21 10:15:02.451308
 
 """
 # pylint: disable=invalid-name
 
-# Remove when https://github.com/PyCQA/pylint/issues/1931 is fixed
-# pylint: disable=no-member,no-name-in-module,import-error
-
 from alembic import op
 from sqlalchemy import Integer, String, cast
 from sqlalchemy.dialects.postgresql import JSONB, UUID
 from sqlalchemy.sql import column, func, select, table
 
 from aiida.storage.psql_dos.backend import get_filepath_container
 from aiida.storage.psql_dos.migrations.utils.utils import load_numpy_array_from_repository
```

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/140c971ae0a3_migrate_builtin_calculations.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/140c971ae0a3_migrate_builtin_calculations.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,16 +12,14 @@
 
 Revision ID: 140c971ae0a3
 Revises: 162b99bca4a2
 Create Date: 2018-12-06 12:42:01.897037
 
 """
 from alembic import op
-# Remove when https://github.com/PyCQA/pylint/issues/1931 is fixed
-# pylint: disable=no-name-in-module,import-error
 from sqlalchemy.sql import text
 
 # revision identifiers, used by Alembic.
 revision = '140c971ae0a3'
 down_revision = '162b99bca4a2'
 branch_labels = None
 depends_on = None
```

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/162b99bca4a2_drop_dbcalcstate.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/162b99bca4a2_drop_dbcalcstate.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/1830c8430131_drop_node_columns_nodeversion_public.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/1830c8430131_drop_node_columns_nodeversion_public.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/1b8ed3425af9_remove_legacy_workflows.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/1b8ed3425af9_remove_legacy_workflows.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/1de112340b16_django_parity_1.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/1de112340b16_django_parity_1.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/1de112340b17_django_parity_2.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/1de112340b17_django_parity_2.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/1de112340b18_django_parity_3.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/1de112340b18_django_parity_3.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/1feaea71bd5a_migrate_repository.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/1feaea71bd5a_migrate_repository.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/239cea6d2452_provenance_redesign.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/239cea6d2452_provenance_redesign.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/26d561acd560_data_migration_legacy_job_calculations.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/26d561acd560_data_migration_legacy_job_calculations.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/34a831f4286d_entry_point_core_prefix.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/34a831f4286d_entry_point_core_prefix.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/35d4ee9a1b0e_code_hidden_attr_to_extra.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/35d4ee9a1b0e_code_hidden_attr_to_extra.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/375c2db70663_dblog_uuid_uniqueness_constraint.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/375c2db70663_dblog_uuid_uniqueness_constraint.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/37f3d4882837_make_all_uuid_columns_unique.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/37f3d4882837_make_all_uuid_columns_unique.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,17 +15,14 @@
 Create Date: 2018-11-17 17:18:58.691209
 
 """
 # pylint: disable=invalid-name
 
 from alembic import op
 
-# Remove when https://github.com/PyCQA/pylint/issues/1931 is fixed
-# pylint: disable=no-member,no-name-in-module,import-error
-
 # revision identifiers, used by Alembic.
 revision = '37f3d4882837'
 down_revision = '6a5c2ea1439d'
 branch_labels = None
 depends_on = None
 
 tables = ['db_dbcomment', 'db_dbcomputer', 'db_dbgroup', 'db_dbworkflow']
```

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/3d6190594e19_remove_dbcomputer_enabled.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/3d6190594e19_remove_dbcomputer_enabled.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,27 +3,24 @@
 # Copyright (c), The AiiDA team. All rights reserved.                     #
 # This file is part of the AiiDA code.                                    #
 #                                                                         #
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-core #
 # For further information on the license, see the LICENSE.txt file        #
 # For further information please visit http://www.aiida.net               #
 ###########################################################################
-# pylint: disable=invalid-name
+# pylint: disable=invalid-name,no-member
 """Remove `db_dbcomputer.enabled`
 
 This is similar to migration django_0031
 
 Revision ID: 3d6190594e19
 Revises: 5a49629f0d45
 Create Date: 2019-04-03 14:38:50.585639
 
 """
-
-# Remove when https://github.com/PyCQA/pylint/issues/1931 is fixed
-# pylint: disable=no-member,no-name-in-module,import-error
 from alembic import op
 import sqlalchemy as sa
 
 # revision identifiers, used by Alembic.
 revision = '3d6190594e19'
 down_revision = '5a49629f0d45'
 branch_labels = None
```

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/535039300e4a_computer_name_to_label.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/535039300e4a_computer_name_to_label.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/59edaf8a8b79_adding_indexes_and_constraints_to_the_.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/59edaf8a8b79_adding_indexes_and_constraints_to_the_.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/5a49629f0d45_dblink_indices.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/5a49629f0d45_dblink_indices.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/5d4d844852b6_invalidating_node_hash.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/5d4d844852b6_invalidating_node_hash.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,16 +12,14 @@
 
 Revision ID: 5d4d844852b6
 Revises: 62fe0d36de90
 Create Date: 2018-10-26 17:14:33.566670
 
 """
 from alembic import op
-# Remove when https://github.com/PyCQA/pylint/issues/1931 is fixed
-# pylint: disable=no-name-in-module,import-error
 from sqlalchemy.sql import text
 
 # revision identifiers, used by Alembic.
 revision = '5d4d844852b6'
 down_revision = '62fe0d36de90'
 branch_labels = None
 depends_on = None
```

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/5ddd24e52864_dbnode_type_to_dbnode_node_type.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/5ddd24e52864_dbnode_type_to_dbnode_node_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,17 +13,14 @@
 This is identical to migration django_0030
 
 Revision ID: 5ddd24e52864
 Revises: d254fdfed416
 Create Date: 2019-02-22 17:09:57.715114
 
 """
-
-# Remove when https://github.com/PyCQA/pylint/issues/1931 is fixed
-# pylint: disable=no-name-in-module,import-error
 from alembic import op
 
 # revision identifiers, used by Alembic.
 revision = '5ddd24e52864'
 down_revision = 'd254fdfed416'
 branch_labels = None
 depends_on = None
```

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/61fc0913fae9_remove_node_prefix.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/61fc0913fae9_remove_node_prefix.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/62fe0d36de90_add_node_uuid_unique_constraint.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/62fe0d36de90_add_node_uuid_unique_constraint.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/6a5c2ea1439d_move_data_within_node_module.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/6a5c2ea1439d_move_data_within_node_module.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/6c629c886f84_process_type.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/6c629c886f84_process_type.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/70c7d732f1b2_delete_dbpath.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/70c7d732f1b2_delete_dbpath.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/7536a82b2cc4_add_node_repository_metadata.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/7536a82b2cc4_add_node_repository_metadata.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/7a6587e16f4c_unique_constraints_for_the_db_dbgroup_.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/7a6587e16f4c_unique_constraints_for_the_db_dbgroup_.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/7b38a9e783e7_seal_unsealed_processes.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/7b38a9e783e7_seal_unsealed_processes.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,17 +22,14 @@
 This is identical to migration django_0041
 
 Revision ID: 7b38a9e783e7
 Revises: e734dd5e50d7
 Create Date: 2019-10-28 13:22:56.224234
 
 """
-
-# Remove when https://github.com/PyCQA/pylint/issues/1931 is fixed
-# pylint: disable=no-name-in-module,import-error
 from alembic import op
 from sqlalchemy.sql import text
 
 # revision identifiers, used by Alembic.
 revision = '7b38a9e783e7'
 down_revision = 'e734dd5e50d7'
 branch_labels = None
```

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/7ca08c391c49_calc_job_option_attribute_keys.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/7ca08c391c49_calc_job_option_attribute_keys.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,17 +11,14 @@
 """Migration of ProcessNode attributes for metadata options whose key changed.
 
 Revision ID: 7ca08c391c49
 Revises: e72ad251bcdb
 Create Date: 2019-01-15 15:03:43.876133
 
 """
-
-# Remove when https://github.com/PyCQA/pylint/issues/1931 is fixed
-# pylint: disable=no-name-in-module,import-error
 from alembic import op
 from sqlalchemy.sql import text
 
 # revision identifiers, used by Alembic.
 revision = '7ca08c391c49'
 down_revision = 'e72ad251bcdb'
 branch_labels = None
```

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/89176227b25_add_indexes_to_dbworkflowdata_table.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/89176227b25_add_indexes_to_dbworkflowdata_table.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/91b573400be5_prepare_schema_reset.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0042_prepare_schema_reset.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,50 +6,45 @@
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-core #
 # For further information on the license, see the LICENSE.txt file        #
 # For further information please visit http://www.aiida.net               #
 ###########################################################################
 # pylint: disable=invalid-name,no-member
 """Prepare schema reset.
 
-This is similar to migration django_0042
+This is similar to migration 91b573400be5
 
-Revision ID: 91b573400be5
-Revises: 7b38a9e783e7
-Create Date: 2019-07-25 14:58:39.866822
+Revision ID: django_0042
+Revises: django_0041
 
 """
-
-# Remove when https://github.com/PyCQA/pylint/issues/1931 is fixed
-# pylint: disable=no-name-in-module,import-error
 from alembic import op
-from sqlalchemy.sql import text
+import sqlalchemy as sa
 
-# revision identifiers, used by Alembic.
-revision = '91b573400be5'
-down_revision = '7b38a9e783e7'
+revision = 'django_0042'
+down_revision = 'django_0041'
 branch_labels = None
 depends_on = None
 
 
 def upgrade():
     """Migrations for the upgrade."""
     conn = op.get_bind()
 
     # The following statement is trying to perform an UPSERT, i.e. an UPDATE of a given key or if it doesn't exist fall
     # back to an INSERT. This problem is notoriously difficult to solve as explained in great detail in this article:
     # https://www.depesz.com/2012/06/10/why-is-upsert-so-complicated/ Postgres 9.5 provides an offical UPSERT method
     # through the `ON CONFLICT` keyword, but since we also support 9.4 we cannot use it here. The snippet used below
     # taken from the provided link, is not safe for concurrent operations, but since our migrations always run in an
     # isolated way, we do not suffer from those problems and can safely use it.
-    statement = text(
+    statement = sa.text(
         """
-        INSERT INTO db_dbsetting (key, val, description)
-        SELECT 'schema_generation', '"1"', 'Database schema generation'
+        INSERT INTO db_dbsetting (key, val, description, time)
+        SELECT 'schema_generation', '"1"', 'Database schema generation', NOW()
         WHERE NOT EXISTS (SELECT * FROM db_dbsetting WHERE key = 'schema_generation');
         """
     )
     conn.execute(statement)
 
 
 def downgrade():
     """Migrations for the downgrade."""
-    raise NotImplementedError('Downgrade of 91b573400be5.')
+    raise NotImplementedError('Downgrade of django_0042.')
```

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/__init__.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/a514d673c163_drop_dblock.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/a514d673c163_drop_dblock.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/a603da2cc809_code_sub_class_of_data.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/a603da2cc809_code_sub_class_of_data.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/a6048f0ffca8_update_linktypes.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/a6048f0ffca8_update_linktypes.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/b8b23ddefad4_dbgroup_name_to_label_type_to_type_string.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/b8b23ddefad4_dbgroup_name_to_label_type_to_type_string.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/bf591f31dd12_dbgroup_type_string.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/bf591f31dd12_dbgroup_type_string.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/ce56d84bcc35_delete_trajectory_symbols_array.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/ce56d84bcc35_delete_trajectory_symbols_array.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/d254fdfed416_rename_parameter_data_to_dict.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/d254fdfed416_rename_parameter_data_to_dict.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/de2eaf6978b4_simplify_user_model.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/de2eaf6978b4_simplify_user_model.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0001_initial.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0001_initial.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0002_db_state_change.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0002_db_state_change.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0003_add_link_type.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0003_add_link_type.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0004_add_daemon_and_uuid_indices.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0004_add_daemon_and_uuid_indices.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0005_add_cmtime_indices.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0005_add_cmtime_indices.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0006_delete_dbpath.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0006_delete_dbpath.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0007_update_linktypes.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0007_update_linktypes.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0008_code_hidden_to_extra.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0008_code_hidden_to_extra.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0009_base_data_plugin_type_string.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0009_base_data_plugin_type_string.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0010_process_type.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0010_process_type.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0011_delete_kombu_tables.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0011_delete_kombu_tables.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0012_drop_dblock.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0012_drop_dblock.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0013_django_1_8.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0013_django_1_8.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0014_add_node_uuid_unique_constraint.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0014_add_node_uuid_unique_constraint.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0015_invalidating_node_hash.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0015_invalidating_node_hash.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0016_code_sub_class_of_data.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0016_code_sub_class_of_data.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0017_drop_dbcalcstate.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0017_drop_dbcalcstate.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0018_django_1_11.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0018_django_1_11.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0019_migrate_builtin_calculations.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0019_migrate_builtin_calculations.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0020_provenance_redesign.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0020_provenance_redesign.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0021_dbgroup_name_to_label_type_to_type_string.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0021_dbgroup_name_to_label_type_to_type_string.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0022_dbgroup_type_string_change_content.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0022_dbgroup_type_string_change_content.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0023_calc_job_option_attribute_keys.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0023_calc_job_option_attribute_keys.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0024a_dblog_update.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0024a_dblog_update.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0024b_dblog_update.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0024b_dblog_update.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0025_move_data_within_node_module.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0025_move_data_within_node_module.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0026_trajectory_symbols_to_attribute.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0026_trajectory_symbols_to_attribute.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0027_delete_trajectory_symbols_array.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0027_delete_trajectory_symbols_array.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0028_remove_node_prefix.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0028_remove_node_prefix.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0029_rename_parameter_data_to_dict.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0029_rename_parameter_data_to_dict.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0030_dbnode_type_to_dbnode_node_type.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0030_dbnode_type_to_dbnode_node_type.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0031_remove_dbcomputer_enabled.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0031_remove_dbcomputer_enabled.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0032_remove_legacy_workflows.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0032_remove_legacy_workflows.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0033_replace_text_field_with_json_field.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0033_replace_text_field_with_json_field.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0034_drop_node_columns_nodeversion_public.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0034_drop_node_columns_nodeversion_public.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0035_simplify_user_model.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0035_simplify_user_model.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0036_drop_computer_transport_params.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0036_drop_computer_transport_params.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0037_attributes_extras_settings_json.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0037_attributes_extras_settings_json.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0038_data_migration_legacy_job_calculations.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0038_data_migration_legacy_job_calculations.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0039_reset_hash.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0039_reset_hash.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,13 +24,13 @@
 down_revision = 'django_0038'
 branch_labels = None
 depends_on = None
 
 
 def upgrade():
     """Migrations for the upgrade."""
-    drop_hashes(op.get_bind())  # pylint: disable=no-member
+    drop_hashes(op.get_bind(), hash_extra_key='_aiida_hash')  # pylint: disable=no-member
 
 
 def downgrade():
     """Migrations for the downgrade."""
-    drop_hashes(op.get_bind())  # pylint: disable=no-member
+    drop_hashes(op.get_bind(), hash_extra_key='_aiida_hash')  # pylint: disable=no-member
```

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0040_data_migration_legacy_process_attributes.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0040_data_migration_legacy_process_attributes.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0041_seal_unsealed_processes.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0041_seal_unsealed_processes.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0042_prepare_schema_reset.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/91b573400be5_prepare_schema_reset.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,45 +6,47 @@
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-core #
 # For further information on the license, see the LICENSE.txt file        #
 # For further information please visit http://www.aiida.net               #
 ###########################################################################
 # pylint: disable=invalid-name,no-member
 """Prepare schema reset.
 
-This is similar to migration 91b573400be5
+This is similar to migration django_0042
 
-Revision ID: django_0042
-Revises: django_0041
+Revision ID: 91b573400be5
+Revises: 7b38a9e783e7
+Create Date: 2019-07-25 14:58:39.866822
 
 """
 from alembic import op
-import sqlalchemy as sa
+from sqlalchemy.sql import text
 
-revision = 'django_0042'
-down_revision = 'django_0041'
+# revision identifiers, used by Alembic.
+revision = '91b573400be5'
+down_revision = '7b38a9e783e7'
 branch_labels = None
 depends_on = None
 
 
 def upgrade():
     """Migrations for the upgrade."""
     conn = op.get_bind()
 
     # The following statement is trying to perform an UPSERT, i.e. an UPDATE of a given key or if it doesn't exist fall
     # back to an INSERT. This problem is notoriously difficult to solve as explained in great detail in this article:
     # https://www.depesz.com/2012/06/10/why-is-upsert-so-complicated/ Postgres 9.5 provides an offical UPSERT method
     # through the `ON CONFLICT` keyword, but since we also support 9.4 we cannot use it here. The snippet used below
     # taken from the provided link, is not safe for concurrent operations, but since our migrations always run in an
     # isolated way, we do not suffer from those problems and can safely use it.
-    statement = sa.text(
+    statement = text(
         """
-        INSERT INTO db_dbsetting (key, val, description, time)
-        SELECT 'schema_generation', '"1"', 'Database schema generation', NOW()
+        INSERT INTO db_dbsetting (key, val, description)
+        SELECT 'schema_generation', '"1"', 'Database schema generation'
         WHERE NOT EXISTS (SELECT * FROM db_dbsetting WHERE key = 'schema_generation');
         """
     )
     conn.execute(statement)
 
 
 def downgrade():
     """Migrations for the downgrade."""
-    raise NotImplementedError('Downgrade of django_0042.')
+    raise NotImplementedError('Downgrade of 91b573400be5.')
```

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0043_default_link_label.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0043_default_link_label.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0044_dbgroup_type_string.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0044_dbgroup_type_string.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0045_dbgroup_extras.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0045_dbgroup_extras.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0046_add_node_repository_metadata.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0046_add_node_repository_metadata.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0047_migrate_repository.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0047_migrate_repository.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0048_computer_name_to_label.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0048_computer_name_to_label.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0049_entry_point_core_prefix.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0049_entry_point_core_prefix.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/django_0050_sqlalchemy_parity.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/django_0050_sqlalchemy_parity.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/e15ef2630a1b_initial_schema.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/e15ef2630a1b_initial_schema.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/e72ad251bcdb_dbgroup_class_change_type_string_values.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/e72ad251bcdb_dbgroup_class_change_type_string_values.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/e734dd5e50d7_data_migration_legacy_process_attributes.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/e734dd5e50d7_data_migration_legacy_process_attributes.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,17 +28,14 @@
 This is identical to migration django_0040
 
 Revision ID: e734dd5e50d7
 Revises: e797afa09270
 Create Date: 2019-07-04 18:23:56.127994
 
 """
-
-# Remove when https://github.com/PyCQA/pylint/issues/1931 is fixed
-# pylint: disable=no-name-in-module,import-error
 from alembic import op
 from sqlalchemy.sql import text
 
 # revision identifiers, used by Alembic.
 revision = 'e734dd5e50d7'
 down_revision = 'e797afa09270'
 branch_labels = None
```

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/e797afa09270_reset_hash.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/e797afa09270_reset_hash.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,13 +26,13 @@
 down_revision = '26d561acd560'
 branch_labels = None
 depends_on = None
 
 
 def upgrade():
     """drop the hashes when upgrading"""
-    drop_hashes(op.get_bind())  # pylint: disable=no-member
+    drop_hashes(op.get_bind(), hash_extra_key='_aiida_hash')  # pylint: disable=no-member
 
 
 def downgrade():
     """drop the hashes also when downgrading"""
-    drop_hashes(op.get_bind())  # pylint: disable=no-member
+    drop_hashes(op.get_bind(), hash_extra_key='_aiida_hash')  # pylint: disable=no-member
```

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/ea2f50e7f615_dblog_create_uuid_column.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/ea2f50e7f615_dblog_create_uuid_column.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/f9a69de76a9a_delete_kombu_tables.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/f9a69de76a9a_delete_kombu_tables.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrations/versions/main_0001_initial.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrations/versions/main_0001_initial.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/migrator.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/migrator.py`

 * *Files 1% similar despite different names*

```diff
@@ -380,14 +380,15 @@
                 context._ensure_version_table(purge=True)  # pylint: disable=protected-access
                 context.stamp(context.script, 'main_0001')
                 self.connection.commit()
 
         # finally migrate to the main head revision
         MIGRATE_LOGGER.report('Migrating to the head of the main branch')
         self.migrate_up('main@head')
+        self.connection.commit()
 
     def migrate_up(self, version: str) -> None:
         """Migrate the database up to a specific version.
 
         :param version: string with schema version to migrate to
         """
         with self._alembic_connect() as config:
```

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/models/__init__.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/models/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/models/authinfo.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/models/authinfo.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/models/base.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/models/base.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/models/comment.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/models/comment.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/models/computer.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/models/computer.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/models/group.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/models/group.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/models/log.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/models/log.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/models/node.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/models/node.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/models/settings.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/models/settings.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/models/user.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/models/user.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/orm/__init__.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/orm/authinfos.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/orm/authinfos.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/orm/comments.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/orm/comments.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/orm/computers.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/orm/computers.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/orm/convert.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/orm/convert.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/orm/entities.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/orm/entities.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from aiida.common.lang import type_check
 from aiida.storage.psql_dos.models.base import Base
 
 from . import utils
 
 ModelType = TypeVar('ModelType')  # pylint: disable=invalid-name
-SelfType = TypeVar('SelfType', bound='SqlaModelEntity')
+SelfType = TypeVar('SelfType', bound='SqlaModelEntity')  # pylint: disable=invalid-name
 
 
 class SqlaModelEntity(Generic[ModelType]):
     """A mixin that adds some common SQLA backend entity methods"""
 
     MODEL_CLASS = None
     _model: utils.ModelWrapper
```

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/orm/extras_mixin.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/orm/extras_mixin.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/orm/groups.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/orm/groups.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/orm/logs.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/orm/logs.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/orm/nodes.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/orm/nodes.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/orm/querybuilder/__init__.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/orm/querybuilder/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/orm/querybuilder/joiner.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/orm/querybuilder/joiner.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # Copyright (c), The AiiDA team. All rights reserved.                     #
 # This file is part of the AiiDA code.                                    #
 #                                                                         #
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-core #
 # For further information on the license, see the LICENSE.txt file        #
 # For further information please visit http://www.aiida.net               #
 ###########################################################################
+# pylint: disable=unnecessary-lambda-assignment
 """A module containing the logic for creating joined queries."""
 from dataclasses import dataclass
 from typing import Any, Callable, Dict, Optional, Protocol, Type
 
 from sqlalchemy import and_, join, select
 from sqlalchemy.dialects.postgresql import array
 from sqlalchemy.orm import Query, aliased
```

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/orm/querybuilder/main.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/orm/querybuilder/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -993,15 +993,16 @@
                 projections += _create_projections(
                     edge_tag, aliases, len(projections), project_dict, get_projectable_entity, tag_to_projected_fields,
                     outer_to_inner_schema
                 )
 
     # check the consistency of projections
     projection_index_to_field = {
-        index_in_sql_result: attrkey for _, projected_entities_dict in tag_to_projected_fields.items()
+        index_in_sql_result: attrkey
+        for _, projected_entities_dict in tag_to_projected_fields.items()
         for attrkey, index_in_sql_result in projected_entities_dict.items()
     }
     if len(projections) > len(projection_index_to_field):
         raise ValueError('You are projecting the same key multiple times within the same node')
     if not projection_index_to_field:
         raise ValueError('No projections requested')
     return projections, tag_to_projected_fields
```

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/orm/users.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/orm/users.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/orm/utils.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/orm/utils.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/psql_dos/utils.py` & `aiida_core-2.4.0/aiida/storage/psql_dos/utils.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/sqlite_temp/__init__.py` & `aiida_core-2.4.0/aiida/storage/sqlite_temp/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/sqlite_temp/backend.py` & `aiida_core-2.4.0/aiida/storage/sqlite_temp/backend.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/sqlite_zip/__init__.py` & `aiida_core-2.4.0/aiida/storage/sqlite_zip/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/sqlite_zip/backend.py` & `aiida_core-2.4.0/aiida/storage/sqlite_zip/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,15 +214,15 @@
             else:
                 raise CorruptStorage(f'repository could not be read: non-existent {self._path / REPO_FOLDER}')
         return self._repo
 
     def query(self) -> orm.SqliteQueryBuilder:
         return orm.SqliteQueryBuilder(self)
 
-    def get_backend_entity(self, model):  # pylint: disable=no-self-use
+    def get_backend_entity(self, model):
         """Return the backend entity that corresponds to the given Model instance."""
         return orm.get_backend_entity(model, self)
 
     @cached_property
     def authinfos(self):
         return orm.SqliteAuthInfoCollection(self)
```

### Comparing `aiida_core-2.3.1/aiida/storage/sqlite_zip/migrations/__init__.py` & `aiida_core-2.4.0/aiida/storage/sqlite_zip/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/sqlite_zip/migrations/env.py` & `aiida_core-2.4.0/aiida/storage/sqlite_zip/migrations/env.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,13 +37,13 @@
     )
 
     context.run_migrations()  # pylint: disable=no-member
 
 
 try:
     if context.is_offline_mode():  # pylint: disable=no-member
-        NotImplementedError('This feature is not currently supported.')
+        raise NotImplementedError('This feature is not currently supported.')
 
     run_migrations_online()
 except NameError:
     # This will occur in an environment that is just compiling the documentation
     pass
```

### Comparing `aiida_core-2.3.1/aiida/storage/sqlite_zip/migrations/legacy/__init__.py` & `aiida_core-2.4.0/aiida/storage/sqlite_zip/migrations/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/sqlite_zip/migrations/legacy/v04_to_v05.py` & `aiida_core-2.4.0/aiida/storage/sqlite_zip/migrations/legacy/v04_to_v05.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/sqlite_zip/migrations/legacy/v05_to_v06.py` & `aiida_core-2.4.0/aiida/storage/sqlite_zip/migrations/legacy/v05_to_v06.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/sqlite_zip/migrations/legacy/v06_to_v07.py` & `aiida_core-2.4.0/aiida/storage/sqlite_zip/migrations/legacy/v06_to_v07.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/sqlite_zip/migrations/legacy/v07_to_v08.py` & `aiida_core-2.4.0/aiida/storage/sqlite_zip/migrations/legacy/v07_to_v08.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/sqlite_zip/migrations/legacy/v08_to_v09.py` & `aiida_core-2.4.0/aiida/storage/sqlite_zip/migrations/legacy/v08_to_v09.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/sqlite_zip/migrations/legacy/v09_to_v10.py` & `aiida_core-2.4.0/aiida/storage/sqlite_zip/migrations/legacy/v09_to_v10.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/sqlite_zip/migrations/legacy/v10_to_v11.py` & `aiida_core-2.4.0/aiida/storage/sqlite_zip/migrations/legacy/v10_to_v11.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/sqlite_zip/migrations/legacy/v11_to_v12.py` & `aiida_core-2.4.0/aiida/storage/sqlite_zip/migrations/legacy/v11_to_v12.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/sqlite_zip/migrations/legacy/v12_to_v13.py` & `aiida_core-2.4.0/aiida/storage/sqlite_zip/migrations/legacy/v12_to_v13.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/sqlite_zip/migrations/legacy_to_main.py` & `aiida_core-2.4.0/aiida/storage/sqlite_zip/migrations/legacy_to_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,16 +175,16 @@
 
     if not (data['groups_uuid'] or data['links_uuid']):
         return None
 
     with engine.begin() as connection:
 
         # get mapping of node IDs to node UUIDs
-        node_uuid_map = {
-            uuid: pk for uuid, pk in connection.execute(select(v1_schema.DbNode.uuid, v1_schema.DbNode.id))  # pylint: disable=unnecessary-comprehension
+        node_uuid_map = {  # pylint: disable=unnecessary-comprehension
+            uuid: pk for uuid, pk in connection.execute(select(v1_schema.DbNode.uuid, v1_schema.DbNode.id))
         }
 
         # links
         if data['links_uuid']:
 
             def _transform_link(link_row):
                 try:
@@ -206,16 +206,16 @@
                 for nrows, rows in batch_iter(data['links_uuid'], batch_size, transform=_transform_link):
                     connection.execute(insert(v1_schema.DbLink.__table__), rows)
                     progress.update(nrows)
 
         # groups to nodes
         if data['groups_uuid']:
             # get mapping of node IDs to node UUIDs
-            group_uuid_map = {
-                uuid: pk for uuid, pk in connection.execute(select(v1_schema.DbGroup.uuid, v1_schema.DbGroup.id))  # pylint: disable=unnecessary-comprehension
+            group_uuid_map = {  # pylint: disable=unnecessary-comprehension
+                uuid: pk for uuid, pk in connection.execute(select(v1_schema.DbGroup.uuid, v1_schema.DbGroup.id))
             }
             length = sum(len(uuids) for uuids in data['groups_uuid'].values())
             unknown_nodes: Dict[str, set] = {}
             with get_progress_reporter()(desc='Adding Group-Nodes', total=length) as progress:
                 for group_uuid, node_uuids in data['groups_uuid'].items():
                     group_id = group_uuid_map[group_uuid]
                     rows = []
@@ -251,15 +251,17 @@
             if pk not in attributes:
                 raise CorruptStorage(f'Unable to find attributes info for Node with Pk={pk}')
             if pk not in extras:
                 raise CorruptStorage(f'Unable to find extra info for Node with Pk={pk}')
             uuid = all_fields['uuid']
             repository_metadata = _create_repo_metadata(node_repos[uuid]) if uuid in node_repos else {}
             yield {
-                **{keys.get(key, key): _convert_datetime(key, val) for key, val in all_fields.items()},
+                **{
+                    keys.get(key, key): _convert_datetime(key, val) for key, val in all_fields.items()
+                },
                 **{
                     'id': pk,
                     'attributes': attributes[pk],
                     'extras': extras[pk],
                     'repository_metadata': repository_metadata
                 }
             }
```

### Comparing `aiida_core-2.3.1/aiida/storage/sqlite_zip/migrations/script.py.mako` & `aiida_core-2.4.0/aiida/storage/sqlite_zip/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/sqlite_zip/migrations/utils.py` & `aiida_core-2.4.0/aiida/storage/sqlite_zip/migrations/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
                         elif subpath.is_dir():
                             new_path_sub.mkdir(exist_ok=True)
                         else:
                             new_path_sub.putfile(subpath)
                         progress.update()
         if overwrite and outpath.exists() and outpath.is_file():
             outpath.unlink()
-        shutil.move(temp_archive, outpath)  # type: ignore[arg-type]
+        shutil.move(temp_archive, outpath)
 
 
 def copy_tar_to_zip(
     inpath: Path,
     outpath: Path,
     path_callback: Callable[[Path, ZipPath], bool],
     *,
@@ -165,8 +165,8 @@
                         # files extracted from the tar do not include a modified time, yet zip requires one
                         os.utime(subpath, (subpath.stat().st_ctime, subpath.stat().st_ctime))
                         new_path_sub.putfile(subpath)
                     progress.update()
 
         if overwrite and outpath.exists() and outpath.is_file():
             outpath.unlink()
-        shutil.move(temp_archive, outpath)  # type: ignore[arg-type]
+        shutil.move(temp_archive, outpath)
```

### Comparing `aiida_core-2.3.1/aiida/storage/sqlite_zip/migrations/v1_db_schema.py` & `aiida_core-2.4.0/aiida/storage/sqlite_zip/migrations/v1_db_schema.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/sqlite_zip/migrations/versions/__init__.py` & `aiida_core-2.4.0/aiida/storage/sqlite_zip/migrations/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/sqlite_zip/migrations/versions/main_0000_initial.py` & `aiida_core-2.4.0/aiida/storage/sqlite_zip/migrations/versions/main_0000_initial.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/sqlite_zip/migrations/versions/main_0000a_replace_nulls.py` & `aiida_core-2.4.0/aiida/storage/sqlite_zip/migrations/versions/main_0000a_replace_nulls.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/sqlite_zip/migrations/versions/main_0000b_non_nullable.py` & `aiida_core-2.4.0/aiida/storage/sqlite_zip/migrations/versions/main_0000b_non_nullable.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/sqlite_zip/migrations/versions/main_0001.py` & `aiida_core-2.4.0/aiida/storage/sqlite_zip/migrations/versions/main_0001.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/sqlite_zip/migrator.py` & `aiida_core-2.4.0/aiida/storage/sqlite_zip/migrator.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/sqlite_zip/models.py` & `aiida_core-2.4.0/aiida/storage/sqlite_zip/models.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/sqlite_zip/orm.py` & `aiida_core-2.4.0/aiida/storage/sqlite_zip/orm.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/storage/sqlite_zip/utils.py` & `aiida_core-2.4.0/aiida/storage/sqlite_zip/utils.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/tools/__init__.py` & `aiida_core-2.4.0/aiida/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/tools/archive/__init__.py` & `aiida_core-2.4.0/aiida/tools/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/tools/archive/abstract.py` & `aiida_core-2.4.0/aiida/tools/archive/abstract.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/tools/archive/common.py` & `aiida_core-2.4.0/aiida/tools/archive/common.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/tools/archive/create.py` & `aiida_core-2.4.0/aiida/tools/archive/create.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright (c), The AiiDA team. All rights reserved.                     #
 # This file is part of the AiiDA code.                                    #
 #                                                                         #
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-core #
 # For further information on the license, see the LICENSE.txt file        #
 # For further information please visit http://www.aiida.net               #
 ###########################################################################
-# pylint: disable=too-many-locals,too-many-branches,too-many-statements
+# pylint: disable=too-many-locals,too-many-branches,too-many-statements,unnecessary-lambda-assignment
 """Create an AiiDA archive.
 
 The archive is a subset of the provenance graph,
 stored in a single file.
 """
 from datetime import datetime
 from pathlib import Path
@@ -277,16 +277,17 @@
     with tempfile.TemporaryDirectory() as tmpdir:
         tmp_filename = Path(tmpdir) / 'export.zip'
         with archive_format.open(tmp_filename, mode='x', compression=compression) as writer:
             # add metadata
             writer.update_metadata({
                 'ctime': datetime.now().isoformat(),
                 'creation_parameters': {
-                    'entities_starting_set': None if entities is None else
-                    {etype.value: list(unique) for etype, unique in starting_uuids.items() if unique},
+                    'entities_starting_set': None if entities is None else {
+                        etype.value: list(unique) for etype, unique in starting_uuids.items() if unique
+                    },
                     'include_authinfos': include_authinfos,
                     'include_comments': include_comments,
                     'include_logs': include_logs,
                     'graph_traversal_rules': full_traversal_rules,
                 }
             })
             # stream entity data to the archive
@@ -340,15 +341,15 @@
             if entity_ids[EntityTypes.NODE]:
                 _stream_repo_files(archive_format.key_format, writer, entity_ids[EntityTypes.NODE], backend, batch_size)
 
             EXPORT_LOGGER.report('Finalizing archive creation...')
 
         if filename.exists():
             filename.unlink()
-        shutil.move(tmp_filename, filename)  # type: ignore[arg-type]
+        shutil.move(tmp_filename, filename)
 
     EXPORT_LOGGER.report('Archive created successfully')
 
     return filename
 
 
 def _collect_all_entities(
```

### Comparing `aiida_core-2.3.1/aiida/tools/archive/exceptions.py` & `aiida_core-2.4.0/aiida/tools/archive/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/tools/archive/implementations/__init__.py` & `aiida_core-2.4.0/aiida/tools/archive/implementations/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/tools/archive/implementations/sqlite_zip/__init__.py` & `aiida_core-2.4.0/aiida/tools/archive/implementations/sqlite_zip/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/tools/archive/implementations/sqlite_zip/main.py` & `aiida_core-2.4.0/aiida/tools/archive/implementations/sqlite_zip/main.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/tools/archive/implementations/sqlite_zip/reader.py` & `aiida_core-2.4.0/aiida/tools/archive/implementations/sqlite_zip/reader.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/tools/archive/implementations/sqlite_zip/writer.py` & `aiida_core-2.4.0/aiida/tools/archive/implementations/sqlite_zip/writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,15 +268,15 @@
         self._copy_old_zip_files()
         if self._zip_path is not None:
             self._zip_path.close()
         self._central_dir = {}
         self._deleted_paths = set()
         # now move it to the original location
         self._path.unlink()
-        shutil.move(self._work_dir / 'archive.zip', self._path)  # type: ignore[arg-type]
+        shutil.move(self._work_dir / 'archive.zip', self._path)
         if self._init_work_dir is None:
             shutil.rmtree(self._work_dir, ignore_errors=True)
         self._zip_path = self._work_dir = self._conn = None
         self._in_context = False
 
     def _copy_old_zip_files(self):
         """Copy the old archive content to the new one (omitting any amended or deleted files)"""
```

### Comparing `aiida_core-2.3.1/aiida/tools/archive/imports.py` & `aiida_core-2.4.0/aiida/tools/archive/imports.py`

 * *Files 0% similar despite different names*

```diff
@@ -370,15 +370,15 @@
     )
 
     # translate user_id / computer_id, from -> to
     try:
         to_user_id_comp_id = [(user_ids_archive_backend[_user_id], computer_ids_archive_backend[_comp_id])
                               for _, _user_id, _comp_id in input_id_user_comp]
     except KeyError as exception:
-        ImportValidationError(f'Archive AuthInfo has unknown User/Computer: {exception}')
+        raise ImportValidationError(f'Archive AuthInfo has unknown User/Computer: {exception}')
 
     # retrieve existing user_id / computer_id
     backend_id_user_comp = []
     if to_user_id_comp_id:
         qbuilder = orm.QueryBuilder(backend=backend_to)
         qbuilder.append(
             orm.AuthInfo,
@@ -481,14 +481,15 @@
 class NodeTransform:
     """Callable to transform a Node DB row, between the source archive and target backend."""
 
     def __init__(
         self, user_ids_archive_backend: Dict[int, int], computer_ids_archive_backend: Dict[int, int],
         import_new_extras: bool
     ):
+        """Construct a new instance."""
         self.user_ids_archive_backend = user_ids_archive_backend
         self.computer_ids_archive_backend = computer_ids_archive_backend
         self.import_new_extras = import_new_extras
 
     def __call__(self, row: dict) -> dict:
         """Perform the transform."""
         data = row['entity']
@@ -693,14 +694,15 @@
     """Callable to transform a Comment DB row, between the source archive and target backend."""
 
     def __init__(
         self,
         user_ids_archive_backend: Dict[int, int],
         node_ids_archive_backend: Dict[int, int],
     ):
+        """Construct a new instance."""
         self.user_ids_archive_backend = user_ids_archive_backend
         self.node_ids_archive_backend = node_ids_archive_backend
 
     def __call__(self, row: dict) -> dict:
         """Perform the transform."""
         data = row['entity']
         pk = data.pop('id')
```

### Comparing `aiida_core-2.3.1/aiida/tools/calculations/__init__.py` & `aiida_core-2.4.0/aiida/tools/calculations/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/tools/calculations/base.py` & `aiida_core-2.4.0/aiida/tools/calculations/base.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/tools/data/__init__.py` & `aiida_core-2.4.0/aiida/tools/data/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/tools/data/array/__init__.py` & `aiida_core-2.4.0/aiida/tools/data/array/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/tools/data/array/kpoints/__init__.py` & `aiida_core-2.4.0/aiida/tools/data/array/kpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/tools/data/array/kpoints/legacy.py` & `aiida_core-2.4.0/aiida/tools/data/array/kpoints/legacy.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/tools/data/array/kpoints/main.py` & `aiida_core-2.4.0/aiida/tools/data/array/kpoints/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     :param structure: a StructureData node
     :param method: the method to use for kpoint generation, options are 'seekpath' and 'legacy'.
         It is strongly advised to use the default 'seekpath' as the 'legacy' implementation is known to have
         bugs for certain structure cells
     :param kwargs: optional keyword arguments that depend on the selected method
     :returns: dictionary as described above in the docstring
     """
-    if method not in _GET_KPOINTS_PATH_METHODS.keys():
+    if method not in _GET_KPOINTS_PATH_METHODS:
         raise ValueError(f"the method '{method}' is not implemented")
 
     method = _GET_KPOINTS_PATH_METHODS[method]
 
     return method(structure, **kwargs)
 
 
@@ -75,15 +75,15 @@
     :param structure: a StructureData node
     :param method: the method to use for kpoint generation, options are 'seekpath' and 'legacy'.
         It is strongly advised to use the default 'seekpath' as the 'legacy' implementation is known to have
         bugs for certain structure cells
     :param kwargs: optional keyword arguments that depend on the selected method
     :returns: dictionary as described above in the docstring
     """
-    if method not in _GET_EXPLICIT_KPOINTS_PATH_METHODS.keys():
+    if method not in _GET_EXPLICIT_KPOINTS_PATH_METHODS:
         raise ValueError(f"the method '{method}' is not implemented")
 
     method = _GET_EXPLICIT_KPOINTS_PATH_METHODS[method]
 
     return method(structure, **kwargs)
 
 
@@ -184,15 +184,15 @@
 
     parameters = {
         'bravais_info': bravais_info,
         'point_coords': point_coords,
         'path': path,
     }
 
-    return {'parameters': Dict(dict=parameters)}
+    return {'parameters': Dict(parameters)}
 
 
 def _legacy_get_explicit_kpoints_path(structure, **kwargs):
     """
     Call the get_explicit_kpoints_path of the legacy implementation
 
     :param structure: a StructureData node
@@ -223,15 +223,15 @@
 
     parameters = {
         'bravais_info': bravais_info,
         'point_coords': point_coords,
         'path': path,
     }
 
-    return {'parameters': Dict(dict=parameters), 'explicit_kpoints': kpoints}
+    return {'parameters': Dict(parameters), 'explicit_kpoints': kpoints}
 
 
 _GET_KPOINTS_PATH_METHODS = {
     'legacy': _legacy_get_kpoints_path,
     'seekpath': _seekpath_get_kpoints_path,
 }
```

### Comparing `aiida_core-2.3.1/aiida/tools/data/array/kpoints/seekpath.py` & `aiida_core-2.4.0/aiida/tools/data/array/kpoints/seekpath.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
     # set_kpoints expects labels like [[0,'X'],[34,'L'],...], so generate it here skipping empty labels
     labels = [[idx, label] for idx, label in enumerate(kpoints_labels) if label]
     kpoints = KpointsData()
     kpoints.set_cell_from_structure(primitive_structure)
     kpoints.set_kpoints(kpoints_abs, cartesian=True, labels=labels)
 
-    result['parameters'] = Dict(dict=rawdict)
+    result['parameters'] = Dict(rawdict)
     result['explicit_kpoints'] = kpoints
     result['primitive_structure'] = primitive_structure
     result['conv_structure'] = conv_structure
 
     return result
 
 
@@ -132,15 +132,15 @@
     from aiida.tools.data.structure import spglib_tuple_to_structure, structure_to_spglib_tuple
 
     structure_tuple, kind_info, kinds = structure_to_spglib_tuple(structure)
 
     result = {}
     rawdict = seekpath.get_path(structure=structure_tuple, **parameters)
 
-    result['parameters'] = Dict(dict=rawdict)
+    result['parameters'] = Dict(rawdict)
 
     # Replace conv structure with AiiDA StructureData
     conv_lattice = rawdict.pop('conv_lattice')
     conv_positions = rawdict.pop('conv_positions')
     conv_types = rawdict.pop('conv_types')
     result['conv_structure'] = spglib_tuple_to_structure((conv_lattice, conv_positions, conv_types), kind_info, kinds)
```

### Comparing `aiida_core-2.3.1/aiida/tools/data/array/trajectory.py` & `aiida_core-2.4.0/aiida/tools/data/array/trajectory.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/tools/data/cif.py` & `aiida_core-2.4.0/aiida/tools/data/cif.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/tools/data/orbital/__init__.py` & `aiida_core-2.4.0/aiida/tools/data/orbital/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/tools/data/orbital/orbital.py` & `aiida_core-2.4.0/aiida/tools/data/orbital/orbital.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/tools/data/orbital/realhydrogen.py` & `aiida_core-2.4.0/aiida/tools/data/orbital/realhydrogen.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/tools/data/structure.py` & `aiida_core-2.4.0/aiida/tools/data/structure.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,16 +184,16 @@
 
     class BlockIterator:
         """
         An iterator for wrapping the iterator returned by `match.finditer`
         to extract the required fields directly from the match object
         """
 
-        def __init__(self, it, natoms):
-            self._it = it
+        def __init__(self, iterator, natoms):
+            self._it = iterator
             self._natoms = natoms
             self._catom = 0
 
         def __iter__(self):
             return self
 
         def __next__(self):  # pylint: disable=missing-docstring
```

### Comparing `aiida_core-2.3.1/aiida/tools/dbexporters/__init__.py` & `aiida_core-2.4.0/aiida/tools/dbexporters/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/tools/dbimporters/__init__.py` & `aiida_core-2.4.0/aiida/tools/dbimporters/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/tools/dbimporters/baseclasses.py` & `aiida_core-2.4.0/aiida/tools/dbimporters/baseclasses.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,15 +178,15 @@
 
 class DbEntry:
     """
     Represents an entry from external database.
     """
     _license: Optional[str] = None
 
-    def __init__(self, db_name=None, db_uri=None, id=None, version=None, extras=None, uri=None):  # pylint: disable=too-many-arguments,redefined-builtin
+    def __init__(self, db_name=None, db_uri=None, id=None, version=None, extras=None, uri=None):  # pylint: disable=too-many-arguments,redefined-builtin,invalid-name
         """
         Sets the basic parameters for the database entry:
 
         :param db_name: name of the source database
         :param db_uri: URI of the source database
         :param id: structure identifyer in the database
         :param version: version of the database
```

### Comparing `aiida_core-2.3.1/aiida/tools/dbimporters/plugins/__init__.py` & `aiida_core-2.4.0/aiida/tools/dbimporters/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/tools/dbimporters/plugins/cod.py` & `aiida_core-2.4.0/aiida/tools/dbimporters/plugins/cod.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (c), The AiiDA team. All rights reserved.                     #
 # This file is part of the AiiDA code.                                    #
 #                                                                         #
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-core #
 # For further information on the license, see the LICENSE.txt file        #
 # For further information please visit http://www.aiida.net               #
 ###########################################################################
-# pylint: disable=no-self-use
 """"Implementation of `DbImporter` for the COD database."""
 from aiida.tools.dbimporters.baseclasses import CifEntry, DbImporter, DbSearchResults
 
 
 class CodDbImporter(DbImporter):
     """
     Database importer for Crystallography Open Database.
```

### Comparing `aiida_core-2.3.1/aiida/tools/dbimporters/plugins/icsd.py` & `aiida_core-2.4.0/aiida/tools/dbimporters/plugins/icsd.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (c), The AiiDA team. All rights reserved.                     #
 # This file is part of the AiiDA code.                                    #
 #                                                                         #
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-core #
 # For further information on the license, see the LICENSE.txt file        #
 # For further information please visit http://www.aiida.net               #
 ###########################################################################
-# pylint: disable=no-self-use
 """Implementation of `DbImporter` for the ICSD database.
 
 Note: The implementation in this file is not compatible with the recent versions
 of ICSD, which are built with Apache Lucene and Tomcat. Older ICSD versions are
 supported, which included a MySQL database and a php-based web interface. The
 last confirmed compatible version was released in 2020.
 """
@@ -77,15 +76,15 @@
     angle_precision = 0.001
     volume_precision = 0.001
     temperature_precision = 0.001
     density_precision = 0.001
     pressure_precision = 1
 
     def __init__(self, **kwargs):
-
+        """Construct a new instance."""
         self.db_parameters = {
             'server': '',
             'urladd': 'index.php?',
             'querydb': True,
             'dl_db': 'icsd',
             'host': '',
             'user': 'dba',
```

### Comparing `aiida_core-2.3.1/aiida/tools/dbimporters/plugins/materialsproject.py` & `aiida_core-2.4.0/aiida/tools/dbimporters/plugins/materialsproject.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         self._mpr = MPRester(self._api_key)
 
     def _verify_api_key(self):
         """
         Verify the supplied API key by issuing a request to Materials Project.
         """
         response = requests.get(
-            'https://www.materialsproject.org/rest/v1/api_check', headers={'X-API-KEY': self._api_key}
+            'https://www.materialsproject.org/rest/v1/api_check', headers={'X-API-KEY': self._api_key}, timeout=5
         )
         response_content = response.json()  # a dict
         if 'error' in response_content:
             raise RuntimeError(response_content['error'])
         if not response_content['valid_response']:
             raise RuntimeError('Materials Project did not give a valid response for the API key check.')
         if not response_content['api_key_valid']:
@@ -127,15 +127,15 @@
 
     def _find(self, query, properties):
         """
         Query the database with a given dictionary of query parameters
 
         :param query: a dictionary with the query parameters
         """
-        for entry in self._mpr.query(criteria=query, properties=properties):
+        for entry in self._mpr.query(criteria=query, properties=properties):  # pylint: disable=no-member
             yield entry
 
 
 class MaterialsProjectCifEntry(CifEntry):  # pylint: disable=abstract-method
     """
     A Materials Project entry class which extends the DbEntry class with a CifEntry class.
```

### Comparing `aiida_core-2.3.1/aiida/tools/dbimporters/plugins/mpds.py` & `aiida_core-2.4.0/aiida/tools/dbimporters/plugins/mpds.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,15 +227,15 @@
         Perform a GET request to the REST API using the kwargs as request parameters
         The url and API key will be used that were set upon construction
 
         :param fmt: the format of the response, 'cif' or json' (default)
         :param kwargs: parameters for the GET request
         """
         kwargs['fmt'] = fmt.value
-        return requests.get(url=self.url, params=kwargs, headers={'Key': self.api_key})
+        return requests.get(url=self.url, params=kwargs, headers={'Key': self.api_key}, timeout=10)
 
     @staticmethod
     def get_response_content(response, fmt=DEFAULT_API_FORMAT):
         """
         Analyze the response of an HTTP GET request, verify that the response code is OK
         and return the json loaded response text
```

### Comparing `aiida_core-2.3.1/aiida/tools/dbimporters/plugins/mpod.py` & `aiida_core-2.4.0/aiida/tools/dbimporters/plugins/mpod.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (c), The AiiDA team. All rights reserved.                     #
 # This file is part of the AiiDA code.                                    #
 #                                                                         #
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-core #
 # For further information on the license, see the LICENSE.txt file        #
 # For further information please visit http://www.aiida.net               #
 ###########################################################################
-# pylint: disable=no-self-use
 """"Implementation of `DbImporter` for the MPOD database."""
 from aiida.tools.dbimporters.baseclasses import CifEntry, DbImporter, DbSearchResults
 
 
 class MpodDbImporter(DbImporter):
     """
     Database importer for Material Properties Open Database.
```

### Comparing `aiida_core-2.3.1/aiida/tools/dbimporters/plugins/nninc.py` & `aiida_core-2.4.0/aiida/tools/dbimporters/plugins/nninc.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (c), The AiiDA team. All rights reserved.                     #
 # This file is part of the AiiDA code.                                    #
 #                                                                         #
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-core #
 # For further information on the license, see the LICENSE.txt file        #
 # For further information please visit http://www.aiida.net               #
 ###########################################################################
-# pylint: disable=no-self-use
 """"Implementation of `DbImporter` for the NNIN/C database."""
 from aiida.tools.dbimporters.baseclasses import DbImporter, DbSearchResults, UpfEntry
 
 
 class NnincDbImporter(DbImporter):
     """
     Database importer for NNIN/C Pseudopotential Virtual Vault.
```

### Comparing `aiida_core-2.3.1/aiida/tools/dbimporters/plugins/oqmd.py` & `aiida_core-2.4.0/aiida/tools/dbimporters/plugins/oqmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # Copyright (c), The AiiDA team. All rights reserved.                     #
 # This file is part of the AiiDA code.                                    #
 #                                                                         #
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-core #
 # For further information on the license, see the LICENSE.txt file        #
 # For further information please visit http://www.aiida.net               #
 ###########################################################################
-# pylint: disable=no-self-use
 """"Implementation of `DbImporter` for the OQMD database."""
 from aiida.tools.dbimporters.baseclasses import CifEntry, DbImporter, DbSearchResults
 
 
 class OqmdDbImporter(DbImporter):
     """
     Database importer for Open Quantum Materials Database.
```

### Comparing `aiida_core-2.3.1/aiida/tools/dbimporters/plugins/pcod.py` & `aiida_core-2.4.0/aiida/tools/dbimporters/plugins/pcod.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/tools/dbimporters/plugins/tcod.py` & `aiida_core-2.4.0/aiida/tools/dbimporters/plugins/tcod.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/tools/graph/__init__.py` & `aiida_core-2.4.0/aiida/tools/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/tools/graph/age_entities.py` & `aiida_core-2.4.0/aiida/tools/graph/age_entities.py`

 * *Files 1% similar despite different names*

```diff
@@ -420,26 +420,27 @@
 
     def __isub__(self, other):
         for key in other.dict:
             self[key] -= other[key]
         return self
 
     def __len__(self):
-        return sum([len(s) for s in self.sets])
+        return sum(len(s) for s in self.sets)
 
     def __eq__(self, other):
         for key in self._dict:
             if self[key] != other[key]:
                 return False
         return True
 
     def __ne__(self, other):
         return not self == other
 
     def __repr__(self):
+        """Return string representation."""
         ret_str = ''
         for key, val in self._dict.items():
             ret_str += f'  {key}: '
             ret_str += f'{str(val)}\n'
         return ret_str
 
     def empty(self):
```

### Comparing `aiida_core-2.3.1/aiida/tools/graph/age_rules.py` & `aiida_core-2.4.0/aiida/tools/graph/age_rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
                 query_dict['path'][idx]['entity_type'].startswith('process') or
                 query_dict['path'][idx]['entity_type'] == ''
             ):
                 result = 'nodes'
             elif query_dict['path'][idx]['entity_type'].startswith(GROUP_ENTITY_TYPE_PREFIX):
                 result = 'groups'
             else:
-                raise Exception(f"not understood entity from ( {query_dict['path'][idx]['entity_type']} )")
+                raise RuntimeError(f"not understood entity from ( {query_dict['path'][idx]['entity_type']} )")
             return result
 
         query_dict = querybuilder.as_dict()
 
         # Check if there is any projection:
         query_projections = query_dict['project']
         for projection_key in query_projections:
```

### Comparing `aiida_core-2.3.1/aiida/tools/graph/deletions.py` & `aiida_core-2.4.0/aiida/tools/graph/deletions.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/tools/graph/graph_traversers.py` & `aiida_core-2.4.0/aiida/tools/graph/graph_traversers.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/tools/groups/__init__.py` & `aiida_core-2.4.0/aiida/tools/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/tools/groups/paths.py` & `aiida_core-2.4.0/aiida/tools/groups/paths.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/tools/ipython/__init__.py` & `aiida_core-2.4.0/aiida/tools/ipython/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/tools/ipython/aiida_magic_register.py` & `aiida_core-2.4.0/aiida/tools/ipython/aiida_magic_register.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/tools/ipython/ipython_magics.py` & `aiida_core-2.4.0/aiida/tools/ipython/ipython_magics.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
 @magic.magics_class
 class AiiDALoaderMagics(magic.Magics):
     """AiiDA magic loader."""
 
     @magic.needs_local_scope
     @magic.line_magic
-    def verdi(self, line='', local_ns=None):  # pylint: disable=no-self-use,unused-argument
+    def verdi(self, line='', local_ns=None):  # pylint: disable=unused-argument
         """Run the AiiDA command line tool, using the currently loaded configuration and profile.
 
         Invoking ``verdi`` normally through the command line follows a different code path, compared to calling it
         directly from within an active Python interpreter. Some of those code paths we actually need here, and others
         can actually cause problems:
 
         * The ``VerdiCommandGroup`` group ensures that the context ``obj`` is set with the loaded ``Config`` and
@@ -107,14 +107,17 @@
             )
 
         # Construct the subcommand that will be executed, thereby circumventing the profile option of ``verdi`` itself.
         # If the caller specified a subcommand that doesn't exist, the following will raise an exception.
         context = Context(verdi)
         command = verdi.get_command(context, command_name)
 
+        if command is None:
+            raise RuntimeError(f'command `{command_name}` not found.')
+
         return command(  # pylint: disable=too-many-function-args,unexpected-keyword-arg
             cmdline_arguments[1:],
             prog_name='%verdi',
             obj=AttributeDict({'config': config, 'profile': profile}),
             standalone_mode=False
         )
```

### Comparing `aiida_core-2.3.1/aiida/tools/query/calculation.py` & `aiida_core-2.4.0/aiida/tools/query/calculation.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/tools/query/formatting.py` & `aiida_core-2.4.0/aiida/tools/query/formatting.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/tools/query/mapping.py` & `aiida_core-2.4.0/aiida/tools/query/mapping.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/tools/visualization/__init__.py` & `aiida_core-2.4.0/aiida/tools/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/tools/visualization/graph.py` & `aiida_core-2.4.0/aiida/tools/visualization/graph.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/transports/__init__.py` & `aiida_core-2.4.0/aiida/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/transports/cli.py` & `aiida_core-2.4.0/aiida/transports/cli.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/transports/plugins/__init__.py` & `aiida_core-2.4.0/aiida/transports/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/transports/plugins/local.py` & `aiida_core-2.4.0/aiida/transports/plugins/local.py`

 * *Files 0% similar despite different names*

```diff
@@ -553,15 +553,15 @@
         """
         if not remotesource:
             raise ValueError('Input remotesource to copy must be a non empty object')
         if not remotedestination:
             raise ValueError('Input remotedestination to copy must be a non empty object')
         if not self.has_magic(remotesource):
             if not os.path.exists(os.path.join(self.curdir, remotesource)):
-                raise OSError('Source not found')
+                raise FileNotFoundError('Source not found')
         if self.normalize(remotesource) == self.normalize(remotedestination):
             raise ValueError('Cannot copy from itself to itself')
 
             # # by default, overwrite old files
         #        if not remotedestination .startswith('.'):
         #            if self.isfile(remotedestination) or self.isdir(remotedestination):
         #                self.rmtree(remotedestination)
@@ -664,15 +664,15 @@
         aiida_attr = FileAttribute()
         # map the paramiko class into the aiida one
         # note that paramiko object contains more informations than the aiida
         for key in aiida_attr._valid_fields:  # pylint: disable=protected-access
             aiida_attr[key] = getattr(os_attr, key)
         return aiida_attr
 
-    def _local_listdir(self, path, pattern=None):  # pylint: disable=no-self-use
+    def _local_listdir(self, path, pattern=None):
         """Act on the local folder, for the rest, same as listdir."""
         import re
 
         if not pattern:
             return os.listdir(path)
 
         if path.startswith('/'):  # always this is the case in the local plugin
```

### Comparing `aiida_core-2.3.1/aiida/transports/plugins/ssh.py` & `aiida_core-2.4.0/aiida/transports/plugins/ssh.py`

 * *Files 1% similar despite different names*

```diff
@@ -1199,24 +1199,28 @@
                 f'Found instead {remotedestination} as remotedestination'
             )
 
         if self.has_magic(remotedestination):
             raise ValueError('Pathname patterns are not allowed in the destination')
 
         if self.has_magic(remotesource):
+
             to_copy_list = self.glob(remotesource)
 
             if len(to_copy_list) > 1:
                 if not self.path_exists(remotedestination) or self.isfile(remotedestination):
                     raise OSError("Can't copy more than one file in the same destination file")
 
             for file in to_copy_list:
                 self._exec_cp(cp_exe, cp_flags, file, remotedestination)
 
         else:
+            if not self.path_exists(remotesource):
+                raise FileNotFoundError('Source not found')
+
             self._exec_cp(cp_exe, cp_flags, remotesource, remotedestination)
 
     def _exec_cp(self, cp_exe, cp_flags, src, dst):
         """Execute the ``cp`` command on the remote machine."""
         # to simplify writing the above copy function
         command = f'{cp_exe} {cp_flags} {escape_for_bash(src)} {escape_for_bash(dst)}'
 
@@ -1346,15 +1350,15 @@
             paramiko.Channel object.
         """
         channel = self.sshclient.get_transport().open_session()
         channel.set_combine_stderr(combine_stderr)
 
         if self.getcwd() is not None:
             escaped_folder = escape_for_bash(self.getcwd())
-            command_to_execute = (f'cd {escaped_folder} && ( {command} )')
+            command_to_execute = f'cd {escaped_folder} && ( {command} )'
         else:
             command_to_execute = command
 
         self.logger.debug(f'Command to be executed: {command_to_execute[:self._MAX_EXEC_COMMAND_LOG_SIZE]}')
 
         # Note: The default shell will eat one level of escaping, while
         # 'bash -l -c ...' will eat another. Thus, we need to escape again.
```

### Comparing `aiida_core-2.3.1/aiida/transports/transport.py` & `aiida_core-2.4.0/aiida/transports/transport.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/transports/util.py` & `aiida_core-2.4.0/aiida/transports/util.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/workflows/__init__.py` & `aiida_core-2.4.0/aiida/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/workflows/arithmetic/__init__.py` & `aiida_core-2.4.0/aiida/workflows/arithmetic/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/workflows/arithmetic/add_multiply.py` & `aiida_core-2.4.0/aiida/workflows/arithmetic/add_multiply.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/aiida/workflows/arithmetic/multiply_add.py` & `aiida_core-2.4.0/aiida/workflows/arithmetic/multiply_add.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/environment.yml` & `aiida_core-2.4.0/environment.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 # Usage: conda env create -n myenvname -f environment.yml
 ---
 name: aiida
 channels:
 - conda-forge
 - defaults
 dependencies:
-- python~=3.8
+- python~=3.9
 - alembic~=1.2
 - archive-path~=0.4.2
 - aio-pika~=6.6
 - circus~=0.18.0
 - click-spinner~=0.1.8
 - click~=8.1
 - disk-objectstore~=0.6.0
 - docstring_parser
 - get-annotations~=0.1
 - python-graphviz~=0.19
-- ipython<9,>=7
+- ipython>=7
 - jinja2~=3.0
 - jsonschema~=3.0
 - kiwipy[rmq]~=0.7.7
 - importlib-metadata~=4.13
-- importlib-resources~=5.0
-- numpy~=1.19
+- numpy~=1.21
 - paramiko>=2.7.2,~=2.7
 - plumpy~=0.21.6
 - pgsu~=0.2.1
 - psutil~=5.6
 - psycopg2-binary~=2.8
 - pytz~=2021.1
 - pyyaml~=6.0
```

### Comparing `aiida_core-2.3.1/open_source_licenses.txt` & `aiida_core-2.4.0/open_source_licenses.txt`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/pyproject.toml` & `aiida_core-2.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -12,40 +12,38 @@
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Framework :: AiiDA",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS :: MacOS X",
     "Programming Language :: Python",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering"
 ]
 keywords = ["aiida", "workflows"]
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 dependencies = [
     "alembic~=1.2",
     "archive-path~=0.4.2",
     "aio-pika~=6.6",
     "circus~=0.18.0",
     "click-spinner~=0.1.8",
     "click~=8.1",
     "disk-objectstore~=0.6.0",
     "docstring-parser",
     "get-annotations~=0.1;python_version<'3.10'",
     "graphviz~=0.19",
-    "ipython>=7,<9",
+    "ipython>=7",
     "jinja2~=3.0",
     "jsonschema~=3.0",
     "kiwipy[rmq]~=0.7.7",
     "importlib-metadata~=4.13",
-    "importlib-resources~=5.0;python_version<'3.9'",
-    "numpy~=1.19",
+    "numpy~=1.21",
     "paramiko~=2.7,>=2.7.2",
     "plumpy~=0.21.6",
     "pgsu~=0.2.1",
     "psutil~=5.6",
     "psycopg2-binary~=2.8",
     "pytz~=2021.1",
     "pyyaml~=6.0",
@@ -66,15 +64,15 @@
 ssh_kerberos = [
     "gssapi~=1.6",
     "pyasn1~=0.4.8"
 ]
 rest = [
     "flask-cors~=3.0",
     "flask-restful~=0.3.7",
-    "flask~=2.0",
+    "flask~=2.2",
     "pyparsing~=2.4",
     "python-memcached~=1.59",
     "seekpath~=1.9,>=1.9.3"
 ]
 docs = [
     "pydata-sphinx-theme~=0.8.0",
     "sphinx~=4.1",
@@ -93,23 +91,23 @@
     "matplotlib~=3.3,>=3.3.4",
     "pymatgen>=2022.1.20",
     "pymysql~=0.9.3",
     "seekpath~=1.9,>=1.9.3",
     "spglib>=1.14,<3.0"
 ]
 notebook = [
-    "jupyter-client~=6.1,<6.1.13",
+    "jupyter-client~=8.0",
     "jupyter~=1.0",
     "notebook~=6.1,>=6.1.5"
 ]
 pre-commit = [
     "mypy==0.991",
     "packaging==20.3",
     "pre-commit~=2.2",
-    "pylint~=2.11.1",
+    "pylint~=2.17.4",
     "pylint-aiida~=0.1.1",
     "sqlalchemy[mypy]~=1.4.29",
     "tomli",
     "types-PyYAML",
 ]
 tests = [
     "aiida-export-migration-tests==0.9.0",
@@ -268,15 +266,14 @@
 load-plugins = ["pylint_aiida"]
 
 [tool.pylint.format]
 max-line-length = 120
 
 [tool.pylint.messages_control]
 disable = [
-    "bad-continuation",
     "consider-using-f-string",
     "cyclic-import",
     "duplicate-code",
     "import-outside-toplevel",
     "inconsistent-return-statements",
     "locally-disabled",
     "logging-fstring-interpolation",
@@ -284,14 +281,17 @@
     "raise-missing-from",
     "too-few-public-methods",
     "too-many-ancestors",
     "too-many-arguments",
     "too-many-instance-attributes",
     # this can be removed when https://github.com/PyCQA/astroid/issues/1015 is fixed
     "not-context-manager",
+    "unnecessary-lambda-assignment",
+    "use-dict-literal",
+    "unnecessary-dunder-call",
 ]
 
 [tool.pylint.basic]
 good-names = [
     "_",
     "x",
     "y",
@@ -302,15 +302,23 @@
     "dt",
     "pk",
     "fg",
     "tz",
     "nl",
     "TemplatereplacerCalculation",
     "ArithmeticAddCalculation",
-    "MultiplyAddWorkChain"
+    "MultiplyAddWorkChain",
+    "SelfType",
+    "EntityType",
+    "MethodType",
+    "ReturnType",
+    "BackendNodeType",
+    "EnumType",
+    "CollectionType",
+    "BackendEntityType",
 ]
 no-docstring-rgx = "^_,setUp,tearDown"
 docstring-min-length = 5
 
 [tool.pylint.design]
 max-locals = 20
 
@@ -437,34 +445,34 @@
 legacy_tox_ini = """
 [tox]
 envlist = py38
 
 [testenv]
 usedevelop=True
 deps =
-    py38: -rrequirements/requirements-py-3.8.txt
     py39: -rrequirements/requirements-py-3.9.txt
     py310: -rrequirements/requirements-py-3.10.txt
+    py311: -rrequirements/requirements-py-3.11.txt
 
-[testenv:py{38,39,310}]
+[testenv:py{39,310,311}]
 passenv =
     PYTHONASYNCIODEBUG
 setenv =
     AIIDA_WARN_v3 = 1
     SQLALCHEMY_WARN_20 = 1
 commands = pytest {posargs}
 
-[testenv:py{38,39,310}-verdi]
+[testenv:py{39,310,311}-verdi]
 passenv =
     AIIDA_TEST_BACKEND
 setenv =
     AIIDA_PATH = {toxinidir}/.tox/.aiida
 commands = verdi {posargs}
 
-[testenv:py{38,39,310}-docs-{clean,update}]
+[testenv:py{39,310,311}-docs-{clean,update}]
 description =
     clean: Build the documentation (remove any existing build)
     update: Build the documentation (modify any existing build)
 passenv = RUN_APIDOC
 setenv =
     update: RUN_APIDOC = False
 changedir = docs
@@ -473,27 +481,27 @@
     clean: make clean
     make debug
 
 [testenv:py{38,39,310}-docs-live]
 # tip: remove apidocs before using this feature (`cd docs; make clean`)
 description = Build the documentation and launch browser (with live updates)
 deps =
-    py38: -rrequirements/requirements-py-3.8.txt
     py39: -rrequirements/requirements-py-3.9.txt
     py310: -rrequirements/requirements-py-3.10.txt
+    py311: -rrequirements/requirements-py-3.11.txt
     sphinx-autobuild
 setenv =
     RUN_APIDOC = False
 commands =
     sphinx-autobuild \
         --re-ignore build/.* \
         --port 0 --open-browser \
         -n -b {posargs:html} docs/source/ docs/build/{posargs:html}
 
-[testenv:py{38,39,310}-pre-commit]
+[testenv:py{39,310,311}-pre-commit]
 description = Run the pre-commit checks
 extras = pre-commit
 commands = pre-commit run {posargs}
 
 [testenv:molecule]
 description = Run the molecule containerised tests
 skip_install = true
```

### Comparing `aiida_core-2.3.1/requirements/requirements-py-3.11.txt` & `aiida_core-2.4.0/requirements/requirements-py-3.11.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,195 +1,214 @@
+#
+# This file is autogenerated by pip-compile with Python 3.11
+# by the following command:
+#
+#    pip-compile --extra=atomic_tools --extra=docs --extra=notebook --extra=rest --extra=tests --no-annotate --output-file=requirements/requirements-py-3.11.txt pyproject.toml
+#
 aiida-export-migration-tests==0.9.0
 aio-pika==6.8.1
 aiormq==3.3.1
-alabaster==0.7.12
-alembic==1.8.1
+alabaster==0.7.13
+alembic==1.11.1
 aniso8601==9.0.1
-anyio==3.6.2
+anyio==3.7.0
 archive-path==0.4.2
 argon2-cffi==21.3.0
 argon2-cffi-bindings==21.2.0
 ase==3.22.1
 asn1crypto==1.5.1
+asttokens==2.2.1
 async-generator==1.10
-attrs==22.1.0
-Babel==2.11.0
+attrs==23.1.0
+babel==2.12.1
 backcall==0.2.0
 bcrypt==4.0.1
-beautifulsoup4==4.11.1
-bleach==5.0.1
-certifi==2022.12.7
+beautifulsoup4==4.12.2
+bleach==6.0.0
+blinker==1.6.2
+certifi==2023.5.7
 cffi==1.15.1
-charset-normalizer==2.1.1
+charset-normalizer==3.1.0
 circus==0.18.0
 click==8.1.3
 click-spinner==0.1.10
-configobj==5.0.6
-contourpy==1.0.6
+comm==0.1.3
+contourpy==1.1.0
 coverage==6.5.0
-cryptography==39.0.1
+cryptography==41.0.1
 cycler==0.11.0
-debugpy==1.6.4
+debugpy==1.6.7
 decorator==5.1.1
 defusedxml==0.7.1
 deprecation==2.1.0
 disk-objectstore==0.6.0
-docstring-parser==0.15.0
+docstring-parser==0.15
 docutils==0.16
-emmet-core==0.39.0
-fastjsonschema==2.16.2
-Flask==2.1.3
-Flask-Cors==3.0.10
-Flask-RESTful==0.3.9
-fonttools==4.38.0
+emmet-core==0.57.1
+executing==1.2.0
+fastjsonschema==2.17.1
+flask==2.3.2
+flask-cors==3.0.10
+flask-restful==0.3.10
+fonttools==4.40.0
 future==0.18.3
 graphviz==0.20.1
-greenlet==2.0.1
+greenlet==2.0.2
 idna==3.4
 imagesize==1.4.1
 importlib-metadata==4.13.0
-iniconfig==1.1.1
-ipykernel==6.17.1
-ipython==8.10.0
+iniconfig==2.0.0
+ipykernel==6.23.2
+ipython==8.14.0
 ipython-genutils==0.2.0
-ipywidgets==8.0.2
+ipywidgets==8.0.6
 itsdangerous==2.1.2
 jedi==0.18.2
-Jinja2==3.1.2
-jsonschema==3.2.0
+jinja2==3.1.2
+jsonschema[format-nongpl]==3.2.0
 jupyter==1.0.0
-jupyter-cache==0.5.0
-jupyter-client==6.1.12
-jupyter-console==6.4.2
-jupyter-server==1.23.3
-jupyter_core==5.1.0
+jupyter-cache==0.6.1
+jupyter-client==8.2.0
+jupyter-console==6.6.3
+jupyter-core==5.3.1
+jupyter-events==0.6.3
+jupyter-server==2.6.0
+jupyter-server-terminals==0.4.4
 jupyterlab-pygments==0.2.2
-jupyterlab-widgets==3.0.3
-kiwipy==0.7.7
+jupyterlab-widgets==3.0.7
+kiwipy[rmq]==0.7.7
 kiwisolver==1.4.4
 latexcodec==2.0.1
-Mako==1.2.4
-markdown-it-py==2.1.0
-MarkupSafe==2.1.1
-matplotlib==3.6.2
+mako==1.2.4
+markdown-it-py==2.2.0
+markupsafe==2.1.3
+matplotlib==3.7.1
 matplotlib-inline==0.1.6
-mdit-py-plugins==0.3.1
+mdit-py-plugins==0.3.5
 mdurl==0.1.2
-mistune==2.0.4
-monty==2022.9.9
-mp-api==0.29.8
-mpmath==1.2.1
-msgpack==1.0.4
-multidict==6.0.2
-myst-nb==0.17.1
+mistune==3.0.1
+monty==2023.5.8
+mp-api==0.33.3
+mpmath==1.3.0
+msgpack==1.0.5
+multidict==6.0.4
+myst-nb==0.17.2
 myst-parser==0.18.1
-nbclassic==0.4.8
-nbclient==0.5.13
-nbconvert==7.2.5
-nbformat==5.7.0
+nbclassic==1.0.0
+nbclient==0.7.4
+nbconvert==7.6.0
+nbformat==5.9.0
 nest-asyncio==1.5.6
-networkx==2.8.8
-notebook==6.5.2
-notebook_shim==0.2.2
-numpy==1.23.5
-packaging==21.3
-palettable==3.3.0
+networkx==3.1
+notebook==6.5.4
+notebook-shim==0.2.3
+numpy==1.25.0
+overrides==7.3.1
+packaging==23.1
+palettable==3.3.3
 pamqp==2.3.0
-pandas==1.5.2
+pandas==2.0.2
 pandocfilters==1.5.0
 paramiko==2.12.0
 parso==0.8.3
 pexpect==4.8.0
-pg8000==1.29.3
+pg8000==1.29.8
 pgsu==0.2.3
 pgtest==1.3.2
 pickleshare==0.7.5
-Pillow==9.3.0
-platformdirs==2.5.4
-plotly==5.11.0
+pillow==9.5.0
+platformdirs==3.6.0
+plotly==5.15.0
 pluggy==1.0.0
-plumpy==0.21.6
-prometheus-client==0.15.0
-prompt-toolkit==3.0.37
-psutil==5.9.4
-psycopg2-binary==2.9.5
+plumpy==0.21.8
+prometheus-client==0.17.0
+prompt-toolkit==3.0.38
+psutil==5.9.5
+psycopg2-binary==2.9.6
 ptyprocess==0.7.0
-py==1.11.0
+pure-eval==0.2.2
 py-cpuinfo==9.0.0
 pybtex==0.24.0
-PyCifRW==4.4.5
+pycifrw==4.4.5
 pycparser==2.21
-pydantic==1.10.2
+pydantic==1.10.9
 pydata-sphinx-theme==0.8.1
-Pygments==2.13.0
-pymatgen==2022.9.21
-Pympler==0.9
-PyMySQL==0.9.3
-PyNaCl==1.5.0
+pygments==2.15.1
+pymatgen==2023.5.31
+pympler==0.9
+pymysql==0.9.3
+pynacl==1.5.0
 pyparsing==2.4.7
-pyrsistent==0.19.2
-pytest==7.2.0
+pyrsistent==0.19.3
+pytest==7.3.2
 pytest-asyncio==0.16.0
 pytest-benchmark==4.0.0
 pytest-cov==2.10.1
 pytest-datadir==1.4.1
-pytest-regressions==2.4.1
+pytest-regressions==2.4.2
 pytest-rerunfailures==9.1.1
 pytest-timeout==1.4.2
 python-dateutil==2.8.2
+python-json-logger==2.0.7
 python-memcached==1.59
 pytray==0.3.4
 pytz==2021.3
-PyYAML==6.0
-pyzmq==24.0.1
-qtconsole==5.4.0
-QtPy==2.3.0
-requests==2.28.1
-ruamel.yaml==0.17.21
-scipy==1.9.3
+pyyaml==6.0
+pyzmq==25.1.0
+qtconsole==5.4.3
+qtpy==2.3.1
+requests==2.31.0
+rfc3339-validator==0.1.4
+rfc3986-validator==0.1.1
+ruamel-yaml==0.17.32
+ruamel-yaml-clib==0.2.7
+scipy==1.10.1
 scramp==1.4.4
 seekpath==1.9.7
-Send2Trash==1.8.0
+send2trash==1.8.2
 shortuuid==1.0.11
 six==1.16.0
 sniffio==1.3.0
 snowballstemmer==2.2.0
-soupsieve==2.3.2.post1
+soupsieve==2.4.1
 spglib==2.0.2
-Sphinx==4.5.0
-sphinx-copybutton==0.5.1
+sphinx==4.5.0
+sphinx-copybutton==0.5.2
 sphinx-design==0.0.13
 sphinx-intl==2.1.0
 sphinx-notfound-page==0.8.3
 sphinx-sqlalchemy==0.1.1
-sphinxcontrib-applehelp==1.0.2
+sphinxcontrib-applehelp==1.0.4
 sphinxcontrib-details-directive==0.1.0
 sphinxcontrib-devhelp==1.0.2
-sphinxcontrib-htmlhelp==2.0.0
+sphinxcontrib-htmlhelp==2.0.1
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
 sphinxext-rediraffe==0.2.7
-SQLAlchemy==1.4.44
-SQLAlchemy-Utils==0.37.9
-sympy==1.11.1
+sqlalchemy==1.4.48
+sqlalchemy-utils==0.37.9
+stack-data==0.6.2
+sympy==1.12
 tabulate==0.8.10
-tenacity==8.1.0
-terminado==0.17.0
+tenacity==8.2.2
+terminado==0.17.1
 tinycss2==1.2.1
-toml==0.10.2
-tornado==6.2
-tqdm==4.64.1
-traitlets==5.6.0
-transifex-client==0.12.5
-typing_extensions==4.4.0
+tornado==6.3.2
+tqdm==4.65.0
+traitlets==5.9.0
+typing-extensions==4.6.3
+tzdata==2023.3
 uncertainties==3.1.7
 upf-to-json==0.9.5
-urllib3==1.26.13
-wcwidth==0.2.5
+urllib3==2.0.3
+wcwidth==0.2.6
 webencodings==0.5.1
-websocket-client==1.4.2
-Werkzeug==2.2.3
-widgetsnbextension==4.0.3
-wrapt==1.14.1
-yarl==1.8.1
-zipp==3.11.0
+websocket-client==1.6.0
+werkzeug==2.3.6
+widgetsnbextension==4.0.7
+wrapt==1.15.0
+yarl==1.9.2
+zipp==3.15.0
+
+# The following packages are considered to be unsafe in a requirements file:
+# setuptools
```

### Comparing `aiida_core-2.3.1/requirements/requirements-py-3.9.txt` & `aiida_core-2.4.0/requirements/requirements-py-3.10.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,175 +1,216 @@
+#
+# This file is autogenerated by pip-compile with Python 3.10
+# by the following command:
+#
+#    pip-compile --extra=atomic_tools --extra=docs --extra=notebook --extra=rest --extra=tests --no-annotate --output-file=requirements/requirements-py-3.10.txt pyproject.toml
+#
 aiida-export-migration-tests==0.9.0
-aio-pika==6.8.0
+aio-pika==6.8.1
 aiormq==3.3.1
-alabaster==0.7.12
-alembic==1.7.5
+alabaster==0.7.13
+alembic==1.11.1
 aniso8601==9.0.1
+anyio==3.7.0
 archive-path==0.4.2
-argon2-cffi==21.1.0
-ase==3.22.0
-asn1crypto==1.4.0
+argon2-cffi==21.3.0
+argon2-cffi-bindings==21.2.0
+ase==3.22.1
+asn1crypto==1.5.1
+asttokens==2.2.1
 async-generator==1.10
-attrs==21.2.0
-Babel==2.9.1
+attrs==23.1.0
+babel==2.12.1
 backcall==0.2.0
-bcrypt==3.2.0
-beautifulsoup4==4.10.0
-bleach==4.1.0
-certifi==2022.12.7
-cffi==1.15.0
-charset-normalizer==2.0.8
+bcrypt==4.0.1
+beautifulsoup4==4.12.2
+bleach==6.0.0
+blinker==1.6.2
+certifi==2023.5.7
+cffi==1.15.1
+charset-normalizer==3.1.0
 circus==0.18.0
-click==8.1.0
+click==8.1.3
 click-spinner==0.1.10
-configobj==5.0.6
+comm==0.1.3
+contourpy==1.1.0
 coverage==6.5.0
-cryptography==39.0.1
+cryptography==41.0.1
 cycler==0.11.0
-debugpy==1.5.1
-decorator==5.1.0
+debugpy==1.6.7
+decorator==5.1.1
 defusedxml==0.7.1
 deprecation==2.1.0
 disk-objectstore==0.6.0
-docstring-parser==0.15.0
+docstring-parser==0.15
 docutils==0.16
-entrypoints==0.3
-Flask==2.0.3
-Flask-Cors==3.0.10
-Flask-RESTful==0.3.9
-fonttools==4.28.2
+emmet-core==0.57.1
+exceptiongroup==1.1.1
+executing==1.2.0
+fastjsonschema==2.17.1
+flask==2.3.2
+flask-cors==3.0.10
+flask-restful==0.3.10
+fonttools==4.40.0
 future==0.18.3
-get-annotations==0.1.2
-graphviz==0.19
-greenlet==1.1.2
-idna==3.3
-imagesize==1.3.0
+graphviz==0.20.1
+greenlet==2.0.2
+idna==3.4
+imagesize==1.4.1
 importlib-metadata==4.13.0
-iniconfig==1.1.1
-ipykernel==6.5.1
-ipython==8.10.0
+iniconfig==2.0.0
+ipykernel==6.23.2
+ipython==8.14.0
 ipython-genutils==0.2.0
-ipywidgets==7.6.5
-itsdangerous==2.0.1
-jedi==0.18.1
-Jinja2==3.0.3
-jsonschema==3.2.0
+ipywidgets==8.0.6
+itsdangerous==2.1.2
+jedi==0.18.2
+jinja2==3.1.2
+jsonschema[format-nongpl]==3.2.0
 jupyter==1.0.0
-jupyter-client==6.1.12
-jupyter-console==6.4.0
-jupyter-core==4.11.2
-jupyterlab-pygments==0.1.2
-jupyterlab-widgets==1.0.2
-kiwipy==0.7.7
-kiwisolver==1.3.2
-Mako==1.2.2
-MarkupSafe==2.1.1
-matplotlib==3.5.0
-matplotlib-inline==0.1.3
-mistune==0.8.4
-monty==2021.8.17
-mpmath==1.2.1
-multidict==5.2.0
-myst-nb==0.17.1
-nbclient==0.5.9
-nbconvert==6.3.0
-nbformat==5.1.3
-nest-asyncio==1.5.5
-networkx==2.6.3
-notebook==6.4.10
-numpy==1.22.0
-packaging==21.3
-palettable==3.3.0
-pandas==1.3.4
+jupyter-cache==0.6.1
+jupyter-client==8.2.0
+jupyter-console==6.6.3
+jupyter-core==5.3.1
+jupyter-events==0.6.3
+jupyter-server==2.6.0
+jupyter-server-terminals==0.4.4
+jupyterlab-pygments==0.2.2
+jupyterlab-widgets==3.0.7
+kiwipy[rmq]==0.7.7
+kiwisolver==1.4.4
+latexcodec==2.0.1
+mako==1.2.4
+markdown-it-py==2.2.0
+markupsafe==2.1.3
+matplotlib==3.7.1
+matplotlib-inline==0.1.6
+mdit-py-plugins==0.3.5
+mdurl==0.1.2
+mistune==3.0.1
+monty==2023.5.8
+mp-api==0.33.3
+mpmath==1.3.0
+msgpack==1.0.5
+multidict==6.0.4
+myst-nb==0.17.2
+myst-parser==0.18.1
+nbclassic==1.0.0
+nbclient==0.7.4
+nbconvert==7.6.0
+nbformat==5.9.0
+nest-asyncio==1.5.6
+networkx==3.1
+notebook==6.5.4
+notebook-shim==0.2.3
+numpy==1.25.0
+overrides==7.3.1
+packaging==23.1
+palettable==3.3.3
+pamqp==2.3.0
+pandas==2.0.2
 pandocfilters==1.5.0
-paramiko==2.10.1
+paramiko==2.12.0
 parso==0.8.3
 pexpect==4.8.0
-pg8000==1.23.0
-pgsu==0.2.1
+pg8000==1.29.8
+pgsu==0.2.3
 pgtest==1.3.2
 pickleshare==0.7.5
-Pillow==9.3.0
-plotly==5.4.0
+pillow==9.5.0
+platformdirs==3.6.0
+plotly==5.15.0
 pluggy==1.0.0
-plumpy==0.21.6
-prometheus-client==0.12.0
-prompt-toolkit==3.0.37
-psutil==5.8.0
-psycopg2-binary==2.9.1
+plumpy==0.21.8
+prometheus-client==0.17.0
+prompt-toolkit==3.0.38
+psutil==5.9.5
+psycopg2-binary==2.9.6
 ptyprocess==0.7.0
-py==1.11.0
-py-cpuinfo==8.0.0
-PyCifRW==4.4.3
+pure-eval==0.2.2
+py-cpuinfo==9.0.0
+pybtex==0.24.0
+pycifrw==4.4.5
 pycparser==2.21
-pydata-sphinx-theme==0.8.0
-Pygments==2.11.2
-pymatgen==2022.1.20
-Pympler==0.9
-PyMySQL==0.9.3
-PyNaCl==1.4.0
+pydantic==1.10.9
+pydata-sphinx-theme==0.8.1
+pygments==2.15.1
+pymatgen==2023.5.31
+pympler==0.9
+pymysql==0.9.3
+pynacl==1.5.0
 pyparsing==2.4.7
-pyrsistent==0.18.0
-pytest==7.2.0
+pyrsistent==0.19.3
+pytest==7.3.2
 pytest-asyncio==0.16.0
 pytest-benchmark==4.0.0
 pytest-cov==2.10.1
-pytest-datadir==1.3.1
-pytest-regressions==2.2.0
+pytest-datadir==1.4.1
+pytest-regressions==2.4.2
 pytest-rerunfailures==9.1.1
 pytest-timeout==1.4.2
+python-dateutil==2.8.2
+python-json-logger==2.0.7
 python-memcached==1.59
-pytray==0.3.2
+pytray==0.3.4
 pytz==2021.3
-PyYAML==6.0.0
-pyzmq==22.3.0
-qtconsole==5.2.1
-QtPy==1.11.2
-requests==2.26.0
-ruamel.yaml==0.17.17
-ruamel.yaml.clib==0.2.6
-scipy==1.7.3
-scramp==1.4.1
+pyyaml==6.0
+pyzmq==25.1.0
+qtconsole==5.4.3
+qtpy==2.3.1
+requests==2.31.0
+rfc3339-validator==0.1.4
+rfc3986-validator==0.1.1
+ruamel-yaml==0.17.32
+ruamel-yaml-clib==0.2.7
+scipy==1.10.1
+scramp==1.4.4
 seekpath==1.9.7
-Send2Trash==1.8.0
-setuptools-scm==6.3.2
-shortuuid==1.0.8
+send2trash==1.8.2
+shortuuid==1.0.11
 six==1.16.0
+sniffio==1.3.0
 snowballstemmer==2.2.0
-soupsieve==2.3.1
+soupsieve==2.4.1
 spglib==2.0.2
-sphinx==4.4.0
-sphinx-copybutton==0.5.0
+sphinx==4.5.0
+sphinx-copybutton==0.5.2
 sphinx-design==0.0.13
 sphinx-intl==2.1.0
-sphinx-notfound-page==0.8
+sphinx-notfound-page==0.8.3
 sphinx-sqlalchemy==0.1.1
-sphinxcontrib-applehelp==1.0.2
+sphinxcontrib-applehelp==1.0.4
 sphinxcontrib-details-directive==0.1.0
 sphinxcontrib-devhelp==1.0.2
-sphinxcontrib-htmlhelp==2.0.0
+sphinxcontrib-htmlhelp==2.0.1
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
 sphinxext-rediraffe==0.2.7
-SQLAlchemy==1.4.27
-SQLAlchemy-Utils==0.37.9
-sympy==1.9
-tabulate==0.8.9
-tenacity==8.0.1
-terminado==0.12.1
-testpath==0.5.0
-toml==0.10.2
-tomli==1.2.2
-tornado==6.1
-tqdm==4.62.3
-traitlets==5.1.1
-uncertainties==3.1.6
-upf-to-json==0.9.3
-urllib3==1.26.7
-wcwidth==0.2.5
+sqlalchemy==1.4.48
+sqlalchemy-utils==0.37.9
+stack-data==0.6.2
+sympy==1.12
+tabulate==0.8.10
+tenacity==8.2.2
+terminado==0.17.1
+tinycss2==1.2.1
+tomli==2.0.1
+tornado==6.3.2
+tqdm==4.65.0
+traitlets==5.9.0
+typing-extensions==4.6.3
+tzdata==2023.3
+uncertainties==3.1.7
+upf-to-json==0.9.5
+urllib3==2.0.3
+wcwidth==0.2.6
 webencodings==0.5.1
-Werkzeug==2.2.3
-widgetsnbextension==3.5.2
-wrapt==1.11.2
-yarl==1.7.2
-zipp==3.6.0
+websocket-client==1.6.0
+werkzeug==2.3.6
+widgetsnbextension==4.0.7
+wrapt==1.15.0
+yarl==1.9.2
+zipp==3.15.0
+
+# The following packages are considered to be unsafe in a requirements file:
+# setuptools
```

### Comparing `aiida_core-2.3.1/utils/__init__.py` & `aiida_core-2.4.0/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/utils/dependency_management.py` & `aiida_core-2.4.0/utils/dependency_management.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
     # Read the requirements from 'pyproject.toml'
     pyproject = _load_pyproject()
     install_requirements = [Requirement.parse(r) for r in pyproject['project']['dependencies']]
 
     # python version cannot be overriden from outside environment.yml
     # (even if it is not specified at all in environment.yml)
     # https://github.com/conda/conda/issues/9506
-    conda_requires = ['python~=3.8']
+    conda_requires = ['python~=3.9']
     for req in install_requirements:
         if req.name == 'python' or any(re.match(ignore, str(req)) for ignore in CONDA_IGNORE):
             continue
         conda_requires.append(str(_setuptools_to_conda(req)))
 
     environment = OrderedDict([
         ('name', 'aiida'),
@@ -408,15 +408,15 @@
     pyproject = _load_pyproject()
 
     to_install = {Requirement.parse(r) for r in pyproject['project']['dependencies']}
     for key in extras:
         to_install.update(Requirement.parse(r) for r in pyproject['project']['optional-dependencies'][key])
 
     def get_package_data(name):
-        req = requests.get(f'https://pypi.python.org/pypi/{name}/json')
+        req = requests.get(f'https://pypi.python.org/pypi/{name}/json', timeout=5)
         req.raise_for_status()
         return req.json()
 
     release_data = {requirement: get_package_data(requirement.name)['releases'] for requirement in to_install}
     for requirement, releases in release_data.items():
         releases_ = list(sorted(map(parse, releases)))
         latest_release = [r for r in releases_ if pre_releases or not r.is_prerelease][-1]
```

### Comparing `aiida_core-2.3.1/utils/make_all.py` & `aiida_core-2.4.0/utils/make_all.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/utils/validate_consistency.py` & `aiida_core-2.4.0/utils/validate_consistency.py`

 * *Files identical despite different names*

### Comparing `aiida_core-2.3.1/PKG-INFO` & `aiida_core-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 Metadata-Version: 2.1
 Name: aiida-core
-Version: 2.3.1
+Version: 2.4.0
 Summary: AiiDA is a workflow manager for computational science with a strong focus on provenance, performance and extensibility.
 Keywords: aiida,workflows
 Author-email: The AiiDA team <developers@aiida.net>
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AiiDA
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: alembic~=1.2
 Requires-Dist: archive-path~=0.4.2
 Requires-Dist: aio-pika~=6.6
 Requires-Dist: circus~=0.18.0
 Requires-Dist: click-spinner~=0.1.8
 Requires-Dist: click~=8.1
 Requires-Dist: disk-objectstore~=0.6.0
 Requires-Dist: docstring-parser
 Requires-Dist: get-annotations~=0.1;python_version<'3.10'
 Requires-Dist: graphviz~=0.19
-Requires-Dist: ipython>=7,<9
+Requires-Dist: ipython>=7
 Requires-Dist: jinja2~=3.0
 Requires-Dist: jsonschema~=3.0
 Requires-Dist: kiwipy[rmq]~=0.7.7
 Requires-Dist: importlib-metadata~=4.13
-Requires-Dist: importlib-resources~=5.0;python_version<'3.9'
-Requires-Dist: numpy~=1.19
+Requires-Dist: numpy~=1.21
 Requires-Dist: paramiko~=2.7,>=2.7.2
 Requires-Dist: plumpy~=0.21.6
 Requires-Dist: pgsu~=0.2.1
 Requires-Dist: psutil~=5.6
 Requires-Dist: psycopg2-binary~=2.8
 Requires-Dist: pytz~=2021.1
 Requires-Dist: pyyaml~=6.0
@@ -61,28 +59,28 @@
 Requires-Dist: sphinx-copybutton~=0.5.0 ; extra == "docs"
 Requires-Dist: sphinx-design~=0.0.13 ; extra == "docs"
 Requires-Dist: sphinx-notfound-page~=0.5 ; extra == "docs"
 Requires-Dist: sphinxext-rediraffe~=0.2.4 ; extra == "docs"
 Requires-Dist: sphinx-sqlalchemy~=0.1.1 ; extra == "docs"
 Requires-Dist: sphinx-intl~=2.1.0 ; extra == "docs"
 Requires-Dist: myst-nb~=0.17.0 ; extra == "docs"
-Requires-Dist: jupyter-client~=6.1,<6.1.13 ; extra == "notebook"
+Requires-Dist: jupyter-client~=8.0 ; extra == "notebook"
 Requires-Dist: jupyter~=1.0 ; extra == "notebook"
 Requires-Dist: notebook~=6.1,>=6.1.5 ; extra == "notebook"
 Requires-Dist: mypy==0.991 ; extra == "pre-commit"
 Requires-Dist: packaging==20.3 ; extra == "pre-commit"
 Requires-Dist: pre-commit~=2.2 ; extra == "pre-commit"
-Requires-Dist: pylint~=2.11.1 ; extra == "pre-commit"
+Requires-Dist: pylint~=2.17.4 ; extra == "pre-commit"
 Requires-Dist: pylint-aiida~=0.1.1 ; extra == "pre-commit"
 Requires-Dist: sqlalchemy[mypy]~=1.4.29 ; extra == "pre-commit"
 Requires-Dist: tomli ; extra == "pre-commit"
 Requires-Dist: types-PyYAML ; extra == "pre-commit"
 Requires-Dist: flask-cors~=3.0 ; extra == "rest"
 Requires-Dist: flask-restful~=0.3.7 ; extra == "rest"
-Requires-Dist: flask~=2.0 ; extra == "rest"
+Requires-Dist: flask~=2.2 ; extra == "rest"
 Requires-Dist: pyparsing~=2.4 ; extra == "rest"
 Requires-Dist: python-memcached~=1.59 ; extra == "rest"
 Requires-Dist: seekpath~=1.9,>=1.9.3 ; extra == "rest"
 Requires-Dist: gssapi~=1.6 ; extra == "ssh_kerberos"
 Requires-Dist: pyasn1~=0.4.8 ; extra == "ssh_kerberos"
 Requires-Dist: aiida-export-migration-tests==0.9.0 ; extra == "tests"
 Requires-Dist: pg8000~=1.13 ; extra == "tests"
```


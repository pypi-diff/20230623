# Comparing `tmp/slpkg-4.8.9.tar.gz` & `tmp/slpkg-4.9.0.tar.gz`

## Comparing `slpkg-4.8.9.tar` & `slpkg-4.9.0.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-09 14:23:14.000000 slpkg-4.8.9/
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-09 14:19:35.000000 slpkg-4.8.9/filelists/
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-09 14:19:35.000000 slpkg-4.8.9/filelists/multilib/
--rw-r--r--   0 dslackw   (1000) users      (100)    15477 2023-06-09 14:19:35.000000 slpkg-4.8.9/filelists/multilib/README.ERIC
--rw-r--r--   0 dslackw   (1000) users      (100)      250 2023-06-09 14:19:35.000000 slpkg-4.8.9/filelists/multilib/glibc_packages.pkgs
--rw-r--r--   0 dslackw   (1000) users      (100)      831 2023-06-09 14:19:35.000000 slpkg-4.8.9/filelists/multilib/README
--rw-r--r--   0 dslackw   (1000) users      (100)     4508 2023-06-09 14:19:35.000000 slpkg-4.8.9/filelists/multilib/compat32.pkgs
--rw-r--r--   0 dslackw   (1000) users      (100)       88 2023-06-09 14:19:35.000000 slpkg-4.8.9/filelists/README
--rw-r--r--   0 dslackw   (1000) users      (100)     1189 2023-06-09 14:19:35.000000 slpkg-4.8.9/repositories.txt
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-09 14:19:35.000000 slpkg-4.8.9/slackbuild/
--rw-r--r--   0 dslackw   (1000) users      (100)      941 2023-06-09 14:19:35.000000 slpkg-4.8.9/slackbuild/slack-desc
--rw-r--r--   0 dslackw   (1000) users      (100)      334 2023-06-09 14:19:35.000000 slpkg-4.8.9/slackbuild/doinst.sh
--rw-r--r--   0 dslackw   (1000) users      (100)      304 2023-06-09 14:19:35.000000 slpkg-4.8.9/slackbuild/README
--rwxr-xr-x   0 dslackw   (1000) users      (100)     4114 2023-06-09 14:19:35.000000 slpkg-4.8.9/slackbuild/slpkg.SlackBuild
--rwxr-xr-x   0 dslackw   (1000) users      (100)       70 2023-06-09 14:19:35.000000 slpkg-4.8.9/setup.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1520 2023-06-09 14:19:35.000000 slpkg-4.8.9/.pyproject.toml
--rw-r--r--   0 dslackw   (1000) users      (100)       84 2023-06-09 14:19:35.000000 slpkg-4.8.9/requirements.txt
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-09 14:19:35.000000 slpkg-4.8.9/configs/
--rw-r--r--   0 dslackw   (1000) users      (100)     8802 2023-06-09 14:19:35.000000 slpkg-4.8.9/configs/repositories.toml
--rw-r--r--   0 dslackw   (1000) users      (100)      483 2023-06-09 14:19:35.000000 slpkg-4.8.9/configs/blacklist.toml
--rw-r--r--   0 dslackw   (1000) users      (100)     4129 2023-06-09 14:19:35.000000 slpkg-4.8.9/configs/slpkg.toml
--rw-r--r--   0 dslackw   (1000) users      (100)      381 2023-06-09 14:19:35.000000 slpkg-4.8.9/configs/rules.toml
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-09 14:19:35.000000 slpkg-4.8.9/tests/
--rw-r--r--   0 dslackw   (1000) users      (100)     2337 2023-06-09 14:19:35.000000 slpkg-4.8.9/tests/test_configs.py
--rw-r--r--   0 dslackw   (1000) users      (100)      765 2023-06-09 14:19:35.000000 slpkg-4.8.9/tests/test_checks.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1961 2023-06-09 14:19:35.000000 slpkg-4.8.9/tests/test_utilities.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1565 2023-06-09 14:19:35.000000 slpkg-4.8.9/tests/test_sbo_queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)      256 2023-06-09 14:19:35.000000 slpkg-4.8.9/tests/test_blacklist.py
--rw-r--r--   0 dslackw   (1000) users      (100)      898 2023-06-09 14:19:35.000000 slpkg-4.8.9/tests/test_colors.py
--rw-r--r--   0 dslackw   (1000) users      (100)      902 2023-06-09 14:19:35.000000 slpkg-4.8.9/tests/check_updates_test.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1460 2023-06-09 14:19:35.000000 slpkg-4.8.9/tests/test_upgrade.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1716 2023-06-09 14:19:35.000000 slpkg-4.8.9/tests/test_bin_queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1076 2023-06-09 14:19:35.000000 slpkg-4.8.9/LICENSE
--rwxr-xr-x   0 dslackw   (1000) users      (100)     1624 2023-06-09 14:19:35.000000 slpkg-4.8.9/install.sh
--rw-r--r--   0 dslackw   (1000) users      (100)    47184 2023-06-09 14:19:35.000000 slpkg-4.8.9/ChangeLog.txt
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-09 14:19:35.000000 slpkg-4.8.9/man/
--rw-r--r--   0 dslackw   (1000) users      (100)     9677 2023-06-09 14:19:35.000000 slpkg-4.8.9/man/slpkg.1
--rw-r--r--   0 dslackw   (1000) users      (100)    10865 2023-06-09 14:19:35.000000 slpkg-4.8.9/man/slpkg-fr.1
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-09 14:19:35.000000 slpkg-4.8.9/completion/
--rw-r--r--   0 dslackw   (1000) users      (100)      910 2023-06-09 14:19:35.000000 slpkg-4.8.9/completion/slpkg
--rw-r--r--   0 dslackw   (1000) users      (100)       93 2023-06-09 14:19:35.000000 slpkg-4.8.9/.gitignore
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/
--rw-r--r--   0 dslackw   (1000) users      (100)     4289 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/dialog_configs.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/binaries/
--rw-r--r--   0 dslackw   (1000) users      (100)     1892 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/binaries/required.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1439 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/binaries/queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/binaries/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     7698 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/binaries/install.py
--rw-r--r--   0 dslackw   (1000) users      (100)    65384 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/install_data.py
--rw-r--r--   0 dslackw   (1000) users      (100)    31419 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/repositories.py
--rw-r--r--   0 dslackw   (1000) users      (100)     4367 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/repo_info.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/sbos/
--rw-r--r--   0 dslackw   (1000) users      (100)     1605 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/sbos/queries.py
--rw-r--r--   0 dslackw   (1000) users      (100)    11675 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/sbos/slackbuild.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1151 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/sbos/dependencies.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/sbos/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     4483 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/sbos/sbo_generate.py
--rw-r--r--   0 dslackw   (1000) users      (100)    36699 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/update_repository.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2627 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/progress_bar.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3510 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/downloader.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/models/
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/models/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2655 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/models/models.py
--rw-r--r--   0 dslackw   (1000) users      (100)      887 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/rules.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/views/
--rw-r--r--   0 dslackw   (1000) users      (100)     6604 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/views/view_package.py
--rw-r--r--   0 dslackw   (1000) users      (100)      629 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/views/version.py
--rw-r--r--   0 dslackw   (1000) users      (100)     6335 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/views/cli_menu.py
--rw-r--r--   0 dslackw   (1000) users      (100)     5935 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/views/asciibox.py
--rw-r--r--   0 dslackw   (1000) users      (100)     4110 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/views/help_commands.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/views/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)    10274 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/views/views.py
--rw-r--r--   0 dslackw   (1000) users      (100)     4004 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/choose_packages.py
--rw-r--r--   0 dslackw   (1000) users      (100)      430 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/error_messages.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3637 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/checks.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1350 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/logging_deps.py
--rw-r--r--   0 dslackw   (1000) users      (100)    13634 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/new_configs.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2058 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/multi_process.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3211 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/cleanings.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1881 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/checksum.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1906 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/dialog_box.py
--rw-r--r--   0 dslackw   (1000) users      (100)     4812 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/configs.py
--rw-r--r--   0 dslackw   (1000) users      (100)     7857 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/utilities.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3867 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/dependees.py
--rw-r--r--   0 dslackw   (1000) users      (100)      587 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/toml_error_message.py
--rw-r--r--   0 dslackw   (1000) users      (100)     6348 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/check_updates.py
--rw-r--r--   0 dslackw   (1000) users      (100)     6716 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/remove_packages.py
--rw-r--r--   0 dslackw   (1000) users      (100)      916 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/blacklist.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3491 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/download_only.py
--rw-r--r--   0 dslackw   (1000) users      (100)     4147 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/tracking.py
--rw-r--r--   0 dslackw   (1000) users      (100)      514 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/logging_config.py
--rw-r--r--   0 dslackw   (1000) users      (100)    29920 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/main.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1609 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/find_installed.py
--rw-r--r--   0 dslackw   (1000) users      (100)     4041 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/upgrade.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3428 2023-06-09 14:19:35.000000 slpkg-4.8.9/slpkg/search.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1466 2023-06-09 14:19:35.000000 slpkg-4.8.9/setup.cfg
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-09 14:23:11.000000 slpkg-4.8.9/slpkg.egg-info/
--rw-r--r--   0 dslackw   (1000) users      (100)       86 2023-06-09 14:23:11.000000 slpkg-4.8.9/slpkg.egg-info/entry_points.txt
--rw-r--r--   0 dslackw   (1000) users      (100)        1 2023-06-09 14:23:11.000000 slpkg-4.8.9/slpkg.egg-info/dependency_links.txt
--rw-r--r--   0 dslackw   (1000) users      (100)     1326 2023-06-09 14:23:11.000000 slpkg-4.8.9/slpkg.egg-info/SOURCES.txt
--rw-r--r--   0 dslackw   (1000) users      (100)        6 2023-06-09 14:23:11.000000 slpkg-4.8.9/slpkg.egg-info/top_level.txt
--rw-r--r--   0 dslackw   (1000) users      (100)       77 2023-06-09 14:23:11.000000 slpkg-4.8.9/slpkg.egg-info/requires.txt
--rw-r--r--   0 dslackw   (1000) users      (100)     1257 2023-06-09 14:23:11.000000 slpkg-4.8.9/slpkg.egg-info/PKG-INFO
--rw-r--r--   0 dslackw   (1000) users      (100)     8595 2023-06-09 14:19:35.000000 slpkg-4.8.9/README.md
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-09 14:19:35.000000 slpkg-4.8.9/tools/
--rwxr-xr-x   0 dslackw   (1000) users      (100)      787 2023-06-09 14:19:35.000000 slpkg-4.8.9/tools/gen_sbo_txt.sh
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-23 06:28:51.000000 slpkg-4.9.0/
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-23 05:30:07.000000 slpkg-4.9.0/filelists/
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-23 05:30:07.000000 slpkg-4.9.0/filelists/multilib/
+-rw-r--r--   0 dslackw   (1000) users      (100)    15477 2023-06-23 05:30:07.000000 slpkg-4.9.0/filelists/multilib/README.ERIC
+-rw-r--r--   0 dslackw   (1000) users      (100)      250 2023-06-23 05:30:07.000000 slpkg-4.9.0/filelists/multilib/glibc_packages.pkgs
+-rw-r--r--   0 dslackw   (1000) users      (100)      818 2023-06-23 05:30:07.000000 slpkg-4.9.0/filelists/multilib/README
+-rw-r--r--   0 dslackw   (1000) users      (100)     4508 2023-06-23 05:30:07.000000 slpkg-4.9.0/filelists/multilib/compat32.pkgs
+-rw-r--r--   0 dslackw   (1000) users      (100)       88 2023-06-23 05:30:07.000000 slpkg-4.9.0/filelists/README
+-rw-r--r--   0 dslackw   (1000) users      (100)     1189 2023-06-23 05:30:07.000000 slpkg-4.9.0/repositories.txt
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-23 06:27:28.000000 slpkg-4.9.0/slackbuild/
+-rw-r--r--   0 dslackw   (1000) users      (100)      941 2023-06-23 05:30:07.000000 slpkg-4.9.0/slackbuild/slack-desc
+-rw-r--r--   0 dslackw   (1000) users      (100)      334 2023-06-23 05:30:07.000000 slpkg-4.9.0/slackbuild/doinst.sh
+-rw-r--r--   0 dslackw   (1000) users      (100)      304 2023-06-23 05:30:07.000000 slpkg-4.9.0/slackbuild/README
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     4114 2023-06-23 05:30:07.000000 slpkg-4.9.0/slackbuild/slpkg.SlackBuild
+-rwxr-xr-x   0 dslackw   (1000) users      (100)       70 2023-06-23 05:30:07.000000 slpkg-4.9.0/setup.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1520 2023-06-23 05:30:07.000000 slpkg-4.9.0/.pyproject.toml
+-rw-r--r--   0 dslackw   (1000) users      (100)       84 2023-06-23 05:30:07.000000 slpkg-4.9.0/requirements.txt
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-23 05:30:07.000000 slpkg-4.9.0/configs/
+-rw-r--r--   0 dslackw   (1000) users      (100)     8802 2023-06-23 05:30:07.000000 slpkg-4.9.0/configs/repositories.toml
+-rw-r--r--   0 dslackw   (1000) users      (100)      483 2023-06-23 05:30:07.000000 slpkg-4.9.0/configs/blacklist.toml
+-rw-r--r--   0 dslackw   (1000) users      (100)     4129 2023-06-23 05:30:07.000000 slpkg-4.9.0/configs/slpkg.toml
+-rw-r--r--   0 dslackw   (1000) users      (100)      381 2023-06-23 05:30:07.000000 slpkg-4.9.0/configs/rules.toml
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-23 05:30:07.000000 slpkg-4.9.0/tests/
+-rw-r--r--   0 dslackw   (1000) users      (100)     2337 2023-06-23 05:30:07.000000 slpkg-4.9.0/tests/test_configs.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      765 2023-06-23 05:30:07.000000 slpkg-4.9.0/tests/test_checks.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1961 2023-06-23 05:30:07.000000 slpkg-4.9.0/tests/test_utilities.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1565 2023-06-23 05:30:07.000000 slpkg-4.9.0/tests/test_sbo_queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      256 2023-06-23 05:30:07.000000 slpkg-4.9.0/tests/test_blacklist.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      898 2023-06-23 05:30:07.000000 slpkg-4.9.0/tests/test_colors.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      902 2023-06-23 05:30:07.000000 slpkg-4.9.0/tests/check_updates_test.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1460 2023-06-23 05:30:07.000000 slpkg-4.9.0/tests/test_upgrade.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1716 2023-06-23 05:30:07.000000 slpkg-4.9.0/tests/test_bin_queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1076 2023-06-23 05:30:07.000000 slpkg-4.9.0/LICENSE
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     1624 2023-06-23 05:30:07.000000 slpkg-4.9.0/install.sh
+-rw-r--r--   0 dslackw   (1000) users      (100)    48793 2023-06-23 05:30:07.000000 slpkg-4.9.0/ChangeLog.txt
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-23 05:30:07.000000 slpkg-4.9.0/man/
+-rw-r--r--   0 dslackw   (1000) users      (100)     9677 2023-06-23 05:30:07.000000 slpkg-4.9.0/man/slpkg.1
+-rw-r--r--   0 dslackw   (1000) users      (100)    10865 2023-06-23 05:30:07.000000 slpkg-4.9.0/man/slpkg-fr.1
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-23 05:30:07.000000 slpkg-4.9.0/completion/
+-rw-r--r--   0 dslackw   (1000) users      (100)      910 2023-06-23 05:30:07.000000 slpkg-4.9.0/completion/slpkg
+-rw-r--r--   0 dslackw   (1000) users      (100)       93 2023-06-23 05:30:07.000000 slpkg-4.9.0/.gitignore
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/
+-rw-r--r--   0 dslackw   (1000) users      (100)     4289 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/dialog_configs.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/binaries/
+-rw-r--r--   0 dslackw   (1000) users      (100)     1892 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/binaries/required.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1439 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/binaries/queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/binaries/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     7698 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/binaries/install.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    65384 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/install_data.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    31419 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/repositories.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4367 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/repo_info.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/sbos/
+-rw-r--r--   0 dslackw   (1000) users      (100)     1605 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/sbos/queries.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    11672 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/sbos/slackbuild.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1151 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/sbos/dependencies.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/sbos/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4480 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/sbos/sbo_generate.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    36699 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/update_repository.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2624 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/progress_bar.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3507 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/downloader.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/models/
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/models/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2655 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/models/models.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      887 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/rules.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/views/
+-rw-r--r--   0 dslackw   (1000) users      (100)     6580 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/views/view_package.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      629 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/views/version.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     6335 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/views/cli_menu.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     5935 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/views/asciibox.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4110 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/views/help_commands.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/views/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    10262 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/views/views.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4004 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/choose_packages.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      430 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/error_messages.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3637 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/checks.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1350 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/logging_deps.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    13598 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/new_configs.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2058 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/multi_process.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3211 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/cleanings.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1881 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/checksum.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1906 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/dialog_box.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4755 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/configs.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     7854 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/utilities.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3864 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/dependees.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      587 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/toml_error_message.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     6373 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/check_updates.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     6716 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/remove_packages.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      916 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/blacklist.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3491 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/download_only.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4132 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/tracking.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      514 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/logging_config.py
+-rw-r--r--   0 dslackw   (1000) users      (100)    29917 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/main.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1609 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/find_installed.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     4041 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/upgrade.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3428 2023-06-23 05:30:07.000000 slpkg-4.9.0/slpkg/search.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1465 2023-06-23 05:30:07.000000 slpkg-4.9.0/setup.cfg
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-23 06:28:40.000000 slpkg-4.9.0/slpkg.egg-info/
+-rw-r--r--   0 dslackw   (1000) users      (100)       86 2023-06-23 06:28:40.000000 slpkg-4.9.0/slpkg.egg-info/entry_points.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)        1 2023-06-23 06:28:40.000000 slpkg-4.9.0/slpkg.egg-info/dependency_links.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)     1326 2023-06-23 06:28:40.000000 slpkg-4.9.0/slpkg.egg-info/SOURCES.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)        6 2023-06-23 06:28:40.000000 slpkg-4.9.0/slpkg.egg-info/top_level.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)       77 2023-06-23 06:28:40.000000 slpkg-4.9.0/slpkg.egg-info/requires.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)     3113 2023-06-23 06:28:40.000000 slpkg-4.9.0/slpkg.egg-info/PKG-INFO
+-rw-r--r--   0 dslackw   (1000) users      (100)     1863 2023-06-23 05:30:07.000000 slpkg-4.9.0/README.md
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-06-23 05:30:07.000000 slpkg-4.9.0/tools/
+-rwxr-xr-x   0 dslackw   (1000) users      (100)      787 2023-06-23 05:30:07.000000 slpkg-4.9.0/tools/gen_sbo_txt.sh
```

### Comparing `slpkg-4.8.9/filelists/multilib/README.ERIC` & `slpkg-4.9.0/filelists/multilib/README.ERIC`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/filelists/multilib/README` & `slpkg-4.9.0/filelists/multilib/README`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-Date: 04/04/2023
+Date: 12/06/2023
 
 Slackware for x86_64 - multilib packages & install instructions
 ---------------------------------------------------------------
 
 Before proceeding with the installation, it is better to read Eric's instructions.
 You will find the file README.ERIC for this purpose, or refer directly to:
 http://www.slackware.com/~alien/multilib/
 
 In this folder, there are two lists, as Eric says, you should install first the glibc packages
 and then the 32-bit compatibility packages. First, edit the '/etc/slpkg/repositories.toml' file
 and enable the 'multilib' repository and then:
 
-  $ slpkg update --bin-repo=multilib
+  $ slpkg update --repository=multilib
 
-  $ slpkg install glibc_packages.pkgs --reinstall --bin-repo=multilib
+  $ slpkg install glibc_packages.pkgs --repository=multilib
 
-  and
-
-  $ slpkg install compat32.pkgs --bin-repo=multilib
+  $ slpkg install compat32.pkgs --repository=multilib
 
 Please read README.ERIC for more or visit the site as I say above.
 
 Enjoy!
```

### Comparing `slpkg-4.8.9/filelists/multilib/compat32.pkgs` & `slpkg-4.9.0/filelists/multilib/compat32.pkgs`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/repositories.txt` & `slpkg-4.9.0/repositories.txt`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/slackbuild/slack-desc` & `slpkg-4.9.0/slackbuild/slack-desc`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/slackbuild/slpkg.SlackBuild` & `slpkg-4.9.0/slackbuild/slpkg.SlackBuild`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/.pyproject.toml` & `slpkg-4.9.0/.pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "slpkg"
-version = "4.8.3"
+version = "4.9.0"
 authors = [
     {name = "Dimitris Zlatanidis", email = "dslackw@gmail.com"},
 ]
 description = "Package manager utility for Slackware Linux"
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = ["slackware", "linux", "package", "manager", "tool"]
```

### Comparing `slpkg-4.8.9/configs/repositories.toml` & `slpkg-4.9.0/configs/repositories.toml`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/configs/slpkg.toml` & `slpkg-4.9.0/configs/slpkg.toml`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/tests/test_configs.py` & `slpkg-4.9.0/tests/test_configs.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/tests/test_checks.py` & `slpkg-4.9.0/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/tests/test_utilities.py` & `slpkg-4.9.0/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/tests/test_sbo_queries.py` & `slpkg-4.9.0/tests/test_sbo_queries.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/tests/test_colors.py` & `slpkg-4.9.0/tests/test_colors.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/tests/check_updates_test.py` & `slpkg-4.9.0/tests/check_updates_test.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/tests/test_upgrade.py` & `slpkg-4.9.0/tests/test_upgrade.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/tests/test_bin_queries.py` & `slpkg-4.9.0/tests/test_bin_queries.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/LICENSE` & `slpkg-4.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/install.sh` & `slpkg-4.9.0/install.sh`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/ChangeLog.txt` & `slpkg-4.9.0/ChangeLog.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,2073 +1,2229 @@
-4.8.9 - 06/06/2023
-Fixed
+## slpkg - ChangeLog
+
+### 4.9.0 - 21/06/2023
+Updated:
+ - For multilib install instructions
+
+ Fixed:
+ - Continuing updating repositories after failing once
+
+### 4.8.9 - 06/06/2023
+Fixed:
 - urllib3.exceptions.NewConnectionError (Thanks to rizitis) #173
 
-4.8.8 - 29/05/2023
+### 4.8.8 - 29/05/2023
 Updated:
 - France manpage
+
 Fixed:
 - Choose dependencies for upgraded packages
 - Build packages with the same source name:
   (nvidia-driver and nvidia-kernel use the same source NVIDIA-Linux-x86_64-<VERSION>.run)
 
-4.8.7 - 23/05/2023
+### 4.8.7 - 23/05/2023
 Fixed:
 - Package tag for slack_patches and salixos_patches
 - Parallel download for slackbuilds repositories (sbo, ponce)
 
-4.8.6 - 21/05/2023
+### 4.8.6 - 21/05/2023
 Updated:
 - Load the database when used #172
+
 Fixed:
 - ValueError with search command
 - Updates some packages to the same version #169
 - For --skip-installed option
+
 Added:
 - Configuration file rules.toml
 
-4.8.5 - 18/05/2023
+### 4.8.5 - 18/05/2023
 Fixed:
 - Case-sensitive with commands find and search
 - For combination options with --repository= and --directory=
 - TypeError for repo-info command #171
 
-4.8.4 - 14/05/2023
+### 4.8.4 - 14/05/2023
 Added:
 - Case-insensitive pattern matching, --no-case option
 - Choose border color via configuration file
 - New processing status view for build, install, upgrade, remove
+
 Fixed:
 - Remove chosen dependencies
 
-4.8.3 - 29/04/2023
+### 4.8.3 - 29/04/2023
 Updated:
 - For synchronization with the local repository (Thanks to Christopher Schrauben) #166
 - Renamed the option --bin-repo with --repository
+
 Added:
 - Options --install-data to install only data into the database
 - Column for package installed version (Thanks to tpiszcze)
 
-4.8.2 - 25/04/2023
+### 4.8.2 - 25/04/2023
 Updated:
 - For exit status code
 - Packages summary for calculating the file sizes
+
 Added:
 - Disable or enable the spinning bar
+
 Fixed:
 - Slackware patches repository tag
 - For skip to download sources if the package is installed (Thanks to kingbeowulf LQ63)
 
-4.8.1 - 21/04/2023
+### 4.8.1 - 21/04/2023
 Updated:
 - For error messages
 - For repository updates (Thanks to rizitis)
 - For reinstall slackware command
+
 Fixed:
 - Double packages as main and as dependency for binaries repos
 - View packages for ponce repository (Thanks to rizitis)
 
-4.8.0 - 19/04/2023
+### 4.8.0 - 19/04/2023
 Fixed:
 - Counting dependencies for tracking and blacklist packages
 - Resolving dependencies when are blacklisted or not included in the repository
 
-4.7.9 - 15/04/2023
+### 4.7.9 - 15/04/2023
 Updated:
 - For proxies configuration
 - For convert file sizes
 - For packages upgrade
+
 Fixed:
 - Clear screen when dialog is disabled
+
 Added:
 - Support to local repositories (Thanks to marav)
 
-4.7.8 - 12/04/2023
+### 4.7.8 - 12/04/2023
 Added:
 - Module to support for Unix shell-style wildcards for blacklist (Thanks to marav)
 - Supports proxies (Thanks to tpiszcze) #160
+
 Updated:
 - Config file for --reinstall option (Thanks to rizitis)
 - Improve speed
 
-4.7.7 - 07/04/2023
+### 4.7.7 - 07/04/2023
 Updated:
 - Improve speed (Replace multi SQL queries)
+
 Fixed:
 - For binaries double dependencies
 - For remove package version
 - Alignment for package name and version
+
 Added:
 - Slots '__slots__' to improve speed
 - Remove local repository data
 
-4.7.6 - 04/04/2023
+### 4.7.6 - 04/04/2023
 Fixed:
 - Upgrade packages with build numbers greater to >= 10
+
 Updated:
 - Indicate colour for upgradable packages
 - Upgrade packages by repository
+
 Added:
 - Packages list for multilib installation
 - To detect the dependencies before removing a package (Thanks to marav)
 - The flag -y, --yes to the remove command
 - To support wget2 downloader
 
-4.7.5 - 04/04/2023
+### 4.7.5 - 04/04/2023
 BugFixed:
 - Upgrade packages from repositories
 
-4.7.4 - 04/04/2023
+### 4.7.4 - 04/04/2023
 Fixed:
 - Python typing hints
 - Upgrade packages
+
 Updated:
 - For upgradable color in installation
 
-4.7.3 - 03/04/2023
+### 4.7.3 - 03/04/2023
 Fixed:
 - Option -B for -u, update and -c, check-updates commands
-- Build packages with the same sources like nvidia-driver and nvidia-kernel
-- Install data mirror for msb, csb, salixos_etxra and salixos_patches repositories
+- Build packages with the same sources as nvidia-driver and nvidia-kernel
+- Install data mirror for msb, csb, salixos_extra and salixos_patches repositories
 
-4.7.2 - 02/04/2023
+### 4.7.2 - 02/04/2023
 Updated:
 - Packaging parse versions
 - For options '-B=', '-z=' to '-B' and '-z'
+
 Fixed:
 - Upgrade dependencies without -r option
 - Patch slackbuild repo tag
 - File pattern '*' for find all installed files
 
-4.7.1 - 02/04/2023
+### 4.7.1 - 02/04/2023
 Fixed:
 - TypeError: can only concatenate str (not "NoneType") to str
 
-4.7.0 - 02/04/2023
+### 4.7.0 - 02/04/2023
 Updated:
 - Checks for recurring options
 - Improve speed and quality
+
 Removed:
 - File pattern from cli menu
+
 Added:
 - Binaries support repositories
 - Sixteen binaries repositories
 - Repositories information
 
-4.6.1 - 15/03/2023
+### 4.6.1 - 15/03/2023
 Updated:
 - For empty arguments
 - Checks for invalid options
 - The error messages
+
 Added:
 - Vimdiff in the slpkg_new-configs command file (Thanks to tkor)
 
+### 4.6.0 - 15/03/2023
 Updated:
 - Dialog text help for dependencies
 - For configs error messages
 - Wget options, removed -N timestamping
+
 Fixed:
 - Summary for upgrade packages
 - Process for KeyboardInterrupt
+
 Added:
 - Progress spinner and color to choose in the config
 
+### 4.5.9 - 14/03/2023
 BugFixed:
 - Default build path /tmp/slpkg/build
 - Build a package with multiple sources
+
 Added:
 - lftp as the source file downloader
 - Support for multiprocess downloading
 - Config for parallel download
 - Option --parallel to download in parallel
 - Build tag to the view packages (Thanks to marav)
+
 Updated:
 - Upgrade packages with the same versions but with different build tags (Thanks to marav)
 - Moved new-configs to slpkg_new-configs
 
-4.5.8 - 09/03/2023
+### 4.5.8 - 09/03/2023
 Updated:
 - View the name of the repository instead of the size
 - Highlighted with grey of the installed packages
 - Ignored question when there are updates available
 
-4.5.7 - 07/03/2023
+### 4.5.7 - 07/03/2023
 Added:
 - Ignore comments for list.pkgs files (Thanks to rizitis)
 - The file pattern in the config file
 - Command new-configs to managing .new files
+
 Updated:
 - Blacklist config file
 - To support '.sqf' files (Thanks to rizitis)
+
 Fixed:
 - TypeError: '<' not supported between instances of 'str' and 'int
 
-4.5.6 - 03/03/2023
+### 4.5.6 - 03/03/2023
 Updated:
 - Ponce repository
 - slpkg.toml file for ponce repository
+
 Added:
 - Option --generate-only for ponce repository
 - Command clean-data to delete repositories data
 - Dialog text help for items
 - Read packages from file
 - Ask question to the config
 
-4.5.5 - 02/03/2023
+### 4.5.5 - 02/03/2023
 Fixed:
-- Genarator type to list return
+- Generator type to list return
 
-4.5.4 - 05/02/2023
+### 4.5.4 - 05/02/2023
 Updated:
 - Message for configs
+
 Added:
 - For concatenating the short options (Thanks to marav)
 - Help command for extra helping
 - Ponce repository
 - lftp downloader
+
 Fixed:
 - TOML decoder error for blacklist file
 - Fixed to compare versions for dependencies (Thanks to marav)
 
-4.5.3 - 27/01/2023
+### 4.5.3 - 27/01/2023
 Added:
 - Short options
 - New configuration for ascii characters
 
-4.5.2 - 21/01/2023
+### 4.5.2 - 21/01/2023
 BugFixed:
 - IndexError: list index out of range
+
 Updated:
- - manpages for options (Thanks to marav)
+ - manapages for options (Thanks to marav)
  Added:
  - Option --file-pattern
  - Curl downloader as the second option
 
-4.5.1 - 16/01/2023
+### 4.5.1 - 16/01/2023
 Added:
 - Option --directory=PATH for download command
 - Option --pkg-version for print repository version
 
-4.5.0 - 14/01/2023
+### 4.5.0 - 14/01/2023
 Updated:
 - Download first all the slackbuilds
 - Rename view_mode to silent_mode
+
 Added:
 - Option --no-silent
 
-4.4.9 - 13/01/2023
+### 4.4.9 - 13/01/2023
 Updated:
 - Color highlight for installed packages
+
 BugFixed:
 - Upgrade packages (Thanks to marav)
 
-4.4.8 - 12/01/2023
+### 4.4.8 - 12/01/2023
 Added:
 - Error ascii box for checksum
 
-4.4.7 - 07/01/2023
+### 4.4.7 - 07/01/2023
 Added:
 - Finished report to download only
 - The French manpage (Thanks to marav)
-- Check if the file dowwnload
+- Check if the file download
+
 Updated:
 - os.istdir method with pathlib module
 
-4.4.6 - 06/01/2023
+### 4.4.6 - 06/01/2023
 Updated:
 - Improve speed for dependees
+
 Fixed:
 - summary for build
+
 Remove:
 - python-toml dependency
 
-4.4.5 - 03/01/2023
+### 4.4.5 - 03/01/2023
 Added:
 - New modern view mode style
 - Progress bar
+
 Updated:
 - Fixed md5sum comparison
 
-4.4.4 - 31/12/2022
+### 4.4.4 - 31/12/2022
 BugFixed:
 - AttributeError: 'PosixPath' object has no attribute 'startswith'
 - KeyError: 'sbo_chglog_txt' #LQ post6401410
 
-4.4.3 - 30/12/2022
+### 4.4.3 - 30/12/2022
 Updated:
 - Switch to pathlib library
 
-4.4.2 - 29/12/2022
+### 4.4.2 - 29/12/2022
 Updated:
 - Improve paths
 
-4.4.1 - 28/12/2022
+### 4.4.1 - 28/12/2022
 Added:
 - configs command to read and edit configuration file
 
-4.4.0 - 23/12/2022
+### 4.4.0 - 23/12/2022
 Added:
 - New command to tracking the dependencies
 - pythondialog as dependency
 - dialog for upgrade, remove and dependencies
 - --full-reverse flag to work with dependees
 - --search flag to enable dialog and choose packages from the repository
 
-4.3.9 - 22/12/2022
+### 4.3.9 - 22/12/2022
 Added:
 - Feature to check the ChangeLog.txt file before update #153
 - Dependees command
 
 BugFixed:
 - View installed version
 - slpkg issue : permission denied #152
+
 Fixed:
 - Colors and messages for upgrade and reinstall
 - Dependencies install order
 
-4.3.7 - 09/12/2022
+### 4.3.7 - 09/12/2022
 Updated:
 - Merge method is_installed in utilities
 
-4.3.6 - 08/12/2022
+### 4.3.6 - 08/12/2022
 Fixed:
 - Remove packages
 
-4.3.5 - 07/12/2022
+### 4.3.5 - 07/12/2022
 Updated:
 - Code style
+
 Fixed:
 - Flags parameter
 
-4.3.4 - 02/12/2022
+### 4.3.4 - 02/12/2022
 Updated:
 - Remove dataclasses and switch to __init__
 - Version print command
+
 Added:
 - Version to the requirements in the view packages command
 - Short cli menu
 
-4.3.3 - 01/12/2022
+### 4.3.3 - 01/12/2022
 Fixed:
 - Blacklist file permissions 0644
 - Typo in the slpkg.toml config file
 - Configuration slpkg.toml file
+
 Updated:
 - Os architecture in the configs
 
-4.3.2 - 28/11/2022
+### 4.3.2 - 28/11/2022
 Fixed:
 - Remove multiple packages with dependencies
+
 Updated:
 - Switch to python toml to load configuration files
 
-4.3.1 - 26/11/2022
+### 4.3.1 - 26/11/2022
 Added:
 - Category in the view command
 - Slackware repo version
-Bugfixed:
+
+Bugfixes:
 - Remove packages equal with the name
 - Install packages with correct sbo tag
 
-4.3.0 - 23/11/2022
+### 4.3.0 - 23/11/2022
 Added:
 - Message for blacklisted packages
 - Homepage in the view command
+
 Updated:
 - The cli menu
 
-4.2.9 - 19/11/2022
-Bugfixed:
+### 4.2.9 - 19/11/2022
+Bugfixes:
 - slpkg upgrade fails when a package is blacklisted #149
+
 Updated:
 - Moved '%README%' to the blacklist
+
 Added:
 - Maintainer info in view command #150
 
-4.2.8 - 06/11/2022
+### 4.2.8 - 06/11/2022
 Updated:
 - Check the SBo script exists before patching the tag
 
-4.2.7 - 05/11/2022
+### 4.2.7 - 05/11/2022
 Fixed:
 - Switch to check ChangeLogs.txt files by size
 
-4.2.6 - 03/11/2022
+### 4.2.6 - 03/11/2022
 Fixed:
 - Check for the file ChangeLog.txt
 
-4.2.5 - 01/11/2022
+### 4.2.5 - 01/11/2022
 Added:
 - Command to check if there is news on ChangeLog.txt
+
 Updated:
 - man page
 
-4.2.4 - 30/10/2022
+### 4.2.4 - 30/10/2022
 Added:
 - Patching SBo TAG from the configuration file
 - Download the SlackBuild script in the view command
+
 Updated:
 - The cli help menu
 
-4.2.3 - 28/10/2022
+### 4.2.3 - 28/10/2022
 Updated:
 - Creating all necessary paths from the config file
 - Logs cleaning view dependencies
+
 Added:
 - Check if database file exists
 - Check if the package exists in the database before upgrade
 
-4.2.2 - 20/10/2022
+### 4.2.2 - 20/10/2022
 Updated:
 - Removed version for skip installed option
 - Removed unused configurations
 - Search command to view
+
 Added:
 - A new search command to search and match packages from the repository
 
-4.2.1 - 18/10/2022
+### 4.2.1 - 18/10/2022
 Added:
 - Print the README file in the search option
+
 Updated:
 - Configs for sbo repository
 
-4.2.0 - 14/10/2022
+### 4.2.0 - 14/10/2022
 Updated:
 - Moved option --download-only to commands
 - Upgrade commands works with all options
 
-4.1.9 - 14/10/2022
+### 4.1.9 - 14/10/2022
 Added:
 - New option --download-only
 
-4.1.8 - 06/10/2022
+### 4.1.8 - 06/10/2022
 Updated:
 - Manpage for .yaml files
 Added:
 - New option --skip-installed
 
-4.1.7 - 28/9/2022
-Bugfixed:
+### 4.1.7 - 28/09/2022
+Bugfixes:
 - Creating /var/lib/slpkg directory
 
-4.1.6 - 26/9/2022
+### 4.1.6 - 26/09/2022
 Added:
 - Configs folder missing from repo
 
-4.1.5 - 9/9/2022
+### 4.1.5 - 09/09/2022
 Updated:
 - Rename config files to .yml
-Bugfixed:
+
+Bugfixes:
 - Show version to noarch packages
 
-4.1.4 - 17/07/2022
+### 4.1.4 - 17/07/2022
 Added:
 - setup.cfg file
 - Option to upgrade sbo packages
 
-4.1.3 - 26/06/2022
-Bugfixed:
+### 4.1.3 - 26/06/2022
+Bugfixes:
 - /tmp permissions after installation
+
 Updated:
 - find installation binary file in /tmp folder
 
-4.1.2 - 24/06/2022
-Bugfixed:
+### 4.1.2 - 24/06/2022
+Bugfixes:
 - Installing noarch packages
 
-4.1.1 - 23/06/2022
+### 4.1.1 - 23/06/2022
 Updated:
 - Cli menu view with colors
 - Switch to yaml configurations
+
 Added:
 - Unittests
 - Command clean-tmp to deletes all downloaded sources from /tmp/slpkg folder
 - Command find installed packages
 
-4.1.0 - 20/06/2022
+### 4.1.0 - 20/06/2022
 Updated:
 - slpkg code re-written from the beginning and currently supports only the SBo repository
 
-4.0.2 - 13/06/2022
+### 4.0.2 - 13/06/2022
 Fixed:
 - database library path
 
-4.0.1 - 30/05/2022
+### 4.0.1 - 30/05/2022
 Added:
 - SQLAlchemy Object Relational Mapper
 
-4.0.0 - 29/05/2022
+### 4.0.0 - 29/05/2022
 Added:
 - sqlite3 database replaced the sbo repository
 - python package 'progress' added as dependency
 
-3.9.9 - 24/05/2022
+### 3.9.9 - 24/05/2022
 Updated:
 - Stderr error output to auto-install packages
 
-3.9.8 - 12/05/2022
+### 3.9.8 - 12/05/2022
 Bugfix:
 - Flag (--repos=) TypeError: exceptions must derive from BaseException
+
 Updated:
 - Slackbuild script switch to bash shell
 
-3.9.7 - 09/05/2022
+### 3.9.7 - 09/05/2022
 Fixed:
 - Stderr error output
+
 Updated:
 - Improve dependencies resolve speed
 - Renamed --repositories to --repos flag
+
 Bugfix:
 - Update custom repositories
 - Passing repositories manual
 
-3.9.6 - 02/04/2022
+### 3.9.6 - 02/04/2022
 Updated:
 - Compared packages version when distribution upgrade
 
-3.9.5 - 02/04/2022
+### 3.9.5 - 02/04/2022
 BugFix:
 - Config variable ONLY_INSTALLED when is set on
 
-3.9.4 - 26/03/2022
+### 3.9.4 - 26/03/2022
 BugFix:
 - Check if a virtual environment exists before run
 
-3.9.3 - 13/02/2022
+### 3.9.3 - 13/02/2022
 Updated:
 - Fix installation crash no TESTING file
 
-3.9.2 - 06/02/2022
+### 3.9.2 - 06/02/2022
 Updated:
 - Slackware mirrors
 - Copyright year
 - urllib3 removed as a dependency it's part of Slackware now
 
-3.9.1 - 01/01/2021
+### 3.9.1 - 01/01/2021
 Updated:
 - Copyright year
+
 Fixed:
 - Fixed --checklist and resolve-off flags #129
 - Bugfix custom repository
 
-3.9.0 - 21/06/2020
+### 3.9.0 - 21/06/2020
 BugFix:
 - Fixed --checklist flag works both with --upgrade option
 
-3.8.9 - 03/06/2020
+### 3.8.9 - 03/06/2020
 BugFix:
 - Fixed Slackware distribution --upgrade flag
 
-3.8.8 - 20/05/2020
+### 3.8.8 - 20/05/2020
 BugFix:
 - Fixed the name of variable flags to flag for patches upgrade option
 
-3.8.7 - 01/04/2020
+### 3.8.7 - 01/04/2020
 BuFix:
-- '--checklist' flag doesn't work since 3.8.1 to 3.8.6 version #127
+- Flag '--checklist' doesn't work since 3.8.1 to 3.8.6 version #127
 
-3.8.6 - 22/03/2020
+### 3.8.6 - 22/03/2020
 BugFix:
 - Message function pkg_not_found arguments
 
-3.8.5 - 5/03/2020
+### 3.8.5 - 05/03/2020
 Added:
 - set export variable $TAG #126
 
-3.8.4 - 25/02/2020
+### 3.8.4 - 25/02/2020
 BugFix:
 - Grab MD5SUM from wrong info file return None
 Updated:
 - Slackware mirrors
 
-3.8.3 - 21/02/2020
+### 3.8.3 - 21/02/2020
 BugFix:
 - Counting packages for binaries repositories
+
 Added:
 - Feature for proxy servers
 
-3.8.2 - 15/02/2020
+### 3.8.2 - 15/02/2020
 Fixed:
 - SBo repository view Packages and New version
 - msb repository PACKAGES.txt file
+
 BugFix:
 - Upgrade distribution with option -c, --check
+
 Added:
 - Managing multi packages in blacklist file
 
-3.8.1 - 13/02/2020
+### 3.8.1 - 13/02/2020
 Fixed:
-- Bugfix double install packages from slack regular repo
+- Double installation packages from slack regular repo
   and patches directory #122
+
 Updated:
 - Removed status progress bar
 - Setup and installing
 - Managed blacklist in the simple way
 
-3.8.0 - 05/02/2020
+### 3.8.0 - 05/02/2020
 Added:
-- Many changes happen in this version, a big part of code has been rewritten
-- to improve the code for support Python 3. Possibly will there are some bugs
-- in the feture versions I would appreciate it if report them.
-
-- Cheers,
-- Dimitris
+- Many changes happen in this version, a big part of code has been rewritten to improve the code for support Python 3. Possibly will there are some bugs in the future versions I would appreciate it if report them.
+  Cheers, Dimitris
 
 Fixed:
 - Bugfix: merge files with slack repository between current and slack versions
 Updated:
 - code to improve for Python 3
 
-3.7.4 - 20/12/2019
+### 3.7.4 - 20/12/2019
 Fixed:
 - Bugfix: UnicodeDecodeError: 'utf-8' codec can't decode byte
 
-3.7.3 - 11/12/2019
-FIxed:
+### 3.7.3 - 11/12/2019
+Fixed:
 - Bugfix: Slackware-current from Alien Bob 20191130 #119
-- Improving call class methods for reposiory updating
+- Improving call class methods for repository updating
 - Replace requests dependency with urllib3
 - Code style to python3 compatibility
 
-3.7.2 - 06/12/2019
+### 3.7.2 - 06/12/2019
 Fixed:
 - Bugfix handle requests raise ConnectionError
 
-3.7.1 - 03/12/2019
+### 3.7.1 - 03/12/2019
 Updated:
 - pythondialog dependency
 - slackware mirrors
 - pip installation method
 - improved setup.py file for python3
 - print function for python3 format
+
 Added:
-- Dependency python requests replace bult-in python urllib
+- Dependency python requests replace built-in python urllib
 
-3.7.0 - 01/12/2019
+### 3.7.0 - 01/12/2019
 Updated:
 - Switch to python3
 
-3.4.3 - 19/05/2019
+### 3.4.3 - 19/05/2019
 Updated:
 - Update gen_repos_files.sh to version 1.94
+
 Fixed:
 - Downloader to recognise the char +
 - Build from sources with char + in name
 
-3.4.2 - 23/01/2019
+### 3.4.2 - 23/01/2019
 Fixed:
-- Bugfixed delete build folder in network option
+- Bugfixes delete build folder in network option
 
-3.4.1 - 23/01/2019
+### 3.4.1 - 23/01/2019
 Fixed:
 - Fix manpage
 
-3.4.0 - 21/01/2019
+### 3.4.0 - 21/01/2019
 Updated:
 - Updated manpage
-- Convert examples, repositories and install text files to markdown format
+- Convert examples, repositories and install text files to Markdown format
 - Merge sbo/remove.py in the slpkg/remove.py file
+
 Fixed:
 - Bugfix: update slpkg itself from gitlab repository
+
 Added:
 - Command 'clean-tmp' to remove the packages and the sources from /tmp/slpkg/ directory
 
-3.3.9 - 14/01/2019
+### 3.3.9 - 14/01/2019
 Updated:
 - Readme file and added example text file
 - Checklist error message
 - Removed unnecessary arguments ALL
+
 Added:
 - Support elilo and grub upgrade boot loader after kernel upgrade
 - View third party packages
 - Remove third party packages
 - Added file size in the removed packages
 
-3.3.8 - 09/06/2018
+### 3.3.8 - 09/06/2018
 Fixed:
 - aria2c (optional downloader) downloading path
+
 Updated:
 - Switch to gitlab repository
 
-3.3.7 - 22/04/2018
+### 3.3.7 - 22/04/2018
 Fixed:
 - Download 'v3.3.6.tar.gz' file [ FAILED ] #109
 
-3.3.6 - 21/04/2018
+### 3.3.6 - 21/04/2018
 Fixed:
 - pip install with print logo #106
 
-3.3.5 - 01/04/2018
+### 3.3.5 - 01/04/2018
 Fixed:
 - pip install fails #106
+
 Updated:
 - Slackware mirrors
 
-3.3.4 - 10/01/2018
+### 3.3.4 - 10/01/2018
 Added:
 - Print the file size per package in option -f, --find
 
-3.3.3 - 01/01/2018
+### 3.3.3 - 01/01/2018
 Updated:
 - README.rst for python modules
-- Remove python3 support temporarily until new Slackware version will be
-release
+- Remove python3 support temporarily until new Slackware version will be release
 - Slackware mirrors
 
-3.3.2 - 21/10/2017
+### 3.3.2 - 21/10/2017
 Fixed:
 - Strange dependency problem (2) #97
 - Msb repository switch to 1.18
+
 Updated:
 - Slackware mirrors
 
-3.3.1 - 07/10/2017
+### 3.3.1 - 07/10/2017
 Added:
 - Set Slackware version via configuration file /etc/slpkg/slpkg.conf
 - Set computer architecture via configuration file /etc/slpkg/slpkg.conf
 
-3.3.0 - 01/10/2017
+### 3.3.0 - 01/10/2017
 Fixed:
-- TypeError: stat() argument 1 must be encoded string without null bytes,
-not str #100
-- Check file script before build (IOError: [Errno 2] No such file or
-directory: )
+- TypeError: stat() argument 1 must be encoded string without null bytes, not str #100
+- Check file script before build (IOError: [Errno 2] No such file or directory:)
 
-3.2.9 - 24/09/2017
+### 3.2.9 - 24/09/2017
 Fixed:
 - Strange dependency problem #97
 
 Added:
 - patches/ directory from slack repository (slpkg -F "slack" fail #98)
 
-3.2.8 - 06/08/2017
+### 3.2.8 - 06/08/2017
 Fixed:
 - BugFix: Package return after build
 
 Updated:
 - Build error message
 
-3.2.7 - 09/04/2017
+### 3.2.7 - 09/04/2017
 Updated:
 - Alien's repositories {alien, ktown, multi} #83 (Thanks to travis-82)
 - Rworkman's repository {rlw} #83
 - Package security message for network and sbo repository
 
 Added:
 - Sbosrcarch as secondary repository for source files #82 (Thanks to
 travis-82)
 - Rebuild packages from sbo repository when upgrading #85 (Thanks to bhreach)
 
-3.2.6 - 22/02/2017
+### 3.2.6 - 22/02/2017
 Updated:
 - Pattern for configuration file
 
 Added:
-- Support the special packages who need attention (OpenGL 32-Bits Libs after
-upgrade #81) Thanks to Edward W. Koenig and Inukaze for the report
+- Support the special packages who need attention (OpenGL 32-Bits Libs after upgrade #81) (Thanks to Edward W. Koenig and Inukaze)
 - pkg_security configuration file
 
-3.2.5 - 17/02/2017
+### 3.2.5 - 17/02/2017
 Updated:
 - Url for mles/mled repository (Thanks Kiki Novak for the report)
 - Switch to arch i586 for sbo repository
 - Switch off progress bar by default
 
 Fixed:
 - Exit codes - another scenario of #73 #79
 
-3.2.4 - 10/02/2017
+### 3.2.4 - 10/02/2017
 Updated:
 - Switch SlackBuild script to arch i586
 - Rename repository slackr to conrad
 - Repository MATE to support Slackware -current x86_64
 
 Added:
 - Repository Cinnamon
 - Repository Connochaetos (slack-n-free)
 - Repository Microlinux {desktop, server, extras}
 
 Fixed:
 - Upgrade package lists
 - Mate repository check for updates
 
-3.2.3 - 07/02/2017
+### 3.2.3 - 07/02/2017
 Updated:
 - Copyright year
 - Slackware mirrors
 
 Fixed:
 - Update package lists after fresh installation (IOError: [Errno 2] No such file
 or directory)
 
-3.2.2 - 26/10/2016
+### 3.2.2 - 26/10/2016
 Added:
 - Support Python3 with 2to3 tool.
 - Build and install with Python 3
 
-3.2.1 - 25/10/2016
+### 3.2.1 - 25/10/2016
 Fixed:
 - Return exit code when packages for installation not found #73
 
-3.2.0 - 19/10/2016
+### 3.2.0 - 19/10/2016
 Added:
-- rlworkman.deps dependencies configuration file
+- Rlworkman.deps dependencies configuration file
 Fixed:
 - BugFix: IndexError: list index out of range, for tracking arguments
+
 Updated:
 - Rworkman's (rlw) repository dependencies for Slackware 14.2
 
-3.1.9 - 17/10/2016
+### 3.1.9 - 17/10/2016
 Updated:
 - Switch to default version 1.16 for msb repository
+
 Fixed:
 - Resolve dependencies for the binaries repositories
 - Remove dependencies for the binaries repositories
+
 Remove:
 - Studioware binary repository because switch to slackbuild type
 
-3.1.8 - 11/10/2016
+### 3.1.8 - 11/10/2016
 Added:
 - Feature rebuild packages for sbo repository and reinstall binaries packages
 - Slackware package management tools. Thanks to Thomas Szteliga #71
+
 Fixed:
 - Print repository error message without usage
 - Count packages in deps-status option
+
 Updated:
 - Help and usage message
 - Slackware mirrors
 - Merge --deps in --check-deps flag in the remove argument
 
-3.1.7 - 14/07/2016
+### 3.1.7 - 14/07/2016
 Fixed:
 - Update only one repository and check and upgrade packages from it #69
 
-3.1.6 - 06/07/2016
+### 3.1.6 - 06/07/2016
 Updated:
 - Slackr (Conraid's) repository url
 - Remove aaa_elflibs from blacklist
 - Slackware mirrors
 
-3.1.5 - 26/05/2016
+### 3.1.5 - 26/05/2016
 Fixed:
 - Option "-l, --list" working with all arguments
 - TypeError: in tracking option when working with binaries repositories
+
 Updated:
 - Code style
 
-3.1.4 - 11/05/2016
+### 3.1.4 - 11/05/2016
 Updated:
 - slackers.it default repository
 
-3.1.3 - 15/04/2016
+### 3.1.3 - 15/04/2016
 Fixed:
-- Working with localy SBo repository
+- Working with locally SBo repository
 
-3.1.2 - 24/02/2016
+### 3.1.2 - 24/02/2016
 Fixed:
 - AttributeError: LooseVersion instance has no attribute 'version'
 - Remove double code
 
-3.1.1 - 23/02/2016
+### 3.1.1 - 23/02/2016
 Added:
 - Feature: don't downgrade packages, setting via configuration file
 
-3.1.0 - 17/02/2016
+### 3.1.0 - 17/02/2016
 Fixed:
 - Downloaded packages for x86 arch in the "slonly" repository #59
 - Continue build and install sbo packages if source link is dead
+
 Updated:
 - Status toolbar
 
-3.0.9 - 09/02/2016
+### 3.0.9 - 09/02/2016
 Fixed:
 - Listed installed packages from repositories with the name only #58
 - Passing char '+' from sources
 
-3.0.8 - 29/01/2016
+### 3.0.8 - 29/01/2016
 Added:
 - Flag "--name" in option list to show only package name
+
 Fixed:
 - Duplicate packages in repository ktown with option list
 
-3.0.7 - 26/01/2016
+### 3.0.7 - 26/01/2016
 Updated:
 - Help menu
 - Positions arguments in "deps-status" for "--tree" and "--graph=" options
 - Slackware mirrors
 
-3.0.6 - 22/01/2016
+### 3.0.6 - 22/01/2016
 Fixed:
 - "IndexError: list index out of range" when remove packages with "--tag" option
+
 Updated:
 - README.rst file
 - Usage and help options
 - Positions arguments in "--desc", "--network" and "--tracking" options
 - Slackware mirrors
 
-3.0.5 - 06/01/2016
+### 3.0.5 - 06/01/2016
 Updated:
-- Positions arguments in queue and blacklist option for "--add" and "--remove"
-flags
+- Positions arguments in queue and blacklist option for "--add" and "--remove" flags
 - Usage arguments
 - Files licence
 
-3.0.4 - 30/12/2015
+### 3.0.4 - 30/12/2015
 Fixed:
 - Cannot install chkrootkit #53
 - Avoid reinstall binary packages if is already installed
 - Reference message when remove one package
+
 Updated:
 - Slackware mirrors
 
-3.0.3 - 01/12/2015
+### 3.0.3 - 01/12/2015
 Fixed:
 - Upgrading/Installing nouveau in slack repository #55
 Updated:
 - Slackware mirrors
 
-3.0.2 - 19/11/2015
+### 3.0.2 - 19/11/2015
 Fixed:
 - Convert string to float when try to remove packages #52
 
-3.0.1 - 12/11/2015
+### 3.0.1 - 12/11/2015
 Added:
-- Option "--download-only" to download packages with all dependencies without
-install.
+- Option "--download-only" to download packages with all dependencies without install.
 - Option "--directory-prefix=" to download packages in specific directory
+
 Fixed:
 - Code style
 
-3.0.0 - 15/10/2015
+### 3.0.0 - 15/10/2015
 Fixed:
 - Return checksums for SBo repository
 
-2.9.7 - 09/10/2015
+### 2.9.7 - 09/10/2015
 Fixed:
 - Find SBo Slackware binary packages from /tmp
 
-2.9.6 - 03/10/2015
+### 2.9.6 - 03/10/2015
 Fixed:
 - "nvidia-kernel" Fails to install #46
 - build fail because of Version is inconsistent #48
 
-2.9.5 - 01/10/2015
+### 2.9.5 - 01/10/2015
 Updated:
 - Check for root privileges
 - Remove header from usage
 
-2.9.4 - 24/09/2015
+### 2.9.4 - 24/09/2015
 Updated:
 - KeyboardInterrupt for main.py
+
 Fixed:
 - Upgrade packages from sbo repository
 - Pylint errors and code health
 
-2.9.3 - 23/09/2015
+### 2.9.3 - 23/09/2015
 Added:
 - Default repositories file to allow editing urls
 - Additional option "--case-ins" case insensitive in "--tracking" option
+
 Fixed:
-- Matching packages with case insensitive option
+- Matching packages with case-insensitive option
 
-2.9.2 - 21/09/2015
+### 2.9.2 - 21/09/2015
 Added:
 - Clear screen in "--network" option
+
 Updated:
 - View doinst.sh in "--network" option if exist
 - Commands in "--network" option
+
 Fixed:
 - Strange problem with node-0.12.7 - uname and rm commands not found. #43
 - 0 package will be installed... Would you like to continue [y/N]? #44
-- Matching packages with case insensitive option
+- Matching packages with case-insensitive option
 - Build package without keep log file
 - Some typos
 
-2.9.1 - 18/09/2015
+### 2.9.1 - 18/09/2015
 Added:
-- Additional option "--deps" in removepkg option for remove dependencies
-instead via configuration file
-- Support ".tbz" and ".tlz" Slackware packages for auto detect option
+- Additional option "--deps" in removepkg option for remove dependencies instead via configuration file
+- Support ".tbz" and ".tlz" Slackware packages for auto-detect option
 
-2.9.0 - 18/09/2015
+### 2.9.0 - 18/09/2015
 Added:
 - Quit option in new-config command
+
 Updated:
 - Installation bash script
 - Messages and references messages
 - Image types for graph
 - View SlackBuilds repository in option "-n, --network"
+
 Fixed:
 - Some typos
 - Print package description
 
-2.8.9 - 15/09/2015
+### 2.8.9 - 15/09/2015
 Added:
 - Additional option "--case-ins" case insensitive
+
 Fixed:
 - Dialog utility crash if exit with Esc key
+
 Update:
 - KeyboardInterrupt with signal
 
-2.8.8 - 14/09/2015
+### 2.8.8 - 14/09/2015
 Added:
 - Additional option "--checklist" in "-n, --network" option
+
 Fixed:
 - Typo in help option
+
 Updated:
 - Optional dependencies
 - "--network" view commands
 
-2.8.7 - 11/09/2015
+### 2.8.7 - 11/09/2015
 Fixed:
 - Check remove dependencies if already installed
 
-2.8.6 - 11/09/2015
+### 2.8.6 - 11/09/2015
 Added:
 - Read doinst.sh file in "--network" option
 - Editor via configuration file
+
 Updated:
 - Rename script view.py in network.py
 
-2.8.5 - 08/09/2015
+### 2.8.5 - 08/09/2015
 Fixed:
 - Remove packages with option "--checklist" and "--check-deps"
 
-2.8.4 - 08/09/2015
+### 2.8.4 - 08/09/2015
 Added:
 - Additional option "--checklist" in option "--check" for upgrade packages
+
 Updated:
 - Slackware mirrors
 
-2.8.3 - 07/09/2015
+### 2.8.3 - 07/09/2015
 Added:
 - Update package lists for repository 'slack' after upgrade distribution
 - Reset slpkg configuration file in the default values
+
 Fixed:
 - pip install
 
-2.8.2 - 04/09/2015
+### 2.8.2 - 04/09/2015
 Updated:
 - Find SBo created Slackware packages
+
 Fixed:
 - Slackpkg update changelog.txt file
 - Pylint errors
 
-2.8.1 - 02/09/2015
+### 2.8.1 - 02/09/2015
 Fixed:
 - Path for build method
 - Check if SBo package created
 - Autobuild sources order list
+
 Updated:
 - Remove check if build
 - Reference for repo-enable command
 
-2.8.0 - 01/09/2015
+### 2.8.0 - 01/09/2015
 Added:
 - NEW configuration file for repositories in /etc/slpkg/repositories.conf
 - Enable and disable repositories with command via dialog utility
+
 Update:
 - All configuration files
 - Command line help logo
 - Flags for packages upgrade
 - Clear screen after exit dialog utility
+
 Fixed:
 - Remove None type packages
 - Remove old sbo folder if exists before start build
 
-2.7.6 - 28/08/2015
+### 2.7.6 - 28/08/2015
 Fixed:
 - Failed checksum message #40
 - Removed calculate size
+
 Updated:
 - Print list packages from repositories
 
-2.7.5 - 25/08/2015
+### 2.7.5 - 25/08/2015
 Added:
 - python2-pythondialog optional dependency
 - "--checklist" option in remove packages
 - Gigabyte unit in package manager
 - Version in removed dependencies
 - Size of removed dependencies
+
 Updated:
 - Function Msg() in self.msg
 - Tracking dependencies
 
-2.7.4 - 21/08/2015
+### 2.7.4 - 21/08/2015
 Added:
 - Support httpie for downloading
 - Remove packages with by TAG
 - Summary for size of removed package
+
 Fixed:
-- Resolving dependencies message for sbo repository when search for matching
-packages
+- Resolving dependencies message for sbo repository when search for matching packages
 - Reference message for installing and upgrading packages
 - Build error message
+
 Updated:
 - Install SBo packages with specific build number
 - For SBo repository select computer architecture
 - Module imports path
 
-2.7.3 - 13/08/2015
+### 2.7.3 - 13/08/2015
 Added:
 - Tree view for deps-status command
+
 Fixed:
 - pasture/ directory for Slackware 14.0
+
 Updated:
 - Comments for Slackware ARM users in REPOSITORIES and slpkg.conf file
 - slackpkg sync with ChangeLog.txt file
 
-2.7.2 - 10/08/2015
+### 2.7.2 - 10/08/2015
 Added:
 - Support Slackware ARM
+
 Fixed:
-- The package build when the sources more than one with the option
-"--autobuild"
+- The package build when the sources more than one with the option "--autobuild"
+
 Updated:
 - Manager to improve installed packages
 - setup.py requirements
 
-2.7.1 - 08/08/2015
+### 2.7.1 - 08/08/2015
 Fixed:
 - Remove package when partial name is supplied #34
 - Removing a package states "package not found" #35
 - Remove and install references
 
-2.7.0 - 06/08/2015
+### 2.7.0 - 06/08/2015
 Fixed:
 - EOFError when user interrupt with "ctrl + d"
+
 Updated:
-- Replace sys.sxit(0) with raise SystemExit() and remove unused sys module
+- Replace sys.exit(0) with raise SystemExit() and remove unused sys module
 - Code, doc strings
 - Slackware mirrors
 
-2.6.9 - 31/07/2015
+### 2.6.9 - 31/07/2015
 Added:
 - new-config command to manage .new configuration files
+
 Fixed:
 - Ignore check packages with version "blacklist" from binary repositories
+
 Updated:
 - slpkg.SlackBuild script
 - Read Slackware version function
 
-2.6.8 - 30/07/2015
+### 2.6.8 - 30/07/2015
 Fixed:
 - SBo dependencies installation order
 
-2.6.7 - 28/07/2015
+### 2.6.7 - 28/07/2015
 Fixed:
 - Fix typo #32
+
 Added:
 - graph-easy optional require to draw dependencies ascii diagram
 
-2.6.6 - 25/07/2015
+### 2.6.6 - 25/07/2015
 Added:
 - Dependencies status (command deps-status) message if no logs found
 - Optional pygraphviz module to drawing image map dependencies
+
 Updated:
 - Write dependencies logs with full packages
 
-2.6.5 - 23/07/2015
+### 2.6.5 - 23/07/2015
 Added:
 - Dependencies status command
 - Check if dependencies used in option "--tracking"
+
 Fixed:
 - Create 'core/' directory for Slackware repository
 
-2.6.4 - 21/07/2015
+### 2.6.4 - 21/07/2015
 Updated:
 - Merge functions into class
+
 Fixed:
-- Auto detect Slackware packages
-- Check dependencies if existis before reference to remove
+- Auto-detect Slackware packages
+- Check dependencies if exists before reference to remove
 - Check directories exists before find
 - Matching packages before remove
 
-2.6.3 - 17/07/2015
+### 2.6.3 - 17/07/2015
 Added:
 - Option via configuration file to choose "on" or "off" progress status bar
+
 Fixed:
 - SBo install and upgrade print view
 - Code style and complexity
 - Matching binary installed packages with repository packages
+
 Updated:
 - Slackware mirrors
 - View SBo version when installing or upgrading
 
-2.6.2 - 16/07/2015
+### 2.6.2 - 16/07/2015
 Added:
 - Health check installed packages
+
 Fixed:
 - Remove directories from slack repo when recreate package lists #29
 - Support Slackware version 13.37 #28
 - Fresh install #30
 
-2.6.1 - 15/07/2015
+### 2.6.1 - 15/07/2015
 Fixed:
 - Get installed version
 - Matching _SBo package name with _SBo installed name
+
 Updated:
 - Turn initialization method from read-write file in download
 
-2.6.0 - 08/07/2015
+### 2.6.0 - 08/07/2015
 Added:
-- Auto detect Slackware packages for installation
+- Auto-detect Slackware packages for installation
+
 Updated:
 - Toolbar progressive status
+
 Fixed:
 - Visible options when using without colors
 - Check remove dependencies #26
 
-2.5.9 - 02/07/2015
+### 2.5.9 - 02/07/2015
 Fixed:
 - Print list file package contents
 - Fixed alien -current repository
 - Fixed multi -current repository
+
 Added:
 - Support slonly -current (x86_64) repository
 
-2.5.8 - 28/06/2015
+### 2.5.8 - 28/06/2015
 Fixed:
 - Checksum for alien repository
 
-2.5.7 - 28/06/2015
+### 2.5.7 - 28/06/2015
 Fixed:
 - Double packages from alien repository
 - Resolve dependencies for binaries packages
+
 Updated:
 - Change mirror for alien repository
 
-2.5.6 - 25/06/2015
+### 2.5.6 - 25/06/2015
 Fixed:
-- Message question capital letter "N" by default. Thanks to Thomas Szteliga
-for report.
+- Message question capital letter "N" by default. Thanks to Thomas Szteliga for report.
 - Source code complexity
+
 Added:
-- MAKEFLAGS option in configuration file "/etc/slpkg/slpkg.conf". Thanks
-to Brenton Earl for the idea.
+- MAKEFLAGS option in configuration file "/etc/slpkg/slpkg.conf". Thanks to Brenton Earl for the idea.
 
-2.5.5 - 23/06/2015
+### 2.5.5 - 23/06/2015
 Added:
 - Summary in option "--FIND", "--check" and "repo-list"
 Updated:
 - Package view align
 - Repositories view list
 
-2.5.4 - 22/06/2015
+### 2.5.4 - 22/06/2015
 Added:
-- Support local repositories and you can add with command "repo-add"
+- Support local repositories, and you can add with command "repo-add"
 - Skip packages by repositories or from local
+
 Fixed:
 - Check repository if exist when package upgrade
 - AttributeError: 'list' object has no attribute 'splitlines' in "--tracking" Thanks to Brenton Earl for report
-- Check exist or enabled repostitories when upgraded in options
+- Check exist or enabled repositories when upgraded in options
 - Update custom repositories
+
 Updated:
 - Toolbar time
 
-2.5.3 - 20/06/2015
+### 2.5.3 - 20/06/2015
 Added:
 - Support blacklist packages by repository priority
-- Instead wget, curl and aria2c as downloader
+- wget, curl and aria2c as downloader
 - Support download jdk from "sbo" repository
+
 Fixed:
 - Resolve dependencies classes
 - Add and remove packages from blacklist and queue
 
-2.5.2 - 19/06/2015
+### 2.5.2 - 19/06/2015
 Added:
 - Repository check in blacklist
+
 Updated:
 - Blacklist options
+
 Fixed:
 - Pylint errors
 
-2.5.1 - 14/06/2015
+### 2.5.1 - 14/06/2015
 Added:
 - Check repositories ChangeLog.txt with command  "slpkg --check [repo]"
+
 Fixed:
 - Argument typo
 
-2.5.0 - 12/06/2015
+### 2.5.0 - 12/06/2015
 Added:
 - Full support Slackware command installpkg, upgradepkg and removepkg with all options. Option '--reinstall' merged into '--upgradepkg'
 - Print installed version
 - Check dependency of package if used before remove
-- MSB (mate) in default repositories.\
+- MSB (mate) in default repositories.
 - Update or upgrade specifically repositories
+
 Fixed:
-- Slonly repopsitory ChangeLog.txt link
+- Slonly repository ChangeLog.txt link
 - Selection foo.pkg removed instead you can use a variable ambient as: pkgs="pip brasero pylint" and then '# slpkg -s sbo $pkgs'
 - Resolve binary dependencies
 - Repository slackers.it mirror
 - Ignore "sbo" repository if not activated
 
-2.4.4 - 10/06/2015
+### 2.4.4 - 10/06/2015
 Fixed:
 - AttributeError: 'Update' object has no attribute 'meta' when try update repositories
 
-2.4.3 - 10/06/2015
+### 2.4.3 - 10/06/2015
 Added:
 - Long options
+
 Fixed:
 - Usage help message
 - Bash and fish completion
 - Man page
 - Configuration file
 
-2.4.2 - 04/06/2015
+### 2.4.2 - 04/06/2015
 Fixed:
 - BugFix TypeError: repo_data() function
 - SBo version compare
 - Code style
 
-2.4.1 - 04/06/2015
+### 2.4.1 - 04/06/2015
 Added:
 - Option to upgrade only the distribution packages installed
 - Option to on/off resolve dependencies
+
 Fixed:
 - Upgrade packages
 - Checksum on/off
 - Upgrade Slackware binary packages resolve dependencies
 
-2.4.0 - 02/06/2015
+### 2.4.0 - 02/06/2015
 Fixed:
 - Comments arguments to '--help' option
+-
 Added:
 - Additional option to skip packages when upgrading
 
-2.3.6 - 30/05/2015
+### 2.3.6 - 30/05/2015
 Fixed:
 - Avoid input the first package for searching when input multiple packages together with the option '-F'
 
-2.3.5 - 30/05/2015
+### 2.3.5 - 30/05/2015
 Fixed:
 - Version for SBo packages when search with option '-F'
 
-2.3.4 - 28/05/2015
+### 2.3.4 - 28/05/2015
 Fixed:
 - Arguments comments
 - Compression slackbuild package
 - Binary dependencies and sizes
 - Pylint errors
 - rlw repository package dependencies
+
 Added:
 - Find packages from enabled repositories
 - Script to remove data. (clean.py)
 
-2.3.3 - 23/05/2015
+### 2.3.3 - 23/05/2015
 Fixed:
 - 'ZeroDivisionError:' for binary package install
 - 'OSError:' if path not exist
 
-2.3.2 - 21/05/2015
+### 2.3.2 - 21/05/2015
 Fixed:
 - Arguments and options
 - Remove view package version when upgrade because conflict with some packages with the same name
 - File license
 
-2.3.1 - 14/05/2015
+### 2.3.1 - 14/05/2015
 Added:
 - The ability to sync with slackpkg and slpkg to update the file ChangeLog.txt when upgrading distribution
 
-2.3.0 - 07/05/2015
+### 2.3.0 - 07/05/2015
 Fixed:
 - BugFix: Find package error #13, Thanks 'lucashpandolfo' for reporting
 
-2.2.9 - 24/4/2015
+### 2.2.9 - 24/04/2015
 Fixed:
 - Reference installed packages after distribution upgrade
 - Double reference after already installed SBo packages
 - Clear master SBo packages
 
-2.2.8 - 23/4/2015
+### 2.2.8 - 23/04/2015
 Fixed:
 - Add new packages when upgrade
 - Man page
 - TypeError: 'NoneType' object has no attribute '__getitem__' when no sbo link found. Many Thanks to 'R S Ananda Murthy' to report.
 - Slackbuilds.org ChangeLog.txt url
 - Install.sh script
-- Binary/install.py, sbo/slackbuild.py and slack/patches.py clases
+- Binary/install.py, sbo/slackbuild.py and slack/patches.py classes
 - Count packages the upgrading of distribution
 
-2.2.7 - 18/3/2015
+### 2.2.7 - 18/03/2015
 Added:
 - bash and fish completion file
+
 Fixed:
 - Synchronization issues when upgrading SBo repository
 - Remove to the right spaces on view
 
-2.2.6 - 26/2/2015
+2### .2.6 - 26/2/2015
 Added:
 - Counter download
+
 Fixed:
 - Slackware release message
 
-2.2.5 - 24/02/2015
+### 2.2.5 - 24/02/2015
 Fixed:
 - Error-prone
 - Rename variable name 'VERSION' to 'RELEASE' in configuration file
 - Merge functions and fix __metadata__ complexity
-- SlackBulid and install script
+- SlackBuild and install script
 - Rename command 're-create' to 'upgrade'
 - IOError: [Errno 13] Permission denied as user
 - Alien repository checksum.
 
-2.2.3 - 16/02/2015
+### 2.2.3 - 16/02/2015
 Fixed:
 - slpkg.SlackBuild script support .zip archives
 - Can't overwrite new sbo scripts
 - Remove master package with dependencies
 
-2.2.2 - 11/02/2015
+### 2.2.2 - 11/02/2015
 Added:
 - BugFix show hidden matching sbo packages
 
-2.2.1 - 6/02/2015
+### 2.2.1 - 06/02/2015
 Added:
-- Support multipackages
+- Support multi packages
 - Passing variables to the script
 - Use file.pkg instead [package...] or [package]
+-
 Fixed:
 - [key error] when you enter wrong name repository as default
 - Rename BUILD variable to BUILD_PATH in configuration file slpkg.conf
 - Fails install if modified OUTPUT variable
 - Change in view list of packages in option '-l'
 - Update option '-f' view installed packages
 - Update option '-l' view installed packages
 
-2.2.0 - 08/01/2015
+### 2.2.0 - 08/01/2015
 Fixed:
 - Queue downloads
 - Find argument
 - Rename commands repolist and repoinfo to repo-list, repo-info
 - Installed package list
+-
 Added:
 - Custom binary repository
 - Slackware 'patches' repository in PACKAGES.txt file
 - Alien's restricted repository
 - Wget option
 - View default repositories in repo-list
 
-2.1.5 - 27/12/2014
+### 2.1.5 - 27/12/2014
 Added:
 - Slacker.it, slackonly.com, Alien's ktown, Alien's multilib, Slacke E17 and E18, SalixOS and Slackel repositories
 - Command 're-create'
 - Command 'repolist'
 - Command 'repoinfo'
+
 Fixed:
 - Slackware current upgrade checksums
-- Ingore hiden files in /var/log/packages/ path
+- Ignore hidden files in /var/log/packages/ path
 - Arguments
 
-2.1.4 - 16/12/2014
+### 2.1.4 - 16/12/2014
 Added:
 - Command 'update' and remove auto update package lists
 - Slpkg update itself
+
 Fixed:
 - 'UnboundLocalError: local variable 'md5' referenced before assignment' after try update alien repository in some packages and for Slackware current users. Thanks to 'Jack Kiersey' for reporting.
 - Checksums after try to update slackware packages
 
-2.1.3 - 06/12/2014
+### 2.1.3 - 06/12/2014
 Fixed:
 - 'IndexError: tuple index out of range' when sbo upgrade
 
 
-2.1.2 - 04/12/2014
+### 2.1.2 - 04/12/2014
 Added:
 - Checksum for all repositories
+
 Fixed:
 - Downloads modules
 
-2.1.1 - 01/12/2014
+### 2.1.1 - 01/12/2014
 Added:
 - Options in /etc/slpkg/slpkg.conf file to select repositories
 - Options to skip unsupported and untested packages
+
 Fixed:
 - BugFix TypeError for unsupported/untested sbo packages
 
-2.1.0 - 28/11/2014
+### 2.1.0 - 28/11/2014
 Fixed:
 - Change build path
 - Creating directories if not exists
+
 Added:
 - Studioware (studio) repository
 
-2.0.9 - 26/11/2014
+### 2.0.9 - 26/11/2014
 Fixed:
 - Setup.py to install configuration files after checksum
 - View slpkg config file
 
-2.0.8 - 25/11/2014
+### 2.0.8 - 25/11/2014
 Added:
 - More options in slpkg configuration file
 
-2.0.7 - 22/11/2014
+### 2.0.7 - 22/11/2014
 Added:
 - More option in slpkg.conf file
 - Slackware-mirrors file in /etc/slpkg
+
 Fixed:
 - Upgrade Slackware packages if installed
 
-2.0.6 - 18/11/2014
+### 2.0.6 - 18/11/2014
 Fixed:
 - Setup.py file
 
-2.0.5 - 18/11/2014
+### 2.0.5 - 18/11/2014
 Added:
 - /etc/slpkg.conf file
 - Move "--current" switch in /etc/slpkg.conf file
 - Local PACKAGES.TXT for Slackware repository
 - Options to view package description
 - All repositories in tracking dependencies options '-t'
-- Configuration file managment
+- Configuration file management
+
 Fixed:
 - BugFix upgrading binary packages
 
-2.0.4 - 07/11/2014
+### 2.0.4 - 07/11/2014
 Added:
 - Robby Workman, Alien Bob (Eric Hameleers) and slacky.eu repositories
+
 Fixed:
 - Remove list reference
 
-2.0.3 - 29/10/2014
+### 2.0.3 - 29/10/2014
 Fixed:
 - Arguments.
-- Spenedencies log
+- Dependencies log
 - Pydoc pager
 - List packaging paging
 
-2.0.2 - 21/10/2014
+### 2.0.2 - 21/10/2014
 Fixed:
 - Source code
 
-2.0.1 - 20/10/2014
+### 2.0.1 - 20/10/2014
 Fixed:
 - BugFix md5 checksum failed
 - Download all sources before build in view options
 
-2.0.0 - 15/10/2014
+### 2.0.0 - 15/10/2014
 Fixed:
 - Align PEP8 code style
 - SBo arch
 - Package splitting
 
-1.9.9 - 11/10/2014
+### 1.9.9 - 11/10/2014
 Added:
 - Queue options
 
-1.9.8 - 07/10/2014
+### 1.9.8 - 07/10/2014
 Fixed:
 - Source code update
 
-1.9.7 - 06/10/2014
+### 1.9.7 - 06/10/2014
 Fixed:
 - BugFix UnboundLocalError: local variable 'arch' referenced before assignment
 
-1.9.6 - 04/10/2014
-FIxed:
+### 1.9.6 - 04/10/2014
+Fixed:
 - BugFix install packages from slack repo
 
-1.9.5 - 04/10/2014
+### 1.9.5 - 04/10/2014
 Fixed:
 - Added 'aaa_elflibs' in blacklist
 - Current version upgrade only installed packages
 - Gzip man page in setup.py
 - Install blacklist configuration file through setup.py
 - Added Gb unit in slack repo
 
-1.9.4 - 01/10/2014
+### 1.9.4 - 01/10/2014
 Added:
 - Support install packages from Slackware current (version) repository
 - Support upgrade current version. (Upgrade all Slackware current tree)
+
 Fixed:
 - Arguments
 
-1.9.3 - 29/09/2014
+### 1.9.3 - 29/09/2014
 Added:
 - Blacklist configuration file
 - Blacklist options
 
-1.9.2 - 27/09/2014
+### 1.9.2 - 27/09/2014
 Fixed:
 - Remove argparse
 - Create downloader module with wget
 
-1.9.9 - 25/09/2014
+### 1.9.9 - 25/09/2014
 Fixed:
 - BugFix v1.9.0 no update slackbuilds packages
 - Arch in sbo upgrade
 
-1.9.0 - 24/09/2014
+### 1.9.0 - 24/09/2014
 Fixed:
 - Arguments.
 - Replace less command with pydoc
 
-1.8.9 - 23/09/2014
+### 1.8.9 - 23/09/2014
 Added:
 - Short description
 - View matching packages from SBo repository
+
 Fixed:
 - Open-close files as SLACKBUILDS.TXT
 
-1.8.8 - 22/09/2014
+### 1.8.8 - 22/09/2014
 Fixed:
 - Alignment viewing packages
 - Build time
+
 Added:
 - Search dependencies from local SLACKBUILDS.TXT file
 
-1.8.7 - 19/09/2014
+### 1.8.7 - 19/09/2014
 Fixed:
 - Build time
 
-1.8.6 - 14/09/2014
+### 1.8.6 - 14/09/2014
 Fixed:
 - Correction of reference installing or upgrading
 - Updated find installed packages
+
 Added:
 - Print total file size of installed packages
 - Highlight upgraded packages from slack repo
 
-1.8.5 - 13/09/2014
+### 1.8.5 - 13/09/2014
 Fixed:
 - Convert kb to mb
 - Build sources with spaces in filenames like "Sublime Text 2.0.2 x64.tar.bz2"
 
-1.8.4 - 10/09/2014
+### 1.8.4 - 10/09/2014
 Added:
 - MD5SUM check file
 - Build time
 
-1.8.3 - 08/09/2014
+### 1.8.3 - 08/09/2014
 Fixed:
 - Messages
 
-1.8.2 - 08/09/2014
+### 1.8.2 - 08/09/2014
 Fixed:
 - Resolving dependencies '-c sbo upgrade' option
-- Update sbo summarys
+- Update sbo summary's
+
 Added:
 - Build log file
 
-Version 1.8.1
-1.8.1 - 04/09/2014
+### 1.8.1 - 04/09/2014
 Fixed:
 - Install.sh script to install wget download tar.gz archive file
 - Install packages like adobe-reader
 
-1.8.0 - 02-09-2014
+### 1.8.0 - 02-09-2014
 Fixed:
 - Arch view dependencies in action -s sbo <package>
 - Find packages with version in action -s sbo <package>
 - Remove to remove packages after download because not useful
-- Download the some package and wget -N command not working
+- Download some package and wget -N command not working
 
-1.7.9 - 30/08/2014
+### 1.7.9 - 30/08/2014
 Added:
 - Extra and pasture packages from official Slackware tree
 - Install.sh script
+
 Fixed:
 - Remove destination file after copy to sbo script directory
 - Fix appearance build tag, the packages that do not include
 - _slack tag
 
-1.7.8 - 28/08/2014
+### 1.7.8 - 28/08/2014
 Fixed:
 - ImportError: No module named __metadata__
 
-1.7.7 - 26/08/2014
+### 1.7.7 - 26/08/2014
 Fixed:
 - Install noarch packages from SBo repository
 - Avoid '%README%' as dependency
 - Arguments
 - Messages
 
-1.7.6 - 25/08/2014
+### 1.7.6 - 25/08/2014
 Fixed:
-- IndexError '-aa' in cli argparseoptions
+- IndexError '-aa' in cli argparse options
 - Arch's
+
 Added:
 - Upgrade all SBo packages
 
-1.7.5 - 22/08/2014
+### 1.7.5 - 22/08/2014
 Added:
 - Report of packages will be installed the options `slpkg -s sbo <package>`, `slpkg -s slack <package>`, `slpkg -c slack upgrade`
+
 Fixed:
 - Mirrors for Slackware x86
 
-1.7.4 - 17/08/2014
+### 1.7.4 - 17/08/2014
 Fixed:
 - BugFix NameError: global name 'getpass' is not defined
+
 Added:
 - Downloaded .asc files to upgrade or install packages from Slackware tree
 - Calculate file sizes in the process of installing
 - Packages or upgrading from Slackware mirrors
 
-1.7.3 - 16/8/2014
+### 1.7.3 - 16/08/2014
 Fixed:
 - Sort the packets in the list view. We thank Dave for help https://github.com/wvragga.
 - BugFix reinstall lilo after upgrading kernel.
 - Removed some code system and replaced with Python code.
 - Reinstall if packages exist and upgrading if not in options slpkg -s slack <packages>
 - New paths created, ChangeLog.txt saved in /var/log/slpkg and SLACKBUILDS.TXT in /var/lib/slpkg/sbo_repo
-- Upgrade initilazation method
+- Upgrade initialization method
 - Replace mkdir -p with os.mkdir and create directories only if not exists
 
-1.7.2 - 13/08/2014
+### 1.7.2 - 13/08/2014
 Fixed:
 - Messages
 
-1.7.1 - 11/08/2014
+### 1.7.1 - 11/08/2014
 Fixed:
 - BugFix OSError: [Errno 2] No such file or directory: '/tmp/slpkg/patches/
+
 Added:
 - Change the way to search packages from slackbuilds.org.
 - The route search package eventually becomes found after ChangeLog.txt change
 
-1.7.0 - 09/08/2014
+### 1.7.0 - 09/08/2014
 Added:
 - Removes packages with all dependencies
 
-1.6.9 - 04/08/2014
+### 1.6.9 - 04/08/2014
 Fixed:
 - Remove non-useful code
 - /tmp/slpkg/readme/ path create
+
 Added:
 - Build path, drop all packages in Slpkg_Build directory
 - Build and install packages only if new version available and
 - Package not installed (slpkg -s sbo)
 - Display installed packages in tracking dependencies
 
-1.6.8 - 01/08/2014
+### 1.6.8 - 01/08/2014
 Fixed:
 - Grap http extra sources with space in line start like
 - Package EMBASSY
 - KeyboardInterrupt
 
-1.6.7 - 31/07/2014
+### 1.6.7 - 31/07/2014
 Fixed:
 - Packages remove
 - OSError: [Errno 2] No such file or directory:
 - Messages
 
-30-07-2014
-Version 1.6.6
-
-[Updated] - Fix 'Wrong file' when build packages
+### 1.6.6 - 30-07-2014
+Updated:
+- Fix 'Wrong file' when build packages
 
-1.6.5 - 28/07/2014
+### 1.6.5 - 28/07/2014
 Added:
 - Slack, noarch and other in list (slpkg -l)
 - Index in list (slpkg -l)
 - Install packages via official Slackware mirrors
+
 Fixed:
 - Messages
 
-[Updated] - Arguments views
+Updated:
+- Arguments views
 
-1.6.3 - 28/07/2014
+### 1.6.3 - 28/07/2014
 Fixed:
 - Messages
 - IndexError: tuple index out of range
 
-1.6.3 - 27/07/2014
+### 1.6.3 - 27/07/2014
 Fixed:
 - Arguments
 - NameError: global name 'sp' is not defined
 
-1.6.2 - 26/07/2014
+### 1.6.2 - 26/07/2014
 Added:
 - Distribution upgrade from official Slackware mirrors `slpkg -c slack upgrade`
+
 Fixed:
 - Change detection packages mode. 2x much faster
 - Messages
 
-1.6.1 - 22/07/2014
+### 1.6.1 - 22/07/2014
 Fixed:
 - Fix messages
 - Package remove
 - Package find
 - Package print contents
 
-1.6.0 - 21/07/2014
+### 1.6.0 - 21/07/2014
 Fixed:
 - Remove package (slpkg -r)
 - Added and fix messages
 - Create __metadata__
 
-1.5.9 - 18-07-2014
+### 1.5.9 - 18-07-2014
 Fixed:
 - Create sub-modules
 
-1.5.8 - 18-07-2014
+### 1.5.8 - 18-07-2014
 Fixed:
 - Report packages before removed (slpkg -r)
 
-1.5.7 - 17-07-2014
+### 1.5.7 - 17-07-2014
 Fixed:
 - IndentationError: expected an indented block
 
-1.5.6 - 17/07/2014
+### 1.5.6 - 17/07/2014
 Added:
 - Setuptools as secondary installer
 
-1.5.5 - 15/07/2014
+### 1.5.5 - 15/07/2014
 Fixed:
 - Create slpkg.py module
 
-1.5.4 - 13/07/2014
+### 1.5.4 - 13/07/2014
 Fixed:
 - Remove files in tmp directory after read
 
-1.5.3 - 24/06/2014
+### 1.5.3 - 24/06/2014
 Fixed:
 - IOError: [Errno 13] Permission denied: (file = open("/tmp/slpkg/readme/" + name + site, "w"))
 
-1.5.2 - 24/06/2014
+### 1.5.2 - 24/06/2014
 Fixed:
 - Urllib2.URLError: <urlopen error [Errno 111] Connection refused>
 
-1.5.1 - 12/06/2014
+### 1.5.1 - 12/06/2014
 Fixed:
 - Return download link on architectures other x86_64
 
-1.5.0 - 07/06/2014
+### 1.5.0 - 07/06/2014
 Fixed:
 - Download if server file is newer than local
 - Source code
 
-1.4.9 - 06/06/2014
+### 1.4.9 - 06/06/2014
 Fixed:
 - Exit from loop after build in option 'network'
 - Source code
 
-1.4.8 - 06/06/2014
+### 1.4.8 - 06/06/2014
 Fixed:
 - Print message to upgrade, install, reinstall and report files to removed
 
-1.4.7 - 04/06/2014
+### 1.4.7 - 04/06/2014
 Added:
-- Download/build/install in choises (-n) network and (-c) check
+- Download/build/install in chooses (-n) network and (-c) check
 
-1.4.6 - 05/06/2014
+### 1.4.6 - 05/06/2014
 Fixed:
 - Build noarch packages
 
-1.4.5 - 04/06/2014
+### 1.4.5 - 04/06/2014
 Added:
 - Support ftp links
 - Report already installed packages
 
-1.4.4 - 03/06/2014
+### 1.4.4 - 03/06/2014
 Added:
 - Support ALL extra sources
+
 Fixed:
 - Out of range in SBo version link with filename
 
-1.4.3 - 03/06/2014
+### 1.4.3 - 03/06/2014
 Fixed:
 - Avoid build packages with more than four arguments
 
-1.4.2 - 03/06/2014
+### 1.4.2 - 03/06/2014
 Fixed:
 - Avoid build package if already installed
 - Download if file already installed
 
-1.4.1 - 31/05/2014
+### 1.4.1 - 31/05/2014
 Fixed:
 - Avoid download package if already installed
 
-1.4.0 - 30/05/2014
+### 1.4.0 - 30/05/2014
 Fixed:
 - Install SBo packages with different tag
 - Avoid build and install already installed packages
 
-1.3.9 - 30/05/2014
+### 1.3.9 - 30/05/2014
 Fixed:
 - Remove to search for SBo script no needed
 - New naming the arguments
 - Source code
 
-1.3.8 - 30/05/2014
+### 1.3.8 - 30/05/2014
 Fixed:
 - No dependencies found
 
-1.3.7 - 29/05/2014
+### 1.3.7 - 29/05/2014
 Fixed:
 - Link filename with version
 
-1.3.6 - 28/05/2014
+### 1.3.6 - 28/05/2014
 Added:
 - Download package with all dependencies build and install all
 
-1.3.5 - 24/05/2014
+### 1.3.5 - 24/05/2014
 Fixed:
-- Print out "no dependecies" tracking function
+- Print out "no dependencies" tracking function
 - Confirmation delete packages
 
-1.3.4 - 23/05/2014
+### 1.3.4 - 23/05/2014
 Fixed:
 - (sre_constants.error) recognize package names with special characters
 
-1.3.3 - 22/05/2014
+### 1.3.3 - 22/05/2014
 Added:
 - Download and build package
 
-1.3.2 - 22/05/2014
+### 1.3.2 - 22/05/2014
 Added:
 - View info and SlackBuild file
+
 Fixed:
-- Bbuild arguments messages
+- Build arguments messages
 - TypeError: unsupported operand type(s) for +: 'NoneType' and 'str' in sbo_requires_pkg function (sbo_url = sbo_url + name + ".info")
 
-1.3.1 - 21/05/2014
+### 1.3.1 - 21/05/2014
 Added:
 - View README file
 
-1.3.0 - 21/05/2014
+### 1.3.0 - 21/05/2014
 Fixed:
 - Argparse view
 
-1.2.9 - 21/05/2014
+### 1.2.9 - 21/05/2014
 Added:
 - Tracking dependencies
 
-1.2.8 - 20/05/2014
+### 1.2.8 - 20/05/2014
 Added:
 - Download package from www.slackbuild.org
 - Support build packages with extra sources
 
-1.2.7 - 20/05/2014
+### 1.2.7 - 20/05/2014
 Fixed:
 - Overwrite code into functions
 
-1.2.6 - 20/05/2014
+### 1.2.6 - 20/05/2014
 Fixed:
 - Better code, better speed... enjoy !!!
 
-1.2.5 - 19/05/2014
-- Fix download source x86_64 arcitecture
+### 1.2.5 - 19/05/2014
+- Fix download source x86_64 architecture
 
-1.2.4 - 19/05/2014
+### 1.2.4 - 19/05/2014
 Added:
-- Download source code by pc arcitecture
+- Download source code by pc architecture
 
-1.2.3 - 19-05-2014
+### 1.2.3 - 19-05-2014
 Fixed:
 - Check packages for updates
 Added:
 - Progress bar to searching
 
-1.2.2 - 19/05/2014
+### 1.2.2 - 19/05/2014
 Fixed:
 - Libraries repository
 
-1.2.1 - 19/05/2014
+### 1.2.1 - 19/05/2014
 Fixed:
 - Functions
 
-1.2.0 - 17/05/2014
+### 1.2.0 - 17/05/2014
 Added:
-- If your packages from www.slackbuilds.org is up to date
+- If your packages from www.slackbuilds.org is up-to-date
 
-1.1.9 - 17/05/2014
+### 1.1.9 - 17/05/2014
 Fixed:
-- Notify message if exist package in fuction remove
+- Notify message if exist package in function remove
 
-1.1.8 - 17/05/2014
+### 1.1.8 - 17/05/2014
 Added:
 - Check root user
 Fixed:
 - Find and display packages
 
-1.1.7 - 16-05-2014
+### 1.1.7 - 16-05-2014
 Fixed:
 - Functions
 
-1.1.6 - 15-05-2014
+### 1.1.6 - 15-05-2014
 Fixed:
 - Removed stupid option binary search
 
-1.1.5 - 15/05/2014
+### 1.1.5 - 15/05/2014
 Added:
 - Multi install, upgrade, remove and find packages
 - Find from network slackbuilds links and sources
 
-1.1.4 - 14/05/2014
+### 1.1.4 - 14/05/2014
 Fixed:
 - Function sbo_requires_pkg do not use .txt file
 
-1.1.3 - 14-05-2014
+### 1.1.3 - 14-05-2014
 Added:
 - Find requirements package from www.slackbuild.org
 
-1.1.2 - 13/05/2014
+### 1.1.2 - 13/05/2014
 Added:
 - Find already binary packages in /tmp directory
 
-1.1.1 - 13/05/2014
+### 1.1.1 - 13/05/2014
 Fixed:
 - List print out
 
-1.1.0 - 12-05-2014
+### 1.1.0 - 12-05-2014
 Added:
 - Search from SBo and print link for download
 
-1.0.9 - 12/05/2014
+### 1.0.9 - 12/05/2014
 Fixed:
 - Warning messages amd colors print out
 
-1.0.8 - 12/05/2014
+### 1.0.8 - 12/05/2014
 Added:
-- Signle install argument
+- Single install argument
 - Two options in list argument
+
 Fixed:
 - Fix arguments
 
-1.0.7 - 11/05/2014
+### 1.0.7 - 11/05/2014
 Fixed:
 - Null arguments
 
-1.0.6 - 11/05/2014
+### 1.0.6 - 11/05/2014
 Fixed:
 - Updated slackbuild argument
 
-1.0.5 - 10/05/2014
+### 1.0.5 - 10/05/2014
 Added:
 - Auto build package choice
 Fixed:
 - Man page and README.rst file
 
-1.0.3 - 10/05/2014
+### 1.0.3 - 10/05/2014
 Added:
 - Function find_package
 
-1.0.2 - 10/05/2014
+### 1.0.2 - 10/05/2014
 Fixed:
 - setup.py file
 - Man page slpkg.8 gziped
 
-1.0.1 - 09-05-2014
+### 1.0.1 - 09-05-2014
 Added:
 - Support install man page
 
-1.0.0 - 09/05/2014
+### 1.0.0 - 09/05/2014
 Added:
 - Added man page
 
-0.0.3 - 09/05/2014
+### 0.0.3 - 09/05/2014
 Added:
 - Support warning message if remove package
 - Replace remove command
 
-0.0.2 - 08/05/2014
+### 0.0.2 - 08/05/2014
 Added:
 - Support reinstall package
+
 Fixed:
 - Version print out
 
--------------------------------------------------------------------
+--------------------------------------------------
 
-0.0.1 - 07/05/2014
+### 0.0.1 - 07/05/2014
 Notes:
-- Released version 0.0.1, developmnet status Aplha
+- Released version 0.0.1, development status Alpha
```

### Comparing `slpkg-4.8.9/man/slpkg.1` & `slpkg-4.9.0/man/slpkg.1`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/man/slpkg-fr.1` & `slpkg-4.9.0/man/slpkg-fr.1`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/completion/slpkg` & `slpkg-4.9.0/completion/slpkg`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/slpkg/dialog_configs.py` & `slpkg-4.9.0/slpkg/dialog_configs.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/slpkg/binaries/required.py` & `slpkg-4.9.0/slpkg/binaries/required.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/slpkg/binaries/queries.py` & `slpkg-4.9.0/slpkg/binaries/queries.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/slpkg/binaries/install.py` & `slpkg-4.9.0/slpkg/binaries/install.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/slpkg/install_data.py` & `slpkg-4.9.0/slpkg/install_data.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/slpkg/repositories.py` & `slpkg-4.9.0/slpkg/repositories.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/slpkg/repo_info.py` & `slpkg-4.9.0/slpkg/repo_info.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/slpkg/sbos/queries.py` & `slpkg-4.9.0/slpkg/sbos/queries.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/slpkg/sbos/slackbuild.py` & `slpkg-4.9.0/slpkg/sbos/slackbuild.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         self.check_md5 = Md5sum(flags)
         self.download = Downloader(flags)
         self.ascii = AsciiBox()
 
         self.sources: dict = {}
         self.install_order: list = []
         self.dependencies: list = []
-        self.slackware_command: str = str()
+        self.slackware_command: str = ''
         self.slackware_command: str = self.installpkg
         self.progress_message: str = f'{self.cyan}Installing{self.endc}'
 
         self.option_for_reinstall: bool = self.utils.is_option(
             ('-r', '--reinstall'), flags)
 
         self.option_for_skip_installed: bool = self.utils.is_option(
```

### Comparing `slpkg-4.8.9/slpkg/sbos/dependencies.py` & `slpkg-4.9.0/slpkg/sbos/dependencies.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/slpkg/sbos/sbo_generate.py` & `slpkg-4.9.0/slpkg/sbos/sbo_generate.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             with open(slack_desc, 'r') as f:
                 slack = f.readlines()
 
             for line in slack:
                 pattern: str = f'{name}: {name}'
                 if line.startswith(pattern):
                     return line[len(name) + 1:].strip()
-        return str()
+        return ''
 
     @staticmethod
     def read_info_file(info_file: Path, start: str, stop: str) -> list:
         """ Reads the .info file and return the line between to variables. """
         begin = end = 0
         with open(info_file, 'r') as f:
             info = f.read().splitlines()
```

### Comparing `slpkg-4.8.9/slpkg/update_repository.py` & `slpkg-4.9.0/slpkg/update_repository.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/slpkg/progress_bar.py` & `slpkg-4.9.0/slpkg/progress_bar.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         super(Configs, self).__init__()
         self.spinner = PixelSpinner
         self.ascii = AsciiBox()
 
         self.color: str = self.endc
         self.spinners: dict = {}
         self.spinners_color: dict = {}
-        self.bar_message: str = str()
+        self.bar_message: str = ''
 
     def progress_bar(self, message: str, filename=None) -> None:
         """ Creating progress bar. """
         self.assign_spinners()
         self.assign_spinner_colors()
         self.set_spinner()
         self.set_color()
```

### Comparing `slpkg-4.8.9/slpkg/downloader.py` & `slpkg-4.9.0/slpkg/downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         super(Configs, self).__init__()
         self.flags: list = flags
 
         self.errors = Errors()
         self.utils = Utilities()
 
         self.filename = None
-        self.downloader_command: str = str()
+        self.downloader_command: str = ''
         self.downloader_tools: dict = {
             'wget': self.wget_downloader,
             'wget2': self.wget_downloader,
             'curl': self.curl_downloader,
             'lftp': self.lftp_downloader
         }
         self.option_for_parallel: bool = self.utils.is_option(
```

### Comparing `slpkg-4.8.9/slpkg/models/models.py` & `slpkg-4.9.0/slpkg/models/models.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/slpkg/rules.py` & `slpkg-4.9.0/slpkg/rules.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/slpkg/views/view_package.py` & `slpkg-4.9.0/slpkg/views/view_package.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,31 +18,31 @@
 
         self.utils = Utilities()
         self.repos = Repositories()
 
         self.repository_packages: tuple = ()
         self.readme: list = []
         self.info_file: list = []
-        self.repo_build_tag: str = str()
-        self.mirror: str = str()
-        self.homepage: str = str()
-        self.maintainer: str = str()
-        self.email: str = str()
-        self.dependencies: str = str()
-        self.repo_tar_suffix: str = str()
+        self.repo_build_tag: str = ''
+        self.mirror: str = ''
+        self.homepage: str = ''
+        self.maintainer: str = ''
+        self.email: str = ''
+        self.dependencies: str = ''
+        self.repo_tar_suffix: str = ''
 
         self.option_for_pkg_version: bool = self.utils.is_option(
             ('-p', '--pkg-version'), flags)
 
     def slackbuild(self, data: dict, slackbuilds: list) -> None:
         """ View slackbuild packages information. """
         print()
         repo: dict = {
             self.repos.sbo_repo_name: self.repos.sbo_repo_tar_suffix,
-            self.repos.ponce_repo_name: str()
+            self.repos.ponce_repo_name: ''
         }
         self.repo_tar_suffix: str = repo[self.repository]
         self.repository_packages: tuple = tuple(data.keys())
 
         for sbo in slackbuilds:
             for name, item in data.items():
```

### Comparing `slpkg-4.8.9/slpkg/views/version.py` & `slpkg-4.9.0/slpkg/views/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 
 class Version:
     """ Print the version. """
 
     def __init__(self):
-        self.version_info: tuple = (4, 8, 9)
+        self.version_info: tuple = (4, 9, 0)
         self.version: str = '{0}.{1}.{2}'.format(*self.version_info)
         self.license: str = 'MIT License'
         self.author: str = 'Dimitris Zlatanidis (dslackw)'
         self.homepage: str = 'https://dslackw.gitlab.io/slpkg'
 
     def view(self) -> None:
         """ Prints the version. """
```

### Comparing `slpkg-4.8.9/slpkg/views/cli_menu.py` & `slpkg-4.9.0/slpkg/views/cli_menu.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/slpkg/views/asciibox.py` & `slpkg-4.9.0/slpkg/views/asciibox.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/slpkg/views/help_commands.py` & `slpkg-4.9.0/slpkg/views/help_commands.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/slpkg/views/views.py` & `slpkg-4.9.0/slpkg/views/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
         self.utils = Utilities()
         self.dialogbox = DialogBox()
         self.ascii = AsciiBox()
         self.upgrade = Upgrade(repository, data)
 
         self.download_only = None
-        self.summary_message: str = str()
+        self.summary_message: str = ''
         self.is_binary: bool = self.utils.is_binary_repo(repository)
 
         self.option_for_resolve_off: bool = self.utils.is_option(
             ('-O', '--resolve-off'), flags)
 
         self.option_for_reinstall: bool = self.utils.is_option(
             ('-r', '--reinstall'), flags)
@@ -99,27 +99,27 @@
 
             for dependency in dependencies:
                 self.view_remove_package(dependency)
 
         self.view_summary(packages, dependencies, option=mode)
 
     def view_build_package(self, package: str) -> None:
-        size: str = str()
+        size: str = ''
         color: str = self.yellow
         version: str = self.data[package]['version']
 
         if self.is_binary:
             # size: str = self.utils.convert_file_sizes(int(self.data[package][4])) <- It's going to replace with this
             size: str = self.utils.convert_file_sizes(
                 int(''.join(re.findall(r'\d+', self.data[package]['size_comp']))))
 
         self.ascii.draw_package_line(package, version, size, color, self.repository)
 
     def view_install_upgrade_package(self, package: str) -> None:
-        size: str = str()
+        size: str = ''
         color: str = self.cyan
         version: str = self.data[package]['version']
         installed: str = self.utils.is_package_installed(package)
         upgradable: bool = self.upgrade.is_package_upgradeable(package)
 
         if self.is_binary:
             # size: str = self.utils.convert_file_sizes(int(self.data[package][4])) <- It's going to replace with this
@@ -136,15 +136,15 @@
         if installed and self.option_for_reinstall and not upgradable:
             color: str = self.violet
             package: str = self.build_package_and_version(package)
 
         self.ascii.draw_package_line(package, version, size, color, self.repository)
 
     def view_download_package(self, package: str) -> None:
-        size: str = str()
+        size: str = ''
         color: str = self.cyan
         version: str = self.data[package]['version']
 
         if self.is_binary:
             # size: str = self.utils.convert_file_sizes(int(self.data[package][4])) <- It's going to replace with this
             size: str = self.utils.convert_file_sizes(
                 int(''.join(re.findall(r'\d+', self.data[package]['size_comp']))))
```

### Comparing `slpkg-4.8.9/slpkg/choose_packages.py` & `slpkg-4.9.0/slpkg/choose_packages.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/slpkg/checks.py` & `slpkg-4.9.0/slpkg/checks.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/slpkg/logging_deps.py` & `slpkg-4.9.0/slpkg/logging_deps.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/slpkg/new_configs.py` & `slpkg-4.9.0/slpkg/new_configs.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,26 +38,26 @@
 
         self.set_no_colors()
 
         self.choice = None
 
     def set_no_colors(self) -> None:
         if '--no-colors' in self.options:
-            self.bold: str = str()
-            self.red: str = str()
-            self.bred: str = str()
-            self.green: str = str()
-            self.bgreen: str = str()
-            self.yellow: str = str()
-            self.byellow: str = str()
-            self.cyan: str = str()
-            self.blue: str = str()
-            self.grey: str = str()
-            self.violet: str = str()
-            self.endc: str = str()
+            self.bold: str = ''
+            self.red: str = ''
+            self.bred: str = ''
+            self.green: str = ''
+            self.bgreen: str = ''
+            self.yellow: str = ''
+            self.byellow: str = ''
+            self.cyan: str = ''
+            self.blue: str = ''
+            self.grey: str = ''
+            self.violet: str = ''
+            self.endc: str = ''
 
     def check(self) -> None:
         """ Checks for .new files. """
         print('\nChecking for NEW configuration files...')
         if (self.slpkg_config_new.is_file() or self.blacklist_config_new.is_file()
                 or self.repositories_config_new.is_file() or self.rules_config_new.is_file()):
             print('\nThere are NEW files:\n')
```

### Comparing `slpkg-4.8.9/slpkg/multi_process.py` & `slpkg-4.9.0/slpkg/multi_process.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/slpkg/cleanings.py` & `slpkg-4.9.0/slpkg/cleanings.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/slpkg/checksum.py` & `slpkg-4.9.0/slpkg/checksum.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/slpkg/dialog_box.py` & `slpkg-4.9.0/slpkg/dialog_box.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/slpkg/configs.py` & `slpkg-4.9.0/slpkg/configs.py`

 * *Files 16% similar despite different names*

```diff
@@ -31,31 +31,31 @@
     installpkg: str = 'upgradepkg --install-new'
     reinstall: str = 'upgradepkg --reinstall'
     removepkg: str = 'removepkg'
     colors: bool = True
     dialog: bool = True
     downloader: str = 'wget'
     wget_options: str = '--c -q --progress=bar:force:noscroll --show-progress'
-    curl_options: str = str()
+    curl_options: str = ''
     lftp_get_options: str = '-c get -e'
     lftp_mirror_options: str = '-c mirror --parallel=100 --only-newer'
     silent_mode: bool = True
     ascii_characters: bool = True
     ask_question: bool = True
     parallel_downloads: bool = False
     file_pattern: str = '*'
     spinning_bar: str = True
     progress_spinner: str = 'pixel'
     spinner_color: str = 'green'
     border_color: str = 'bgreen'
     case_sensitive: bool = True
 
-    proxy_address: str = str()
-    proxy_username: str = str()
-    proxy_password: str = str()
+    proxy_address: str = ''
+    proxy_username: str = ''
+    proxy_password: str = ''
 
     try:
         # Load user configuration.
         config_path_file = Path(etc_path, f'{prog_name}.toml')
         if config_path_file.exists():
             with open(config_path_file, 'rb') as conf:
                 configs = tomli.load(conf)
@@ -89,29 +89,29 @@
             proxy_address: str = config['PROXY_ADDRESS']
             proxy_username: str = config['PROXY_USERNAME']
             proxy_password: str = config['PROXY_PASSWORD']
 
     except (KeyError, tomli.TOMLDecodeError) as error:
         errors.raise_toml_error_message(error, toml_file='/etc/slpkg/slpkg.toml')
 
-    blink: str = str()
-    bold: str = str()
-    red: str = str()
-    bred: str = str()
-    green: str = str()
-    bgreen: str = str()
-    yellow: str = str()
-    byellow: str = str()
-    cyan: str = str()
-    bcyan: str = str()
-    blue: str = str()
-    bblue: str = str()
-    grey: str = str()
-    violet: str = str()
-    endc: str = str()
+    blink: str = ''
+    bold: str = ''
+    red: str = ''
+    bred: str = ''
+    green: str = ''
+    bgreen: str = ''
+    yellow: str = ''
+    byellow: str = ''
+    cyan: str = ''
+    bcyan: str = ''
+    blue: str = ''
+    bblue: str = ''
+    grey: str = ''
+    violet: str = ''
+    endc: str = ''
 
     if colors:
         blink: str = '\033[32;5m'
         bold: str = '\033[1m'
         red: str = '\x1b[91m'
         bred: str = f'{bold}{red}'
         green: str = '\x1b[32m'
```

### Comparing `slpkg-4.8.9/slpkg/utilities.py` & `slpkg-4.9.0/slpkg/utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         """ Printing the elapsed time. """
         print(f'\n{self.yellow}Finished successfully:{self.endc}',
               time.strftime(f'{self.cyan}%H:%M:%S{self.endc}',
                             time.gmtime(elapsed_time)))
 
     def read_slackbuild_build_tag(self, sbo: str, location: str, repository: str) -> str:
         """ Returns build tag from .SlackBuild file. """
-        build: str = str()
+        build: str = ''
         sbo_script = Path(self.repos.repositories[repository]['path'], location, sbo, f'{sbo}.SlackBuild')
 
         if sbo_script.is_file():
             lines = self.read_text_file(sbo_script)
 
             for line in lines:
                 if line.startswith('BUILD=$'):
```

### Comparing `slpkg-4.8.9/slpkg/dependees.py` & `slpkg-4.9.0/slpkg/dependees.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
         self.ascii = AsciiBox()
         self.utils = Utilities()
 
         self.llc: str = self.ascii.lower_left_corner
         self.hl: str = self.ascii.horizontal_line
         self.var: str = self.ascii.vertical_and_right
-        self.package_version: str = str()
+        self.package_version: str = ''
 
         self.is_binary: bool = self.utils.is_binary_repo(repository)
 
         self.option_for_full_reverse: bool = self.utils.is_option(
             ('-E', '--full-reverse'), flags)
 
         self.option_for_pkg_version: bool = self.utils.is_option(
```

### Comparing `slpkg-4.8.9/slpkg/toml_error_message.py` & `slpkg-4.9.0/slpkg/toml_error_message.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/slpkg/check_updates.py` & `slpkg-4.9.0/slpkg/check_updates.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,14 +102,15 @@
         try:
             repo = self.http.request('GET', repo_chg_txt)
         except KeyboardInterrupt:
             raise SystemExit(1)
         except HTTPError:
             print(f'\n\n{self.endc}{self.prog_name}: {self.bred}Error:{self.endc} '
                   f'Failed to connect to {repo_chg_txt}\n')
+            return False
         else:
             repo_size: int = int(repo.headers['Content-Length'])
 
         if local_chg_txt.is_file():
             local_size: int = int(os.stat(local_chg_txt).st_size)
 
         logger = logging.getLogger(LoggingConfig.date_time)
```

### Comparing `slpkg-4.8.9/slpkg/remove_packages.py` & `slpkg-4.9.0/slpkg/remove_packages.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/slpkg/blacklist.py` & `slpkg-4.9.0/slpkg/blacklist.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/slpkg/download_only.py` & `slpkg-4.9.0/slpkg/download_only.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/slpkg/tracking.py` & `slpkg-4.9.0/slpkg/tracking.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 
         self.ascii = AsciiBox()
         self.utils = Utilities()
 
         self.llc: str = self.ascii.lower_left_corner
         self.hl: str = self.ascii.horizontal_line
         self.vl: str = self.ascii.vertical_line
-        self.package_version: str = str()
-        self.package_dependency_version: str = str()
+        self.package_version: str = ''
+        self.package_dependency_version: str = ''
         self.package_requires: tuple = tuple()
-        self.package_line: str = str()
-        self.require_line: str = str()
+        self.package_line: str = ''
+        self.require_line: str = ''
         self.count_requires: int = 0
         self.require_length: int = 0
 
         self.is_binary: bool = self.utils.is_binary_repo(repository)
 
         self.option_for_pkg_version: bool = self.utils.is_option(
             ('-p', '--pkg-version'), flags)
@@ -86,15 +86,15 @@
 
     def set_package_dependency_version(self, require: str) -> None:
         try:
             self.package_dependency_version: str = f"{'':>1}(not included)"
             if self.data.get(require):
                 self.package_dependency_version: str = f"{'':>1}{self.yellow}{self.data[require]['version']}{self.endc}"
         except KeyError:  # KeyError here because of the '%README%' as dependency
-            self.package_dependency_version: str = str()
+            self.package_dependency_version: str = ''
 
     def set_package_version(self, package: str) -> None:
         self.package_version: str = self.data[package]['version']
 
     def set_package_requires(self, package: str) -> None:
         self.package_requires: tuple = self.data[package]['requires'].split()
         if self.package_requires:
```

### Comparing `slpkg-4.8.9/slpkg/logging_config.py` & `slpkg-4.9.0/slpkg/logging_config.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/slpkg/main.py` & `slpkg-4.9.0/slpkg/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -424,15 +424,15 @@
 
             try:
                 if arg.startswith(self.flag_short_repository):
                     self.repository: str = self.args[self.args.index(arg) + 1]
                     self.args.remove(self.repository)
                     break
             except IndexError:
-                self.repository: str = str()
+                self.repository: str = ''
 
     def move_options(self) -> None:
         """ Move options to the flags and removes from the arguments. """
         new_args: list = []
 
         for arg in self.args:
             if arg in self.options:
```

### Comparing `slpkg-4.8.9/slpkg/find_installed.py` & `slpkg-4.9.0/slpkg/find_installed.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/slpkg/upgrade.py` & `slpkg-4.9.0/slpkg/upgrade.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/slpkg/search.py` & `slpkg-4.9.0/slpkg/search.py`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/setup.cfg` & `slpkg-4.9.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [metadata]
 name = slpkg
-version = 4.8.9
+version = 4.9.0
 license_file = LICENSE
 author = Dimitris Zlatanidis
 author_email = dslackw@gmail.com
 description = Package manager utility for Slackware Linux.
-long_description = file:README.rst
+long_description = file:README.md
 url = https://dslackw.gitlab.io/slpkg/
 project_urls = 
 	Source = https://dslackw.gitlab.io/slpkg/
 	Documentation = https://dslackw.gitlab.io/slpkg/
 classifiers = 
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
```

### Comparing `slpkg-4.8.9/slpkg.egg-info/SOURCES.txt` & `slpkg-4.9.0/slpkg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `slpkg-4.8.9/tools/gen_sbo_txt.sh` & `slpkg-4.9.0/tools/gen_sbo_txt.sh`

 * *Files identical despite different names*


# Comparing `tmp/swh.lister-5.6.3.tar.gz` & `tmp/swh.lister-5.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swh.lister-5.6.3.tar", last modified: Thu Jun  8 09:39:35 2023, max compression
+gzip compressed data, was "swh.lister-5.7.0.tar", last modified: Fri Jun 23 10:04:08 2023, max compression
```

## Comparing `swh.lister-5.6.3.tar` & `swh.lister-5.7.0.tar`

### file list

```diff
@@ -1,607 +1,619 @@
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/
--rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-06-08 09:39:33.000000 swh.lister-5.6.3/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) docker     (999)      113 2023-06-08 09:39:33.000000 swh.lister-5.6.3/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      922 2023-06-08 09:39:33.000000 swh.lister-5.6.3/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)      186 2023-06-08 09:39:33.000000 swh.lister-5.6.3/ACKNOWLEDGEMENTS
--rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-06-08 09:39:33.000000 swh.lister-5.6.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) docker     (999)      153 2023-06-08 09:39:33.000000 swh.lister-5.6.3/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-06-08 09:39:33.000000 swh.lister-5.6.3/LICENSE
--rw-r--r--   0 jenkins    (115) docker     (999)      218 2023-06-08 09:39:33.000000 swh.lister-5.6.3/MANIFEST.in
--rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-06-08 09:39:33.000000 swh.lister-5.6.3/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     4108 2023-06-08 09:39:35.000000 swh.lister-5.6.3/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     3218 2023-06-08 09:39:33.000000 swh.lister-5.6.3/README.md
--rw-r--r--   0 jenkins    (115) docker     (999)      554 2023-06-08 09:39:33.000000 swh.lister-5.6.3/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/docs/
--rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-06-08 09:39:33.000000 swh.lister-5.6.3/docs/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-06-08 09:39:33.000000 swh.lister-5.6.3/docs/Makefile
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/docs/_static/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:33.000000 swh.lister-5.6.3/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/docs/_templates/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:33.000000 swh.lister-5.6.3/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) docker     (999)      137 2023-06-08 09:39:33.000000 swh.lister-5.6.3/docs/cli.rst
--rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-06-08 09:39:33.000000 swh.lister-5.6.3/docs/conf.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/docs/images/
--rw-r--r--   0 jenkins    (115) docker     (999)    77777 2023-06-08 09:39:33.000000 swh.lister-5.6.3/docs/images/new_base.png
--rw-r--r--   0 jenkins    (115) docker     (999)     5612 2023-06-08 09:39:33.000000 swh.lister-5.6.3/docs/images/new_bitbucket_lister.png
--rw-r--r--   0 jenkins    (115) docker     (999)     6675 2023-06-08 09:39:33.000000 swh.lister-5.6.3/docs/images/new_github_lister.png
--rw-r--r--   0 jenkins    (115) docker     (999)    30902 2023-06-08 09:39:33.000000 swh.lister-5.6.3/docs/images/old_github_lister.png
--rw-r--r--   0 jenkins    (115) docker     (999)      677 2023-06-08 09:39:33.000000 swh.lister-5.6.3/docs/index.rst
--rw-r--r--   0 jenkins    (115) docker     (999)     4996 2023-06-08 09:39:33.000000 swh.lister-5.6.3/docs/new_lister_template.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3381 2023-06-08 09:39:33.000000 swh.lister-5.6.3/docs/run_a_new_lister.rst
--rw-r--r--   0 jenkins    (115) docker     (999)     2452 2023-06-08 09:39:33.000000 swh.lister-5.6.3/docs/save_forge.rst
--rw-r--r--   0 jenkins    (115) docker     (999)    17094 2023-06-08 09:39:33.000000 swh.lister-5.6.3/docs/tutorial.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      952 2023-06-08 09:39:33.000000 swh.lister-5.6.3/mypy.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-06-08 09:39:33.000000 swh.lister-5.6.3/pyproject.toml
--rw-r--r--   0 jenkins    (115) docker     (999)      196 2023-06-08 09:39:33.000000 swh.lister-5.6.3/pytest.ini
--rw-r--r--   0 jenkins    (115) docker     (999)       51 2023-06-08 09:39:33.000000 swh.lister-5.6.3/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       73 2023-06-08 09:39:33.000000 swh.lister-5.6.3/requirements-test.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      134 2023-06-08 09:39:33.000000 swh.lister-5.6.3/requirements.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-06-08 09:39:35.000000 swh.lister-5.6.3/setup.cfg
--rwxr-xr-x   0 jenkins    (115) docker     (999)     3962 2023-06-08 09:39:33.000000 swh.lister-5.6.3/setup.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/sql/
--rw-r--r--   0 jenkins    (115) docker     (999)     2918 2023-06-08 09:39:33.000000 swh.lister-5.6.3/sql/crawler.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1073 2023-06-08 09:39:33.000000 swh.lister-5.6.3/sql/pimp_db.sql
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/
--rw-r--r--   0 jenkins    (115) docker     (999)     2155 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/arch/
--rw-r--r--   0 jenkins    (115) docker     (999)     8141 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/arch/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)    18461 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/arch/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      577 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/arch/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/arch/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)     1146 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/arch/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/arch/tests/data/
--rwxr-xr-x   0 jenkins    (115) docker     (999)    43737 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/arch/tests/data/fake_archlinux_archives_init.sh
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/arch/tests/data/https_archive.archlinux.org/
--rw-r--r--   0 jenkins    (115) docker     (999)     6401 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_d_dialog
--rw-r--r--   0 jenkins    (115) docker     (999)     3443 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_g_gnome-code-assistance
--rw-r--r--   0 jenkins    (115) docker     (999)     1373 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_g_gzip
--rw-r--r--   0 jenkins    (115) docker     (999)     1034 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_l_libasyncns
--rw-r--r--   0 jenkins    (115) docker     (999)    11596 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_m_mercurial
--rw-r--r--   0 jenkins    (115) docker     (999)     1453 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_p_python-hglib
--rw-r--r--   0 jenkins    (115) docker     (999)     1958 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/arch/tests/data/https_archive.archlinux.org/repos_last_community_os_x86_64_community.files.tar.gz
--rw-r--r--   0 jenkins    (115) docker     (999)     1750 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/arch/tests/data/https_archive.archlinux.org/repos_last_core_os_x86_64_core.files.tar.gz
--rw-r--r--   0 jenkins    (115) docker     (999)     1758 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/arch/tests/data/https_archive.archlinux.org/repos_last_extra_os_x86_64_extra.files.tar.gz
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/
--rw-r--r--   0 jenkins    (115) docker     (999)     1190 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/aarch64_community_community.files.tar.gz
--rw-r--r--   0 jenkins    (115) docker     (999)     1128 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/aarch64_core_core.files.tar.gz
--rw-r--r--   0 jenkins    (115) docker     (999)     1120 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/aarch64_extra_extra.files.tar.gz
--rw-r--r--   0 jenkins    (115) docker     (999)     1184 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/armv7h_community_community.files.tar.gz
--rw-r--r--   0 jenkins    (115) docker     (999)     1123 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/armv7h_core_core.files.tar.gz
--rw-r--r--   0 jenkins    (115) docker     (999)     1120 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/armv7h_extra_extra.files.tar.gz
--rw-r--r--   0 jenkins    (115) docker     (999)    70402 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/arch/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1121 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/arch/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/aur/
--rw-r--r--   0 jenkins    (115) docker     (999)     4847 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/aur/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6072 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/aur/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      588 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/aur/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/aur/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/aur/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/aur/tests/data/
--rwxr-xr-x   0 jenkins    (115) docker     (999)     2084 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/aur/tests/data/fake_aur_packages.sh
--rw-r--r--   0 jenkins    (115) docker     (999)      701 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/aur/tests/data/packages-meta-v1.json.gz
--rw-r--r--   0 jenkins    (115) docker     (999)     5066 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/aur/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1113 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/aur/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/bitbucket/
--rw-r--r--   0 jenkins    (115) docker     (999)      341 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/bitbucket/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6927 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/bitbucket/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1200 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/bitbucket/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/bitbucket/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/bitbucket/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/bitbucket/tests/data/
--rw-r--r--   0 jenkins    (115) docker     (999)     4330 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/bitbucket/tests/data/bb_api_repositories_page1.json
--rw-r--r--   0 jenkins    (115) docker     (999)     4213 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/bitbucket/tests/data/bb_api_repositories_page2.json
--rw-r--r--   0 jenkins    (115) docker     (999)     6600 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/bitbucket/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1762 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/bitbucket/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/bower/
--rw-r--r--   0 jenkins    (115) docker     (999)     2171 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/bower/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2412 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/bower/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      615 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/bower/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/bower/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/bower/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/bower/tests/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/bower/tests/data/https_registry.bower.io/
--rw-r--r--   0 jenkins    (115) docker     (999)      255 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/bower/tests/data/https_registry.bower.io/packages
--rw-r--r--   0 jenkins    (115) docker     (999)     1160 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/bower/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1129 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/bower/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/cgit/
--rw-r--r--   0 jenkins    (115) docker     (999)      331 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cgit/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     8596 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cgit/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      557 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cgit/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/cgit/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cgit/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/cgit/tests/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.acdw.net/
--rw-r--r--   0 jenkins    (115) docker     (999)       67 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.acdw.net/README
--rw-r--r--   0 jenkins    (115) docker     (999)     2055 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.acdw.net/cgit
--rw-r--r--   0 jenkins    (115) docker     (999)     1098 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.acdw.net/foo
--rw-r--r--   0 jenkins    (115) docker     (999)     1098 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.acdw.net/foo_summary
--rw-r--r--   0 jenkins    (115) docker     (999)     2375 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.acdw.net/sfeed
--rw-r--r--   0 jenkins    (115) docker     (999)     5382 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.acdw.net/sfeed_summary
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.baserock.org/
--rw-r--r--   0 jenkins    (115) docker     (999)     3213 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.baserock.org/cgit
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.eclipse.org/
--rw-r--r--   0 jenkins    (115) docker     (999)     3377 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.eclipse.org/c
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.savannah.gnu.org/
--rw-r--r--   0 jenkins    (115) docker     (999)       67 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.savannah.gnu.org/README
--rw-r--r--   0 jenkins    (115) docker     (999)   530004 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.savannah.gnu.org/cgit
--rw-r--r--   0 jenkins    (115) docker     (999)     7459 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.savannah.gnu.org/cgit_elisp-es.git
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.tizen/
--rw-r--r--   0 jenkins    (115) docker     (999)       61 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.tizen/README
--rw-r--r--   0 jenkins    (115) docker     (999)    11062 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.tizen/cgit
--rw-r--r--   0 jenkins    (115) docker     (999)     3157 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.tizen/cgit,ofs=100
--rw-r--r--   0 jenkins    (115) docker     (999)    11407 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.tizen/cgit,ofs=50
--rw-r--r--   0 jenkins    (115) docker     (999)     2719 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.tizen/cgit_All-Projects
--rw-r--r--   0 jenkins    (115) docker     (999)     2656 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.tizen/cgit_All-Users
--rw-r--r--   0 jenkins    (115) docker     (999)     2612 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.tizen/cgit_Lock-Projects
--rw-r--r--   0 jenkins    (115) docker     (999)    15289 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_alsa-scenario-scn-data-0-base
--rw-r--r--   0 jenkins    (115) docker     (999)    14966 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_alsa-scenario-scn-data-0-mc1n2
--rw-r--r--   0 jenkins    (115) docker     (999)     9662 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_ap_samsung_audio-hal-e3250
--rw-r--r--   0 jenkins    (115) docker     (999)     9662 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_ap_samsung_audio-hal-e4x12
--rw-r--r--   0 jenkins    (115) docker     (999)    15849 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_devices_nfc-plugin-nxp
--rw-r--r--   0 jenkins    (115) docker     (999)    15926 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_intel_mfld_bootstub-mfld-blackbay
--rw-r--r--   0 jenkins    (115) docker     (999)    12968 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_mtdev
--rw-r--r--   0 jenkins    (115) docker     (999)    16116 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_opengl-es-virtual-drv
--rw-r--r--   0 jenkins    (115) docker     (999)     9041 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_panda_libdrm
--rw-r--r--   0 jenkins    (115) docker     (999)     6692 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_panda_libnl
--rw-r--r--   0 jenkins    (115) docker     (999)    17765 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_xorg_driver_xserver-xorg-misc
--rw-r--r--   0 jenkins    (115) docker     (999)    29634 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.tizen/cgit_apps_core_preloaded_ug-setting-gallery-efl
--rw-r--r--   0 jenkins    (115) docker     (999)    28967 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.tizen/cgit_apps_core_preloaded_ug-setting-homescreen-efl
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/cgit/tests/data/https_jff.email/
--rw-r--r--   0 jenkins    (115) docker     (999)     3442 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cgit/tests/data/https_jff.email/cgit
--rw-r--r--   0 jenkins    (115) docker     (999)     7243 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cgit/tests/repo_list.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     9441 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cgit/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1237 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cgit/tests/test_tasks.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1877 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cli.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/conda/
--rw-r--r--   0 jenkins    (115) docker     (999)     4336 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/conda/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4757 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/conda/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      589 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/conda/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/conda/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/conda/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/conda/tests/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/conda/tests/data/https_conda.anaconda.org/
--rw-r--r--   0 jenkins    (115) docker     (999)      955 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/conda/tests/data/https_conda.anaconda.org/conda-forge_linux-64_repodata.json.bz2
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/conda/tests/data/https_repo.anaconda.com/
--rw-r--r--   0 jenkins    (115) docker     (999)      634 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/conda/tests/data/https_repo.anaconda.com/pkgs_free_linux-64_repodata.json.bz2
--rw-r--r--   0 jenkins    (115) docker     (999)      513 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/conda/tests/data/https_repo.anaconda.com/pkgs_free_osx-64_repodata.json.bz2
--rw-r--r--   0 jenkins    (115) docker     (999)     1529 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/conda/tests/data/https_repo.anaconda.com/pkgs_free_win-64_repodata.json.bz2
--rw-r--r--   0 jenkins    (115) docker     (999)     1445 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/conda/tests/data/https_repo.anaconda.com/pkgs_main_linux-64_repodata.json.bz2
--rw-r--r--   0 jenkins    (115) docker     (999)      770 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/conda/tests/data/https_repo.anaconda.com/pkgs_pro_linux-64_repodata.json.bz2
--rw-r--r--   0 jenkins    (115) docker     (999)     4332 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/conda/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1129 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/conda/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/cpan/
--rw-r--r--   0 jenkins    (115) docker     (999)     1990 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cpan/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7360 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cpan/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      571 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cpan/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/cpan/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cpan/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/cpan/tests/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/cpan/tests/data/https_fastapi.metacpan.org/
--rw-r--r--   0 jenkins    (115) docker     (999)     9011 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cpan/tests/data/https_fastapi.metacpan.org/v1__search_scroll_page1
--rw-r--r--   0 jenkins    (115) docker     (999)     1102 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cpan/tests/data/https_fastapi.metacpan.org/v1__search_scroll_page2
--rw-r--r--   0 jenkins    (115) docker     (999)     2458 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cpan/tests/data/https_fastapi.metacpan.org/v1__search_scroll_page3
--rw-r--r--   0 jenkins    (115) docker     (999)     4089 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cpan/tests/data/https_fastapi.metacpan.org/v1__search_scroll_page4
--rw-r--r--   0 jenkins    (115) docker     (999)     9128 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cpan/tests/data/https_fastapi.metacpan.org/v1_release__search
--rw-r--r--   0 jenkins    (115) docker     (999)     5367 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cpan/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1121 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cpan/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/cran/
--rw-r--r--   0 jenkins    (115) docker     (999)      331 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cran/__init__.py
--rwxr-xr-x   0 jenkins    (115) docker     (999)      305 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cran/list_all_packages.R
--rw-r--r--   0 jenkins    (115) docker     (999)     4959 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cran/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      512 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cran/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/cran/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cran/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/cran/tests/data/
--rw-r--r--   0 jenkins    (115) docker     (999)      883 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cran/tests/data/list-r-packages.json
--rw-r--r--   0 jenkins    (115) docker     (999)     4854 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cran/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1118 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/cran/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/crates/
--rw-r--r--   0 jenkins    (115) docker     (999)     4779 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/crates/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     9337 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/crates/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      599 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/crates/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/crates/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)      174 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/crates/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/crates/tests/data/
--rwxr-xr-x   0 jenkins    (115) docker     (999)     3851 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/crates/tests/data/fake_crates_repository_init.sh
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/crates/tests/data/https_static.crates.io/
--rw-r--r--   0 jenkins    (115) docker     (999)     1358 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/crates/tests/data/https_static.crates.io/db-dump.tar.gz
--rw-r--r--   0 jenkins    (115) docker     (999)     1534 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/crates/tests/data/https_static.crates.io/db-dump.tar.gz_visit1
--rw-r--r--   0 jenkins    (115) docker     (999)     7982 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/crates/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1137 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/crates/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/debian/
--rw-r--r--   0 jenkins    (115) docker     (999)      460 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/debian/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)    11355 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/debian/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      516 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/debian/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/debian/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/debian/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/debian/tests/data/
--rw-r--r--   0 jenkins    (115) docker     (999)     5970 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/debian/tests/data/Sources_bullseye
--rw-r--r--   0 jenkins    (115) docker     (999)     4413 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/debian/tests/data/Sources_buster
--rw-r--r--   0 jenkins    (115) docker     (999)     4893 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/debian/tests/data/Sources_stretch
--rw-r--r--   0 jenkins    (115) docker     (999)     9160 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/debian/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1440 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/debian/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/fedora/
--rw-r--r--   0 jenkins    (115) docker     (999)      400 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/fedora/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)    10356 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/fedora/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      581 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/fedora/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/fedora/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/fedora/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/fedora/tests/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/fedora/tests/data/archives.fedoraproject.org/
--rw-r--r--   0 jenkins    (115) docker     (999)     1982 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/fedora/tests/data/archives.fedoraproject.org/primary26.xml.gz
--rw-r--r--   0 jenkins    (115) docker     (999)     1214 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/fedora/tests/data/archives.fedoraproject.org/primary36-altered.xml.gz
--rw-r--r--   0 jenkins    (115) docker     (999)     1172 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/fedora/tests/data/archives.fedoraproject.org/primary36.xml.gz
--rw-r--r--   0 jenkins    (115) docker     (999)     3112 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/fedora/tests/data/archives.fedoraproject.org/repomd26.xml
--rw-r--r--   0 jenkins    (115) docker     (999)     4971 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/fedora/tests/data/archives.fedoraproject.org/repomd36.xml
--rw-r--r--   0 jenkins    (115) docker     (999)     7582 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/fedora/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1944 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/fedora/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/gitea/
--rw-r--r--   0 jenkins    (115) docker     (999)      328 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/gitea/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)      749 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/gitea/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      581 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/gitea/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/gitea/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/gitea/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/gitea/tests/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/gitea/tests/data/https_try.gitea.io/
--rw-r--r--   0 jenkins    (115) docker     (999)     5856 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/gitea/tests/data/https_try.gitea.io/repos_page1
--rw-r--r--   0 jenkins    (115) docker     (999)     7652 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/gitea/tests/data/https_try.gitea.io/repos_page2
--rw-r--r--   0 jenkins    (115) docker     (999)     6224 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/gitea/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1838 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/gitea/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/github/
--rw-r--r--   0 jenkins    (115) docker     (999)      330 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/github/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7559 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/github/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1859 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/github/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/github/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/github/tests/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     9015 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/github/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3036 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/github/tests/test_tasks.py
--rw-r--r--   0 jenkins    (115) docker     (999)      296 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/github/utils.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/gitlab/
--rw-r--r--   0 jenkins    (115) docker     (999)      335 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/gitlab/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)    10135 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/gitlab/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      831 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/gitlab/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/gitlab/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/gitlab/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/gitlab/tests/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/gitlab/tests/data/https_foss.heptapod.net/
--rw-r--r--   0 jenkins    (115) docker     (999)    12380 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/gitlab/tests/data/https_foss.heptapod.net/api_response_page1.json
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/gitlab/tests/data/https_gite.lirmm.fr/
--rw-r--r--   0 jenkins    (115) docker     (999)     1605 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/gitlab/tests/data/https_gite.lirmm.fr/api_response_page1.json
--rw-r--r--   0 jenkins    (115) docker     (999)     1750 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/gitlab/tests/data/https_gite.lirmm.fr/api_response_page2.json
--rw-r--r--   0 jenkins    (115) docker     (999)      910 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/gitlab/tests/data/https_gite.lirmm.fr/api_response_page3.json
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/gitlab/tests/data/https_gitlab.com/
--rw-r--r--   0 jenkins    (115) docker     (999)     6065 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/gitlab/tests/data/https_gitlab.com/api_response_page1.json
--rw-r--r--   0 jenkins    (115) docker     (999)    13570 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/gitlab/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1492 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/gitlab/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/gnu/
--rw-r--r--   0 jenkins    (115) docker     (999)      329 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/gnu/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2663 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/gnu/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      513 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/gnu/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/gnu/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/gnu/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/gnu/tests/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/gnu/tests/data/https_ftp.gnu.org/
--rw-r--r--   0 jenkins    (115) docker     (999)   622168 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/gnu/tests/data/https_ftp.gnu.org/tree.json.gz
--rw-r--r--   0 jenkins    (115) docker     (999)     6450 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/gnu/tests/data/tree.json
--rw-r--r--   0 jenkins    (115) docker     (999)      982 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/gnu/tests/data/tree.min.json
--rw-r--r--   0 jenkins    (115) docker     (999)     1290 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/gnu/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1077 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/gnu/tests/test_tasks.py
--rw-r--r--   0 jenkins    (115) docker     (999)     8690 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/gnu/tests/test_tree.py
--rw-r--r--   0 jenkins    (115) docker     (999)     9207 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/gnu/tree.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/gogs/
--rw-r--r--   0 jenkins    (115) docker     (999)      396 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/gogs/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7401 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/gogs/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      571 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/gogs/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/gogs/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/gogs/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/gogs/tests/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/gogs/tests/data/https_try.gogs.io/
--rw-r--r--   0 jenkins    (115) docker     (999)     2949 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/gogs/tests/data/https_try.gogs.io/repos_page1
--rw-r--r--   0 jenkins    (115) docker     (999)     3072 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/gogs/tests/data/https_try.gogs.io/repos_page2
--rw-r--r--   0 jenkins    (115) docker     (999)     5873 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/gogs/tests/data/https_try.gogs.io/repos_page3
--rw-r--r--   0 jenkins    (115) docker     (999)     3051 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/gogs/tests/data/https_try.gogs.io/repos_page4
--rw-r--r--   0 jenkins    (115) docker     (999)    12373 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/gogs/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1830 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/gogs/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/golang/
--rw-r--r--   0 jenkins    (115) docker     (999)      330 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/golang/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6327 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/golang/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      756 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/golang/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/golang/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/golang/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/golang/tests/data/
--rw-r--r--   0 jenkins    (115) docker     (999)      489 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/golang/tests/data/page-1.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      418 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/golang/tests/data/page-2.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     1118 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/golang/tests/data/page-3.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     7644 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/golang/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1743 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/golang/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/hackage/
--rw-r--r--   0 jenkins    (115) docker     (999)     2804 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/hackage/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5183 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/hackage/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      621 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/hackage/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/hackage/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/hackage/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/hackage/tests/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/hackage/tests/data/https_fake49.haskell.org/
--rw-r--r--   0 jenkins    (115) docker     (999)    23107 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/hackage/tests/data/https_fake49.haskell.org/packages_search_0
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/hackage/tests/data/https_fake51.haskell.org/
--rw-r--r--   0 jenkins    (115) docker     (999)    23804 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/hackage/tests/data/https_fake51.haskell.org/packages_search_0
--rw-r--r--   0 jenkins    (115) docker     (999)      577 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/hackage/tests/data/https_fake51.haskell.org/packages_search_1
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/hackage/tests/data/https_hackage.haskell.org/
--rw-r--r--   0 jenkins    (115) docker     (999)    23805 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/hackage/tests/data/https_hackage.haskell.org/packages_search_0
--rw-r--r--   0 jenkins    (115) docker     (999)     1616 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/hackage/tests/data/https_hackage.haskell.org/packages_search_0_visit1
--rw-r--r--   0 jenkins    (115) docker     (999)       40 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/hackage/tests/data/https_hackage.haskell.org/packages_search_0_visit2
--rw-r--r--   0 jenkins    (115) docker     (999)    23353 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/hackage/tests/data/https_hackage.haskell.org/packages_search_1
--rw-r--r--   0 jenkins    (115) docker     (999)    22764 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/hackage/tests/data/https_hackage.haskell.org/packages_search_2
--rw-r--r--   0 jenkins    (115) docker     (999)     6472 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/hackage/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1159 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/hackage/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/hex/
--rw-r--r--   0 jenkins    (115) docker     (999)      394 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/hex/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4692 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/hex/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      595 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/hex/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/hex/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/hex/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/hex/tests/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/hex/tests/data/https_hex.pm/
--rw-r--r--   0 jenkins    (115) docker     (999)     6247 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/hex/tests/data/https_hex.pm/page1.json
--rw-r--r--   0 jenkins    (115) docker     (999)     7468 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/hex/tests/data/https_hex.pm/page2.json
--rw-r--r--   0 jenkins    (115) docker     (999)     3554 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/hex/tests/data/https_hex.pm/page3.json
--rw-r--r--   0 jenkins    (115) docker     (999)     5203 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/hex/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1737 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/hex/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/launchpad/
--rw-r--r--   0 jenkins    (115) docker     (999)      341 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/launchpad/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7518 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/launchpad/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      926 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/launchpad/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/launchpad/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/launchpad/tests/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1747 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/launchpad/tests/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/launchpad/tests/data/
--rw-r--r--   0 jenkins    (115) docker     (999)     5814 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/launchpad/tests/data/launchpad_bzr_response.json
--rw-r--r--   0 jenkins    (115) docker     (999)     5119 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/launchpad/tests/data/launchpad_response1.json
--rw-r--r--   0 jenkins    (115) docker     (999)     4960 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/launchpad/tests/data/launchpad_response2.json
--rw-r--r--   0 jenkins    (115) docker     (999)     8457 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/launchpad/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1793 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/launchpad/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/maven/
--rw-r--r--   0 jenkins    (115) docker     (999)     9772 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/maven/README.md
--rw-r--r--   0 jenkins    (115) docker     (999)      328 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/maven/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)    16142 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/maven/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      888 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/maven/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/maven/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/maven/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/maven/tests/data/
--rw-r--r--   0 jenkins    (115) docker     (999)    31940 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/maven/tests/data/citrus-parent-3.0.7.pom
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/maven/tests/data/http_indexes/
--rw-r--r--   0 jenkins    (115) docker     (999)     2312 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/maven/tests/data/http_indexes/export_full.fld
--rw-r--r--   0 jenkins    (115) docker     (999)      740 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/maven/tests/data/http_indexes/export_incr_first.fld
--rw-r--r--   0 jenkins    (115) docker     (999)      362 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/maven/tests/data/http_indexes/export_null_mtime.fld
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/maven/tests/data/https_api.github.com/
--rw-r--r--   0 jenkins    (115) docker     (999)     5749 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/maven/tests/data/https_api.github.com/repos_aldialimucaj_sprova4j
--rw-r--r--   0 jenkins    (115) docker     (999)     7821 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/maven/tests/data/https_api.github.com/repos_arangodb-community_arangodb-graphql-java
--rw-r--r--   0 jenkins    (115) docker     (999)     6110 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/maven/tests/data/https_api.github.com/repos_webx_citrus
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/maven/tests/data/https_repo1.maven.org/
--rw-r--r--   0 jenkins    (115) docker     (999)     2834 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/maven/tests/data/https_repo1.maven.org/maven2_al_aldi_sprova4j_0.1.0_sprova4j-0.1.0.pom
--rw-r--r--   0 jenkins    (115) docker     (999)     2823 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/maven/tests/data/https_repo1.maven.org/maven2_al_aldi_sprova4j_0.1.1_sprova4j-0.1.1.pom
--rwxr-xr-x   0 jenkins    (115) docker     (999)     7586 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/maven/tests/data/https_repo1.maven.org/maven2_com_arangodb_arangodb-graphql_1.2_arangodb-graphql-1.2.pom
--rw-r--r--   0 jenkins    (115) docker     (999)     1094 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/maven/tests/data/sprova4j-0.1.0.invalidurl.pom
--rw-r--r--   0 jenkins    (115) docker     (999)     2831 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/maven/tests/data/sprova4j-0.1.0.malformed.pom
--rw-r--r--   0 jenkins    (115) docker     (999)    13122 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/maven/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1403 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/maven/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/nixguix/
--rw-r--r--   0 jenkins    (115) docker     (999)     1221 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/nixguix/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)    24552 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/nixguix/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      527 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/nixguix/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/nixguix/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/nixguix/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/nixguix/tests/data/
--rw-r--r--   0 jenkins    (115) docker     (999)     6666 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/nixguix/tests/data/sources-failure.json
--rw-r--r--   0 jenkins    (115) docker     (999)    10741 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/nixguix/tests/data/sources-success.json
--rw-r--r--   0 jenkins    (115) docker     (999)    15509 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/nixguix/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      933 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/nixguix/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/npm/
--rw-r--r--   0 jenkins    (115) docker     (999)      540 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/npm/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5999 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/npm/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      827 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/npm/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/npm/tests/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/npm/tests/data/
--rw-r--r--   0 jenkins    (115) docker     (999)    10583 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/npm/tests/data/npm_full_page1.json
--rw-r--r--   0 jenkins    (115) docker     (999)     7301 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/npm/tests/data/npm_full_page2.json
--rw-r--r--   0 jenkins    (115) docker     (999)     5759 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/npm/tests/data/npm_incremental_page1.json
--rw-r--r--   0 jenkins    (115) docker     (999)    22638 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/npm/tests/data/npm_incremental_page2.json
--rw-r--r--   0 jenkins    (115) docker     (999)     6441 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/npm/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1784 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/npm/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/nuget/
--rw-r--r--   0 jenkins    (115) docker     (999)     3249 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/nuget/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5875 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/nuget/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      615 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/nuget/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/nuget/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/nuget/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/nuget/tests/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/nuget/tests/data/https_api.nuget.org/
--rw-r--r--   0 jenkins    (115) docker     (999)     1336 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/nuget/tests/data/https_api.nuget.org/v3-flatcontainer_intersoft.crosslight.logging.entityframework_5.0.5000.1235-experimental_intersoft.crosslight.logging.entityframework.nuspec
--rw-r--r--   0 jenkins    (115) docker     (999)     1284 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/nuget/tests/data/https_api.nuget.org/v3-flatcontainer_moq.automock_3.5.0-ci0287_moq.automock.nuspec
--rw-r--r--   0 jenkins    (115) docker     (999)     2832 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/nuget/tests/data/https_api.nuget.org/v3-flatcontainer_sil.core.desktop_10.0.1-beta0012_sil.core.desktop.nuspec
--rw-r--r--   0 jenkins    (115) docker     (999)     8037 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_data_2022.09.23.08.07.54_sil.core.desktop.10.0.1-beta0012.json
--rw-r--r--   0 jenkins    (115) docker     (999)     5322 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_data_2022.09.23.09.10.26_intersoft.crosslight.logging.entityframework.5.0.5000.1235-experimental.json
--rw-r--r--   0 jenkins    (115) docker     (999)     6791 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_data_2022.10.10.04.04.00_moq.automock.3.5.0-ci0287.json
--rw-r--r--   0 jenkins    (115) docker     (999)     1519 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_index.json
--rw-r--r--   0 jenkins    (115) docker     (999)     1287 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_index.json_visit1
--rw-r--r--   0 jenkins    (115) docker     (999)     2567 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_page11702.json
--rw-r--r--   0 jenkins    (115) docker     (999)     2146 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_page16958.json
--rw-r--r--   0 jenkins    (115) docker     (999)     1575 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_page17100.json
--rw-r--r--   0 jenkins    (115) docker     (999)     3634 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/nuget/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1129 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/nuget/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/opam/
--rw-r--r--   0 jenkins    (115) docker     (999)      326 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/opam/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4737 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/opam/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      512 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/opam/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/opam/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/opam/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/opam/tests/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/opam/tests/data/fake_opam_repo/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/opam/tests/data/fake_opam_repo/packages/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/opam/tests/data/fake_opam_repo/packages/agrid/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/opam/tests/data/fake_opam_repo/packages/agrid/agrid.0.1/
--rw-r--r--   0 jenkins    (115) docker     (999)     1123 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/opam/tests/data/fake_opam_repo/packages/agrid/agrid.0.1/opam
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.1/
--rw-r--r--   0 jenkins    (115) docker     (999)     1389 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.1/opam
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.2/
--rw-r--r--   0 jenkins    (115) docker     (999)     1176 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.2/opam
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.3/
--rw-r--r--   0 jenkins    (115) docker     (999)     1129 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.3/opam
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.4/
--rw-r--r--   0 jenkins    (115) docker     (999)     1097 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.4/opam
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.5/
--rw-r--r--   0 jenkins    (115) docker     (999)     1085 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.5/opam
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.6/
--rw-r--r--   0 jenkins    (115) docker     (999)     1092 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.6/opam
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/opam/tests/data/fake_opam_repo/packages/directories/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/opam/tests/data/fake_opam_repo/packages/directories/directories.0.1/
--rw-r--r--   0 jenkins    (115) docker     (999)     1535 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/opam/tests/data/fake_opam_repo/packages/directories/directories.0.1/opam
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/opam/tests/data/fake_opam_repo/packages/directories/directories.0.2/
--rw-r--r--   0 jenkins    (115) docker     (999)     1529 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/opam/tests/data/fake_opam_repo/packages/directories/directories.0.2/opam
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/opam/tests/data/fake_opam_repo/packages/directories/directories.0.3/
--rw-r--r--   0 jenkins    (115) docker     (999)     1472 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/opam/tests/data/fake_opam_repo/packages/directories/directories.0.3/opam
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/opam/tests/data/fake_opam_repo/packages/ocb/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/opam/tests/data/fake_opam_repo/packages/ocb/ocb.0.1/
--rw-r--r--   0 jenkins    (115) docker     (999)     1004 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/opam/tests/data/fake_opam_repo/packages/ocb/ocb.0.1/opam
--rw-r--r--   0 jenkins    (115) docker     (999)       20 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/opam/tests/data/fake_opam_repo/repo
--rw-r--r--   0 jenkins    (115) docker     (999)        6 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/opam/tests/data/fake_opam_repo/version
--rw-r--r--   0 jenkins    (115) docker     (999)     5843 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/opam/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1121 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/opam/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/packagist/
--rw-r--r--   0 jenkins    (115) docker     (999)      341 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/packagist/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7053 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/packagist/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      518 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/packagist/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/packagist/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/packagist/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/packagist/tests/data/
--rw-r--r--   0 jenkins    (115) docker     (999)     2281 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/packagist/tests/data/den1n_contextmenu.json
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/packagist/tests/data/https_api.github.com/
--rw-r--r--   0 jenkins    (115) docker     (999)       53 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/packagist/tests/data/https_api.github.com/repos_gitlky_wx_article
--rw-r--r--   0 jenkins    (115) docker     (999)     6972 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/packagist/tests/data/https_api.github.com/repos_spryker-eco_computop-api
--rw-r--r--   0 jenkins    (115) docker     (999)     5394 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/packagist/tests/data/https_api.github.com/repos_ycms_module-main
--rw-r--r--   0 jenkins    (115) docker     (999)     9749 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/packagist/tests/data/idevlab_essential.json
--rw-r--r--   0 jenkins    (115) docker     (999)     2545 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/packagist/tests/data/ljjackson_linnworks.json
--rw-r--r--   0 jenkins    (115) docker     (999)     6911 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/packagist/tests/data/lky_wx_article.json
--rw-r--r--   0 jenkins    (115) docker     (999)     4632 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/packagist/tests/data/payrix_payrix-php.json
--rw-r--r--   0 jenkins    (115) docker     (999)     4062 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/packagist/tests/data/spryker-eco_computop-api.json
--rw-r--r--   0 jenkins    (115) docker     (999)      595 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/packagist/tests/data/with_invalid_url.json
--rw-r--r--   0 jenkins    (115) docker     (999)     1097 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/packagist/tests/data/ycms_module-main.json
--rw-r--r--   0 jenkins    (115) docker     (999)     6680 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/packagist/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1052 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/packagist/tests/test_tasks.py
--rw-r--r--   0 jenkins    (115) docker     (999)    15575 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/pattern.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/phabricator/
--rw-r--r--   0 jenkins    (115) docker     (999)      345 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/phabricator/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6039 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/phabricator/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      753 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/phabricator/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/phabricator/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/phabricator/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/phabricator/tests/data/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/phabricator/tests/data/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)    44289 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/phabricator/tests/data/phabricator_api_repositories_page1.json
--rw-r--r--   0 jenkins    (115) docker     (999)    46784 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/phabricator/tests/data/phabricator_api_repositories_page2.json
--rw-r--r--   0 jenkins    (115) docker     (999)     4330 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/phabricator/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1284 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/phabricator/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/pubdev/
--rw-r--r--   0 jenkins    (115) docker     (999)     2064 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/pubdev/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3573 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/pubdev/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      609 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/pubdev/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/pubdev/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/pubdev/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/pubdev/tests/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/pubdev/tests/data/https_pub.dev/
--rw-r--r--   0 jenkins    (115) docker     (999)       74 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/pubdev/tests/data/https_pub.dev/api_package-names
--rw-r--r--   0 jenkins    (115) docker     (999)     1578 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/pubdev/tests/data/https_pub.dev/api_packages_Autolinker
--rw-r--r--   0 jenkins    (115) docker     (999)     1557 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/pubdev/tests/data/https_pub.dev/api_packages_Babylon
--rw-r--r--   0 jenkins    (115) docker     (999)     1508 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/pubdev/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1137 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/pubdev/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/puppet/
--rw-r--r--   0 jenkins    (115) docker     (999)     3557 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/puppet/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6203 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/puppet/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      583 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/puppet/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/puppet/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/puppet/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/puppet/tests/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/puppet/tests/data/https_forgeapi.puppet.com/
--rw-r--r--   0 jenkins    (115) docker     (999)    94411 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/puppet/tests/data/https_forgeapi.puppet.com/v3_modules,limit=100
--rw-r--r--   0 jenkins    (115) docker     (999)    10141 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/puppet/tests/data/https_forgeapi.puppet.com/v3_modules,limit=100,offset=100
--rw-r--r--   0 jenkins    (115) docker     (999)    92818 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/puppet/tests/data/https_forgeapi.puppet.com/v3_modules,limit=100,with_release_since=2022-09-26
--rw-r--r--   0 jenkins    (115) docker     (999)     5702 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/puppet/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1137 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/puppet/tests/test_tasks.py
--rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/py.typed
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/pypi/
--rw-r--r--   0 jenkins    (115) docker     (999)      331 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/pypi/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6736 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/pypi/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      492 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/pypi/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/pypi/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/pypi/tests/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     8171 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/pypi/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1040 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/pypi/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/rubygems/
--rw-r--r--   0 jenkins    (115) docker     (999)     1616 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/rubygems/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     9375 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/rubygems/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      595 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/rubygems/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/rubygems/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/rubygems/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/rubygems/tests/data/
--rw-r--r--   0 jenkins    (115) docker     (999)      894 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/rubygems/tests/data/rubygems_dumps.xml
--rw-r--r--   0 jenkins    (115) docker     (999)     2867 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/rubygems/tests/data/rubygems_pgsql_dump.tar
--rw-r--r--   0 jenkins    (115) docker     (999)     1361 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/rubygems/tests/data/small_rubygems_dump.sh
--rw-r--r--   0 jenkins    (115) docker     (999)     6208 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/rubygems/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1167 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/rubygems/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/sourceforge/
--rw-r--r--   0 jenkins    (115) docker     (999)      340 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/sourceforge/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)    18526 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/sourceforge/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      820 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/sourceforge/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/sourceforge/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/sourceforge/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/sourceforge/tests/data/
--rw-r--r--   0 jenkins    (115) docker     (999)     1632 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/sourceforge/tests/data/aaron.html
--rw-r--r--   0 jenkins    (115) docker     (999)     6332 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/sourceforge/tests/data/aaron.json
--rw-r--r--   0 jenkins    (115) docker     (999)     2242 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/sourceforge/tests/data/adobexmp.json
--rw-r--r--   0 jenkins    (115) docker     (999)     3993 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/sourceforge/tests/data/backapps-website.json
--rw-r--r--   0 jenkins    (115) docker     (999)     5614 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/sourceforge/tests/data/backapps.json
--rw-r--r--   0 jenkins    (115) docker     (999)      384 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/sourceforge/tests/data/main-sitemap.xml
--rw-r--r--   0 jenkins    (115) docker     (999)     3041 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/sourceforge/tests/data/mojunk.json
--rw-r--r--   0 jenkins    (115) docker     (999)     3938 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/sourceforge/tests/data/mramm.json
--rw-r--r--   0 jenkins    (115) docker     (999)     2404 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/sourceforge/tests/data/ocaml-lpd.html
--rw-r--r--   0 jenkins    (115) docker     (999)     5477 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/sourceforge/tests/data/ocaml-lpd.json
--rw-r--r--   0 jenkins    (115) docker     (999)     3209 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/sourceforge/tests/data/os3dmodels.json
--rw-r--r--   0 jenkins    (115) docker     (999)     1218 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/sourceforge/tests/data/random-mercurial.json
--rw-r--r--   0 jenkins    (115) docker     (999)     2757 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/sourceforge/tests/data/subsitemap-0.xml
--rw-r--r--   0 jenkins    (115) docker     (999)     1523 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/sourceforge/tests/data/subsitemap-1.xml
--rw-r--r--   0 jenkins    (115) docker     (999)     7836 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/sourceforge/tests/data/t12eksandbox.html
--rw-r--r--   0 jenkins    (115) docker     (999)     7904 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/sourceforge/tests/data/t12eksandbox.json
--rw-r--r--   0 jenkins    (115) docker     (999)    19233 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/sourceforge/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1827 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/sourceforge/tests/test_tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/tests/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2012 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/tests/test_cli.py
--rw-r--r--   0 jenkins    (115) docker     (999)     9972 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/tests/test_pattern.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1191 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/tests/test_utils.py
--rw-r--r--   0 jenkins    (115) docker     (999)      386 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/tests/utils.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/tuleap/
--rw-r--r--   0 jenkins    (115) docker     (999)      330 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/tuleap/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4611 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/tuleap/lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)      579 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/tuleap/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/tuleap/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/tuleap/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/tuleap/tests/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh/lister/tuleap/tests/data/https_tuleap.net/
--rw-r--r--   0 jenkins    (115) docker     (999)     4552 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/tuleap/tests/data/https_tuleap.net/projects
--rw-r--r--   0 jenkins    (115) docker     (999)      422 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/tuleap/tests/data/https_tuleap.net/repo_1
--rw-r--r--   0 jenkins    (115) docker     (999)      338 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/tuleap/tests/data/https_tuleap.net/repo_2
--rw-r--r--   0 jenkins    (115) docker     (999)       20 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/tuleap/tests/data/https_tuleap.net/repo_3
--rw-r--r--   0 jenkins    (115) docker     (999)     5639 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/tuleap/tests/test_lister.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1788 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/tuleap/tests/test_tasks.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2215 2023-06-08 09:39:33.000000 swh.lister-5.6.3/swh/lister/utils.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh.lister.egg-info/
--rw-r--r--   0 jenkins    (115) docker     (999)     4108 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh.lister.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)    21059 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh.lister.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh.lister.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     1464 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh.lister.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      263 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh.lister.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-06-08 09:39:35.000000 swh.lister-5.6.3/swh.lister.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     1599 2023-06-08 09:39:33.000000 swh.lister-5.6.3/tox.ini
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.535358 swh.lister-5.7.0/
+-rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-06-23 10:04:04.000000 swh.lister-5.7.0/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) docker     (999)      113 2023-06-23 10:04:04.000000 swh.lister-5.7.0/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      922 2023-06-23 10:04:04.000000 swh.lister-5.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)      186 2023-06-23 10:04:04.000000 swh.lister-5.7.0/ACKNOWLEDGEMENTS
+-rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-06-23 10:04:04.000000 swh.lister-5.7.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) docker     (999)      153 2023-06-23 10:04:04.000000 swh.lister-5.7.0/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-06-23 10:04:04.000000 swh.lister-5.7.0/LICENSE
+-rw-r--r--   0 jenkins    (115) docker     (999)      218 2023-06-23 10:04:04.000000 swh.lister-5.7.0/MANIFEST.in
+-rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-06-23 10:04:04.000000 swh.lister-5.7.0/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     4108 2023-06-23 10:04:08.535358 swh.lister-5.7.0/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     3218 2023-06-23 10:04:04.000000 swh.lister-5.7.0/README.md
+-rw-r--r--   0 jenkins    (115) docker     (999)      554 2023-06-23 10:04:04.000000 swh.lister-5.7.0/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.423357 swh.lister-5.7.0/docs/
+-rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-06-23 10:04:04.000000 swh.lister-5.7.0/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-06-23 10:04:04.000000 swh.lister-5.7.0/docs/Makefile
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.423357 swh.lister-5.7.0/docs/_static/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:04.000000 swh.lister-5.7.0/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.423357 swh.lister-5.7.0/docs/_templates/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:04.000000 swh.lister-5.7.0/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) docker     (999)      137 2023-06-23 10:04:04.000000 swh.lister-5.7.0/docs/cli.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-06-23 10:04:04.000000 swh.lister-5.7.0/docs/conf.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.423357 swh.lister-5.7.0/docs/images/
+-rw-r--r--   0 jenkins    (115) docker     (999)    77777 2023-06-23 10:04:04.000000 swh.lister-5.7.0/docs/images/new_base.png
+-rw-r--r--   0 jenkins    (115) docker     (999)     5612 2023-06-23 10:04:04.000000 swh.lister-5.7.0/docs/images/new_bitbucket_lister.png
+-rw-r--r--   0 jenkins    (115) docker     (999)     6675 2023-06-23 10:04:04.000000 swh.lister-5.7.0/docs/images/new_github_lister.png
+-rw-r--r--   0 jenkins    (115) docker     (999)    30902 2023-06-23 10:04:04.000000 swh.lister-5.7.0/docs/images/old_github_lister.png
+-rw-r--r--   0 jenkins    (115) docker     (999)      677 2023-06-23 10:04:04.000000 swh.lister-5.7.0/docs/index.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     4996 2023-06-23 10:04:04.000000 swh.lister-5.7.0/docs/new_lister_template.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3381 2023-06-23 10:04:04.000000 swh.lister-5.7.0/docs/run_a_new_lister.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     2452 2023-06-23 10:04:04.000000 swh.lister-5.7.0/docs/save_forge.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)    17094 2023-06-23 10:04:04.000000 swh.lister-5.7.0/docs/tutorial.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      952 2023-06-23 10:04:04.000000 swh.lister-5.7.0/mypy.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-06-23 10:04:04.000000 swh.lister-5.7.0/pyproject.toml
+-rw-r--r--   0 jenkins    (115) docker     (999)      196 2023-06-23 10:04:04.000000 swh.lister-5.7.0/pytest.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)       51 2023-06-23 10:04:04.000000 swh.lister-5.7.0/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       73 2023-06-23 10:04:04.000000 swh.lister-5.7.0/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      134 2023-06-23 10:04:04.000000 swh.lister-5.7.0/requirements.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-06-23 10:04:08.535358 swh.lister-5.7.0/setup.cfg
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     4011 2023-06-23 10:04:04.000000 swh.lister-5.7.0/setup.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.427358 swh.lister-5.7.0/sql/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2918 2023-06-23 10:04:04.000000 swh.lister-5.7.0/sql/crawler.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1073 2023-06-23 10:04:04.000000 swh.lister-5.7.0/sql/pimp_db.sql
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.427358 swh.lister-5.7.0/swh/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.427358 swh.lister-5.7.0/swh/lister/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2155 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.427358 swh.lister-5.7.0/swh/lister/arch/
+-rw-r--r--   0 jenkins    (115) docker     (999)     8141 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/arch/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    18461 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/arch/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      577 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/arch/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.427358 swh.lister-5.7.0/swh/lister/arch/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1146 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/arch/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.427358 swh.lister-5.7.0/swh/lister/arch/tests/data/
+-rwxr-xr-x   0 jenkins    (115) docker     (999)    43737 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/arch/tests/data/fake_archlinux_archives_init.sh
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.431357 swh.lister-5.7.0/swh/lister/arch/tests/data/https_archive.archlinux.org/
+-rw-r--r--   0 jenkins    (115) docker     (999)     6401 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_d_dialog
+-rw-r--r--   0 jenkins    (115) docker     (999)     3443 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_g_gnome-code-assistance
+-rw-r--r--   0 jenkins    (115) docker     (999)     1373 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_g_gzip
+-rw-r--r--   0 jenkins    (115) docker     (999)     1034 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_l_libasyncns
+-rw-r--r--   0 jenkins    (115) docker     (999)    11596 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_m_mercurial
+-rw-r--r--   0 jenkins    (115) docker     (999)     1453 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_p_python-hglib
+-rw-r--r--   0 jenkins    (115) docker     (999)     1958 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/arch/tests/data/https_archive.archlinux.org/repos_last_community_os_x86_64_community.files.tar.gz
+-rw-r--r--   0 jenkins    (115) docker     (999)     1750 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/arch/tests/data/https_archive.archlinux.org/repos_last_core_os_x86_64_core.files.tar.gz
+-rw-r--r--   0 jenkins    (115) docker     (999)     1758 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/arch/tests/data/https_archive.archlinux.org/repos_last_extra_os_x86_64_extra.files.tar.gz
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.431357 swh.lister-5.7.0/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1190 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/aarch64_community_community.files.tar.gz
+-rw-r--r--   0 jenkins    (115) docker     (999)     1128 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/aarch64_core_core.files.tar.gz
+-rw-r--r--   0 jenkins    (115) docker     (999)     1120 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/aarch64_extra_extra.files.tar.gz
+-rw-r--r--   0 jenkins    (115) docker     (999)     1184 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/armv7h_community_community.files.tar.gz
+-rw-r--r--   0 jenkins    (115) docker     (999)     1123 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/armv7h_core_core.files.tar.gz
+-rw-r--r--   0 jenkins    (115) docker     (999)     1120 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/armv7h_extra_extra.files.tar.gz
+-rw-r--r--   0 jenkins    (115) docker     (999)    70402 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/arch/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1121 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/arch/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.431357 swh.lister-5.7.0/swh/lister/aur/
+-rw-r--r--   0 jenkins    (115) docker     (999)     4847 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/aur/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6072 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/aur/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      588 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/aur/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.431357 swh.lister-5.7.0/swh/lister/aur/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/aur/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.431357 swh.lister-5.7.0/swh/lister/aur/tests/data/
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     2084 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/aur/tests/data/fake_aur_packages.sh
+-rw-r--r--   0 jenkins    (115) docker     (999)      701 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/aur/tests/data/packages-meta-v1.json.gz
+-rw-r--r--   0 jenkins    (115) docker     (999)     5066 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/aur/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1113 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/aur/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.431357 swh.lister-5.7.0/swh/lister/bitbucket/
+-rw-r--r--   0 jenkins    (115) docker     (999)      341 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/bitbucket/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6927 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/bitbucket/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1200 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/bitbucket/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.439357 swh.lister-5.7.0/swh/lister/bitbucket/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/bitbucket/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.439357 swh.lister-5.7.0/swh/lister/bitbucket/tests/data/
+-rw-r--r--   0 jenkins    (115) docker     (999)     4330 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/bitbucket/tests/data/bb_api_repositories_page1.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     4213 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/bitbucket/tests/data/bb_api_repositories_page2.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     6600 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/bitbucket/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1762 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/bitbucket/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.439357 swh.lister-5.7.0/swh/lister/bower/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2171 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/bower/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2412 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/bower/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      615 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/bower/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.439357 swh.lister-5.7.0/swh/lister/bower/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/bower/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.367357 swh.lister-5.7.0/swh/lister/bower/tests/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.439357 swh.lister-5.7.0/swh/lister/bower/tests/data/https_registry.bower.io/
+-rw-r--r--   0 jenkins    (115) docker     (999)      255 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/bower/tests/data/https_registry.bower.io/packages
+-rw-r--r--   0 jenkins    (115) docker     (999)     1160 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/bower/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1129 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/bower/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.439357 swh.lister-5.7.0/swh/lister/cgit/
+-rw-r--r--   0 jenkins    (115) docker     (999)      331 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cgit/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     8596 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cgit/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      557 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cgit/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.439357 swh.lister-5.7.0/swh/lister/cgit/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cgit/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.367357 swh.lister-5.7.0/swh/lister/cgit/tests/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.447358 swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.acdw.net/
+-rw-r--r--   0 jenkins    (115) docker     (999)       67 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.acdw.net/README
+-rw-r--r--   0 jenkins    (115) docker     (999)     2055 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.acdw.net/cgit
+-rw-r--r--   0 jenkins    (115) docker     (999)     1098 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.acdw.net/foo
+-rw-r--r--   0 jenkins    (115) docker     (999)     1098 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.acdw.net/foo_summary
+-rw-r--r--   0 jenkins    (115) docker     (999)     2375 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.acdw.net/sfeed
+-rw-r--r--   0 jenkins    (115) docker     (999)     5382 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.acdw.net/sfeed_summary
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.447358 swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.baserock.org/
+-rw-r--r--   0 jenkins    (115) docker     (999)     3213 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.baserock.org/cgit
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.447358 swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.eclipse.org/
+-rw-r--r--   0 jenkins    (115) docker     (999)     3377 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.eclipse.org/c
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.447358 swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.savannah.gnu.org/
+-rw-r--r--   0 jenkins    (115) docker     (999)       67 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.savannah.gnu.org/README
+-rw-r--r--   0 jenkins    (115) docker     (999)   530004 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.savannah.gnu.org/cgit
+-rw-r--r--   0 jenkins    (115) docker     (999)     7459 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.savannah.gnu.org/cgit_elisp-es.git
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.455358 swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.tizen/
+-rw-r--r--   0 jenkins    (115) docker     (999)       61 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.tizen/README
+-rw-r--r--   0 jenkins    (115) docker     (999)    11062 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.tizen/cgit
+-rw-r--r--   0 jenkins    (115) docker     (999)     3157 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.tizen/cgit,ofs=100
+-rw-r--r--   0 jenkins    (115) docker     (999)    11407 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.tizen/cgit,ofs=50
+-rw-r--r--   0 jenkins    (115) docker     (999)     2719 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_All-Projects
+-rw-r--r--   0 jenkins    (115) docker     (999)     2656 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_All-Users
+-rw-r--r--   0 jenkins    (115) docker     (999)     2612 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_Lock-Projects
+-rw-r--r--   0 jenkins    (115) docker     (999)    15289 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_alsa-scenario-scn-data-0-base
+-rw-r--r--   0 jenkins    (115) docker     (999)    14966 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_alsa-scenario-scn-data-0-mc1n2
+-rw-r--r--   0 jenkins    (115) docker     (999)     9662 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_ap_samsung_audio-hal-e3250
+-rw-r--r--   0 jenkins    (115) docker     (999)     9662 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_ap_samsung_audio-hal-e4x12
+-rw-r--r--   0 jenkins    (115) docker     (999)    15849 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_devices_nfc-plugin-nxp
+-rw-r--r--   0 jenkins    (115) docker     (999)    15926 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_intel_mfld_bootstub-mfld-blackbay
+-rw-r--r--   0 jenkins    (115) docker     (999)    12968 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_mtdev
+-rw-r--r--   0 jenkins    (115) docker     (999)    16116 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_opengl-es-virtual-drv
+-rw-r--r--   0 jenkins    (115) docker     (999)     9041 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_panda_libdrm
+-rw-r--r--   0 jenkins    (115) docker     (999)     6692 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_panda_libnl
+-rw-r--r--   0 jenkins    (115) docker     (999)    17765 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_xorg_driver_xserver-xorg-misc
+-rw-r--r--   0 jenkins    (115) docker     (999)    29634 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_apps_core_preloaded_ug-setting-gallery-efl
+-rw-r--r--   0 jenkins    (115) docker     (999)    28967 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_apps_core_preloaded_ug-setting-homescreen-efl
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.455358 swh.lister-5.7.0/swh/lister/cgit/tests/data/https_jff.email/
+-rw-r--r--   0 jenkins    (115) docker     (999)     3442 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cgit/tests/data/https_jff.email/cgit
+-rw-r--r--   0 jenkins    (115) docker     (999)     7243 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cgit/tests/repo_list.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     9441 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cgit/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1237 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cgit/tests/test_tasks.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1877 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cli.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.455358 swh.lister-5.7.0/swh/lister/conda/
+-rw-r--r--   0 jenkins    (115) docker     (999)     4336 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/conda/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4757 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/conda/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      589 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/conda/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.455358 swh.lister-5.7.0/swh/lister/conda/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/conda/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.367357 swh.lister-5.7.0/swh/lister/conda/tests/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.455358 swh.lister-5.7.0/swh/lister/conda/tests/data/https_conda.anaconda.org/
+-rw-r--r--   0 jenkins    (115) docker     (999)      955 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/conda/tests/data/https_conda.anaconda.org/conda-forge_linux-64_repodata.json.bz2
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.455358 swh.lister-5.7.0/swh/lister/conda/tests/data/https_repo.anaconda.com/
+-rw-r--r--   0 jenkins    (115) docker     (999)      634 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/conda/tests/data/https_repo.anaconda.com/pkgs_free_linux-64_repodata.json.bz2
+-rw-r--r--   0 jenkins    (115) docker     (999)      513 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/conda/tests/data/https_repo.anaconda.com/pkgs_free_osx-64_repodata.json.bz2
+-rw-r--r--   0 jenkins    (115) docker     (999)     1529 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/conda/tests/data/https_repo.anaconda.com/pkgs_free_win-64_repodata.json.bz2
+-rw-r--r--   0 jenkins    (115) docker     (999)     1445 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/conda/tests/data/https_repo.anaconda.com/pkgs_main_linux-64_repodata.json.bz2
+-rw-r--r--   0 jenkins    (115) docker     (999)      770 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/conda/tests/data/https_repo.anaconda.com/pkgs_pro_linux-64_repodata.json.bz2
+-rw-r--r--   0 jenkins    (115) docker     (999)     4332 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/conda/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1129 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/conda/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.455358 swh.lister-5.7.0/swh/lister/cpan/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1990 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cpan/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7360 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cpan/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      571 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cpan/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.455358 swh.lister-5.7.0/swh/lister/cpan/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cpan/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.367357 swh.lister-5.7.0/swh/lister/cpan/tests/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.459358 swh.lister-5.7.0/swh/lister/cpan/tests/data/https_fastapi.metacpan.org/
+-rw-r--r--   0 jenkins    (115) docker     (999)     9011 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cpan/tests/data/https_fastapi.metacpan.org/v1__search_scroll_page1
+-rw-r--r--   0 jenkins    (115) docker     (999)     1102 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cpan/tests/data/https_fastapi.metacpan.org/v1__search_scroll_page2
+-rw-r--r--   0 jenkins    (115) docker     (999)     2458 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cpan/tests/data/https_fastapi.metacpan.org/v1__search_scroll_page3
+-rw-r--r--   0 jenkins    (115) docker     (999)     4089 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cpan/tests/data/https_fastapi.metacpan.org/v1__search_scroll_page4
+-rw-r--r--   0 jenkins    (115) docker     (999)     9128 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cpan/tests/data/https_fastapi.metacpan.org/v1_release__search
+-rw-r--r--   0 jenkins    (115) docker     (999)     5367 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cpan/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1121 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cpan/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.459358 swh.lister-5.7.0/swh/lister/cran/
+-rw-r--r--   0 jenkins    (115) docker     (999)      331 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cran/__init__.py
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      305 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cran/list_all_packages.R
+-rw-r--r--   0 jenkins    (115) docker     (999)     4959 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cran/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      512 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cran/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.459358 swh.lister-5.7.0/swh/lister/cran/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cran/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.459358 swh.lister-5.7.0/swh/lister/cran/tests/data/
+-rw-r--r--   0 jenkins    (115) docker     (999)      883 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cran/tests/data/list-r-packages.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     4854 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cran/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1118 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/cran/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.459358 swh.lister-5.7.0/swh/lister/crates/
+-rw-r--r--   0 jenkins    (115) docker     (999)     4779 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/crates/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     9645 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/crates/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      599 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/crates/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.459358 swh.lister-5.7.0/swh/lister/crates/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)      174 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/crates/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.459358 swh.lister-5.7.0/swh/lister/crates/tests/data/
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     3851 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/crates/tests/data/fake_crates_repository_init.sh
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.459358 swh.lister-5.7.0/swh/lister/crates/tests/data/https_static.crates.io/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1358 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/crates/tests/data/https_static.crates.io/db-dump.tar.gz
+-rw-r--r--   0 jenkins    (115) docker     (999)     1534 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/crates/tests/data/https_static.crates.io/db-dump.tar.gz_visit1
+-rw-r--r--   0 jenkins    (115) docker     (999)     7982 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/crates/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1137 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/crates/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.459358 swh.lister-5.7.0/swh/lister/debian/
+-rw-r--r--   0 jenkins    (115) docker     (999)      460 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/debian/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    11302 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/debian/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      516 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/debian/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.459358 swh.lister-5.7.0/swh/lister/debian/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/debian/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.459358 swh.lister-5.7.0/swh/lister/debian/tests/data/
+-rw-r--r--   0 jenkins    (115) docker     (999)     5970 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/debian/tests/data/Sources_bullseye
+-rw-r--r--   0 jenkins    (115) docker     (999)     4413 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/debian/tests/data/Sources_buster
+-rw-r--r--   0 jenkins    (115) docker     (999)     4893 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/debian/tests/data/Sources_stretch
+-rw-r--r--   0 jenkins    (115) docker     (999)     9160 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/debian/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1440 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/debian/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.463358 swh.lister-5.7.0/swh/lister/fedora/
+-rw-r--r--   0 jenkins    (115) docker     (999)      400 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/fedora/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    10356 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/fedora/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      581 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/fedora/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.463358 swh.lister-5.7.0/swh/lister/fedora/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/fedora/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.371357 swh.lister-5.7.0/swh/lister/fedora/tests/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.463358 swh.lister-5.7.0/swh/lister/fedora/tests/data/archives.fedoraproject.org/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1982 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/fedora/tests/data/archives.fedoraproject.org/primary26.xml.gz
+-rw-r--r--   0 jenkins    (115) docker     (999)     1214 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/fedora/tests/data/archives.fedoraproject.org/primary36-altered.xml.gz
+-rw-r--r--   0 jenkins    (115) docker     (999)     1172 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/fedora/tests/data/archives.fedoraproject.org/primary36.xml.gz
+-rw-r--r--   0 jenkins    (115) docker     (999)     3112 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/fedora/tests/data/archives.fedoraproject.org/repomd26.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)     4971 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/fedora/tests/data/archives.fedoraproject.org/repomd36.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)     7582 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/fedora/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1944 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/fedora/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.463358 swh.lister-5.7.0/swh/lister/gitea/
+-rw-r--r--   0 jenkins    (115) docker     (999)      328 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/gitea/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      749 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/gitea/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      581 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/gitea/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.463358 swh.lister-5.7.0/swh/lister/gitea/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/gitea/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.371357 swh.lister-5.7.0/swh/lister/gitea/tests/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.463358 swh.lister-5.7.0/swh/lister/gitea/tests/data/https_try.gitea.io/
+-rw-r--r--   0 jenkins    (115) docker     (999)     5856 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/gitea/tests/data/https_try.gitea.io/repos_page1
+-rw-r--r--   0 jenkins    (115) docker     (999)     7652 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/gitea/tests/data/https_try.gitea.io/repos_page2
+-rw-r--r--   0 jenkins    (115) docker     (999)     6224 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/gitea/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1838 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/gitea/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.463358 swh.lister-5.7.0/swh/lister/github/
+-rw-r--r--   0 jenkins    (115) docker     (999)      330 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/github/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7559 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/github/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1859 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/github/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.463358 swh.lister-5.7.0/swh/lister/github/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/github/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     9015 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/github/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3036 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/github/tests/test_tasks.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      296 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/github/utils.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.487358 swh.lister-5.7.0/swh/lister/gitlab/
+-rw-r--r--   0 jenkins    (115) docker     (999)      335 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/gitlab/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    10135 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/gitlab/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      831 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/gitlab/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.491358 swh.lister-5.7.0/swh/lister/gitlab/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/gitlab/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.371357 swh.lister-5.7.0/swh/lister/gitlab/tests/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.491358 swh.lister-5.7.0/swh/lister/gitlab/tests/data/https_foss.heptapod.net/
+-rw-r--r--   0 jenkins    (115) docker     (999)    12380 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/gitlab/tests/data/https_foss.heptapod.net/api_response_page1.json
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.491358 swh.lister-5.7.0/swh/lister/gitlab/tests/data/https_gite.lirmm.fr/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1605 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/gitlab/tests/data/https_gite.lirmm.fr/api_response_page1.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     1750 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/gitlab/tests/data/https_gite.lirmm.fr/api_response_page2.json
+-rw-r--r--   0 jenkins    (115) docker     (999)      910 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/gitlab/tests/data/https_gite.lirmm.fr/api_response_page3.json
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.491358 swh.lister-5.7.0/swh/lister/gitlab/tests/data/https_gitlab.com/
+-rw-r--r--   0 jenkins    (115) docker     (999)     6065 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/gitlab/tests/data/https_gitlab.com/api_response_page1.json
+-rw-r--r--   0 jenkins    (115) docker     (999)    13570 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/gitlab/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1492 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/gitlab/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.491358 swh.lister-5.7.0/swh/lister/gnu/
+-rw-r--r--   0 jenkins    (115) docker     (999)      329 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/gnu/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2663 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/gnu/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      513 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/gnu/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.491358 swh.lister-5.7.0/swh/lister/gnu/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/gnu/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.491358 swh.lister-5.7.0/swh/lister/gnu/tests/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.491358 swh.lister-5.7.0/swh/lister/gnu/tests/data/https_ftp.gnu.org/
+-rw-r--r--   0 jenkins    (115) docker     (999)   622168 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/gnu/tests/data/https_ftp.gnu.org/tree.json.gz
+-rw-r--r--   0 jenkins    (115) docker     (999)     6450 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/gnu/tests/data/tree.json
+-rw-r--r--   0 jenkins    (115) docker     (999)      982 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/gnu/tests/data/tree.min.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     1290 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/gnu/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1077 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/gnu/tests/test_tasks.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     8690 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/gnu/tests/test_tree.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     9207 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/gnu/tree.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.495358 swh.lister-5.7.0/swh/lister/gogs/
+-rw-r--r--   0 jenkins    (115) docker     (999)      396 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/gogs/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7401 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/gogs/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      571 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/gogs/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.495358 swh.lister-5.7.0/swh/lister/gogs/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/gogs/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.371357 swh.lister-5.7.0/swh/lister/gogs/tests/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.495358 swh.lister-5.7.0/swh/lister/gogs/tests/data/https_try.gogs.io/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2949 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/gogs/tests/data/https_try.gogs.io/repos_page1
+-rw-r--r--   0 jenkins    (115) docker     (999)     3072 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/gogs/tests/data/https_try.gogs.io/repos_page2
+-rw-r--r--   0 jenkins    (115) docker     (999)     5873 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/gogs/tests/data/https_try.gogs.io/repos_page3
+-rw-r--r--   0 jenkins    (115) docker     (999)     3051 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/gogs/tests/data/https_try.gogs.io/repos_page4
+-rw-r--r--   0 jenkins    (115) docker     (999)    12373 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/gogs/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1830 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/gogs/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.495358 swh.lister-5.7.0/swh/lister/golang/
+-rw-r--r--   0 jenkins    (115) docker     (999)      330 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/golang/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6327 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/golang/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      756 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/golang/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.495358 swh.lister-5.7.0/swh/lister/golang/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/golang/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.495358 swh.lister-5.7.0/swh/lister/golang/tests/data/
+-rw-r--r--   0 jenkins    (115) docker     (999)      489 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/golang/tests/data/page-1.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      418 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/golang/tests/data/page-2.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     1118 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/golang/tests/data/page-3.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     7644 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/golang/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1743 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/golang/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.495358 swh.lister-5.7.0/swh/lister/hackage/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2804 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/hackage/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5183 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/hackage/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      621 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/hackage/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.495358 swh.lister-5.7.0/swh/lister/hackage/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/hackage/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.371357 swh.lister-5.7.0/swh/lister/hackage/tests/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.495358 swh.lister-5.7.0/swh/lister/hackage/tests/data/https_fake49.haskell.org/
+-rw-r--r--   0 jenkins    (115) docker     (999)    23107 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/hackage/tests/data/https_fake49.haskell.org/packages_search_0
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.499358 swh.lister-5.7.0/swh/lister/hackage/tests/data/https_fake51.haskell.org/
+-rw-r--r--   0 jenkins    (115) docker     (999)    23804 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/hackage/tests/data/https_fake51.haskell.org/packages_search_0
+-rw-r--r--   0 jenkins    (115) docker     (999)      577 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/hackage/tests/data/https_fake51.haskell.org/packages_search_1
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.499358 swh.lister-5.7.0/swh/lister/hackage/tests/data/https_hackage.haskell.org/
+-rw-r--r--   0 jenkins    (115) docker     (999)    23805 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/hackage/tests/data/https_hackage.haskell.org/packages_search_0
+-rw-r--r--   0 jenkins    (115) docker     (999)     1616 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/hackage/tests/data/https_hackage.haskell.org/packages_search_0_visit1
+-rw-r--r--   0 jenkins    (115) docker     (999)       40 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/hackage/tests/data/https_hackage.haskell.org/packages_search_0_visit2
+-rw-r--r--   0 jenkins    (115) docker     (999)    23353 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/hackage/tests/data/https_hackage.haskell.org/packages_search_1
+-rw-r--r--   0 jenkins    (115) docker     (999)    22764 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/hackage/tests/data/https_hackage.haskell.org/packages_search_2
+-rw-r--r--   0 jenkins    (115) docker     (999)     6472 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/hackage/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1159 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/hackage/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.499358 swh.lister-5.7.0/swh/lister/hex/
+-rw-r--r--   0 jenkins    (115) docker     (999)      394 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/hex/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4692 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/hex/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      595 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/hex/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.499358 swh.lister-5.7.0/swh/lister/hex/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/hex/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.371357 swh.lister-5.7.0/swh/lister/hex/tests/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.499358 swh.lister-5.7.0/swh/lister/hex/tests/data/https_hex.pm/
+-rw-r--r--   0 jenkins    (115) docker     (999)     6247 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/hex/tests/data/https_hex.pm/page1.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     7468 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/hex/tests/data/https_hex.pm/page2.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     3554 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/hex/tests/data/https_hex.pm/page3.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     5203 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/hex/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1737 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/hex/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.499358 swh.lister-5.7.0/swh/lister/launchpad/
+-rw-r--r--   0 jenkins    (115) docker     (999)      341 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/launchpad/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7518 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/launchpad/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      926 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/launchpad/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.499358 swh.lister-5.7.0/swh/lister/launchpad/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/launchpad/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1747 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/launchpad/tests/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.499358 swh.lister-5.7.0/swh/lister/launchpad/tests/data/
+-rw-r--r--   0 jenkins    (115) docker     (999)     5814 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/launchpad/tests/data/launchpad_bzr_response.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     5119 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/launchpad/tests/data/launchpad_response1.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     4960 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/launchpad/tests/data/launchpad_response2.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     8457 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/launchpad/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1793 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/launchpad/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.503358 swh.lister-5.7.0/swh/lister/maven/
+-rw-r--r--   0 jenkins    (115) docker     (999)     9772 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/maven/README.md
+-rw-r--r--   0 jenkins    (115) docker     (999)      328 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/maven/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    16142 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/maven/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      888 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/maven/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.503358 swh.lister-5.7.0/swh/lister/maven/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/maven/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.503358 swh.lister-5.7.0/swh/lister/maven/tests/data/
+-rw-r--r--   0 jenkins    (115) docker     (999)    31940 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/maven/tests/data/citrus-parent-3.0.7.pom
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.503358 swh.lister-5.7.0/swh/lister/maven/tests/data/http_indexes/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2312 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/maven/tests/data/http_indexes/export_full.fld
+-rw-r--r--   0 jenkins    (115) docker     (999)      740 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/maven/tests/data/http_indexes/export_incr_first.fld
+-rw-r--r--   0 jenkins    (115) docker     (999)      362 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/maven/tests/data/http_indexes/export_null_mtime.fld
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.507358 swh.lister-5.7.0/swh/lister/maven/tests/data/https_api.github.com/
+-rw-r--r--   0 jenkins    (115) docker     (999)     5749 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/maven/tests/data/https_api.github.com/repos_aldialimucaj_sprova4j
+-rw-r--r--   0 jenkins    (115) docker     (999)     7821 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/maven/tests/data/https_api.github.com/repos_arangodb-community_arangodb-graphql-java
+-rw-r--r--   0 jenkins    (115) docker     (999)     6110 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/maven/tests/data/https_api.github.com/repos_webx_citrus
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.507358 swh.lister-5.7.0/swh/lister/maven/tests/data/https_repo1.maven.org/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2834 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/maven/tests/data/https_repo1.maven.org/maven2_al_aldi_sprova4j_0.1.0_sprova4j-0.1.0.pom
+-rw-r--r--   0 jenkins    (115) docker     (999)     2823 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/maven/tests/data/https_repo1.maven.org/maven2_al_aldi_sprova4j_0.1.1_sprova4j-0.1.1.pom
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     7586 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/maven/tests/data/https_repo1.maven.org/maven2_com_arangodb_arangodb-graphql_1.2_arangodb-graphql-1.2.pom
+-rw-r--r--   0 jenkins    (115) docker     (999)     1094 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/maven/tests/data/sprova4j-0.1.0.invalidurl.pom
+-rw-r--r--   0 jenkins    (115) docker     (999)     2831 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/maven/tests/data/sprova4j-0.1.0.malformed.pom
+-rw-r--r--   0 jenkins    (115) docker     (999)    13122 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/maven/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1403 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/maven/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.511358 swh.lister-5.7.0/swh/lister/nixguix/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1221 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/nixguix/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    24552 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/nixguix/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      527 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/nixguix/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.511358 swh.lister-5.7.0/swh/lister/nixguix/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/nixguix/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.511358 swh.lister-5.7.0/swh/lister/nixguix/tests/data/
+-rw-r--r--   0 jenkins    (115) docker     (999)     6666 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/nixguix/tests/data/sources-failure.json
+-rw-r--r--   0 jenkins    (115) docker     (999)    10741 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/nixguix/tests/data/sources-success.json
+-rw-r--r--   0 jenkins    (115) docker     (999)    15509 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/nixguix/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      933 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/nixguix/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.511358 swh.lister-5.7.0/swh/lister/npm/
+-rw-r--r--   0 jenkins    (115) docker     (999)      540 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/npm/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5999 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/npm/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      827 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/npm/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.511358 swh.lister-5.7.0/swh/lister/npm/tests/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.511358 swh.lister-5.7.0/swh/lister/npm/tests/data/
+-rw-r--r--   0 jenkins    (115) docker     (999)    10583 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/npm/tests/data/npm_full_page1.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     7301 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/npm/tests/data/npm_full_page2.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     5759 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/npm/tests/data/npm_incremental_page1.json
+-rw-r--r--   0 jenkins    (115) docker     (999)    22638 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/npm/tests/data/npm_incremental_page2.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     6441 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/npm/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1784 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/npm/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.511358 swh.lister-5.7.0/swh/lister/nuget/
+-rw-r--r--   0 jenkins    (115) docker     (999)     3249 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/nuget/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5875 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/nuget/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      615 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/nuget/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.511358 swh.lister-5.7.0/swh/lister/nuget/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/nuget/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.375357 swh.lister-5.7.0/swh/lister/nuget/tests/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.515358 swh.lister-5.7.0/swh/lister/nuget/tests/data/https_api.nuget.org/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1336 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3-flatcontainer_intersoft.crosslight.logging.entityframework_5.0.5000.1235-experimental_intersoft.crosslight.logging.entityframework.nuspec
+-rw-r--r--   0 jenkins    (115) docker     (999)     1284 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3-flatcontainer_moq.automock_3.5.0-ci0287_moq.automock.nuspec
+-rw-r--r--   0 jenkins    (115) docker     (999)     2832 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3-flatcontainer_sil.core.desktop_10.0.1-beta0012_sil.core.desktop.nuspec
+-rw-r--r--   0 jenkins    (115) docker     (999)     8037 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_data_2022.09.23.08.07.54_sil.core.desktop.10.0.1-beta0012.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     5322 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_data_2022.09.23.09.10.26_intersoft.crosslight.logging.entityframework.5.0.5000.1235-experimental.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     6791 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_data_2022.10.10.04.04.00_moq.automock.3.5.0-ci0287.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     1519 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_index.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     1287 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_index.json_visit1
+-rw-r--r--   0 jenkins    (115) docker     (999)     2567 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_page11702.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     2146 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_page16958.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     1575 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_page17100.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     3634 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/nuget/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1129 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/nuget/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.515358 swh.lister-5.7.0/swh/lister/opam/
+-rw-r--r--   0 jenkins    (115) docker     (999)      326 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/opam/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5042 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/opam/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      512 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/opam/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.515358 swh.lister-5.7.0/swh/lister/opam/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/opam/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.375357 swh.lister-5.7.0/swh/lister/opam/tests/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.515358 swh.lister-5.7.0/swh/lister/opam/tests/data/fake_opam_repo/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.375357 swh.lister-5.7.0/swh/lister/opam/tests/data/fake_opam_repo/packages/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.375357 swh.lister-5.7.0/swh/lister/opam/tests/data/fake_opam_repo/packages/agrid/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.515358 swh.lister-5.7.0/swh/lister/opam/tests/data/fake_opam_repo/packages/agrid/agrid.0.1/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1123 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/opam/tests/data/fake_opam_repo/packages/agrid/agrid.0.1/opam
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.375357 swh.lister-5.7.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.515358 swh.lister-5.7.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.1/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1389 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.1/opam
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.515358 swh.lister-5.7.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.2/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1176 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.2/opam
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.515358 swh.lister-5.7.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.3/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1129 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.3/opam
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.515358 swh.lister-5.7.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.4/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1097 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.4/opam
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.515358 swh.lister-5.7.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.5/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1085 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.5/opam
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.519358 swh.lister-5.7.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.6/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1092 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.6/opam
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.375357 swh.lister-5.7.0/swh/lister/opam/tests/data/fake_opam_repo/packages/directories/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.519358 swh.lister-5.7.0/swh/lister/opam/tests/data/fake_opam_repo/packages/directories/directories.0.1/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1535 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/opam/tests/data/fake_opam_repo/packages/directories/directories.0.1/opam
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.519358 swh.lister-5.7.0/swh/lister/opam/tests/data/fake_opam_repo/packages/directories/directories.0.2/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1529 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/opam/tests/data/fake_opam_repo/packages/directories/directories.0.2/opam
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.519358 swh.lister-5.7.0/swh/lister/opam/tests/data/fake_opam_repo/packages/directories/directories.0.3/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1472 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/opam/tests/data/fake_opam_repo/packages/directories/directories.0.3/opam
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.375357 swh.lister-5.7.0/swh/lister/opam/tests/data/fake_opam_repo/packages/ocb/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.519358 swh.lister-5.7.0/swh/lister/opam/tests/data/fake_opam_repo/packages/ocb/ocb.0.1/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1004 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/opam/tests/data/fake_opam_repo/packages/ocb/ocb.0.1/opam
+-rw-r--r--   0 jenkins    (115) docker     (999)       20 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/opam/tests/data/fake_opam_repo/repo
+-rw-r--r--   0 jenkins    (115) docker     (999)        6 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/opam/tests/data/fake_opam_repo/version
+-rw-r--r--   0 jenkins    (115) docker     (999)     5843 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/opam/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1121 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/opam/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.519358 swh.lister-5.7.0/swh/lister/packagist/
+-rw-r--r--   0 jenkins    (115) docker     (999)      341 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/packagist/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7053 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/packagist/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      518 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/packagist/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.519358 swh.lister-5.7.0/swh/lister/packagist/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/packagist/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.519358 swh.lister-5.7.0/swh/lister/packagist/tests/data/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2281 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/packagist/tests/data/den1n_contextmenu.json
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.519358 swh.lister-5.7.0/swh/lister/packagist/tests/data/https_api.github.com/
+-rw-r--r--   0 jenkins    (115) docker     (999)       53 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/packagist/tests/data/https_api.github.com/repos_gitlky_wx_article
+-rw-r--r--   0 jenkins    (115) docker     (999)     6972 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/packagist/tests/data/https_api.github.com/repos_spryker-eco_computop-api
+-rw-r--r--   0 jenkins    (115) docker     (999)     5394 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/packagist/tests/data/https_api.github.com/repos_ycms_module-main
+-rw-r--r--   0 jenkins    (115) docker     (999)     9749 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/packagist/tests/data/idevlab_essential.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     2545 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/packagist/tests/data/ljjackson_linnworks.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     6911 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/packagist/tests/data/lky_wx_article.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     4632 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/packagist/tests/data/payrix_payrix-php.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     4062 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/packagist/tests/data/spryker-eco_computop-api.json
+-rw-r--r--   0 jenkins    (115) docker     (999)      595 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/packagist/tests/data/with_invalid_url.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     1097 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/packagist/tests/data/ycms_module-main.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     6680 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/packagist/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1052 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/packagist/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.519358 swh.lister-5.7.0/swh/lister/pagure/
+-rw-r--r--   0 jenkins    (115) docker     (999)      330 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/pagure/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2497 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/pagure/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      531 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/pagure/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.523358 swh.lister-5.7.0/swh/lister/pagure/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/pagure/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.419357 swh.lister-5.7.0/swh/lister/pagure/tests/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.523358 swh.lister-5.7.0/swh/lister/pagure/tests/data/https_pagure.io/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2593 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/pagure/tests/data/https_pagure.io/api_0_projects,per_page=2
+-rw-r--r--   0 jenkins    (115) docker     (999)     2718 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/pagure/tests/data/https_pagure.io/api_0_projects,per_page=2,page=2
+-rw-r--r--   0 jenkins    (115) docker     (999)     1146 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/pagure/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1137 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/pagure/tests/test_tasks.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    15575 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/pattern.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.523358 swh.lister-5.7.0/swh/lister/phabricator/
+-rw-r--r--   0 jenkins    (115) docker     (999)      345 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/phabricator/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6039 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/phabricator/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      753 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/phabricator/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.523358 swh.lister-5.7.0/swh/lister/phabricator/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/phabricator/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.523358 swh.lister-5.7.0/swh/lister/phabricator/tests/data/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/phabricator/tests/data/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    44289 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/phabricator/tests/data/phabricator_api_repositories_page1.json
+-rw-r--r--   0 jenkins    (115) docker     (999)    46784 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/phabricator/tests/data/phabricator_api_repositories_page2.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     4330 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/phabricator/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1284 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/phabricator/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.523358 swh.lister-5.7.0/swh/lister/pubdev/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2064 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/pubdev/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3573 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/pubdev/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      609 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/pubdev/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.523358 swh.lister-5.7.0/swh/lister/pubdev/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/pubdev/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.419357 swh.lister-5.7.0/swh/lister/pubdev/tests/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.523358 swh.lister-5.7.0/swh/lister/pubdev/tests/data/https_pub.dev/
+-rw-r--r--   0 jenkins    (115) docker     (999)       74 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/pubdev/tests/data/https_pub.dev/api_package-names
+-rw-r--r--   0 jenkins    (115) docker     (999)     1578 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/pubdev/tests/data/https_pub.dev/api_packages_Autolinker
+-rw-r--r--   0 jenkins    (115) docker     (999)     1557 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/pubdev/tests/data/https_pub.dev/api_packages_Babylon
+-rw-r--r--   0 jenkins    (115) docker     (999)     1508 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/pubdev/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1137 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/pubdev/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.523358 swh.lister-5.7.0/swh/lister/puppet/
+-rw-r--r--   0 jenkins    (115) docker     (999)     3557 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/puppet/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6203 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/puppet/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      583 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/puppet/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.527358 swh.lister-5.7.0/swh/lister/puppet/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/puppet/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.419357 swh.lister-5.7.0/swh/lister/puppet/tests/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.527358 swh.lister-5.7.0/swh/lister/puppet/tests/data/https_forgeapi.puppet.com/
+-rw-r--r--   0 jenkins    (115) docker     (999)    94411 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/puppet/tests/data/https_forgeapi.puppet.com/v3_modules,limit=100
+-rw-r--r--   0 jenkins    (115) docker     (999)    10141 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/puppet/tests/data/https_forgeapi.puppet.com/v3_modules,limit=100,offset=100
+-rw-r--r--   0 jenkins    (115) docker     (999)    92818 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/puppet/tests/data/https_forgeapi.puppet.com/v3_modules,limit=100,with_release_since=2022-09-26
+-rw-r--r--   0 jenkins    (115) docker     (999)     5702 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/puppet/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1137 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/puppet/tests/test_tasks.py
+-rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/py.typed
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.527358 swh.lister-5.7.0/swh/lister/pypi/
+-rw-r--r--   0 jenkins    (115) docker     (999)      331 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/pypi/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6736 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/pypi/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      492 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/pypi/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.527358 swh.lister-5.7.0/swh/lister/pypi/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/pypi/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     8171 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/pypi/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1040 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/pypi/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.527358 swh.lister-5.7.0/swh/lister/rubygems/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1616 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/rubygems/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     9375 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/rubygems/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      595 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/rubygems/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.527358 swh.lister-5.7.0/swh/lister/rubygems/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/rubygems/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.527358 swh.lister-5.7.0/swh/lister/rubygems/tests/data/
+-rw-r--r--   0 jenkins    (115) docker     (999)      894 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/rubygems/tests/data/rubygems_dumps.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)     2867 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/rubygems/tests/data/rubygems_pgsql_dump.tar
+-rw-r--r--   0 jenkins    (115) docker     (999)     1361 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/rubygems/tests/data/small_rubygems_dump.sh
+-rw-r--r--   0 jenkins    (115) docker     (999)     6208 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/rubygems/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1167 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/rubygems/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.531358 swh.lister-5.7.0/swh/lister/sourceforge/
+-rw-r--r--   0 jenkins    (115) docker     (999)      340 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/sourceforge/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    18526 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/sourceforge/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      820 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/sourceforge/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.531358 swh.lister-5.7.0/swh/lister/sourceforge/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/sourceforge/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.535358 swh.lister-5.7.0/swh/lister/sourceforge/tests/data/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1632 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/sourceforge/tests/data/aaron.html
+-rw-r--r--   0 jenkins    (115) docker     (999)     6332 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/sourceforge/tests/data/aaron.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     2242 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/sourceforge/tests/data/adobexmp.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     3993 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/sourceforge/tests/data/backapps-website.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     5614 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/sourceforge/tests/data/backapps.json
+-rw-r--r--   0 jenkins    (115) docker     (999)      384 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/sourceforge/tests/data/main-sitemap.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)     3041 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/sourceforge/tests/data/mojunk.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     3938 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/sourceforge/tests/data/mramm.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     2404 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/sourceforge/tests/data/ocaml-lpd.html
+-rw-r--r--   0 jenkins    (115) docker     (999)     5477 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/sourceforge/tests/data/ocaml-lpd.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     3209 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/sourceforge/tests/data/os3dmodels.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     1218 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/sourceforge/tests/data/random-mercurial.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     2757 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/sourceforge/tests/data/subsitemap-0.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)     1523 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/sourceforge/tests/data/subsitemap-1.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)     7836 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/sourceforge/tests/data/t12eksandbox.html
+-rw-r--r--   0 jenkins    (115) docker     (999)     7904 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/sourceforge/tests/data/t12eksandbox.json
+-rw-r--r--   0 jenkins    (115) docker     (999)    19233 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/sourceforge/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1827 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/sourceforge/tests/test_tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.535358 swh.lister-5.7.0/swh/lister/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2053 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/tests/test_cli.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     9972 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/tests/test_pattern.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1191 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/tests/test_utils.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      386 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/tests/utils.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.535358 swh.lister-5.7.0/swh/lister/tuleap/
+-rw-r--r--   0 jenkins    (115) docker     (999)      330 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/tuleap/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4611 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/tuleap/lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      579 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/tuleap/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.535358 swh.lister-5.7.0/swh/lister/tuleap/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/tuleap/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.419357 swh.lister-5.7.0/swh/lister/tuleap/tests/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.535358 swh.lister-5.7.0/swh/lister/tuleap/tests/data/https_tuleap.net/
+-rw-r--r--   0 jenkins    (115) docker     (999)     4552 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/tuleap/tests/data/https_tuleap.net/projects
+-rw-r--r--   0 jenkins    (115) docker     (999)      422 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/tuleap/tests/data/https_tuleap.net/repo_1
+-rw-r--r--   0 jenkins    (115) docker     (999)      338 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/tuleap/tests/data/https_tuleap.net/repo_2
+-rw-r--r--   0 jenkins    (115) docker     (999)       20 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/tuleap/tests/data/https_tuleap.net/repo_3
+-rw-r--r--   0 jenkins    (115) docker     (999)     5639 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/tuleap/tests/test_lister.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1788 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/tuleap/tests/test_tasks.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2215 2023-06-23 10:04:04.000000 swh.lister-5.7.0/swh/lister/utils.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-23 10:04:08.427358 swh.lister-5.7.0/swh.lister.egg-info/
+-rw-r--r--   0 jenkins    (115) docker     (999)     4108 2023-06-23 10:04:08.000000 swh.lister-5.7.0/swh.lister.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)    21406 2023-06-23 10:04:08.000000 swh.lister-5.7.0/swh.lister.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-06-23 10:04:08.000000 swh.lister-5.7.0/swh.lister.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     1507 2023-06-23 10:04:08.000000 swh.lister-5.7.0/swh.lister.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      263 2023-06-23 10:04:08.000000 swh.lister-5.7.0/swh.lister.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-06-23 10:04:08.000000 swh.lister-5.7.0/swh.lister.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     1599 2023-06-23 10:04:04.000000 swh.lister-5.7.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `swh.lister-5.6.3/.pre-commit-config.yaml` & `swh.lister-5.7.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/CODE_OF_CONDUCT.md` & `swh.lister-5.7.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/LICENSE` & `swh.lister-5.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/PKG-INFO` & `swh.lister-5.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.lister
-Version: 5.6.3
+Version: 5.7.0
 Summary: Software Heritage lister
 Home-page: https://forge.softwareheritage.org/diffusion/DLSGH/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-lister
```

### Comparing `swh.lister-5.6.3/README.md` & `swh.lister-5.7.0/README.md`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/conftest.py` & `swh.lister-5.7.0/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/docs/images/new_base.png` & `swh.lister-5.7.0/docs/images/new_base.png`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/docs/images/new_bitbucket_lister.png` & `swh.lister-5.7.0/docs/images/new_bitbucket_lister.png`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/docs/images/new_github_lister.png` & `swh.lister-5.7.0/docs/images/new_github_lister.png`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/docs/images/old_github_lister.png` & `swh.lister-5.7.0/docs/images/old_github_lister.png`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/docs/index.rst` & `swh.lister-5.7.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/docs/new_lister_template.py` & `swh.lister-5.7.0/docs/new_lister_template.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/docs/run_a_new_lister.rst` & `swh.lister-5.7.0/docs/run_a_new_lister.rst`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/docs/save_forge.rst` & `swh.lister-5.7.0/docs/save_forge.rst`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/docs/tutorial.rst` & `swh.lister-5.7.0/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/mypy.ini` & `swh.lister-5.7.0/mypy.ini`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/setup.py` & `swh.lister-5.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,14 +76,15 @@
         lister.hex=swh.lister.hex:register
         lister.launchpad=swh.lister.launchpad:register
         lister.nixguix=swh.lister.nixguix:register
         lister.npm=swh.lister.npm:register
         lister.nuget=swh.lister.nuget:register
         lister.opam=swh.lister.opam:register
         lister.packagist=swh.lister.packagist:register
+        lister.pagure=swh.lister.pagure:register
         lister.phabricator=swh.lister.phabricator:register
         lister.pubdev=swh.lister.pubdev:register
         lister.puppet=swh.lister.puppet:register
         lister.pypi=swh.lister.pypi:register
         lister.rubygems=swh.lister.rubygems:register
         lister.sourceforge=swh.lister.sourceforge:register
         lister.tuleap=swh.lister.tuleap:register
```

### Comparing `swh.lister-5.6.3/sql/crawler.sql` & `swh.lister-5.7.0/sql/crawler.sql`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/sql/pimp_db.sql` & `swh.lister-5.7.0/sql/pimp_db.sql`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/__init__.py` & `swh.lister-5.7.0/swh/lister/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/arch/__init__.py` & `swh.lister-5.7.0/swh/lister/arch/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/arch/lister.py` & `swh.lister-5.7.0/swh/lister/arch/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/arch/tasks.py` & `swh.lister-5.7.0/swh/lister/arch/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/arch/tests/__init__.py` & `swh.lister-5.7.0/swh/lister/arch/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/arch/tests/data/fake_archlinux_archives_init.sh` & `swh.lister-5.7.0/swh/lister/arch/tests/data/fake_archlinux_archives_init.sh`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_d_dialog` & `swh.lister-5.7.0/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_d_dialog`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_g_gnome-code-assistance` & `swh.lister-5.7.0/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_g_gnome-code-assistance`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_g_gzip` & `swh.lister-5.7.0/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_g_gzip`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_l_libasyncns` & `swh.lister-5.7.0/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_l_libasyncns`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_m_mercurial` & `swh.lister-5.7.0/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_m_mercurial`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_p_python-hglib` & `swh.lister-5.7.0/swh/lister/arch/tests/data/https_archive.archlinux.org/packages_p_python-hglib`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/arch/tests/data/https_archive.archlinux.org/repos_last_community_os_x86_64_community.files.tar.gz` & `swh.lister-5.7.0/swh/lister/arch/tests/data/https_archive.archlinux.org/repos_last_community_os_x86_64_community.files.tar.gz`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/arch/tests/data/https_archive.archlinux.org/repos_last_core_os_x86_64_core.files.tar.gz` & `swh.lister-5.7.0/swh/lister/arch/tests/data/https_archive.archlinux.org/repos_last_core_os_x86_64_core.files.tar.gz`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/arch/tests/data/https_archive.archlinux.org/repos_last_extra_os_x86_64_extra.files.tar.gz` & `swh.lister-5.7.0/swh/lister/arch/tests/data/https_archive.archlinux.org/repos_last_extra_os_x86_64_extra.files.tar.gz`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/aarch64_community_community.files.tar.gz` & `swh.lister-5.7.0/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/aarch64_community_community.files.tar.gz`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/aarch64_core_core.files.tar.gz` & `swh.lister-5.7.0/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/aarch64_core_core.files.tar.gz`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/aarch64_extra_extra.files.tar.gz` & `swh.lister-5.7.0/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/aarch64_extra_extra.files.tar.gz`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/armv7h_community_community.files.tar.gz` & `swh.lister-5.7.0/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/armv7h_community_community.files.tar.gz`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/armv7h_core_core.files.tar.gz` & `swh.lister-5.7.0/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/armv7h_core_core.files.tar.gz`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/armv7h_extra_extra.files.tar.gz` & `swh.lister-5.7.0/swh/lister/arch/tests/data/https_uk.mirror.archlinuxarm.org/armv7h_extra_extra.files.tar.gz`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/arch/tests/test_lister.py` & `swh.lister-5.7.0/swh/lister/arch/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/arch/tests/test_tasks.py` & `swh.lister-5.7.0/swh/lister/arch/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/aur/__init__.py` & `swh.lister-5.7.0/swh/lister/aur/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/aur/lister.py` & `swh.lister-5.7.0/swh/lister/aur/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/aur/tasks.py` & `swh.lister-5.7.0/swh/lister/aur/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/aur/tests/data/fake_aur_packages.sh` & `swh.lister-5.7.0/swh/lister/aur/tests/data/fake_aur_packages.sh`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/aur/tests/data/packages-meta-v1.json.gz` & `swh.lister-5.7.0/swh/lister/aur/tests/data/packages-meta-v1.json.gz`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/aur/tests/test_lister.py` & `swh.lister-5.7.0/swh/lister/aur/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/aur/tests/test_tasks.py` & `swh.lister-5.7.0/swh/lister/aur/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/bitbucket/lister.py` & `swh.lister-5.7.0/swh/lister/bitbucket/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/bitbucket/tasks.py` & `swh.lister-5.7.0/swh/lister/bitbucket/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/bitbucket/tests/data/bb_api_repositories_page1.json` & `swh.lister-5.7.0/swh/lister/bitbucket/tests/data/bb_api_repositories_page1.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/bitbucket/tests/data/bb_api_repositories_page2.json` & `swh.lister-5.7.0/swh/lister/bitbucket/tests/data/bb_api_repositories_page2.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/bitbucket/tests/test_lister.py` & `swh.lister-5.7.0/swh/lister/bitbucket/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/bitbucket/tests/test_tasks.py` & `swh.lister-5.7.0/swh/lister/bitbucket/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/bower/__init__.py` & `swh.lister-5.7.0/swh/lister/bower/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/bower/lister.py` & `swh.lister-5.7.0/swh/lister/bower/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/bower/tasks.py` & `swh.lister-5.7.0/swh/lister/bower/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/bower/tests/test_lister.py` & `swh.lister-5.7.0/swh/lister/bower/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/bower/tests/test_tasks.py` & `swh.lister-5.7.0/swh/lister/bower/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cgit/lister.py` & `swh.lister-5.7.0/swh/lister/cgit/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cgit/tasks.py` & `swh.lister-5.7.0/swh/lister/cgit/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.acdw.net/cgit` & `swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.acdw.net/cgit`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.acdw.net/foo` & `swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.acdw.net/foo`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.acdw.net/foo_summary` & `swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.acdw.net/foo_summary`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.acdw.net/sfeed` & `swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.acdw.net/sfeed`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.acdw.net/sfeed_summary` & `swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.acdw.net/sfeed_summary`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.baserock.org/cgit` & `swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.baserock.org/cgit`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.eclipse.org/c` & `swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.eclipse.org/c`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.savannah.gnu.org/cgit` & `swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.savannah.gnu.org/cgit`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.savannah.gnu.org/cgit_elisp-es.git` & `swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.savannah.gnu.org/cgit_elisp-es.git`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.tizen/cgit` & `swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.tizen/cgit`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.tizen/cgit,ofs=100` & `swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.tizen/cgit,ofs=100`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.tizen/cgit,ofs=50` & `swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.tizen/cgit,ofs=50`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.tizen/cgit_All-Projects` & `swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_All-Projects`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.tizen/cgit_All-Users` & `swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_All-Users`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.tizen/cgit_Lock-Projects` & `swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_Lock-Projects`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_alsa-scenario-scn-data-0-base` & `swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_alsa-scenario-scn-data-0-base`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_alsa-scenario-scn-data-0-mc1n2` & `swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_alsa-scenario-scn-data-0-mc1n2`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_ap_samsung_audio-hal-e3250` & `swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_ap_samsung_audio-hal-e3250`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_ap_samsung_audio-hal-e4x12` & `swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_ap_samsung_audio-hal-e4x12`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_devices_nfc-plugin-nxp` & `swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_devices_nfc-plugin-nxp`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_intel_mfld_bootstub-mfld-blackbay` & `swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_intel_mfld_bootstub-mfld-blackbay`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_mtdev` & `swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_mtdev`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_opengl-es-virtual-drv` & `swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_opengl-es-virtual-drv`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_panda_libdrm` & `swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_panda_libdrm`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_panda_libnl` & `swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_panda_libnl`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_xorg_driver_xserver-xorg-misc` & `swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_adaptation_xorg_driver_xserver-xorg-misc`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.tizen/cgit_apps_core_preloaded_ug-setting-gallery-efl` & `swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_apps_core_preloaded_ug-setting-gallery-efl`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cgit/tests/data/https_git.tizen/cgit_apps_core_preloaded_ug-setting-homescreen-efl` & `swh.lister-5.7.0/swh/lister/cgit/tests/data/https_git.tizen/cgit_apps_core_preloaded_ug-setting-homescreen-efl`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cgit/tests/data/https_jff.email/cgit` & `swh.lister-5.7.0/swh/lister/cgit/tests/data/https_jff.email/cgit`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cgit/tests/repo_list.txt` & `swh.lister-5.7.0/swh/lister/cgit/tests/repo_list.txt`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cgit/tests/test_lister.py` & `swh.lister-5.7.0/swh/lister/cgit/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cgit/tests/test_tasks.py` & `swh.lister-5.7.0/swh/lister/cgit/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cli.py` & `swh.lister-5.7.0/swh/lister/cli.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/conda/__init__.py` & `swh.lister-5.7.0/swh/lister/conda/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/conda/lister.py` & `swh.lister-5.7.0/swh/lister/conda/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/conda/tasks.py` & `swh.lister-5.7.0/swh/lister/conda/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/conda/tests/data/https_conda.anaconda.org/conda-forge_linux-64_repodata.json.bz2` & `swh.lister-5.7.0/swh/lister/conda/tests/data/https_conda.anaconda.org/conda-forge_linux-64_repodata.json.bz2`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/conda/tests/data/https_repo.anaconda.com/pkgs_free_linux-64_repodata.json.bz2` & `swh.lister-5.7.0/swh/lister/conda/tests/data/https_repo.anaconda.com/pkgs_free_linux-64_repodata.json.bz2`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/conda/tests/data/https_repo.anaconda.com/pkgs_free_osx-64_repodata.json.bz2` & `swh.lister-5.7.0/swh/lister/conda/tests/data/https_repo.anaconda.com/pkgs_free_osx-64_repodata.json.bz2`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/conda/tests/data/https_repo.anaconda.com/pkgs_free_win-64_repodata.json.bz2` & `swh.lister-5.7.0/swh/lister/conda/tests/data/https_repo.anaconda.com/pkgs_free_win-64_repodata.json.bz2`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/conda/tests/data/https_repo.anaconda.com/pkgs_main_linux-64_repodata.json.bz2` & `swh.lister-5.7.0/swh/lister/conda/tests/data/https_repo.anaconda.com/pkgs_main_linux-64_repodata.json.bz2`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/conda/tests/data/https_repo.anaconda.com/pkgs_pro_linux-64_repodata.json.bz2` & `swh.lister-5.7.0/swh/lister/conda/tests/data/https_repo.anaconda.com/pkgs_pro_linux-64_repodata.json.bz2`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/conda/tests/test_lister.py` & `swh.lister-5.7.0/swh/lister/conda/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/conda/tests/test_tasks.py` & `swh.lister-5.7.0/swh/lister/conda/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cpan/__init__.py` & `swh.lister-5.7.0/swh/lister/cpan/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cpan/lister.py` & `swh.lister-5.7.0/swh/lister/cpan/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cpan/tasks.py` & `swh.lister-5.7.0/swh/lister/cpan/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cpan/tests/data/https_fastapi.metacpan.org/v1__search_scroll_page1` & `swh.lister-5.7.0/swh/lister/cpan/tests/data/https_fastapi.metacpan.org/v1__search_scroll_page1`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cpan/tests/data/https_fastapi.metacpan.org/v1__search_scroll_page2` & `swh.lister-5.7.0/swh/lister/cpan/tests/data/https_fastapi.metacpan.org/v1__search_scroll_page2`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cpan/tests/data/https_fastapi.metacpan.org/v1__search_scroll_page3` & `swh.lister-5.7.0/swh/lister/cpan/tests/data/https_fastapi.metacpan.org/v1__search_scroll_page3`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cpan/tests/data/https_fastapi.metacpan.org/v1__search_scroll_page4` & `swh.lister-5.7.0/swh/lister/cpan/tests/data/https_fastapi.metacpan.org/v1__search_scroll_page4`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cpan/tests/data/https_fastapi.metacpan.org/v1_release__search` & `swh.lister-5.7.0/swh/lister/cpan/tests/data/https_fastapi.metacpan.org/v1_release__search`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cpan/tests/test_lister.py` & `swh.lister-5.7.0/swh/lister/cpan/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cpan/tests/test_tasks.py` & `swh.lister-5.7.0/swh/lister/cpan/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cran/lister.py` & `swh.lister-5.7.0/swh/lister/cran/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cran/tasks.py` & `swh.lister-5.7.0/swh/lister/cran/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cran/tests/data/list-r-packages.json` & `swh.lister-5.7.0/swh/lister/cran/tests/data/list-r-packages.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cran/tests/test_lister.py` & `swh.lister-5.7.0/swh/lister/cran/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/cran/tests/test_tasks.py` & `swh.lister-5.7.0/swh/lister/cran/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/crates/__init__.py` & `swh.lister-5.7.0/swh/lister/crates/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/crates/lister.py` & `swh.lister-5.7.0/swh/lister/crates/lister.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,23 +117,28 @@
             with self.http_request(self.DB_DUMP_URL, stream=True) as res:
                 with open(archive_path, "wb") as out_file:
                     for chunk in res.iter_content(chunk_size=1024):
                         out_file.write(chunk)
 
             # Extract the Db dump
             db_dump_path = Path(str(archive_path).split(".tar.gz")[0])
-            tar = tarfile.open(archive_path)
-            tar.extractall(path=db_dump_path)
-            tar.close()
+            members_to_extract = []
+            with tarfile.open(archive_path) as tf:
+                for member in tf.getmembers():
+                    if member.name.endswith(
+                        ("/data/crates.csv", "/data/versions.csv", "/metadata.json")
+                    ):
+                        members_to_extract.append(member)
+                tf.extractall(members=members_to_extract, path=db_dump_path)
 
             csv.field_size_limit(1000000)
 
             (crates_csv_path,) = list(db_dump_path.glob("*/data/crates.csv"))
             (versions_csv_path,) = list(db_dump_path.glob("*/data/versions.csv"))
-            (index_metadata_json_path,) = list(db_dump_path.rglob("*metadata.json"))
+            (index_metadata_json_path,) = list(db_dump_path.rglob("*/metadata.json"))
 
             with index_metadata_json_path.open("rb") as index_metadata_json:
                 self.index_metadata = json.load(index_metadata_json)
 
             crates: Dict[str, Any] = {}
             with crates_csv_path.open() as crates_fd:
                 crates_csv = csv.DictReader(crates_fd)
```

### Comparing `swh.lister-5.6.3/swh/lister/crates/tasks.py` & `swh.lister-5.7.0/swh/lister/crates/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/crates/tests/data/fake_crates_repository_init.sh` & `swh.lister-5.7.0/swh/lister/crates/tests/data/fake_crates_repository_init.sh`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/crates/tests/data/https_static.crates.io/db-dump.tar.gz` & `swh.lister-5.7.0/swh/lister/crates/tests/data/https_static.crates.io/db-dump.tar.gz`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/crates/tests/data/https_static.crates.io/db-dump.tar.gz_visit1` & `swh.lister-5.7.0/swh/lister/crates/tests/data/https_static.crates.io/db-dump.tar.gz_visit1`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/crates/tests/test_lister.py` & `swh.lister-5.7.0/swh/lister/crates/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/crates/tests/test_tasks.py` & `swh.lister-5.7.0/swh/lister/crates/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/debian/lister.py` & `swh.lister-5.7.0/swh/lister/debian/lister.py`

 * *Files 3% similar despite different names*

```diff
@@ -228,36 +228,37 @@
                     extra_loader_arguments={"packages": {}},
                     last_update=self.last_sources_update,
                 )
                 # init set that will contain all listed package versions
                 self.package_versions[package_name] = set()
 
             # origin will be yielded at the end of that method
-            origins_to_send[origin_url] = self.listed_origins[origin_url]
+            current_origin = origins_to_send[origin_url] = self.listed_origins[
+                origin_url
+            ]
 
             # update package versions data in parameter that will be provided
             # to the debian loader
-            self.listed_origins[origin_url].extra_loader_arguments["packages"].update(
+            current_origin.extra_loader_arguments["packages"].update(
                 {
                     package_version_key: {
                         "name": package_name,
                         "version": package_version,
                         "files": files,
                     }
                 }
             )
 
-            if self.listed_origins[origin_url].last_update is None or (
+            if current_origin.last_update is None or (
                 self.last_sources_update is not None
-                and self.last_sources_update  # type: ignore
-                > self.listed_origins[origin_url].last_update
+                and self.last_sources_update > current_origin.last_update
             ):
                 # update debian package last update if current processed sources index
                 # has a greater modification date
-                self.listed_origins[origin_url].last_update = self.last_sources_update
+                current_origin.last_update = self.last_sources_update
 
             # add package version key to the set of found versions
             self.package_versions[package_name].add(package_version_key)
 
             # package has already been listed during a previous listing process
             if package_name in self.state.package_versions:
                 new_versions = (
```

### Comparing `swh.lister-5.6.3/swh/lister/debian/tasks.py` & `swh.lister-5.7.0/swh/lister/debian/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/debian/tests/data/Sources_bullseye` & `swh.lister-5.7.0/swh/lister/debian/tests/data/Sources_bullseye`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/debian/tests/data/Sources_buster` & `swh.lister-5.7.0/swh/lister/debian/tests/data/Sources_buster`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/debian/tests/data/Sources_stretch` & `swh.lister-5.7.0/swh/lister/debian/tests/data/Sources_stretch`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/debian/tests/test_lister.py` & `swh.lister-5.7.0/swh/lister/debian/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/debian/tests/test_tasks.py` & `swh.lister-5.7.0/swh/lister/debian/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/fedora/lister.py` & `swh.lister-5.7.0/swh/lister/fedora/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/fedora/tasks.py` & `swh.lister-5.7.0/swh/lister/fedora/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/fedora/tests/data/archives.fedoraproject.org/primary26.xml.gz` & `swh.lister-5.7.0/swh/lister/fedora/tests/data/archives.fedoraproject.org/primary26.xml.gz`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/fedora/tests/data/archives.fedoraproject.org/primary36-altered.xml.gz` & `swh.lister-5.7.0/swh/lister/fedora/tests/data/archives.fedoraproject.org/primary36-altered.xml.gz`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/fedora/tests/data/archives.fedoraproject.org/primary36.xml.gz` & `swh.lister-5.7.0/swh/lister/fedora/tests/data/archives.fedoraproject.org/primary36.xml.gz`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/fedora/tests/data/archives.fedoraproject.org/repomd26.xml` & `swh.lister-5.7.0/swh/lister/fedora/tests/data/archives.fedoraproject.org/repomd26.xml`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/fedora/tests/data/archives.fedoraproject.org/repomd36.xml` & `swh.lister-5.7.0/swh/lister/fedora/tests/data/archives.fedoraproject.org/repomd36.xml`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/fedora/tests/test_lister.py` & `swh.lister-5.7.0/swh/lister/fedora/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/fedora/tests/test_tasks.py` & `swh.lister-5.7.0/swh/lister/fedora/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/gitea/lister.py` & `swh.lister-5.7.0/swh/lister/gitea/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/gitea/tasks.py` & `swh.lister-5.7.0/swh/lister/gitea/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/gitea/tests/data/https_try.gitea.io/repos_page1` & `swh.lister-5.7.0/swh/lister/gitea/tests/data/https_try.gitea.io/repos_page1`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/gitea/tests/data/https_try.gitea.io/repos_page2` & `swh.lister-5.7.0/swh/lister/gitea/tests/data/https_try.gitea.io/repos_page2`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/gitea/tests/test_lister.py` & `swh.lister-5.7.0/swh/lister/gitea/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/gitea/tests/test_tasks.py` & `swh.lister-5.7.0/swh/lister/gitea/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/github/lister.py` & `swh.lister-5.7.0/swh/lister/github/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/github/tasks.py` & `swh.lister-5.7.0/swh/lister/github/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/github/tests/test_lister.py` & `swh.lister-5.7.0/swh/lister/github/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/github/tests/test_tasks.py` & `swh.lister-5.7.0/swh/lister/github/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/gitlab/lister.py` & `swh.lister-5.7.0/swh/lister/gitlab/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/gitlab/tasks.py` & `swh.lister-5.7.0/swh/lister/gitlab/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/gitlab/tests/data/https_foss.heptapod.net/api_response_page1.json` & `swh.lister-5.7.0/swh/lister/gitlab/tests/data/https_foss.heptapod.net/api_response_page1.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/gitlab/tests/data/https_gite.lirmm.fr/api_response_page1.json` & `swh.lister-5.7.0/swh/lister/gitlab/tests/data/https_gite.lirmm.fr/api_response_page1.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/gitlab/tests/data/https_gite.lirmm.fr/api_response_page2.json` & `swh.lister-5.7.0/swh/lister/gitlab/tests/data/https_gite.lirmm.fr/api_response_page2.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/gitlab/tests/data/https_gite.lirmm.fr/api_response_page3.json` & `swh.lister-5.7.0/swh/lister/gitlab/tests/data/https_gite.lirmm.fr/api_response_page3.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/gitlab/tests/data/https_gitlab.com/api_response_page1.json` & `swh.lister-5.7.0/swh/lister/gitlab/tests/data/https_gitlab.com/api_response_page1.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/gitlab/tests/test_lister.py` & `swh.lister-5.7.0/swh/lister/gitlab/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/gitlab/tests/test_tasks.py` & `swh.lister-5.7.0/swh/lister/gitlab/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/gnu/lister.py` & `swh.lister-5.7.0/swh/lister/gnu/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/gnu/tasks.py` & `swh.lister-5.7.0/swh/lister/gnu/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/gnu/tests/data/https_ftp.gnu.org/tree.json.gz` & `swh.lister-5.7.0/swh/lister/gnu/tests/data/https_ftp.gnu.org/tree.json.gz`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/gnu/tests/data/tree.json` & `swh.lister-5.7.0/swh/lister/gnu/tests/data/tree.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/gnu/tests/data/tree.min.json` & `swh.lister-5.7.0/swh/lister/gnu/tests/data/tree.min.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/gnu/tests/test_lister.py` & `swh.lister-5.7.0/swh/lister/gnu/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/gnu/tests/test_tasks.py` & `swh.lister-5.7.0/swh/lister/gnu/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/gnu/tests/test_tree.py` & `swh.lister-5.7.0/swh/lister/gnu/tests/test_tree.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/gnu/tree.py` & `swh.lister-5.7.0/swh/lister/gnu/tree.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/gogs/lister.py` & `swh.lister-5.7.0/swh/lister/gogs/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/gogs/tasks.py` & `swh.lister-5.7.0/swh/lister/gogs/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/gogs/tests/data/https_try.gogs.io/repos_page1` & `swh.lister-5.7.0/swh/lister/gogs/tests/data/https_try.gogs.io/repos_page1`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/gogs/tests/data/https_try.gogs.io/repos_page2` & `swh.lister-5.7.0/swh/lister/gogs/tests/data/https_try.gogs.io/repos_page2`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/gogs/tests/data/https_try.gogs.io/repos_page3` & `swh.lister-5.7.0/swh/lister/gogs/tests/data/https_try.gogs.io/repos_page3`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/gogs/tests/data/https_try.gogs.io/repos_page4` & `swh.lister-5.7.0/swh/lister/gogs/tests/data/https_try.gogs.io/repos_page4`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/gogs/tests/test_lister.py` & `swh.lister-5.7.0/swh/lister/gogs/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/gogs/tests/test_tasks.py` & `swh.lister-5.7.0/swh/lister/gogs/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/golang/lister.py` & `swh.lister-5.7.0/swh/lister/golang/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/golang/tasks.py` & `swh.lister-5.7.0/swh/lister/golang/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/golang/tests/data/page-3.txt` & `swh.lister-5.7.0/swh/lister/golang/tests/data/page-3.txt`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/golang/tests/test_lister.py` & `swh.lister-5.7.0/swh/lister/golang/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/golang/tests/test_tasks.py` & `swh.lister-5.7.0/swh/lister/golang/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/hackage/__init__.py` & `swh.lister-5.7.0/swh/lister/hackage/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/hackage/lister.py` & `swh.lister-5.7.0/swh/lister/hackage/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/hackage/tasks.py` & `swh.lister-5.7.0/swh/lister/hackage/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/hackage/tests/data/https_fake49.haskell.org/packages_search_0` & `swh.lister-5.7.0/swh/lister/hackage/tests/data/https_fake49.haskell.org/packages_search_0`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/hackage/tests/data/https_fake51.haskell.org/packages_search_0` & `swh.lister-5.7.0/swh/lister/hackage/tests/data/https_fake51.haskell.org/packages_search_0`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/hackage/tests/data/https_fake51.haskell.org/packages_search_1` & `swh.lister-5.7.0/swh/lister/hackage/tests/data/https_fake51.haskell.org/packages_search_1`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/hackage/tests/data/https_hackage.haskell.org/packages_search_0` & `swh.lister-5.7.0/swh/lister/hackage/tests/data/https_hackage.haskell.org/packages_search_0`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/hackage/tests/data/https_hackage.haskell.org/packages_search_0_visit1` & `swh.lister-5.7.0/swh/lister/hackage/tests/data/https_hackage.haskell.org/packages_search_0_visit1`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/hackage/tests/data/https_hackage.haskell.org/packages_search_1` & `swh.lister-5.7.0/swh/lister/hackage/tests/data/https_hackage.haskell.org/packages_search_1`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/hackage/tests/data/https_hackage.haskell.org/packages_search_2` & `swh.lister-5.7.0/swh/lister/hackage/tests/data/https_hackage.haskell.org/packages_search_2`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/hackage/tests/test_lister.py` & `swh.lister-5.7.0/swh/lister/hackage/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/hackage/tests/test_tasks.py` & `swh.lister-5.7.0/swh/lister/hackage/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/hex/lister.py` & `swh.lister-5.7.0/swh/lister/hex/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/hex/tasks.py` & `swh.lister-5.7.0/swh/lister/hex/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/hex/tests/data/https_hex.pm/page1.json` & `swh.lister-5.7.0/swh/lister/hex/tests/data/https_hex.pm/page1.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/hex/tests/data/https_hex.pm/page2.json` & `swh.lister-5.7.0/swh/lister/hex/tests/data/https_hex.pm/page2.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/hex/tests/data/https_hex.pm/page3.json` & `swh.lister-5.7.0/swh/lister/hex/tests/data/https_hex.pm/page3.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/hex/tests/test_lister.py` & `swh.lister-5.7.0/swh/lister/hex/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/hex/tests/test_tasks.py` & `swh.lister-5.7.0/swh/lister/hex/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/launchpad/lister.py` & `swh.lister-5.7.0/swh/lister/launchpad/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/launchpad/tasks.py` & `swh.lister-5.7.0/swh/lister/launchpad/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/launchpad/tests/conftest.py` & `swh.lister-5.7.0/swh/lister/launchpad/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/launchpad/tests/data/launchpad_bzr_response.json` & `swh.lister-5.7.0/swh/lister/launchpad/tests/data/launchpad_bzr_response.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/launchpad/tests/data/launchpad_response1.json` & `swh.lister-5.7.0/swh/lister/launchpad/tests/data/launchpad_response1.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/launchpad/tests/data/launchpad_response2.json` & `swh.lister-5.7.0/swh/lister/launchpad/tests/data/launchpad_response2.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/launchpad/tests/test_lister.py` & `swh.lister-5.7.0/swh/lister/launchpad/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/launchpad/tests/test_tasks.py` & `swh.lister-5.7.0/swh/lister/launchpad/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/maven/README.md` & `swh.lister-5.7.0/swh/lister/maven/README.md`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/maven/lister.py` & `swh.lister-5.7.0/swh/lister/maven/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/maven/tasks.py` & `swh.lister-5.7.0/swh/lister/maven/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/maven/tests/data/citrus-parent-3.0.7.pom` & `swh.lister-5.7.0/swh/lister/maven/tests/data/citrus-parent-3.0.7.pom`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/maven/tests/data/http_indexes/export_full.fld` & `swh.lister-5.7.0/swh/lister/maven/tests/data/http_indexes/export_full.fld`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/maven/tests/data/http_indexes/export_incr_first.fld` & `swh.lister-5.7.0/swh/lister/maven/tests/data/http_indexes/export_incr_first.fld`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/maven/tests/data/https_api.github.com/repos_aldialimucaj_sprova4j` & `swh.lister-5.7.0/swh/lister/maven/tests/data/https_api.github.com/repos_aldialimucaj_sprova4j`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/maven/tests/data/https_api.github.com/repos_arangodb-community_arangodb-graphql-java` & `swh.lister-5.7.0/swh/lister/maven/tests/data/https_api.github.com/repos_arangodb-community_arangodb-graphql-java`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/maven/tests/data/https_api.github.com/repos_webx_citrus` & `swh.lister-5.7.0/swh/lister/maven/tests/data/https_api.github.com/repos_webx_citrus`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/maven/tests/data/https_repo1.maven.org/maven2_al_aldi_sprova4j_0.1.0_sprova4j-0.1.0.pom` & `swh.lister-5.7.0/swh/lister/maven/tests/data/https_repo1.maven.org/maven2_al_aldi_sprova4j_0.1.0_sprova4j-0.1.0.pom`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/maven/tests/data/https_repo1.maven.org/maven2_al_aldi_sprova4j_0.1.1_sprova4j-0.1.1.pom` & `swh.lister-5.7.0/swh/lister/maven/tests/data/https_repo1.maven.org/maven2_al_aldi_sprova4j_0.1.1_sprova4j-0.1.1.pom`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/maven/tests/data/https_repo1.maven.org/maven2_com_arangodb_arangodb-graphql_1.2_arangodb-graphql-1.2.pom` & `swh.lister-5.7.0/swh/lister/maven/tests/data/https_repo1.maven.org/maven2_com_arangodb_arangodb-graphql_1.2_arangodb-graphql-1.2.pom`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/maven/tests/data/sprova4j-0.1.0.invalidurl.pom` & `swh.lister-5.7.0/swh/lister/maven/tests/data/sprova4j-0.1.0.invalidurl.pom`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/maven/tests/data/sprova4j-0.1.0.malformed.pom` & `swh.lister-5.7.0/swh/lister/maven/tests/data/sprova4j-0.1.0.malformed.pom`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/maven/tests/test_lister.py` & `swh.lister-5.7.0/swh/lister/maven/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/maven/tests/test_tasks.py` & `swh.lister-5.7.0/swh/lister/maven/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/nixguix/__init__.py` & `swh.lister-5.7.0/swh/lister/nixguix/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/nixguix/lister.py` & `swh.lister-5.7.0/swh/lister/nixguix/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/nixguix/tasks.py` & `swh.lister-5.7.0/swh/lister/nixguix/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/nixguix/tests/data/sources-failure.json` & `swh.lister-5.7.0/swh/lister/nixguix/tests/data/sources-failure.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/nixguix/tests/data/sources-success.json` & `swh.lister-5.7.0/swh/lister/nixguix/tests/data/sources-success.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/nixguix/tests/test_lister.py` & `swh.lister-5.7.0/swh/lister/nixguix/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/nixguix/tests/test_tasks.py` & `swh.lister-5.7.0/swh/lister/nixguix/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/npm/__init__.py` & `swh.lister-5.7.0/swh/lister/npm/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/npm/lister.py` & `swh.lister-5.7.0/swh/lister/npm/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/npm/tasks.py` & `swh.lister-5.7.0/swh/lister/npm/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/npm/tests/data/npm_full_page1.json` & `swh.lister-5.7.0/swh/lister/npm/tests/data/npm_full_page1.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/npm/tests/data/npm_full_page2.json` & `swh.lister-5.7.0/swh/lister/npm/tests/data/npm_full_page2.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/npm/tests/data/npm_incremental_page1.json` & `swh.lister-5.7.0/swh/lister/npm/tests/data/npm_incremental_page1.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/npm/tests/data/npm_incremental_page2.json` & `swh.lister-5.7.0/swh/lister/npm/tests/data/npm_incremental_page2.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/npm/tests/test_lister.py` & `swh.lister-5.7.0/swh/lister/npm/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/npm/tests/test_tasks.py` & `swh.lister-5.7.0/swh/lister/npm/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/nuget/__init__.py` & `swh.lister-5.7.0/swh/lister/nuget/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/nuget/lister.py` & `swh.lister-5.7.0/swh/lister/nuget/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/nuget/tasks.py` & `swh.lister-5.7.0/swh/lister/nuget/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/nuget/tests/data/https_api.nuget.org/v3-flatcontainer_intersoft.crosslight.logging.entityframework_5.0.5000.1235-experimental_intersoft.crosslight.logging.entityframework.nuspec` & `swh.lister-5.7.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3-flatcontainer_intersoft.crosslight.logging.entityframework_5.0.5000.1235-experimental_intersoft.crosslight.logging.entityframework.nuspec`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/nuget/tests/data/https_api.nuget.org/v3-flatcontainer_moq.automock_3.5.0-ci0287_moq.automock.nuspec` & `swh.lister-5.7.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3-flatcontainer_moq.automock_3.5.0-ci0287_moq.automock.nuspec`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/nuget/tests/data/https_api.nuget.org/v3-flatcontainer_sil.core.desktop_10.0.1-beta0012_sil.core.desktop.nuspec` & `swh.lister-5.7.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3-flatcontainer_sil.core.desktop_10.0.1-beta0012_sil.core.desktop.nuspec`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_data_2022.09.23.08.07.54_sil.core.desktop.10.0.1-beta0012.json` & `swh.lister-5.7.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_data_2022.09.23.08.07.54_sil.core.desktop.10.0.1-beta0012.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_data_2022.09.23.09.10.26_intersoft.crosslight.logging.entityframework.5.0.5000.1235-experimental.json` & `swh.lister-5.7.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_data_2022.09.23.09.10.26_intersoft.crosslight.logging.entityframework.5.0.5000.1235-experimental.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_data_2022.10.10.04.04.00_moq.automock.3.5.0-ci0287.json` & `swh.lister-5.7.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_data_2022.10.10.04.04.00_moq.automock.3.5.0-ci0287.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_index.json` & `swh.lister-5.7.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_index.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_index.json_visit1` & `swh.lister-5.7.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_index.json_visit1`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_page11702.json` & `swh.lister-5.7.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_page11702.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_page16958.json` & `swh.lister-5.7.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_page16958.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_page17100.json` & `swh.lister-5.7.0/swh/lister/nuget/tests/data/https_api.nuget.org/v3_catalog0_page17100.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/nuget/tests/test_lister.py` & `swh.lister-5.7.0/swh/lister/nuget/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/nuget/tests/test_tasks.py` & `swh.lister-5.7.0/swh/lister/nuget/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/opam/lister.py` & `swh.lister-5.7.0/swh/lister/opam/lister.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,28 +2,42 @@
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import io
 import logging
 import os
+import shutil
 from subprocess import PIPE, Popen, call
 from typing import Any, Dict, Iterator, Optional
 
 from swh.lister.pattern import StatelessLister
 from swh.scheduler.interface import SchedulerInterface
 from swh.scheduler.model import ListedOrigin
 
 from ..pattern import CredentialsType
 
 logger = logging.getLogger(__name__)
 
 PageType = str
 
 
+def opam() -> str:
+    """Get the path to the opam executable.
+
+    Raises:
+      EnvironmentError if no opam executable is found
+    """
+    ret = shutil.which("opam")
+    if not ret:
+        raise EnvironmentError("No opam executable found in path {os.environ['PATH']}")
+
+    return ret
+
+
 class OpamLister(StatelessLister[PageType]):
     """
     List all repositories hosted on an opam repository.
 
     On initialisation, we create an opam root, with no ocaml compiler (no switch)
     as we won't need it and it's costly. In this opam root, we add a single opam
     repository (url) and give it a name (instance). Then, to get pages, we just ask
@@ -67,15 +81,15 @@
     def get_pages(self) -> Iterator[PageType]:
         # Initialize the opam root directory
         opam_init(self.opam_root, self.instance, self.url, self.env)
 
         # Actually list opam instance data
         proc = Popen(
             [
-                "opam",
+                opam(),
                 "list",
                 "--all",
                 "--no-switch",
                 "--safe",
                 "--repos",
                 self.instance,
                 "--root",
@@ -120,29 +134,29 @@
 
     Returns:
         None.
 
     """
     if not os.path.exists(opam_root) or not os.listdir(opam_root):
         command = [
-            "opam",
+            opam(),
             "init",
             "--reinit",
             "--bare",
             "--no-setup",
             "--root",
             opam_root,
             instance,
             url,
         ]
     else:
         # The repository exists and is populated, we just add another instance in the
         # repository. If it's already setup, it's a noop
         command = [
-            "opam",
+            opam(),
             "repository",
             "add",
             "--root",
             opam_root,
             instance,
             url,
         ]
```

### Comparing `swh.lister-5.6.3/swh/lister/opam/tasks.py` & `swh.lister-5.7.0/swh/lister/opam/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/opam/tests/data/fake_opam_repo/packages/agrid/agrid.0.1/opam` & `swh.lister-5.7.0/swh/lister/opam/tests/data/fake_opam_repo/packages/agrid/agrid.0.1/opam`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.1/opam` & `swh.lister-5.7.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.1/opam`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.2/opam` & `swh.lister-5.7.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.2/opam`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.3/opam` & `swh.lister-5.7.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.3/opam`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.4/opam` & `swh.lister-5.7.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.4/opam`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.5/opam` & `swh.lister-5.7.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.5/opam`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.6/opam` & `swh.lister-5.7.0/swh/lister/opam/tests/data/fake_opam_repo/packages/calculon/calculon.0.6/opam`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/opam/tests/data/fake_opam_repo/packages/directories/directories.0.1/opam` & `swh.lister-5.7.0/swh/lister/opam/tests/data/fake_opam_repo/packages/directories/directories.0.1/opam`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/opam/tests/data/fake_opam_repo/packages/directories/directories.0.2/opam` & `swh.lister-5.7.0/swh/lister/opam/tests/data/fake_opam_repo/packages/directories/directories.0.2/opam`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/opam/tests/data/fake_opam_repo/packages/directories/directories.0.3/opam` & `swh.lister-5.7.0/swh/lister/opam/tests/data/fake_opam_repo/packages/directories/directories.0.3/opam`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/opam/tests/data/fake_opam_repo/packages/ocb/ocb.0.1/opam` & `swh.lister-5.7.0/swh/lister/opam/tests/data/fake_opam_repo/packages/ocb/ocb.0.1/opam`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/opam/tests/test_lister.py` & `swh.lister-5.7.0/swh/lister/opam/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/opam/tests/test_tasks.py` & `swh.lister-5.7.0/swh/lister/opam/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/packagist/lister.py` & `swh.lister-5.7.0/swh/lister/packagist/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/packagist/tasks.py` & `swh.lister-5.7.0/swh/lister/packagist/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/packagist/tests/data/den1n_contextmenu.json` & `swh.lister-5.7.0/swh/lister/packagist/tests/data/den1n_contextmenu.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/packagist/tests/data/https_api.github.com/repos_spryker-eco_computop-api` & `swh.lister-5.7.0/swh/lister/packagist/tests/data/https_api.github.com/repos_spryker-eco_computop-api`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/packagist/tests/data/https_api.github.com/repos_ycms_module-main` & `swh.lister-5.7.0/swh/lister/packagist/tests/data/https_api.github.com/repos_ycms_module-main`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/packagist/tests/data/idevlab_essential.json` & `swh.lister-5.7.0/swh/lister/packagist/tests/data/idevlab_essential.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/packagist/tests/data/ljjackson_linnworks.json` & `swh.lister-5.7.0/swh/lister/packagist/tests/data/ljjackson_linnworks.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/packagist/tests/data/lky_wx_article.json` & `swh.lister-5.7.0/swh/lister/packagist/tests/data/lky_wx_article.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/packagist/tests/data/payrix_payrix-php.json` & `swh.lister-5.7.0/swh/lister/packagist/tests/data/payrix_payrix-php.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/packagist/tests/data/spryker-eco_computop-api.json` & `swh.lister-5.7.0/swh/lister/packagist/tests/data/spryker-eco_computop-api.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/packagist/tests/data/with_invalid_url.json` & `swh.lister-5.7.0/swh/lister/packagist/tests/data/with_invalid_url.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/packagist/tests/data/ycms_module-main.json` & `swh.lister-5.7.0/swh/lister/packagist/tests/data/ycms_module-main.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/packagist/tests/test_lister.py` & `swh.lister-5.7.0/swh/lister/packagist/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/packagist/tests/test_tasks.py` & `swh.lister-5.7.0/swh/lister/packagist/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/pattern.py` & `swh.lister-5.7.0/swh/lister/pattern.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/phabricator/lister.py` & `swh.lister-5.7.0/swh/lister/phabricator/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/phabricator/tasks.py` & `swh.lister-5.7.0/swh/lister/phabricator/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/phabricator/tests/data/phabricator_api_repositories_page1.json` & `swh.lister-5.7.0/swh/lister/phabricator/tests/data/phabricator_api_repositories_page1.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/phabricator/tests/data/phabricator_api_repositories_page2.json` & `swh.lister-5.7.0/swh/lister/phabricator/tests/data/phabricator_api_repositories_page2.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/phabricator/tests/test_lister.py` & `swh.lister-5.7.0/swh/lister/phabricator/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/phabricator/tests/test_tasks.py` & `swh.lister-5.7.0/swh/lister/phabricator/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/pubdev/__init__.py` & `swh.lister-5.7.0/swh/lister/pubdev/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/pubdev/lister.py` & `swh.lister-5.7.0/swh/lister/pubdev/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/pubdev/tasks.py` & `swh.lister-5.7.0/swh/lister/pubdev/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/pubdev/tests/data/https_pub.dev/api_packages_Autolinker` & `swh.lister-5.7.0/swh/lister/pubdev/tests/data/https_pub.dev/api_packages_Autolinker`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/pubdev/tests/data/https_pub.dev/api_packages_Babylon` & `swh.lister-5.7.0/swh/lister/pubdev/tests/data/https_pub.dev/api_packages_Babylon`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/pubdev/tests/test_lister.py` & `swh.lister-5.7.0/swh/lister/pubdev/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/pubdev/tests/test_tasks.py` & `swh.lister-5.7.0/swh/lister/pubdev/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/puppet/__init__.py` & `swh.lister-5.7.0/swh/lister/puppet/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/puppet/lister.py` & `swh.lister-5.7.0/swh/lister/puppet/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/puppet/tasks.py` & `swh.lister-5.7.0/swh/lister/puppet/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/puppet/tests/data/https_forgeapi.puppet.com/v3_modules,limit=100` & `swh.lister-5.7.0/swh/lister/puppet/tests/data/https_forgeapi.puppet.com/v3_modules,limit=100`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/puppet/tests/data/https_forgeapi.puppet.com/v3_modules,limit=100,offset=100` & `swh.lister-5.7.0/swh/lister/puppet/tests/data/https_forgeapi.puppet.com/v3_modules,limit=100,offset=100`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/puppet/tests/data/https_forgeapi.puppet.com/v3_modules,limit=100,with_release_since=2022-09-26` & `swh.lister-5.7.0/swh/lister/puppet/tests/data/https_forgeapi.puppet.com/v3_modules,limit=100,with_release_since=2022-09-26`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/puppet/tests/test_lister.py` & `swh.lister-5.7.0/swh/lister/puppet/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/puppet/tests/test_tasks.py` & `swh.lister-5.7.0/swh/lister/puppet/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/pypi/lister.py` & `swh.lister-5.7.0/swh/lister/pypi/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/pypi/tests/test_lister.py` & `swh.lister-5.7.0/swh/lister/pypi/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/pypi/tests/test_tasks.py` & `swh.lister-5.7.0/swh/lister/pypi/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/rubygems/__init__.py` & `swh.lister-5.7.0/swh/lister/rubygems/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/rubygems/lister.py` & `swh.lister-5.7.0/swh/lister/rubygems/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/rubygems/tasks.py` & `swh.lister-5.7.0/swh/lister/rubygems/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/rubygems/tests/data/rubygems_dumps.xml` & `swh.lister-5.7.0/swh/lister/rubygems/tests/data/rubygems_dumps.xml`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/rubygems/tests/data/rubygems_pgsql_dump.tar` & `swh.lister-5.7.0/swh/lister/rubygems/tests/data/rubygems_pgsql_dump.tar`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/rubygems/tests/data/small_rubygems_dump.sh` & `swh.lister-5.7.0/swh/lister/rubygems/tests/data/small_rubygems_dump.sh`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/rubygems/tests/test_lister.py` & `swh.lister-5.7.0/swh/lister/rubygems/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/rubygems/tests/test_tasks.py` & `swh.lister-5.7.0/swh/lister/rubygems/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/sourceforge/lister.py` & `swh.lister-5.7.0/swh/lister/sourceforge/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/sourceforge/tasks.py` & `swh.lister-5.7.0/swh/lister/sourceforge/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/sourceforge/tests/data/aaron.html` & `swh.lister-5.7.0/swh/lister/sourceforge/tests/data/aaron.html`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/sourceforge/tests/data/aaron.json` & `swh.lister-5.7.0/swh/lister/sourceforge/tests/data/aaron.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/sourceforge/tests/data/adobexmp.json` & `swh.lister-5.7.0/swh/lister/sourceforge/tests/data/adobexmp.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/sourceforge/tests/data/backapps-website.json` & `swh.lister-5.7.0/swh/lister/sourceforge/tests/data/backapps-website.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/sourceforge/tests/data/backapps.json` & `swh.lister-5.7.0/swh/lister/sourceforge/tests/data/backapps.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/sourceforge/tests/data/mojunk.json` & `swh.lister-5.7.0/swh/lister/sourceforge/tests/data/mojunk.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/sourceforge/tests/data/mramm.json` & `swh.lister-5.7.0/swh/lister/sourceforge/tests/data/mramm.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/sourceforge/tests/data/ocaml-lpd.html` & `swh.lister-5.7.0/swh/lister/sourceforge/tests/data/ocaml-lpd.html`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/sourceforge/tests/data/ocaml-lpd.json` & `swh.lister-5.7.0/swh/lister/sourceforge/tests/data/ocaml-lpd.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/sourceforge/tests/data/os3dmodels.json` & `swh.lister-5.7.0/swh/lister/sourceforge/tests/data/os3dmodels.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/sourceforge/tests/data/random-mercurial.json` & `swh.lister-5.7.0/swh/lister/sourceforge/tests/data/random-mercurial.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/sourceforge/tests/data/subsitemap-0.xml` & `swh.lister-5.7.0/swh/lister/sourceforge/tests/data/subsitemap-0.xml`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/sourceforge/tests/data/subsitemap-1.xml` & `swh.lister-5.7.0/swh/lister/sourceforge/tests/data/subsitemap-1.xml`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/sourceforge/tests/data/t12eksandbox.html` & `swh.lister-5.7.0/swh/lister/sourceforge/tests/data/t12eksandbox.html`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/sourceforge/tests/data/t12eksandbox.json` & `swh.lister-5.7.0/swh/lister/sourceforge/tests/data/t12eksandbox.json`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/sourceforge/tests/test_lister.py` & `swh.lister-5.7.0/swh/lister/sourceforge/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/sourceforge/tests/test_tasks.py` & `swh.lister-5.7.0/swh/lister/sourceforge/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/tests/test_cli.py` & `swh.lister-5.7.0/swh/lister/tests/test_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     "nixguix": {
         "url": "https://guix.gnu.org/sources.json",
         "origin_upstream": "https://git.savannah.gnu.org/cgit/guix.git/",
     },
     "fedora": {
         "url": "https://archives.fedoraproject.org/pub/archive/fedora/linux/releases/",
     },
+    "pagure": {"instance": "pagure.io"},
 }
 
 
 def test_get_lister_wrong_input():
     """Unsupported lister should raise"""
     with pytest.raises(ValueError) as e:
         get_lister("unknown", "db-url")
```

### Comparing `swh.lister-5.6.3/swh/lister/tests/test_pattern.py` & `swh.lister-5.7.0/swh/lister/tests/test_pattern.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/tests/test_utils.py` & `swh.lister-5.7.0/swh/lister/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/tuleap/lister.py` & `swh.lister-5.7.0/swh/lister/tuleap/lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/tuleap/tasks.py` & `swh.lister-5.7.0/swh/lister/tuleap/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/tuleap/tests/data/https_tuleap.net/projects` & `swh.lister-5.7.0/swh/lister/tuleap/tests/data/https_tuleap.net/projects`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/tuleap/tests/test_lister.py` & `swh.lister-5.7.0/swh/lister/tuleap/tests/test_lister.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/tuleap/tests/test_tasks.py` & `swh.lister-5.7.0/swh/lister/tuleap/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh/lister/utils.py` & `swh.lister-5.7.0/swh/lister/utils.py`

 * *Files identical despite different names*

### Comparing `swh.lister-5.6.3/swh.lister.egg-info/PKG-INFO` & `swh.lister-5.7.0/swh.lister.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.lister
-Version: 5.6.3
+Version: 5.7.0
 Summary: Software Heritage lister
 Home-page: https://forge.softwareheritage.org/diffusion/DLSGH/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-lister
```

### Comparing `swh.lister-5.6.3/swh.lister.egg-info/SOURCES.txt` & `swh.lister-5.7.0/swh.lister.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -365,14 +365,22 @@
 swh/lister/packagist/tests/data/payrix_payrix-php.json
 swh/lister/packagist/tests/data/spryker-eco_computop-api.json
 swh/lister/packagist/tests/data/with_invalid_url.json
 swh/lister/packagist/tests/data/ycms_module-main.json
 swh/lister/packagist/tests/data/https_api.github.com/repos_gitlky_wx_article
 swh/lister/packagist/tests/data/https_api.github.com/repos_spryker-eco_computop-api
 swh/lister/packagist/tests/data/https_api.github.com/repos_ycms_module-main
+swh/lister/pagure/__init__.py
+swh/lister/pagure/lister.py
+swh/lister/pagure/tasks.py
+swh/lister/pagure/tests/__init__.py
+swh/lister/pagure/tests/test_lister.py
+swh/lister/pagure/tests/test_tasks.py
+swh/lister/pagure/tests/data/https_pagure.io/api_0_projects,per_page=2
+swh/lister/pagure/tests/data/https_pagure.io/api_0_projects,per_page=2,page=2
 swh/lister/phabricator/__init__.py
 swh/lister/phabricator/lister.py
 swh/lister/phabricator/tasks.py
 swh/lister/phabricator/tests/__init__.py
 swh/lister/phabricator/tests/test_lister.py
 swh/lister/phabricator/tests/test_tasks.py
 swh/lister/phabricator/tests/data/__init__.py
```

### Comparing `swh.lister-5.6.3/swh.lister.egg-info/entry_points.txt` & `swh.lister-5.7.0/swh.lister.egg-info/entry_points.txt`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 lister.launchpad = swh.lister.launchpad:register
 lister.maven = swh.lister.maven:register
 lister.nixguix = swh.lister.nixguix:register
 lister.npm = swh.lister.npm:register
 lister.nuget = swh.lister.nuget:register
 lister.opam = swh.lister.opam:register
 lister.packagist = swh.lister.packagist:register
+lister.pagure = swh.lister.pagure:register
 lister.phabricator = swh.lister.phabricator:register
 lister.pubdev = swh.lister.pubdev:register
 lister.puppet = swh.lister.puppet:register
 lister.pypi = swh.lister.pypi:register
 lister.rubygems = swh.lister.rubygems:register
 lister.sourceforge = swh.lister.sourceforge:register
 lister.tuleap = swh.lister.tuleap:register
```

### Comparing `swh.lister-5.6.3/tox.ini` & `swh.lister-5.7.0/tox.ini`

 * *Files identical despite different names*


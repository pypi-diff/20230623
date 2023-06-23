# Comparing `tmp/snakecdysis-0.0.4.tar.gz` & `tmp/snakecdysis-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakecdysis-0.0.4.tar", last modified: Mon Feb 27 10:10:48 2023, max compression
+gzip compressed data, was "snakecdysis-0.0.5.tar", last modified: Thu Jun 22 09:08:16 2023, max compression
```

## Comparing `snakecdysis-0.0.4.tar` & `snakecdysis-0.0.5.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxrwxr-x   0 sravel   (100301) sravel   (100301)        0 2023-02-27 10:10:48.000000 snakecdysis-0.0.4/
--rw-rw-r--   0 sravel   (100301) sravel   (100301)     3167 2023-02-23 13:52:58.000000 snakecdysis-0.0.4/.gitignore
--rw-rw-r--   0 sravel   (100301) sravel   (100301)      507 2023-02-23 13:52:58.000000 snakecdysis-0.0.4/.readthedocs.yml
--rw-rw-r--   0 sravel   (100301) sravel   (100301)     1070 2023-02-23 13:52:59.000000 snakecdysis-0.0.4/LICENSE
--rw-rw-r--   0 sravel   (100301) sravel   (100301)     4319 2023-02-27 10:10:48.000000 snakecdysis-0.0.4/PKG-INFO
--rw-rw-r--   0 sravel   (100301) sravel   (100301)     1569 2023-02-23 14:17:43.000000 snakecdysis-0.0.4/README.rst
-drwxrwxr-x   0 sravel   (100301) sravel   (100301)        0 2023-02-27 10:10:48.000000 snakecdysis-0.0.4/docs/
--rw-rw-r--   0 sravel   (100301) sravel   (100301)      655 2023-02-23 13:52:59.000000 snakecdysis-0.0.4/docs/Makefile
--rw-rw-r--   0 sravel   (100301) sravel   (100301)      258 2023-02-23 14:10:07.000000 snakecdysis-0.0.4/docs/requirements.txt
-drwxrwxr-x   0 sravel   (100301) sravel   (100301)        0 2023-02-27 10:10:48.000000 snakecdysis-0.0.4/docs/source/
-drwxrwxr-x   0 sravel   (100301) sravel   (100301)        0 2023-02-27 10:10:48.000000 snakecdysis-0.0.4/docs/source/_images/
--rw-rw-r--   0 sravel   (100301) sravel   (100301)    33751 2023-02-23 13:52:59.000000 snakecdysis-0.0.4/docs/source/_images/directory.png
--rw-rw-r--   0 sravel   (100301) sravel   (100301)   285846 2023-02-23 13:52:59.000000 snakecdysis-0.0.4/docs/source/_images/snakecdysis_logo.png
--rw-rw-r--   0 sravel   (100301) sravel   (100301)   212350 2023-02-23 13:52:59.000000 snakecdysis-0.0.4/docs/source/_images/snakecdysis_logo_short.png
-drwxrwxr-x   0 sravel   (100301) sravel   (100301)        0 2023-02-27 10:10:48.000000 snakecdysis-0.0.4/docs/source/_static/
--rw-rw-r--   0 sravel   (100301) sravel   (100301)      741 2023-02-23 13:52:59.000000 snakecdysis-0.0.4/docs/source/_static/logo.css
--rw-rw-r--   0 sravel   (100301) sravel   (100301)     5645 2023-02-24 08:23:11.000000 snakecdysis-0.0.4/docs/source/conf.py
--rw-rw-r--   0 sravel   (100301) sravel   (100301)      739 2023-02-23 13:52:59.000000 snakecdysis-0.0.4/docs/source/index.rst
--rw-rw-r--   0 sravel   (100301) sravel   (100301)      839 2023-02-23 13:52:59.000000 snakecdysis-0.0.4/docs/source/install.rst
--rw-rw-r--   0 sravel   (100301) sravel   (100301)     3222 2023-02-23 13:53:00.000000 snakecdysis-0.0.4/docs/source/package.rst
--rw-rw-r--   0 sravel   (100301) sravel   (100301)      342 2023-02-23 13:53:00.000000 snakecdysis-0.0.4/docs/source/snakecdysis.rst
--rw-rw-r--   0 sravel   (100301) sravel   (100301)      170 2023-02-23 13:53:00.000000 snakecdysis-0.0.4/docs/source/usefulfunctions.rst
--rw-rw-r--   0 sravel   (100301) sravel   (100301)      471 2023-02-23 13:53:00.000000 snakecdysis-0.0.4/docs/source/workflow.rst
--rw-rw-r--   0 sravel   (100301) sravel   (100301)     2427 2023-02-27 10:09:25.000000 snakecdysis-0.0.4/pyproject.toml
--rw-rw-r--   0 sravel   (100301) sravel   (100301)       38 2023-02-27 10:10:48.000000 snakecdysis-0.0.4/setup.cfg
-drwxrwxr-x   0 sravel   (100301) sravel   (100301)        0 2023-02-27 10:10:48.000000 snakecdysis-0.0.4/snakecdysis/
--rw-rw-r--   0 sravel   (100301) sravel   (100301)   285846 2023-02-23 13:53:00.000000 snakecdysis-0.0.4/snakecdysis/Snakecdysis_logo.png
--rw-rw-r--   0 sravel   (100301) sravel   (100301)        6 2023-02-27 10:09:45.000000 snakecdysis-0.0.4/snakecdysis/VERSION
--rw-rw-r--   0 sravel   (100301) sravel   (100301)      466 2023-02-23 13:57:01.000000 snakecdysis-0.0.4/snakecdysis/__init__.py
--rw-rw-r--   0 sravel   (100301) sravel   (100301)     1396 2023-02-23 13:53:00.000000 snakecdysis-0.0.4/snakecdysis/__main__.py
--rw-rw-r--   0 sravel   (100301) sravel   (100301)      160 2023-02-27 10:10:48.000000 snakecdysis-0.0.4/snakecdysis/_version.py
--rw-rw-r--   0 sravel   (100301) sravel   (100301)    12989 2023-02-27 10:09:51.000000 snakecdysis-0.0.4/snakecdysis/cli_wrapper.py
--rw-rw-r--   0 sravel   (100301) sravel   (100301)     2207 2023-02-23 13:53:00.000000 snakecdysis-0.0.4/snakecdysis/edit_files.py
--rw-rw-r--   0 sravel   (100301) sravel   (100301)      280 2023-02-23 13:53:00.000000 snakecdysis-0.0.4/snakecdysis/global_variable.py
--rw-rw-r--   0 sravel   (100301) sravel   (100301)     8241 2023-02-27 10:09:51.000000 snakecdysis-0.0.4/snakecdysis/install.py
--rw-rw-r--   0 sravel   (100301) sravel   (100301)     5255 2023-02-23 13:53:00.000000 snakecdysis-0.0.4/snakecdysis/run.py
-drwxrwxr-x   0 sravel   (100301) sravel   (100301)        0 2023-02-27 10:10:48.000000 snakecdysis-0.0.4/snakecdysis/scripts/
--rw-rw-r--   0 sravel   (100301) sravel   (100301)     1321 2023-02-23 13:53:01.000000 snakecdysis-0.0.4/snakecdysis/scripts/generate_template.py
--rw-rw-r--   0 sravel   (100301) sravel   (100301)    25376 2023-02-27 10:09:51.000000 snakecdysis-0.0.4/snakecdysis/snake_wrapper.py
-drwxrwxr-x   0 sravel   (100301) sravel   (100301)        0 2023-02-27 10:10:48.000000 snakecdysis-0.0.4/snakecdysis/templates/
-drwxrwxr-x   0 sravel   (100301) sravel   (100301)        0 2023-02-27 10:10:48.000000 snakecdysis-0.0.4/snakecdysis/templates/PKGNAME/
--rw-rw-r--   0 sravel   (100301) sravel   (100301)        6 2023-02-23 13:53:01.000000 snakecdysis-0.0.4/snakecdysis/templates/PKGNAME/VERSION
--rw-rw-r--   0 sravel   (100301) sravel   (100301)      963 2023-02-23 13:53:01.000000 snakecdysis-0.0.4/snakecdysis/templates/PKGNAME/__init__.py
--rw-rw-r--   0 sravel   (100301) sravel   (100301)      710 2023-02-23 13:53:01.000000 snakecdysis-0.0.4/snakecdysis/templates/PKGNAME/global_variables.py
-drwxrwxr-x   0 sravel   (100301) sravel   (100301)        0 2023-02-27 10:10:48.000000 snakecdysis-0.0.4/snakecdysis/templates/PKGNAME/install_files/
--rwxrwxr-x   0 sravel   (100301) sravel   (100301)      183 2023-02-23 13:53:01.000000 snakecdysis-0.0.4/snakecdysis/templates/PKGNAME/install_files/cluster_config_SLURM.yaml
--rw-rw-r--   0 sravel   (100301) sravel   (100301)      147 2023-02-23 13:53:01.000000 snakecdysis-0.0.4/snakecdysis/templates/PKGNAME/install_files/config.yaml
--rw-rw-r--   0 sravel   (100301) sravel   (100301)      612 2023-02-23 13:53:01.000000 snakecdysis-0.0.4/snakecdysis/templates/PKGNAME/install_files/tools_path.yaml
--rwxrwxr-x   0 sravel   (100301) sravel   (100301)      164 2023-02-23 13:53:01.000000 snakecdysis-0.0.4/snakecdysis/templates/PKGNAME/main.py
--rwxrwxr-x   0 sravel   (100301) sravel   (100301)      602 2023-02-23 13:53:01.000000 snakecdysis-0.0.4/snakecdysis/templates/PKGNAME/module.py
-drwxrwxr-x   0 sravel   (100301) sravel   (100301)        0 2023-02-27 10:10:48.000000 snakecdysis-0.0.4/snakecdysis/templates/PKGNAME/snakefiles/
--rw-rw-r--   0 sravel   (100301) sravel   (100301)     3030 2023-02-23 13:53:01.000000 snakecdysis-0.0.4/snakecdysis/templates/PKGNAME/snakefiles/snakefile
--rw-rw-r--   0 sravel   (100301) sravel   (100301)     1871 2023-02-23 13:53:01.000000 snakecdysis-0.0.4/snakecdysis/templates/pyproject.toml
--rw-rw-r--   0 sravel   (100301) sravel   (100301)     5326 2023-02-23 13:53:01.000000 snakecdysis-0.0.4/snakecdysis/useful_function.py
-drwxrwxr-x   0 sravel   (100301) sravel   (100301)        0 2023-02-27 10:10:48.000000 snakecdysis-0.0.4/snakecdysis.egg-info/
--rw-rw-r--   0 sravel   (100301) sravel   (100301)     4319 2023-02-27 10:10:48.000000 snakecdysis-0.0.4/snakecdysis.egg-info/PKG-INFO
--rw-rw-r--   0 sravel   (100301) sravel   (100301)     1469 2023-02-27 10:10:48.000000 snakecdysis-0.0.4/snakecdysis.egg-info/SOURCES.txt
--rw-rw-r--   0 sravel   (100301) sravel   (100301)        1 2023-02-27 10:10:48.000000 snakecdysis-0.0.4/snakecdysis.egg-info/dependency_links.txt
--rw-rw-r--   0 sravel   (100301) sravel   (100301)      119 2023-02-27 10:10:48.000000 snakecdysis-0.0.4/snakecdysis.egg-info/entry_points.txt
--rw-rw-r--   0 sravel   (100301) sravel   (100301)      130 2023-02-27 10:10:48.000000 snakecdysis-0.0.4/snakecdysis.egg-info/requires.txt
--rw-rw-r--   0 sravel   (100301) sravel   (100301)       12 2023-02-27 10:10:48.000000 snakecdysis-0.0.4/snakecdysis.egg-info/top_level.txt
+drwxrwxr-x   0 sravel   (100301) sravel   (100301)        0 2023-06-22 09:08:16.000000 snakecdysis-0.0.5/
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)     3167 2023-02-23 13:52:58.000000 snakecdysis-0.0.5/.gitignore
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)      507 2023-02-23 13:52:58.000000 snakecdysis-0.0.5/.readthedocs.yml
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)    10414 2023-06-22 08:37:07.000000 snakecdysis-0.0.5/CHANGELOG.md
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)     1070 2023-02-23 13:52:59.000000 snakecdysis-0.0.5/LICENSE
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)     4319 2023-06-22 09:08:16.000000 snakecdysis-0.0.5/PKG-INFO
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)     1569 2023-02-23 14:17:43.000000 snakecdysis-0.0.5/README.rst
+drwxrwxr-x   0 sravel   (100301) sravel   (100301)        0 2023-06-22 09:08:16.000000 snakecdysis-0.0.5/docs/
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)      655 2023-02-23 13:52:59.000000 snakecdysis-0.0.5/docs/Makefile
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)      258 2023-02-23 14:10:07.000000 snakecdysis-0.0.5/docs/requirements.txt
+drwxrwxr-x   0 sravel   (100301) sravel   (100301)        0 2023-06-22 09:08:16.000000 snakecdysis-0.0.5/docs/source/
+drwxrwxr-x   0 sravel   (100301) sravel   (100301)        0 2023-06-22 09:08:16.000000 snakecdysis-0.0.5/docs/source/_images/
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)    33751 2023-02-23 13:52:59.000000 snakecdysis-0.0.5/docs/source/_images/directory.png
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)   285846 2023-02-23 13:52:59.000000 snakecdysis-0.0.5/docs/source/_images/snakecdysis_logo.png
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)   212350 2023-02-23 13:52:59.000000 snakecdysis-0.0.5/docs/source/_images/snakecdysis_logo_short.png
+drwxrwxr-x   0 sravel   (100301) sravel   (100301)        0 2023-06-22 09:08:16.000000 snakecdysis-0.0.5/docs/source/_static/
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)      741 2023-02-23 13:52:59.000000 snakecdysis-0.0.5/docs/source/_static/logo.css
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)     5645 2023-02-24 08:23:11.000000 snakecdysis-0.0.5/docs/source/conf.py
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)      739 2023-02-23 13:52:59.000000 snakecdysis-0.0.5/docs/source/index.rst
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)      839 2023-02-23 13:52:59.000000 snakecdysis-0.0.5/docs/source/install.rst
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)     3222 2023-02-23 13:53:00.000000 snakecdysis-0.0.5/docs/source/package.rst
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)      342 2023-02-23 13:53:00.000000 snakecdysis-0.0.5/docs/source/snakecdysis.rst
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)      170 2023-02-23 13:53:00.000000 snakecdysis-0.0.5/docs/source/usefulfunctions.rst
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)      471 2023-02-23 13:53:00.000000 snakecdysis-0.0.5/docs/source/workflow.rst
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)     2427 2023-02-27 10:09:25.000000 snakecdysis-0.0.5/pyproject.toml
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)       38 2023-06-22 09:08:16.000000 snakecdysis-0.0.5/setup.cfg
+drwxrwxr-x   0 sravel   (100301) sravel   (100301)        0 2023-06-22 09:08:16.000000 snakecdysis-0.0.5/snakecdysis/
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)   285846 2023-02-23 13:53:00.000000 snakecdysis-0.0.5/snakecdysis/Snakecdysis_logo.png
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)        6 2023-06-22 09:03:55.000000 snakecdysis-0.0.5/snakecdysis/VERSION
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)      466 2023-02-23 13:57:01.000000 snakecdysis-0.0.5/snakecdysis/__init__.py
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)     1396 2023-02-23 13:53:00.000000 snakecdysis-0.0.5/snakecdysis/__main__.py
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)      160 2023-06-22 09:08:16.000000 snakecdysis-0.0.5/snakecdysis/_version.py
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)    12989 2023-06-14 12:45:17.000000 snakecdysis-0.0.5/snakecdysis/cli_wrapper.py
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)     2207 2023-02-23 13:53:00.000000 snakecdysis-0.0.5/snakecdysis/edit_files.py
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)      280 2023-02-23 13:53:00.000000 snakecdysis-0.0.5/snakecdysis/global_variable.py
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)     8608 2023-06-16 09:06:05.000000 snakecdysis-0.0.5/snakecdysis/install.py
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)     5259 2023-06-21 13:37:22.000000 snakecdysis-0.0.5/snakecdysis/run.py
+drwxrwxr-x   0 sravel   (100301) sravel   (100301)        0 2023-06-22 09:08:16.000000 snakecdysis-0.0.5/snakecdysis/scripts/
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)     1601 2023-06-21 11:25:10.000000 snakecdysis-0.0.5/snakecdysis/scripts/generate_template.py
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)    25216 2023-06-21 12:59:41.000000 snakecdysis-0.0.5/snakecdysis/snake_wrapper.py
+drwxrwxr-x   0 sravel   (100301) sravel   (100301)        0 2023-06-22 09:08:16.000000 snakecdysis-0.0.5/snakecdysis/templates/
+drwxrwxr-x   0 sravel   (100301) sravel   (100301)        0 2023-06-22 09:08:16.000000 snakecdysis-0.0.5/snakecdysis/templates/PKGNAME/
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)        6 2023-02-23 13:53:01.000000 snakecdysis-0.0.5/snakecdysis/templates/PKGNAME/VERSION
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)      963 2023-02-23 13:53:01.000000 snakecdysis-0.0.5/snakecdysis/templates/PKGNAME/__init__.py
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)      710 2023-02-23 13:53:01.000000 snakecdysis-0.0.5/snakecdysis/templates/PKGNAME/global_variables.py
+drwxrwxr-x   0 sravel   (100301) sravel   (100301)        0 2023-06-22 09:08:16.000000 snakecdysis-0.0.5/snakecdysis/templates/PKGNAME/install_files/
+-rwxrwxr-x   0 sravel   (100301) sravel   (100301)      183 2023-02-23 13:53:01.000000 snakecdysis-0.0.5/snakecdysis/templates/PKGNAME/install_files/cluster_config_SLURM.yaml
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)      147 2023-02-23 13:53:01.000000 snakecdysis-0.0.5/snakecdysis/templates/PKGNAME/install_files/config.yaml
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)      612 2023-02-23 13:53:01.000000 snakecdysis-0.0.5/snakecdysis/templates/PKGNAME/install_files/tools_path.yaml
+-rwxrwxr-x   0 sravel   (100301) sravel   (100301)      164 2023-02-23 13:53:01.000000 snakecdysis-0.0.5/snakecdysis/templates/PKGNAME/main.py
+-rwxrwxr-x   0 sravel   (100301) sravel   (100301)      602 2023-02-23 13:53:01.000000 snakecdysis-0.0.5/snakecdysis/templates/PKGNAME/module.py
+drwxrwxr-x   0 sravel   (100301) sravel   (100301)        0 2023-06-22 09:08:16.000000 snakecdysis-0.0.5/snakecdysis/templates/PKGNAME/snakefiles/
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)     3030 2023-02-23 13:53:01.000000 snakecdysis-0.0.5/snakecdysis/templates/PKGNAME/snakefiles/snakefile
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)     1871 2023-02-23 13:53:01.000000 snakecdysis-0.0.5/snakecdysis/templates/pyproject.toml
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)     5326 2023-02-23 13:53:01.000000 snakecdysis-0.0.5/snakecdysis/useful_function.py
+drwxrwxr-x   0 sravel   (100301) sravel   (100301)        0 2023-06-22 09:08:16.000000 snakecdysis-0.0.5/snakecdysis.egg-info/
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)     4319 2023-06-22 09:08:16.000000 snakecdysis-0.0.5/snakecdysis.egg-info/PKG-INFO
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)     1482 2023-06-22 09:08:16.000000 snakecdysis-0.0.5/snakecdysis.egg-info/SOURCES.txt
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)        1 2023-06-22 09:08:16.000000 snakecdysis-0.0.5/snakecdysis.egg-info/dependency_links.txt
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)      119 2023-06-22 09:08:16.000000 snakecdysis-0.0.5/snakecdysis.egg-info/entry_points.txt
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)      130 2023-06-22 09:08:16.000000 snakecdysis-0.0.5/snakecdysis.egg-info/requires.txt
+-rw-rw-r--   0 sravel   (100301) sravel   (100301)       12 2023-06-22 09:08:16.000000 snakecdysis-0.0.5/snakecdysis.egg-info/top_level.txt
```

### Comparing `snakecdysis-0.0.4/.gitignore` & `snakecdysis-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `snakecdysis-0.0.4/LICENSE` & `snakecdysis-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `snakecdysis-0.0.4/PKG-INFO` & `snakecdysis-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snakecdysis
-Version: 0.0.4
+Version: 0.0.5
 Summary: You want to wrap your best snakemake workflow to be easy install and run, Snakecdysis is for you !!!!! Tha aim of Snakecdysis is to easy-wrapped snakemake workflow as python package and then build sub-commands to manage this. !!!!!
 Author-email: "Ravel Sebastien (CIRAD)" <sebastien.ravel@cirad.fr>
 License: MIT License
         
         Copyright (c) 2023 PHIM / sravel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `snakecdysis-0.0.4/README.rst` & `snakecdysis-0.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `snakecdysis-0.0.4/docs/Makefile` & `snakecdysis-0.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `snakecdysis-0.0.4/docs/source/_images/directory.png` & `snakecdysis-0.0.5/docs/source/_images/directory.png`

 * *Files identical despite different names*

### Comparing `snakecdysis-0.0.4/docs/source/_images/snakecdysis_logo.png` & `snakecdysis-0.0.5/docs/source/_images/snakecdysis_logo.png`

 * *Files identical despite different names*

### Comparing `snakecdysis-0.0.4/docs/source/_images/snakecdysis_logo_short.png` & `snakecdysis-0.0.5/docs/source/_images/snakecdysis_logo_short.png`

 * *Files identical despite different names*

### Comparing `snakecdysis-0.0.4/docs/source/_static/logo.css` & `snakecdysis-0.0.5/docs/source/_static/logo.css`

 * *Files identical despite different names*

### Comparing `snakecdysis-0.0.4/docs/source/conf.py` & `snakecdysis-0.0.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `snakecdysis-0.0.4/docs/source/index.rst` & `snakecdysis-0.0.5/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `snakecdysis-0.0.4/docs/source/install.rst` & `snakecdysis-0.0.5/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `snakecdysis-0.0.4/docs/source/package.rst` & `snakecdysis-0.0.5/docs/source/package.rst`

 * *Files identical despite different names*

### Comparing `snakecdysis-0.0.4/pyproject.toml` & `snakecdysis-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `snakecdysis-0.0.4/snakecdysis/Snakecdysis_logo.png` & `snakecdysis-0.0.5/snakecdysis/Snakecdysis_logo.png`

 * *Files identical despite different names*

### Comparing `snakecdysis-0.0.4/snakecdysis/__main__.py` & `snakecdysis-0.0.5/snakecdysis/__main__.py`

 * *Files identical despite different names*

### Comparing `snakecdysis-0.0.4/snakecdysis/cli_wrapper.py` & `snakecdysis-0.0.5/snakecdysis/cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `snakecdysis-0.0.4/snakecdysis/edit_files.py` & `snakecdysis-0.0.5/snakecdysis/edit_files.py`

 * *Files identical despite different names*

### Comparing `snakecdysis-0.0.4/snakecdysis/install.py` & `snakecdysis-0.0.5/snakecdysis/install.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,16 +20,19 @@
                 click.style(f'    Profile "{default_profile}" exist do you want to remove and continue?\n\n', fg="red"),
                 default=False, abort=True):
             rmtree(default_profile, ignore_errors=True)
         default_profile.mkdir(exist_ok=True)
 
         default_cluster = snake_installer.install_path.joinpath("install_files", f"cluster_config_{scheduler.upper()}.yaml").open(
             "r").read()
-        command = r"""sinfo -s | grep "*" | cut -d"*" -f1 """
+        command = r"""sinfo -s | grep "*" | cut -d"*" -f1 """   # used admin default partition
         default_partition = subprocess.check_output(command, shell=True).decode("utf8").strip()
+        if not default_partition:      # used in case of non default partition define by admin system
+            command = r"""sinfo -s | cut -d" " -f1 | sed '/PARTITION/d' | head -n 1"""
+            default_partition = subprocess.check_output(command, shell=True).decode("utf8").strip()
         if not default_partition:
             click.secho("    Error: Slurm was not found on your system !!", fg="red", err=True)
             snake_installer.fail()
             raise SystemExit
         default_profile.joinpath("cluster_config.yaml").open("w").write(
             default_cluster.replace("PARTITION", default_partition))
 
@@ -50,20 +53,20 @@
                      replay=False, overwrite_if_exists=True,
                      output_dir=f'{default_profile}', config_file=None,
                      default_config=False, password=None, directory=None, skip_if_file_exists=True)
 
         try:
             # default slurm cookiecutter not contain all snakemake variables
             if scheduler == "slurm":
-                default_slurm = 'restart-times: 0\njobscript: "slurm-jobscript.sh"\ncluster: ' \
+                default_slurm = 'cluster-cancel: "scancel"\nrestart-times: 0\njobscript: "slurm-jobscript.sh"\ncluster: ' \
                                 '"slurm-submit.py"\ncluster-status: "slurm-status.py"\nmax-jobs-per-second: ' \
                                 '1\nmax-status-checks-per-second: 10\nlocal-cores: 1\njobs: 200\nlatency-wait: ' \
                                 '1296000\nprintshellcmds: true\n'
                 extra_slurm = f"use-envmodules: {'true' if env == 'modules' else 'false'}\nuse-singularity: " \
-                              f"{'true' if env == 'singularity' else 'false'}\nrerun-incomplete: true"
+                              f"{'true' if env == 'singularity' else 'false'}\nrerun-incomplete: true\nkeep-going: true"
                 with open(f"{default_profile}/config.yaml", "w") as config_file:
                     config_file.write(f"{default_slurm}{extra_slurm}")
 
                 # adding a line in RESOURCES_MAPPING dico in slurm profile
                 with open(f"{default_profile}/slurm-submit.py", "r") as slurm_submit_script:
                     search_text = '"nodes": ("nodes", "nnodes"),'
                     replace_text = '"nodes": ("nodes", "nnodes"),\n    "nodelist" : ("w", "nodelist"),'
```

### Comparing `snakecdysis-0.0.4/snakecdysis/run.py` & `snakecdysis-0.0.5/snakecdysis/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,18 +62,18 @@
         clusterconfig = snake_installer.user_cluster_config
     else:
         click.secho(f"    Please run command line '{snake_installer.soft_name} edit_cluster_config' before the first run of {snake_installer.soft_name} see {snake_installer.docs}", fg="red", err=True)
         exit()
     cmd_clusterconfig = f"--cluster-config {clusterconfig}"
     click.secho(f'    Cluster config file load: {clusterconfig}', fg='yellow')
 
-    if tools != snake_installer.git_tools_path.as_posix():
-        snake_installer.args_tools_path.parent.mkdir(parents=True, exist_ok=True)
-        copyfile(tools, snake_installer.args_tools_path)
-    elif snake_installer.user_tools_path.exists():
+    # if tools != snake_installer.git_tools_path.as_posix():
+    #     snake_installer.args_tools_path.parent.mkdir(parents=True, exist_ok=True)
+    #     copyfile(tools, snake_installer.args_tools_path)
+    if snake_installer.user_tools_path.exists():
         tools = snake_installer.user_tools_path
     click.secho(f'    Tools Path file: {tools}', fg='yellow')
 
     cmd_snakemake_base = f"snakemake --show-failed-logs -p -s {snake_installer.snakefile} --configfile {config} --profile {profile} {cmd_clusterconfig} {' '.join(rewrite_if_bind(snakemake_other))}"
     click.secho(f"\n    {cmd_snakemake_base}\n", fg='bright_blue')
     process = subprocess.run(cmd_snakemake_base, shell=True, check=False, stdout=sys.stdout, stderr=sys.stderr)
     if int(process.returncode) >= 1:
```

### Comparing `snakecdysis-0.0.4/snakecdysis/scripts/generate_template.py` & `snakecdysis-0.0.5/snakecdysis/scripts/generate_template.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,30 +2,36 @@
 from pathlib import Path
 from snakecdysis.global_variable import pkg_templates_path
 import shutil
 
 
 @click.command("generate_template")
 @click.option("--path", "-p", default=".", type=click.Path(exists=False, file_okay=False, dir_okay=True, readable=True, resolve_path=True, path_type=Path),
-              required=True, show_default=True, help='Path to create template python wrapped package')
+              required=True, show_default=True, help='Path to create template python wrapped package (')
 @click.option("--name", '-n', type=str, required=True, help='The wrapper workflow name')
 def main(path, name):
     """Generate the template of repository to create python package"""
     install_path = Path(path)
     click.secho(f"\n    Create path '{path}'", fg="yellow")
-    install_path.mkdir(parents=True, exist_ok=True)
+    try:
+        install_path.mkdir(parents=True, exist_ok=False)
+    except FileExistsError:
+        files_list = list(install_path.glob("*"))
+        if len(files_list) > 0:
+            raise FileExistsError(f"Error: directory {install_path} already existed and is not empty!!")
+
     click.secho(f"\n    Copy templates files from {pkg_templates_path} to {install_path}", fg="yellow")
     pkg_name_dest = install_path.joinpath(name)
     if pkg_name_dest.exists():
         shutil.rmtree(pkg_name_dest)
     shutil.copytree(pkg_templates_path, install_path, dirs_exist_ok=True, copy_function=shutil.copy2)
     install_path.joinpath("PKGNAME").rename(pkg_name_dest)
 
     for file in install_path.glob("**/*"):
-        if file.is_file():
+        if file.is_file() and "__pycache__" not in file.parent.as_posix():
             print(file)
             file.write_text(file.read_text().replace("PKGNAME",name))
```

### Comparing `snakecdysis-0.0.4/snakecdysis/snake_wrapper.py` & `snakecdysis-0.0.5/snakecdysis/snake_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
             git_config_path (str): Path to default config file yaml (default: toto/install_files/config.yaml)
             git_tools_path (str): Path to default tools config yaml(default: toto/install_files/tools_path.yaml)
             git_cluster_config (str): Path to slurm cluster config file (default: toto/install_files/cluster_config_SLURM.yaml)
 
     """
 
     def __init__(self, soft_path=None, url=None, docs=None, description_tool=None, singularity_url_files=None, datatest_url_files=None, **kargs):
-        # TODO, add kargs to change default snakefile name/path, ....
         self.install_path = soft_path
         self.git_url = url
         self.docs = docs
         self.description_tool = description_tool
         self.singularity_url_files = singularity_url_files
         self.datatest_url_files = datatest_url_files
         self.dico_args = kargs
@@ -267,15 +266,15 @@
                     print(project_name_with_namespace)
                     gl = gitlab.Gitlab(self.git_url.replace(f'/{project_name_with_namespace}', ""))
                     project = gl.projects.get(f"{project_name_with_namespace}")
                     # print(project.releases.list())
                     tags_list = project.tags.list(order_by='updated', sort='desc')
                     lastRelease = tags_list[0].name
             except Exception as e:
-                print(e)
+                # print(e)
                 lastRelease = "There aren’t any releases"
             epilogTools = "\n"
             if str(self.version) != lastRelease:
                 if lastRelease < str(self.version):
                     epilogTools = click.style(f"\n    ** NOTE: This {self.soft_name} version ({self.version}) is higher than the production version ({lastRelease}), you are using a dev version\n\n", fg="yellow", bold=True)
                 elif lastRelease > str(self.version) and lastRelease != "There aren’t any releases":
                     epilogTools = click.style(f"\n    ** NOTE: The Latest version of {self.soft_name} {lastRelease} is available at {self.git_url}\n\n", fg="yellow", underline=True)
@@ -367,16 +366,14 @@
             docs (str): Url of documentation
             description_tool (str):The header print on terminal when run programme. Please add string values 'VERSION', 'GIT_URL' and 'DOCS' and wrapper automatically replace by th good values
             singularity_ur_files (list(tuple()): List of tuple with downloaded url and install destination with INSTALL_PATH. like INSTALL_PATH/containers/Singularity.CulebrONT_tools.sif
             datatest_url_files (tuple): Tuple with 2 values, first the url of datatest, second download name.
 
     """
     def __init__(self, dico_tool=None, workflow=None, config=None, **kargs):
-        # TODO add workflow and config value
-        # TODO add dico_tool or unpack version
         if dico_tool:
             super().__init__(**dico_tool)
         else:
             super().__init__(**kargs)
         # workflow is available only in __init__
         # print("\n".join(list(workflow.__dict__.keys())))
         # print(workflow.__dict__)
```

### Comparing `snakecdysis-0.0.4/snakecdysis/templates/PKGNAME/__init__.py` & `snakecdysis-0.0.5/snakecdysis/templates/PKGNAME/__init__.py`

 * *Files identical despite different names*

### Comparing `snakecdysis-0.0.4/snakecdysis/templates/PKGNAME/global_variables.py` & `snakecdysis-0.0.5/snakecdysis/templates/PKGNAME/global_variables.py`

 * *Files identical despite different names*

### Comparing `snakecdysis-0.0.4/snakecdysis/templates/PKGNAME/install_files/tools_path.yaml` & `snakecdysis-0.0.5/snakecdysis/templates/PKGNAME/install_files/tools_path.yaml`

 * *Files identical despite different names*

### Comparing `snakecdysis-0.0.4/snakecdysis/templates/PKGNAME/module.py` & `snakecdysis-0.0.5/snakecdysis/templates/PKGNAME/module.py`

 * *Files identical despite different names*

### Comparing `snakecdysis-0.0.4/snakecdysis/templates/PKGNAME/snakefiles/snakefile` & `snakecdysis-0.0.5/snakecdysis/templates/PKGNAME/snakefiles/snakefile`

 * *Files identical despite different names*

### Comparing `snakecdysis-0.0.4/snakecdysis/templates/pyproject.toml` & `snakecdysis-0.0.5/snakecdysis/templates/pyproject.toml`

 * *Files identical despite different names*

### Comparing `snakecdysis-0.0.4/snakecdysis/useful_function.py` & `snakecdysis-0.0.5/snakecdysis/useful_function.py`

 * *Files identical despite different names*

### Comparing `snakecdysis-0.0.4/snakecdysis.egg-info/PKG-INFO` & `snakecdysis-0.0.5/snakecdysis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snakecdysis
-Version: 0.0.4
+Version: 0.0.5
 Summary: You want to wrap your best snakemake workflow to be easy install and run, Snakecdysis is for you !!!!! Tha aim of Snakecdysis is to easy-wrapped snakemake workflow as python package and then build sub-commands to manage this. !!!!!
 Author-email: "Ravel Sebastien (CIRAD)" <sebastien.ravel@cirad.fr>
 License: MIT License
         
         Copyright (c) 2023 PHIM / sravel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `snakecdysis-0.0.4/snakecdysis.egg-info/SOURCES.txt` & `snakecdysis-0.0.5/snakecdysis.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .gitignore
 .readthedocs.yml
+CHANGELOG.md
 LICENSE
 README.rst
 pyproject.toml
 docs/Makefile
 docs/requirements.txt
 docs/source/conf.py
 docs/source/index.rst
```


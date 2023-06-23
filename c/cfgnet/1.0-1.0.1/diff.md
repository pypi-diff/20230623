# Comparing `tmp/cfgnet-1.0.tar.gz` & `tmp/cfgnet-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfgnet-1.0.tar", max compression
+gzip compressed data, was "cfgnet-1.0.1.tar", max compression
```

## Comparing `cfgnet-1.0.tar` & `cfgnet-1.0.1.tar`

### file list

```diff
@@ -1,61 +1,62 @@
--rw-r--r--   0        0        0     5446 2023-05-17 08:33:17.002499 cfgnet-1.0/README.md
--rw-r--r--   0        0        0     1678 2023-05-17 09:23:47.851387 cfgnet-1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2021-12-09 09:18:09.441783 cfgnet-1.0/src/cfgnet/__init__.py
--rw-r--r--   0        0        0        0 2022-01-11 10:11:28.996292 cfgnet-1.0/src/cfgnet/analyze/__init__.py
--rw-r--r--   0        0        0     4149 2023-01-03 09:32:28.547287 cfgnet-1.0/src/cfgnet/analyze/analyzer.py
--rw-r--r--   0        0        0     2168 2022-10-12 09:28:24.308895 cfgnet-1.0/src/cfgnet/analyze/csv_writer.py
--rw-r--r--   0        0        0     1158 2022-02-01 08:40:08.485767 cfgnet-1.0/src/cfgnet/analyze/timeout.py
--rw-r--r--   0        0        0        0 2022-01-11 10:11:28.998274 cfgnet-1.0/src/cfgnet/config_types/__init__.py
--rw-r--r--   0        0        0     7957 2023-04-24 06:43:35.292451 cfgnet-1.0/src/cfgnet/config_types/config_type_inferer.py
--rw-r--r--   0        0        0     1466 2023-04-19 14:44:57.555330 cfgnet-1.0/src/cfgnet/config_types/config_types.py
--rw-r--r--   0        0        0        0 2021-12-09 09:18:10.962151 cfgnet-1.0/src/cfgnet/conflicts/__init__.py
--rw-r--r--   0        0        0     7829 2022-10-12 09:28:24.309896 cfgnet-1.0/src/cfgnet/conflicts/conflict.py
--rw-r--r--   0        0        0     8481 2023-01-03 09:32:28.547287 cfgnet-1.0/src/cfgnet/conflicts/conflict_detector.py
--rw-r--r--   0        0        0        0 2021-12-09 09:18:09.751940 cfgnet-1.0/src/cfgnet/exceptions/__init__.py
--rw-r--r--   0        0        0     1011 2021-12-09 09:18:09.751940 cfgnet-1.0/src/cfgnet/exceptions/exceptions.py
--rw-r--r--   0        0        0        0 2021-12-09 09:18:11.876286 cfgnet-1.0/src/cfgnet/exporter/__init__.py
--rw-r--r--   0        0        0     5409 2021-12-16 14:50:35.744366 cfgnet-1.0/src/cfgnet/exporter/exporter.py
--rw-r--r--   0        0        0     8420 2023-04-21 06:44:52.417363 cfgnet-1.0/src/cfgnet/launcher.py
--rw-r--r--   0        0        0      378 2021-12-09 09:18:10.597639 cfgnet-1.0/src/cfgnet/launcher_configuration.py
--rw-r--r--   0        0        0        0 2021-12-09 09:18:10.773422 cfgnet-1.0/src/cfgnet/linker/__init__.py
--rw-r--r--   0        0        0     3179 2023-03-14 14:58:57.734481 cfgnet-1.0/src/cfgnet/linker/equality_linker.py
--rw-r--r--   0        0        0     2806 2021-12-09 09:18:10.964151 cfgnet-1.0/src/cfgnet/linker/link.py
--rw-r--r--   0        0        0     2521 2022-02-07 15:11:06.458181 cfgnet-1.0/src/cfgnet/linker/linker.py
--rw-r--r--   0        0        0     1843 2022-02-07 15:11:06.458181 cfgnet-1.0/src/cfgnet/linker/linker_manager.py
--rw-r--r--   0        0        0      954 2021-12-09 09:18:10.776422 cfgnet-1.0/src/cfgnet/linker/static_blacklist.py
--rw-r--r--   0        0        0        0 2021-12-09 09:18:09.751940 cfgnet-1.0/src/cfgnet/network/__init__.py
--rw-r--r--   0        0        0     2421 2022-09-02 07:16:03.544920 cfgnet-1.0/src/cfgnet/network/ignorefile.py
--rw-r--r--   0        0        0    11097 2023-03-15 13:46:16.800491 cfgnet-1.0/src/cfgnet/network/network.py
--rw-r--r--   0        0        0     1108 2022-11-30 08:55:06.018788 cfgnet-1.0/src/cfgnet/network/network_configuration.py
--rw-r--r--   0        0        0     8584 2023-04-24 06:43:35.293451 cfgnet-1.0/src/cfgnet/network/nodes.py
--rw-r--r--   0        0        0        0 2021-12-09 09:18:09.752938 cfgnet-1.0/src/cfgnet/plugins/__init__.py
--rw-r--r--   0        0        0        0 2021-12-09 09:18:09.752938 cfgnet-1.0/src/cfgnet/plugins/concept/__init__.py
--rw-r--r--   0        0        0     2343 2023-04-19 13:29:40.290485 cfgnet-1.0/src/cfgnet/plugins/concept/ansible_playbook_plugin.py
--rw-r--r--   0        0        0      999 2023-04-19 13:29:40.291000 cfgnet-1.0/src/cfgnet/plugins/concept/ansible_plugin.py
--rw-r--r--   0        0        0    12301 2022-11-29 13:37:38.698777 cfgnet-1.0/src/cfgnet/plugins/concept/apache_webserver_plugin.py
--rw-r--r--   0        0        0     3316 2023-03-14 14:58:57.735485 cfgnet-1.0/src/cfgnet/plugins/concept/cypress_plugin.py
--rw-r--r--   0        0        0     6381 2023-04-19 14:44:57.556331 cfgnet-1.0/src/cfgnet/plugins/concept/docker_compose_plugin.py
--rw-r--r--   0        0        0     9525 2023-03-14 14:58:57.736482 cfgnet-1.0/src/cfgnet/plugins/concept/docker_plugin.py
--rw-r--r--   0        0        0    12193 2023-01-03 09:32:28.551803 cfgnet-1.0/src/cfgnet/plugins/concept/maven_plugin.py
--rw-r--r--   0        0        0     3308 2023-04-24 06:43:35.293451 cfgnet-1.0/src/cfgnet/plugins/concept/mongodb_plugin.py
--rw-r--r--   0        0        0     5467 2022-12-01 11:51:39.429563 cfgnet-1.0/src/cfgnet/plugins/concept/mysql_plugin.py
--rw-r--r--   0        0        0     2485 2022-06-15 13:01:29.552275 cfgnet-1.0/src/cfgnet/plugins/concept/nodejs_plugin.py
--rw-r--r--   0        0        0     4665 2023-03-14 14:58:57.736482 cfgnet-1.0/src/cfgnet/plugins/concept/php_plugin.py
--rw-r--r--   0        0        0     2154 2022-09-02 07:16:03.551935 cfgnet-1.0/src/cfgnet/plugins/concept/poetry_plugin.py
--rw-r--r--   0        0        0     1395 2023-04-24 06:43:35.294451 cfgnet-1.0/src/cfgnet/plugins/concept/postgresql_plugin.py
--rw-r--r--   0        0        0    11319 2023-04-19 11:22:15.733789 cfgnet-1.0/src/cfgnet/plugins/concept/spring_plugin.py
--rw-r--r--   0        0        0     3674 2022-09-02 07:16:03.553927 cfgnet-1.0/src/cfgnet/plugins/concept/travis_plugin.py
--rw-r--r--   0        0        0     2562 2022-09-02 07:16:03.554922 cfgnet-1.0/src/cfgnet/plugins/concept/tsconfig_plugin.py
--rw-r--r--   0        0        0        0 2022-01-11 10:11:29.006269 cfgnet-1.0/src/cfgnet/plugins/file_type/__init__.py
--rw-r--r--   0        0        0     6270 2023-04-24 06:43:35.295451 cfgnet-1.0/src/cfgnet/plugins/file_type/configparser_plugin.py
--rw-r--r--   0        0        0     5585 2022-06-15 13:01:29.557274 cfgnet-1.0/src/cfgnet/plugins/file_type/json_plugin.py
--rw-r--r--   0        0        0     4544 2023-01-03 09:32:28.552802 cfgnet-1.0/src/cfgnet/plugins/file_type/toml_plugin.py
--rw-r--r--   0        0        0     5002 2023-04-24 06:43:35.295451 cfgnet-1.0/src/cfgnet/plugins/file_type/yaml_plugin.py
--rw-r--r--   0        0        0     3352 2023-01-03 09:32:28.553802 cfgnet-1.0/src/cfgnet/plugins/plugin.py
--rw-r--r--   0        0        0     3222 2023-04-24 06:43:35.296450 cfgnet-1.0/src/cfgnet/plugins/plugin_manager.py
--rw-r--r--   0        0        0        0 2022-01-11 10:11:29.008270 cfgnet-1.0/src/cfgnet/utility/__init__.py
--rw-r--r--   0        0        0     2282 2022-01-11 10:11:29.008270 cfgnet-1.0/src/cfgnet/utility/logger.py
--rw-r--r--   0        0        0        0 2021-12-09 09:18:09.597379 cfgnet-1.0/src/cfgnet/vcs/__init__.py
--rw-r--r--   0        0        0     2716 2022-07-29 13:07:51.929869 cfgnet-1.0/src/cfgnet/vcs/git.py
--rw-r--r--   0        0        0     1657 2022-01-11 10:11:29.009268 cfgnet-1.0/src/cfgnet/vcs/git_history.py
--rw-r--r--   0        0        0     6775 1970-01-01 00:00:00.000000 cfgnet-1.0/PKG-INFO
+-rw-r--r--   0        0        0     5494 2023-06-23 08:35:30.526104 cfgnet-1.0.1/README.md
+-rw-r--r--   0        0        0     1680 2023-06-23 08:35:30.526104 cfgnet-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-23 08:35:30.526104 cfgnet-1.0.1/src/cfgnet/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-23 08:35:30.526104 cfgnet-1.0.1/src/cfgnet/analyze/__init__.py
+-rw-r--r--   0        0        0     4149 2023-06-23 08:35:30.526104 cfgnet-1.0.1/src/cfgnet/analyze/analyzer.py
+-rw-r--r--   0        0        0     2168 2023-06-23 08:35:30.526104 cfgnet-1.0.1/src/cfgnet/analyze/csv_writer.py
+-rw-r--r--   0        0        0     1158 2023-06-23 08:35:30.526104 cfgnet-1.0.1/src/cfgnet/analyze/timeout.py
+-rw-r--r--   0        0        0        0 2023-06-23 08:35:30.526104 cfgnet-1.0.1/src/cfgnet/config_types/__init__.py
+-rw-r--r--   0        0        0     7952 2023-06-23 08:35:30.526104 cfgnet-1.0.1/src/cfgnet/config_types/config_type_inferer.py
+-rw-r--r--   0        0        0     1485 2023-06-23 08:35:30.526104 cfgnet-1.0.1/src/cfgnet/config_types/config_types.py
+-rw-r--r--   0        0        0        0 2023-06-23 08:35:30.526104 cfgnet-1.0.1/src/cfgnet/conflicts/__init__.py
+-rw-r--r--   0        0        0     7829 2023-06-23 08:35:30.526104 cfgnet-1.0.1/src/cfgnet/conflicts/conflict.py
+-rw-r--r--   0        0        0     8481 2023-06-23 08:35:30.526104 cfgnet-1.0.1/src/cfgnet/conflicts/conflict_detector.py
+-rw-r--r--   0        0        0        0 2023-06-23 08:35:30.526104 cfgnet-1.0.1/src/cfgnet/exceptions/__init__.py
+-rw-r--r--   0        0        0     1011 2023-06-23 08:35:30.526104 cfgnet-1.0.1/src/cfgnet/exceptions/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-23 08:35:30.526104 cfgnet-1.0.1/src/cfgnet/exporter/__init__.py
+-rw-r--r--   0        0        0     5409 2023-06-23 08:35:30.526104 cfgnet-1.0.1/src/cfgnet/exporter/exporter.py
+-rw-r--r--   0        0        0     8420 2023-06-23 08:35:30.526104 cfgnet-1.0.1/src/cfgnet/launcher.py
+-rw-r--r--   0        0        0      378 2023-06-23 08:35:30.526104 cfgnet-1.0.1/src/cfgnet/launcher_configuration.py
+-rw-r--r--   0        0        0        0 2023-06-23 08:35:30.526104 cfgnet-1.0.1/src/cfgnet/linker/__init__.py
+-rw-r--r--   0        0        0     3179 2023-06-23 08:35:30.526104 cfgnet-1.0.1/src/cfgnet/linker/equality_linker.py
+-rw-r--r--   0        0        0     2806 2023-06-23 08:35:30.526104 cfgnet-1.0.1/src/cfgnet/linker/link.py
+-rw-r--r--   0        0        0     2521 2023-06-23 08:35:30.526104 cfgnet-1.0.1/src/cfgnet/linker/linker.py
+-rw-r--r--   0        0        0     1843 2023-06-23 08:35:30.526104 cfgnet-1.0.1/src/cfgnet/linker/linker_manager.py
+-rw-r--r--   0        0        0      954 2023-06-23 08:35:30.526104 cfgnet-1.0.1/src/cfgnet/linker/static_blacklist.py
+-rw-r--r--   0        0        0        0 2023-06-23 08:35:30.526104 cfgnet-1.0.1/src/cfgnet/network/__init__.py
+-rw-r--r--   0        0        0     2421 2023-06-23 08:35:30.526104 cfgnet-1.0.1/src/cfgnet/network/ignorefile.py
+-rw-r--r--   0        0        0    11097 2023-06-23 08:35:30.526104 cfgnet-1.0.1/src/cfgnet/network/network.py
+-rw-r--r--   0        0        0     1108 2023-06-23 08:35:30.526104 cfgnet-1.0.1/src/cfgnet/network/network_configuration.py
+-rw-r--r--   0        0        0     8584 2023-06-23 08:35:30.526104 cfgnet-1.0.1/src/cfgnet/network/nodes.py
+-rw-r--r--   0        0        0        0 2023-06-23 08:35:30.526104 cfgnet-1.0.1/src/cfgnet/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-23 08:35:30.526104 cfgnet-1.0.1/src/cfgnet/plugins/concept/__init__.py
+-rw-r--r--   0        0        0     2343 2023-06-23 08:35:30.526104 cfgnet-1.0.1/src/cfgnet/plugins/concept/ansible_playbook_plugin.py
+-rw-r--r--   0        0        0      999 2023-06-23 08:35:30.526104 cfgnet-1.0.1/src/cfgnet/plugins/concept/ansible_plugin.py
+-rw-r--r--   0        0        0    12301 2023-06-23 08:35:30.530104 cfgnet-1.0.1/src/cfgnet/plugins/concept/apache_webserver_plugin.py
+-rw-r--r--   0        0        0     3316 2023-06-23 08:35:30.530104 cfgnet-1.0.1/src/cfgnet/plugins/concept/cypress_plugin.py
+-rw-r--r--   0        0        0     8538 2023-06-23 08:35:30.530104 cfgnet-1.0.1/src/cfgnet/plugins/concept/django_plugin.py
+-rw-r--r--   0        0        0     6744 2023-06-23 08:35:30.530104 cfgnet-1.0.1/src/cfgnet/plugins/concept/docker_compose_plugin.py
+-rw-r--r--   0        0        0     9525 2023-06-23 08:35:30.530104 cfgnet-1.0.1/src/cfgnet/plugins/concept/docker_plugin.py
+-rw-r--r--   0        0        0    12193 2023-06-23 08:35:30.530104 cfgnet-1.0.1/src/cfgnet/plugins/concept/maven_plugin.py
+-rw-r--r--   0        0        0     3308 2023-06-23 08:35:30.530104 cfgnet-1.0.1/src/cfgnet/plugins/concept/mongodb_plugin.py
+-rw-r--r--   0        0        0     5467 2023-06-23 08:35:30.530104 cfgnet-1.0.1/src/cfgnet/plugins/concept/mysql_plugin.py
+-rw-r--r--   0        0        0     2485 2023-06-23 08:35:30.530104 cfgnet-1.0.1/src/cfgnet/plugins/concept/nodejs_plugin.py
+-rw-r--r--   0        0        0     4665 2023-06-23 08:35:30.530104 cfgnet-1.0.1/src/cfgnet/plugins/concept/php_plugin.py
+-rw-r--r--   0        0        0     2154 2023-06-23 08:35:30.530104 cfgnet-1.0.1/src/cfgnet/plugins/concept/poetry_plugin.py
+-rw-r--r--   0        0        0     1395 2023-06-23 08:35:30.530104 cfgnet-1.0.1/src/cfgnet/plugins/concept/postgresql_plugin.py
+-rw-r--r--   0        0        0    10995 2023-06-23 08:35:30.530104 cfgnet-1.0.1/src/cfgnet/plugins/concept/spring_plugin.py
+-rw-r--r--   0        0        0     3674 2023-06-23 08:35:30.530104 cfgnet-1.0.1/src/cfgnet/plugins/concept/travis_plugin.py
+-rw-r--r--   0        0        0     2562 2023-06-23 08:35:30.530104 cfgnet-1.0.1/src/cfgnet/plugins/concept/tsconfig_plugin.py
+-rw-r--r--   0        0        0        0 2023-06-23 08:35:30.530104 cfgnet-1.0.1/src/cfgnet/plugins/file_type/__init__.py
+-rw-r--r--   0        0        0     6270 2023-06-23 08:35:30.530104 cfgnet-1.0.1/src/cfgnet/plugins/file_type/configparser_plugin.py
+-rw-r--r--   0        0        0     5585 2023-06-23 08:35:30.530104 cfgnet-1.0.1/src/cfgnet/plugins/file_type/json_plugin.py
+-rw-r--r--   0        0        0     4544 2023-06-23 08:35:30.530104 cfgnet-1.0.1/src/cfgnet/plugins/file_type/toml_plugin.py
+-rw-r--r--   0        0        0     5002 2023-06-23 08:35:30.530104 cfgnet-1.0.1/src/cfgnet/plugins/file_type/yaml_plugin.py
+-rw-r--r--   0        0        0     3352 2023-06-23 08:35:30.530104 cfgnet-1.0.1/src/cfgnet/plugins/plugin.py
+-rw-r--r--   0        0        0     3308 2023-06-23 08:35:30.530104 cfgnet-1.0.1/src/cfgnet/plugins/plugin_manager.py
+-rw-r--r--   0        0        0        0 2023-06-23 08:35:30.530104 cfgnet-1.0.1/src/cfgnet/utility/__init__.py
+-rw-r--r--   0        0        0     2282 2023-06-23 08:35:30.530104 cfgnet-1.0.1/src/cfgnet/utility/logger.py
+-rw-r--r--   0        0        0        0 2023-06-23 08:35:30.530104 cfgnet-1.0.1/src/cfgnet/vcs/__init__.py
+-rw-r--r--   0        0        0     2716 2023-06-23 08:35:30.530104 cfgnet-1.0.1/src/cfgnet/vcs/git.py
+-rw-r--r--   0        0        0     1657 2023-06-23 08:35:30.530104 cfgnet-1.0.1/src/cfgnet/vcs/git_history.py
+-rw-r--r--   0        0        0     6825 1970-01-01 00:00:00.000000 cfgnet-1.0.1/PKG-INFO
```

### Comparing `cfgnet-1.0/README.md` & `cfgnet-1.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 We envision that CfgNet is used within a Git hook (e.g., pre-commit hook) to prevent dependency conflicts during the development and maintenance of software systems. 
 That is, whenever changes are made, CfgNet can check the changes before the actual commit gets pushed to the repository and reports a warning if it has detected possible dependency conflicts. 
 This way, developer can check the changes again and even use the information that CfgNet provides to fix the dependency conflicts.
 
 ## Installation
 
-CfgNet is a package on PyPI
+CfgNet is a package on PyPI. You can install it with the following command:
 
     pip install cfgnet
 
 You can also build it locally with [poetry](https://python-poetry.org/).
 Please refer to the documentation of poetry for further details.
 
 ## Basic Usage
```

### Comparing `cfgnet-1.0/pyproject.toml` & `cfgnet-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['poetry>=0.12']
 build-backend = 'poetry.masonry.api'
 
 [tool.poetry]
 name = 'CfgNet'
-version = '1.0'
+version = '1.0.1'
 description = 'A Framework for Tracking Configuration Dependencies Across a Software Project'
 authors = [
   'Sebastian Simon <ssimon@informatik.uni-leipzig.de>',
   'Nicolai Ruckel <nicolai.ruckel@uni-weimar.de>',
   'Jakob Ruckel <jakob.bela.ruckel@uni-weimar.de>'
   ]
 maintainers = [
```

### Comparing `cfgnet-1.0/src/cfgnet/analyze/analyzer.py` & `cfgnet-1.0.1/src/cfgnet/analyze/analyzer.py`

 * *Files identical despite different names*

### Comparing `cfgnet-1.0/src/cfgnet/analyze/csv_writer.py` & `cfgnet-1.0.1/src/cfgnet/analyze/csv_writer.py`

 * *Files identical despite different names*

### Comparing `cfgnet-1.0/src/cfgnet/analyze/timeout.py` & `cfgnet-1.0.1/src/cfgnet/analyze/timeout.py`

 * *Files identical despite different names*

### Comparing `cfgnet-1.0/src/cfgnet/config_types/config_type_inferer.py` & `cfgnet-1.0.1/src/cfgnet/config_types/config_type_inferer.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     regex_username_option = re.compile(r"user|usr|username")
     regex_username_value = re.compile(r"[a-zA-Z][a-zA-Z0-9_]+")
     regex_time_option = re.compile(
         r"time|interval|day|month|year|hour|minute|second|millisecond"
     )
     regex_time_value = re.compile(r"[\d]+ ?(s|min|h|d|ms)*")
     regex_filepath_option = re.compile(
-        r"file|path|dir|directory|folder|destination"
+        r"path|dir|directory|folder|destination"
     )
     # regex_filepath_value = re.compile(r"\/?([^\/]+\/)+[^\/]*")
     regex_filepath_value = re.compile(r"^([~.\w\d]*\/[.\w\d]+)+(\.[\w\d]+)*$")
     regex_version_number_option = re.compile(r"version|target|source")
     regex_version_number_value = re.compile(
         r"^(\^|~)?(?:[0-9]{1,3}\.){2}[0-9]{1,3}(-[\w]+)?$"
     )
```

### Comparing `cfgnet-1.0/src/cfgnet/config_types/config_types.py` & `cfgnet-1.0.1/src/cfgnet/config_types/config_types.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     PATTERN = auto()
     PLATFORM = auto()
     LANGUAGE = auto()
     TYPE = auto()
     MIME = auto()
     HOST = auto()
     STATE = auto()
+    CLASS = auto()
 
     # Booleans
     BOOLEAN = auto()
     MODE = auto()
 
     # UNKNOWN
     UNKNOWN = auto()
```

### Comparing `cfgnet-1.0/src/cfgnet/conflicts/conflict.py` & `cfgnet-1.0.1/src/cfgnet/conflicts/conflict.py`

 * *Files identical despite different names*

### Comparing `cfgnet-1.0/src/cfgnet/conflicts/conflict_detector.py` & `cfgnet-1.0.1/src/cfgnet/conflicts/conflict_detector.py`

 * *Files identical despite different names*

### Comparing `cfgnet-1.0/src/cfgnet/exceptions/exceptions.py` & `cfgnet-1.0.1/src/cfgnet/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `cfgnet-1.0/src/cfgnet/exporter/exporter.py` & `cfgnet-1.0.1/src/cfgnet/exporter/exporter.py`

 * *Files identical despite different names*

### Comparing `cfgnet-1.0/src/cfgnet/launcher.py` & `cfgnet-1.0.1/src/cfgnet/launcher.py`

 * *Files identical despite different names*

### Comparing `cfgnet-1.0/src/cfgnet/linker/equality_linker.py` & `cfgnet-1.0.1/src/cfgnet/linker/equality_linker.py`

 * *Files identical despite different names*

### Comparing `cfgnet-1.0/src/cfgnet/linker/link.py` & `cfgnet-1.0.1/src/cfgnet/linker/link.py`

 * *Files identical despite different names*

### Comparing `cfgnet-1.0/src/cfgnet/linker/linker.py` & `cfgnet-1.0.1/src/cfgnet/linker/linker.py`

 * *Files identical despite different names*

### Comparing `cfgnet-1.0/src/cfgnet/linker/linker_manager.py` & `cfgnet-1.0.1/src/cfgnet/linker/linker_manager.py`

 * *Files identical despite different names*

### Comparing `cfgnet-1.0/src/cfgnet/linker/static_blacklist.py` & `cfgnet-1.0.1/src/cfgnet/linker/static_blacklist.py`

 * *Files identical despite different names*

### Comparing `cfgnet-1.0/src/cfgnet/network/ignorefile.py` & `cfgnet-1.0.1/src/cfgnet/network/ignorefile.py`

 * *Files identical despite different names*

### Comparing `cfgnet-1.0/src/cfgnet/network/network.py` & `cfgnet-1.0.1/src/cfgnet/network/network.py`

 * *Files identical despite different names*

### Comparing `cfgnet-1.0/src/cfgnet/network/network_configuration.py` & `cfgnet-1.0.1/src/cfgnet/network/network_configuration.py`

 * *Files identical despite different names*

### Comparing `cfgnet-1.0/src/cfgnet/network/nodes.py` & `cfgnet-1.0.1/src/cfgnet/network/nodes.py`

 * *Files identical despite different names*

### Comparing `cfgnet-1.0/src/cfgnet/plugins/concept/ansible_playbook_plugin.py` & `cfgnet-1.0.1/src/cfgnet/plugins/concept/ansible_playbook_plugin.py`

 * *Files identical despite different names*

### Comparing `cfgnet-1.0/src/cfgnet/plugins/concept/ansible_plugin.py` & `cfgnet-1.0.1/src/cfgnet/plugins/concept/ansible_plugin.py`

 * *Files identical despite different names*

### Comparing `cfgnet-1.0/src/cfgnet/plugins/concept/apache_webserver_plugin.py` & `cfgnet-1.0.1/src/cfgnet/plugins/concept/apache_webserver_plugin.py`

 * *Files identical despite different names*

### Comparing `cfgnet-1.0/src/cfgnet/plugins/concept/cypress_plugin.py` & `cfgnet-1.0.1/src/cfgnet/plugins/concept/cypress_plugin.py`

 * *Files identical despite different names*

### Comparing `cfgnet-1.0/src/cfgnet/plugins/concept/docker_compose_plugin.py` & `cfgnet-1.0.1/src/cfgnet/plugins/concept/mysql_plugin.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,177 +8,166 @@
 # This program is distributed in the hope that it will be useful, but WITHOUT
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more
 # details.
 #
 # You should have received a copy of the GNU General Public License along with
 # this program.  If not, see <https://www.gnu.org/licenses/>.
-import re
-from yaml.nodes import ScalarNode
-from cfgnet.config_types.config_types import ConfigType
-
-from cfgnet.network.nodes import ArtifactNode, OptionNode, ValueNode
-from cfgnet.plugins.file_type.yaml_plugin import YAMLPlugin
 
+from cfgnet.plugins.file_type.configparser_plugin import ConfigParserPlugin
+from cfgnet.config_types.config_types import ConfigType
 
-class DockerComposePlugin(YAMLPlugin):
-    file_name = re.compile(r"docker-compose(.\w+)?.yml")
-    ports = re.compile(r"(?P<in>[0-9]{4}):(?P<out>[0-9]{4})")
 
+class MysqlPlugin(ConfigParserPlugin):
     def __init__(self):
-        super().__init__("docker-compose")
+        super().__init__("mysql")
 
-    def is_responsible(self, abs_file_path):
-        if self.file_name.search(abs_file_path):
+    def is_responsible(self, abs_file_path) -> bool:
+        if abs_file_path.endswith(("my.cnf", "my.ini")):
             return True
         return False
 
-    def _parse_scalar_node(self, node, parent):
-        if node.value != "":
-            match = DockerComposePlugin.ports.match(node.value)
-            if match is not None:
-                port_in = ValueNode(name=match.group("in"))
-                port_out = ValueNode(name=match.group("out"))
-                option_port_in = OptionNode(
-                    "in", node.start_mark.line + 1, ConfigType.PORT
-                )
-                option_port_out = OptionNode(
-                    "out", node.start_mark.line + 1, ConfigType.PORT
-                )
-                parent.add_child(option_port_in)
-                parent.add_child(option_port_out)
-                option_port_in.add_child(port_in)
-                option_port_out.add_child(port_out)
-            else:
-                if len(node.value.split("=")) == 2:
-                    self._parse_value_assignment(node=node, parent=parent)
-                    return
-
-                name = (
-                    f"{parent.name}:{node.value}"
-                    if parent.config_type == ConfigType.VERSION_NUMBER
-                    else node.value
-                )
-
-                value = ValueNode(name=name)
-
-                if isinstance(parent, ArtifactNode):
-                    option = OptionNode(
-                        "unnamed_option", node.start_mark.line + 1
-                    )
-                    parent.add_child(option)
-                    option.add_child(value)
-                else:
-                    parent.add_child(value)
-
-    def _parse_value_assignment(
-        self, node: ScalarNode, parent: OptionNode
-    ) -> None:
-        value_parts = node.value.split("=")
-        config_type = self.get_config_type(option_name=value_parts[0])
-        variable = OptionNode(
-            name=value_parts[0],
-            location=str(node.start_mark.line + 1),
-            config_type=config_type,
-        )
-        parent.add_child(variable)
-        value = ValueNode(name=value_parts[1])
-        variable.add_child(value)
-
-    # pylint: disable=too-many-return-statements
+    # pylint: disable=unused-argument,too-many-return-statements
     def get_config_type(self, option_name: str) -> ConfigType:  # noqa: C901
         """
         Find config type based on option name.
 
+        Option types included from:
+        https://dev.mysql.com/doc/refman/8.0/en/server-system-variables.html
+
         :param option_name: name of option
         :return: config type
         """
         option_name = option_name.lower()
+        if option_name.endswith(("dir", "file", "directory", "path")):
+            if not option_name == "core_file":
+                return ConfigType.PATH
 
-        if option_name == "version":
-            return ConfigType.VERSION_NUMBER
-        if option_name in ("ports", "port", "expose", "PORT", "tmpfs"):
-            return ConfigType.PORT
-        if option_name == "image":
-            return ConfigType.IMAGE
-        if option_name == ("size", "weight", "height"):
-            return ConfigType.SIZE
-        if option_name in ("path", "file", "env_file"):
-            return ConfigType.PATH
-        if option_name == "environment":
-            return ConfigType.ENVIRONMENT
-        if option_name in ("command", "entrypoint", "test"):
-            return ConfigType.COMMAND
         if option_name in (
-            "name",
-            "driver",
-            "labels",
-            "hostname",
-            "cap_add",
-            "cap_drop",
-            "cgroup_parent",
-            "source",
-            "container_name",
-            "depends_on",
-            "registry",
-            "service",
-            "external_links",
+            "admin_ssl_ca",
+            "admin_ssl_cert",
+            "admin_ssl_crl",
+            "admin_ssl_key",
+            "log_error",
+            "secure_file_priv",
+            "socket",
+            "ssl_ca",
+            "ssl_cert",
+            "ssl_crl",
+            "ssl_key",
         ):
-            return ConfigType.NAME
-        if option_name == "rate":
-            return ConfigType.SPEED
+            return ConfigType.PATH
+
+        if option_name in ("port"):
+            return ConfigType.PORT
+
+        if option_name == "password":
+            return ConfigType.PASSWORD
+
+        if option_name in ("user", "external_user", "proxy_user"):
+            return ConfigType.USERNAME
+
+        if option_name in ("admin_address", "bind_address"):
+            return ConfigType.IP_ADDRESS
+
+        if option_name.endswith(("version", "version_compile_zlib")):
+            return ConfigType.VERSION_NUMBER
+
         if option_name in (
-            "cpu_rt_runtime",
-            "cpu_rt_period",
-            "start_period",
-            "interval",
-            "timeout",
-            "stop_grace_period",
+            "thread_pool_query_threads_per_group",
+            "temptable_max_mmap",
+            "back_log",
+            "caching_sha2_password_digest_rounds",
+            "default_week_format",
+            "div_precision_increment",
+            "ft_max_word_len",
+            "information_schema_stats_expiry",
+            "log_throttle_queries_not_using_indexes",
+            "max_connect_errors",
+            "max_length_for_sort_data",
+            "max_points_in_geometry",
+            "password_history",
+            "password_reuse_interval",
+            "rand_seed1",
+            "rand_seed2",
         ):
-            return ConfigType.TIME
-        if option_name in (
-            "cpu_count",
-            "cpu_shares",
-            "uid",
-            "gid",
-            "retries",
-            "priority",
-            "pids_limit",
-            "sysctls",
+            return ConfigType.NUMBER
+
+        if option_name.endswith(
+            (
+                "max_len",
+                "min_len",
+                "length",
+                "threshold",
+                "threads",
+                "count",
+                "depth",
+                "connections",
+                "offset",
+                "instances",
+            )
         ):
             return ConfigType.NUMBER
-        if option_name == "cpu_percent":
-            return ConfigType.FRACTION
-        if option_name in ("external", "disable", "init", "attachable"):
-            return ConfigType.BOOLEAN
+
+        if option_name.endswith("mode"):
+            return ConfigType.MODE
+
+        if option_name.endswith(
+            (
+                "size",
+                "limit",
+                "cache",
+                "max_allowed_packet",
+                "max_ram",
+                "thread_stack",
+            )
+        ):
+            return ConfigType.SIZE
+
         if option_name in (
-            "mode",
-            "condition",
-            "network_mode",
-            "restart",
-            "userns_mode",
+            "use_secondary_engine",
+            "transaction_isolation",
+            "thread_handling",
+            "completion_type",
+            "concurrent_insert",
+            "default_authentication_plugin",
+            "default_collation_for_utf8mb4",
+            "delay_key_write",
+            "event_scheduler",
+            "authentication_windows_log_level",
+            "internal_tmp_disk_storage_engine",
+            "internal_tmp_mem_storage_engine",
+            "log_error_verbosity",
+            "myisam_recover_options",
+            "myisam_stats_method",
+            "offline_mode",
+            "optimizer_prune_level",
+            "protocol_compression_algorithms",
+            "rbr_exec_mode",
+            "session_track_gtids",
+            "sql_mode",
+            "ssl_fips_mode",
+            "ssl_session_cache_mode",
         ):
             return ConfigType.MODE
-        if option_name in (
-            "dns",
-            "ipv4_address",
-            "ipv6_address",
-            "subnet",
-            "link_local_ips",
-            "host_ip",
-            "ip_range",
-            "gateway",
-            "aux_addresses",
+
+        if option_name.endswith(
+            ("timeout", "time", "delay", "timer", "timestamp")
         ):
-            return ConfigType.IP_ADDRESS
-        if option_name in ("dns_search", "extra_hosts"):
-            return ConfigType.URL
-        if any(option_name.endswith(x) for x in ["user", "username"]):
-            return ConfigType.USERNAME
-        if any(option_name.endswith(x) for x in ["password"]):
-            return ConfigType.PASSWORD
-        if option_name == "platform":
+            return ConfigType.TIME
+
+        if option_name in ("ft_boolean_syntax"):
+            return ConfigType.PATTERN
+
+        if option_name in ("hostname", "shared_memory_base_name"):
+            return ConfigType.NAME
+
+        if option_name in ("license"):
+            return ConfigType.LICENSE
+
+        if option_name.endswith(("pseudo_thread_id", "_id")):
+            return ConfigType.ID
+
+        if option_name in ("version_compile_os"):
             return ConfigType.PLATFORM
-        if option_name == "protocol":
-            return ConfigType.PROTOCOL
 
         return ConfigType.UNKNOWN
```

### Comparing `cfgnet-1.0/src/cfgnet/plugins/concept/docker_plugin.py` & `cfgnet-1.0.1/src/cfgnet/plugins/concept/docker_plugin.py`

 * *Files identical despite different names*

### Comparing `cfgnet-1.0/src/cfgnet/plugins/concept/maven_plugin.py` & `cfgnet-1.0.1/src/cfgnet/plugins/concept/maven_plugin.py`

 * *Files identical despite different names*

### Comparing `cfgnet-1.0/src/cfgnet/plugins/concept/mongodb_plugin.py` & `cfgnet-1.0.1/src/cfgnet/plugins/concept/mongodb_plugin.py`

 * *Files identical despite different names*

### Comparing `cfgnet-1.0/src/cfgnet/plugins/concept/mysql_plugin.py` & `cfgnet-1.0.1/src/cfgnet/plugins/concept/php_plugin.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,166 +8,147 @@
 # This program is distributed in the hope that it will be useful, but WITHOUT
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more
 # details.
 #
 # You should have received a copy of the GNU General Public License along with
 # this program.  If not, see <https://www.gnu.org/licenses/>.
-
-from cfgnet.plugins.file_type.configparser_plugin import ConfigParserPlugin
+from typing import List
 from cfgnet.config_types.config_types import ConfigType
+from cfgnet.plugins.file_type.configparser_plugin import ConfigParserPlugin
 
 
-class MysqlPlugin(ConfigParserPlugin):
+class PhpPlugin(ConfigParserPlugin):
     def __init__(self):
-        super().__init__("mysql")
+        super().__init__("php")
+        self.excluded_keys: List[str] = ["extension"]
 
     def is_responsible(self, abs_file_path) -> bool:
-        if abs_file_path.endswith(("my.cnf", "my.ini")):
+        if abs_file_path.endswith("php.ini"):
             return True
         return False
 
     # pylint: disable=unused-argument,too-many-return-statements
     def get_config_type(self, option_name: str) -> ConfigType:  # noqa: C901
         """
         Find config type based on option name.
 
         Option types included from:
-        https://dev.mysql.com/doc/refman/8.0/en/server-system-variables.html
+        https://www.php.net/manual/de/ini.list.php
+        Not all options are included, but only those for which
+        the type could be easily derived manually.
 
         :param option_name: name of option
         :return: config type
         """
-        option_name = option_name.lower()
-        if option_name.endswith(("dir", "file", "directory", "path")):
-            if not option_name == "core_file":
-                return ConfigType.PATH
-
-        if option_name in (
-            "admin_ssl_ca",
-            "admin_ssl_cert",
-            "admin_ssl_crl",
-            "admin_ssl_key",
-            "log_error",
-            "secure_file_priv",
-            "socket",
-            "ssl_ca",
-            "ssl_cert",
-            "ssl_crl",
-            "ssl_key",
-        ):
-            return ConfigType.PATH
-
-        if option_name in ("port"):
+        if option_name.endswith("port"):
             return ConfigType.PORT
 
-        if option_name == "password":
-            return ConfigType.PASSWORD
-
-        if option_name in ("user", "external_user", "proxy_user"):
+        if option_name.endswith("user"):
             return ConfigType.USERNAME
 
-        if option_name in ("admin_address", "bind_address"):
-            return ConfigType.IP_ADDRESS
+        if option_name.endswith(("password", "default_pw")):
+            return ConfigType.USERNAME
 
-        if option_name.endswith(("version", "version_compile_zlib")):
-            return ConfigType.VERSION_NUMBER
+        if option_name.endswith(
+            ("path", "dir", "file", "root", "filename", "directory", "log")
+        ):
+            return ConfigType.PATH
 
         if option_name in (
-            "thread_pool_query_threads_per_group",
-            "temptable_max_mmap",
-            "back_log",
-            "caching_sha2_password_digest_rounds",
-            "default_week_format",
-            "div_precision_increment",
-            "ft_max_word_len",
-            "information_schema_stats_expiry",
-            "log_throttle_queries_not_using_indexes",
-            "max_connect_errors",
-            "max_length_for_sort_data",
-            "max_points_in_geometry",
-            "password_history",
-            "password_reuse_interval",
-            "rand_seed1",
-            "rand_seed2",
+            "instance_name",
+            "default_db",
+            "name",
+            "user_agent",
+            "timezone",
+            "default_db",
+            "default_charset",
+            "default_socket",
+            "default_host",
+            "SMTP",
         ):
-            return ConfigType.NUMBER
+            return ConfigType.NAME
+
+        if option_name.endswith(("format", "http_output_conv_mimetypes")):
+            return ConfigType.PATTERN
 
         if option_name.endswith(
             (
                 "max_len",
-                "min_len",
-                "length",
-                "threshold",
-                "threads",
-                "count",
-                "depth",
-                "connections",
-                "offset",
-                "instances",
+                "precision",
+                "file_uploads",
+                "number",
             )
         ):
             return ConfigType.NUMBER
 
-        if option_name.endswith("mode"):
-            return ConfigType.MODE
-
-        if option_name.endswith(
-            (
-                "size",
-                "limit",
-                "cache",
-                "max_allowed_packet",
-                "max_ram",
-                "thread_stack",
-            )
+        if option_name in (
+            "max_persistent",
+            "max_links",
+            "regex_retry_limit",
+            "regex_stack_limit",
+            "max_failover_attempts",
+            "default_prefetch",
+            "max_accelerated_files",
+            "jit_blacklist_root_trace",
+            "jit_blacklist_side_trace",
+            "jit_max_loop_unrolls",
+            "jit_max_recursive_calls",
+            "jit_max_recursive_returns",
+            "jit_max_polymorphic_calls",
+            "backtrack_limit",
+            "recursion_limit",
+            "sid_length",
         ):
-            return ConfigType.SIZE
+            return ConfigType.NUMBER
 
         if option_name in (
-            "use_secondary_engine",
-            "transaction_isolation",
-            "thread_handling",
-            "completion_type",
-            "concurrent_insert",
-            "default_authentication_plugin",
-            "default_collation_for_utf8mb4",
-            "delay_key_write",
-            "event_scheduler",
-            "authentication_windows_log_level",
-            "internal_tmp_disk_storage_engine",
-            "internal_tmp_mem_storage_engine",
-            "log_error_verbosity",
-            "myisam_recover_options",
-            "myisam_stats_method",
-            "offline_mode",
-            "optimizer_prune_level",
-            "protocol_compression_algorithms",
-            "rbr_exec_mode",
-            "session_track_gtids",
-            "sql_mode",
-            "ssl_fips_mode",
-            "ssl_session_cache_mode",
+            "memory_limit",
+            "memory_consumption",
+            "interned_strings_buffer",
+            "max_file_size",
+            "wsdl_cache_limit",
         ):
-            return ConfigType.MODE
+            return ConfigType.SIZE
 
-        if option_name.endswith(
-            ("timeout", "time", "delay", "timer", "timestamp")
-        ):
+        if option_name.endswith(("size", "match_max")):
+            return ConfigType.SIZE
+
+        if option_name.endswith(("cache_ttl", "timeout")):
             return ConfigType.TIME
 
-        if option_name in ("ft_boolean_syntax"):
-            return ConfigType.PATTERN
+        if option_name in (
+            "ping_interval",
+            "cookie_lifetime",
+            "cache_expire",
+            "upload_progress.min_freq",
+        ):
+            return ConfigType.TIME
 
-        if option_name in ("hostname", "shared_memory_base_name"):
-            return ConfigType.NAME
+        if option_name in ("default_mimetype"):
+            return ConfigType.MIME
 
-        if option_name in ("license"):
-            return ConfigType.LICENSE
+        if option_name.endswith(
+            (
+                "mode",
+                "error_reporting",
+                "log_mode",
+                "facility",
+                "filter",
+                "binmode",
+            )
+        ):
+            return ConfigType.MODE
 
-        if option_name.endswith(("pseudo_thread_id", "_id")):
-            return ConfigType.ID
+        if option_name in (
+            "wsdl_cache",
+            "i5_allow_commit",
+            "i5_dbcs_allo",
+            "error_level",
+            "optimization_level",
+        ):
+            return ConfigType.MODE
 
-        if option_name in ("version_compile_os"):
-            return ConfigType.PLATFORM
+        if option_name in ("cookie_domain"):
+            return ConfigType.DOMAIN_NAME
 
         return ConfigType.UNKNOWN
```

### Comparing `cfgnet-1.0/src/cfgnet/plugins/concept/nodejs_plugin.py` & `cfgnet-1.0.1/src/cfgnet/plugins/concept/nodejs_plugin.py`

 * *Files identical despite different names*

### Comparing `cfgnet-1.0/src/cfgnet/plugins/concept/php_plugin.py` & `cfgnet-1.0.1/src/cfgnet/plugins/concept/docker_compose_plugin.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,147 +8,188 @@
 # This program is distributed in the hope that it will be useful, but WITHOUT
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more
 # details.
 #
 # You should have received a copy of the GNU General Public License along with
 # this program.  If not, see <https://www.gnu.org/licenses/>.
-from typing import List
+import re
+from yaml.nodes import ScalarNode
 from cfgnet.config_types.config_types import ConfigType
-from cfgnet.plugins.file_type.configparser_plugin import ConfigParserPlugin
 
+from cfgnet.network.nodes import ArtifactNode, OptionNode, ValueNode
+from cfgnet.plugins.file_type.yaml_plugin import YAMLPlugin
+
+
+class DockerComposePlugin(YAMLPlugin):
+    file_name = re.compile(r"docker-compose(.\w+)?.yml")
+    ports = re.compile(r"(?P<in>[0-9]{4}):(?P<out>[0-9]{4})")
 
-class PhpPlugin(ConfigParserPlugin):
     def __init__(self):
-        super().__init__("php")
-        self.excluded_keys: List[str] = ["extension"]
+        super().__init__("docker-compose")
 
-    def is_responsible(self, abs_file_path) -> bool:
-        if abs_file_path.endswith("php.ini"):
+    def is_responsible(self, abs_file_path):
+        if self.file_name.search(abs_file_path):
             return True
         return False
 
-    # pylint: disable=unused-argument,too-many-return-statements
+    def _parse_scalar_node(self, node, parent):
+        if node.value != "":
+            match = DockerComposePlugin.ports.match(node.value)
+            if match is not None:
+                port_in = ValueNode(name=match.group("in"))
+                port_out = ValueNode(name=match.group("out"))
+                option_port_in = OptionNode(
+                    "in", node.start_mark.line + 1, ConfigType.PORT
+                )
+                option_port_out = OptionNode(
+                    "out", node.start_mark.line + 1, ConfigType.PORT
+                )
+                parent.add_child(option_port_in)
+                parent.add_child(option_port_out)
+                option_port_in.add_child(port_in)
+                option_port_out.add_child(port_out)
+            else:
+                if len(node.value.split("=")) == 2:
+                    self._parse_value_assignment(node=node, parent=parent)
+                    return
+
+                name = (
+                    f"{parent.name}:{node.value}"
+                    if parent.config_type == ConfigType.VERSION_NUMBER
+                    else node.value
+                )
+
+                value = ValueNode(name=name)
+
+                if isinstance(parent, ArtifactNode):
+                    option = OptionNode(
+                        "unnamed_option", node.start_mark.line + 1
+                    )
+                    parent.add_child(option)
+                    option.add_child(value)
+                else:
+                    parent.add_child(value)
+
+    def _parse_value_assignment(
+        self, node: ScalarNode, parent: OptionNode
+    ) -> None:
+        value_parts = node.value.split("=")
+        config_type = self.get_config_type(option_name=value_parts[0])
+        variable = OptionNode(
+            name=value_parts[0],
+            location=str(node.start_mark.line + 1),
+            config_type=config_type,
+        )
+        parent.add_child(variable)
+        value = ValueNode(name=value_parts[1])
+        variable.add_child(value)
+
+    # pylint: disable=too-many-return-statements
     def get_config_type(self, option_name: str) -> ConfigType:  # noqa: C901
         """
         Find config type based on option name.
 
-        Option types included from:
-        https://www.php.net/manual/de/ini.list.php
-        Not all options are included, but only those for which
-        the type could be easily derived manually.
-
         :param option_name: name of option
         :return: config type
         """
-        if option_name.endswith("port"):
-            return ConfigType.PORT
+        option_name = option_name.lower()
 
-        if option_name.endswith("user"):
-            return ConfigType.USERNAME
-
-        if option_name.endswith(("password", "default_pw")):
-            return ConfigType.USERNAME
-
-        if option_name.endswith(
-            ("path", "dir", "file", "root", "filename", "directory", "log")
-        ):
+        if option_name == "version":
+            return ConfigType.VERSION_NUMBER
+        if option_name.endswith(("ports", "port", "expose", "PORT", "tmpfs")):
+            return ConfigType.PORT
+        if option_name == "image":
+            return ConfigType.IMAGE
+        if option_name.endswith(("size", "weight", "height")):
+            return ConfigType.SIZE
+        if option_name.endswith(("path", "env_file")):
             return ConfigType.PATH
-
-        if option_name in (
-            "instance_name",
-            "default_db",
-            "name",
-            "user_agent",
-            "timezone",
-            "default_db",
-            "default_charset",
-            "default_socket",
-            "default_host",
-            "SMTP",
+        if option_name == "environment":
+            return ConfigType.ENVIRONMENT
+        if option_name.endswith(("command", "entrypoint", "test")):
+            return ConfigType.COMMAND
+        if option_name.endswith(
+            (
+                "name",
+                "driver",
+                "labels",
+                "hostname",
+                "cap_add",
+                "cap_drop",
+                "cgroup_parent",
+                "source",
+                "container_name",
+                "depends_on",
+                "registry",
+                "service",
+                "external_links",
+                "build",
+            )
         ):
             return ConfigType.NAME
-
-        if option_name.endswith(("format", "http_output_conv_mimetypes")):
-            return ConfigType.PATTERN
-
+        if option_name == "rate":
+            return ConfigType.SPEED
         if option_name.endswith(
             (
-                "max_len",
-                "precision",
-                "file_uploads",
-                "number",
+                "cpu_rt_runtime",
+                "cpu_rt_period",
+                "start_period",
+                "interval",
+                "timeout",
+                "stop_grace_period",
             )
         ):
-            return ConfigType.NUMBER
-
-        if option_name in (
-            "max_persistent",
-            "max_links",
-            "regex_retry_limit",
-            "regex_stack_limit",
-            "max_failover_attempts",
-            "default_prefetch",
-            "max_accelerated_files",
-            "jit_blacklist_root_trace",
-            "jit_blacklist_side_trace",
-            "jit_max_loop_unrolls",
-            "jit_max_recursive_calls",
-            "jit_max_recursive_returns",
-            "jit_max_polymorphic_calls",
-            "backtrack_limit",
-            "recursion_limit",
-            "sid_length",
-        ):
-            return ConfigType.NUMBER
-
-        if option_name in (
-            "memory_limit",
-            "memory_consumption",
-            "interned_strings_buffer",
-            "max_file_size",
-            "wsdl_cache_limit",
-        ):
-            return ConfigType.SIZE
-
-        if option_name.endswith(("size", "match_max")):
-            return ConfigType.SIZE
-
-        if option_name.endswith(("cache_ttl", "timeout")):
             return ConfigType.TIME
-
-        if option_name in (
-            "ping_interval",
-            "cookie_lifetime",
-            "cache_expire",
-            "upload_progress.min_freq",
+        if option_name.endswith(
+            (
+                "cpu_count",
+                "cpu_shares",
+                "uid",
+                "gid",
+                "retries",
+                "priority",
+                "pids_limit",
+                "sysctls",
+            )
         ):
-            return ConfigType.TIME
-
-        if option_name in ("default_mimetype"):
-            return ConfigType.MIME
-
+            return ConfigType.NUMBER
+        if option_name == "cpu_percent":
+            return ConfigType.FRACTION
+        if option_name.endswith(("external", "disable", "init", "attachable")):
+            return ConfigType.BOOLEAN
         if option_name.endswith(
             (
                 "mode",
-                "error_reporting",
-                "log_mode",
-                "facility",
-                "filter",
-                "binmode",
+                "condition",
+                "network_mode",
+                "restart",
+                "userns_mode",
             )
         ):
             return ConfigType.MODE
-
-        if option_name in (
-            "wsdl_cache",
-            "i5_allow_commit",
-            "i5_dbcs_allo",
-            "error_level",
-            "optimization_level",
+        if option_name.endswith(
+            (
+                "dns",
+                "ipv4_address",
+                "ipv6_address",
+                "subnet",
+                "link_local_ips",
+                "host_ip",
+                "ip_range",
+                "gateway",
+                "aux_addresses",
+            )
         ):
-            return ConfigType.MODE
-
-        if option_name in ("cookie_domain"):
-            return ConfigType.DOMAIN_NAME
+            return ConfigType.IP_ADDRESS
+        if option_name.endswith(("dns_search", "extra_hosts")):
+            return ConfigType.URL
+        if option_name.endswith(("user", "username")):
+            return ConfigType.USERNAME
+        if option_name.endswith(("password", "pwd")):
+            return ConfigType.PASSWORD
+        if option_name == "platform":
+            return ConfigType.PLATFORM
+        if option_name == "protocol":
+            return ConfigType.PROTOCOL
 
         return ConfigType.UNKNOWN
```

### Comparing `cfgnet-1.0/src/cfgnet/plugins/concept/poetry_plugin.py` & `cfgnet-1.0.1/src/cfgnet/plugins/concept/poetry_plugin.py`

 * *Files identical despite different names*

### Comparing `cfgnet-1.0/src/cfgnet/plugins/concept/postgresql_plugin.py` & `cfgnet-1.0.1/src/cfgnet/plugins/concept/postgresql_plugin.py`

 * *Files identical despite different names*

### Comparing `cfgnet-1.0/src/cfgnet/plugins/concept/spring_plugin.py` & `cfgnet-1.0.1/src/cfgnet/plugins/concept/spring_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -220,17 +220,16 @@
     def get_config_type(option_name: str) -> ConfigType:
         """
         Get config type based on the option name.
 
         :param name: option name
         :return: ConfigType
         """
-        if any(
-            option_name.endswith(x)
-            for x in [
+        if option_name.endswith(
+            (
                 ".show-sql",
                 ".cache",
                 ".trace",
                 ".await-termination",
                 ".pool.allow-core-thread-timeout",
                 ".wait-for-jobs-to-complete-on-shutdown",
                 ".auto-startup",
@@ -249,111 +248,104 @@
                 ".image.invert",
                 "debug",
                 ".clean-history-on-start",
                 ".register-shutdown-hook",
                 ".aop.auto",
                 ".proxy-target-class",
                 ".enabled",
-            ]
+            )
         ):
             return ConfigType.BOOLEAN
 
-        if any(
-            option_name.endswith(x)
-            for x in [
+        if option_name.endswith(
+            (
                 "size",
                 ".max-file-size",
                 ".total-size-cap",
                 ".image.width",
                 ".max-in-memory-size",
                 ".image.height",
                 ".pool.size",
-            ]
+            )
         ):
             return ConfigType.SIZE
 
-        if any(
-            option_name.endswith(x)
-            for x in [
+        if option_name.endswith(
+            (
                 ".max-history",
                 ".image.bitdepth",
                 ".image.margin",
                 ".core-size",
                 ".pool.max-size",
-            ]
+            )
         ):
             return ConfigType.NUMBER
 
-        if any(
-            option_name.endswith(x)
-            for x in [".pattern.dateformat", ".pattern.file", ".pattern.level"]
+        if option_name.endswith(
+            (".pattern.dateformat", ".pattern.file", ".pattern.level")
         ):
             return ConfigType.PATTERN
 
-        if any(
-            option_name.endswith(x)
-            for x in [
+        if option_name.endswith(
+            (
                 "platform",
                 "-name",
                 ".database",
                 ".authentication-database",
                 ".provider",
                 ".scheduler-name",
                 ".jmx-name",
                 ".name",
                 ".jmx.server",
                 ".active",
                 ".basenames",
                 ".profiles.default",
-            ]
+            )
         ):
             return ConfigType.NAME
 
-        if any(
-            option_name.endswith(x)
-            for x in [
+        if option_name.endswith(
+            (
                 ".location",
                 ".file",
                 ".jdbc.schema",
                 ".config",
                 ".path",
                 ".image",
-            ]
+            )
         ):
             return ConfigType.PATH
 
-        if any(option_name.endswith(x) for x in [".image.pixelmode"]):
+        if option_name.endswith(".image.pixelmode"):
             return ConfigType.MODE
 
-        if any(
-            option_name.endswith(x)
-            for x in [".default-domain", ".host", ".uri", "url"]
+        if option_name.endswith(
+            (".default-domain", ".host", ".uri", "url", "-uri")
         ):
             return ConfigType.URL
 
-        if any(
-            option_name.endswith(x)
-            for x in [
+        if option_name.endswith(
+            (
                 ".timeout-per-shutdown-phase",
                 ".startup-delay",
                 "pool.keep-alive",
                 ".await-termination-period",
-            ]
+            )
         ):
             return ConfigType.TIME
 
-        if any(option_name.endswith(x) for x in [".port"]):
+        if option_name.endswith(".port"):
             return ConfigType.PORT
 
-        if any(option_name.endswith(x) for x in [".username"]):
+        if option_name.endswith(".username"):
             return ConfigType.USERNAME
 
-        if any(option_name.endswith(x) for x in [".password"]):
+        if option_name.endswith(".password"):
             return ConfigType.PASSWORD
 
-        if any(option_name.endswith(x) for x in [".protocol"]):
+        if option_name.endswith(".protocol"):
             return ConfigType.PROTOCOL
 
-        if any(option_name.endswith(x) for x in [".mail"]):
+        if option_name.endswith(".mail"):
             return ConfigType.EMAIL
 
         return ConfigType.UNKNOWN
```

### Comparing `cfgnet-1.0/src/cfgnet/plugins/concept/travis_plugin.py` & `cfgnet-1.0.1/src/cfgnet/plugins/concept/travis_plugin.py`

 * *Files identical despite different names*

### Comparing `cfgnet-1.0/src/cfgnet/plugins/concept/tsconfig_plugin.py` & `cfgnet-1.0.1/src/cfgnet/plugins/concept/tsconfig_plugin.py`

 * *Files identical despite different names*

### Comparing `cfgnet-1.0/src/cfgnet/plugins/file_type/configparser_plugin.py` & `cfgnet-1.0.1/src/cfgnet/plugins/file_type/configparser_plugin.py`

 * *Files identical despite different names*

### Comparing `cfgnet-1.0/src/cfgnet/plugins/file_type/json_plugin.py` & `cfgnet-1.0.1/src/cfgnet/plugins/file_type/json_plugin.py`

 * *Files identical despite different names*

### Comparing `cfgnet-1.0/src/cfgnet/plugins/file_type/toml_plugin.py` & `cfgnet-1.0.1/src/cfgnet/plugins/file_type/toml_plugin.py`

 * *Files identical despite different names*

### Comparing `cfgnet-1.0/src/cfgnet/plugins/file_type/yaml_plugin.py` & `cfgnet-1.0.1/src/cfgnet/plugins/file_type/yaml_plugin.py`

 * *Files identical despite different names*

### Comparing `cfgnet-1.0/src/cfgnet/plugins/plugin.py` & `cfgnet-1.0.1/src/cfgnet/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `cfgnet-1.0/src/cfgnet/plugins/plugin_manager.py` & `cfgnet-1.0.1/src/cfgnet/plugins/plugin_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 from cfgnet.plugins.concept.mysql_plugin import MysqlPlugin
 from cfgnet.plugins.concept.ansible_plugin import AnsiblePlugin
 from cfgnet.plugins.concept.ansible_playbook_plugin import (
     AnsiblePlaybookPlugin,
 )
 from cfgnet.plugins.concept.postgresql_plugin import PostgreSQLPlugin
 from cfgnet.plugins.concept.mongodb_plugin import MongoDBPlugin
+from cfgnet.plugins.concept.django_plugin import DjangoPlugin
 
 
 class PluginManager:
     """Manager for plugin implementations."""
 
     concept_plugins: List[Plugin] = [
         DockerPlugin(),
@@ -55,14 +56,15 @@
         SpringPlugin(),
         ApacheWebserverPlugin(),
         MysqlPlugin(),
         AnsiblePlugin(),
         AnsiblePlaybookPlugin(),
         PostgreSQLPlugin(),
         MongoDBPlugin(),
+        DjangoPlugin(),
     ]
 
     file_type_plugins: List[Plugin] = [
         ConfigParserPlugin(),
         YAMLPlugin(),
         TomlPlugin(),
     ]
```

### Comparing `cfgnet-1.0/src/cfgnet/utility/logger.py` & `cfgnet-1.0.1/src/cfgnet/utility/logger.py`

 * *Files identical despite different names*

### Comparing `cfgnet-1.0/src/cfgnet/vcs/git.py` & `cfgnet-1.0.1/src/cfgnet/vcs/git.py`

 * *Files identical despite different names*

### Comparing `cfgnet-1.0/src/cfgnet/vcs/git_history.py` & `cfgnet-1.0.1/src/cfgnet/vcs/git_history.py`

 * *Files identical despite different names*

### Comparing `cfgnet-1.0/PKG-INFO` & `cfgnet-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfgnet
-Version: 1.0
+Version: 1.0.1
 Summary: A Framework for Tracking Configuration Dependencies Across a Software Project
 Home-page: https://github.com/digital-bauhaus/CfgNet
 License: GPL-3.0+
 Keywords: configuration
 Author: Sebastian Simon
 Author-email: ssimon@informatik.uni-leipzig.de
 Maintainer: Sebastian Simon
@@ -43,15 +43,15 @@
 
 We envision that CfgNet is used within a Git hook (e.g., pre-commit hook) to prevent dependency conflicts during the development and maintenance of software systems. 
 That is, whenever changes are made, CfgNet can check the changes before the actual commit gets pushed to the repository and reports a warning if it has detected possible dependency conflicts. 
 This way, developer can check the changes again and even use the information that CfgNet provides to fix the dependency conflicts.
 
 ## Installation
 
-CfgNet is a package on PyPI
+CfgNet is a package on PyPI. You can install it with the following command:
 
     pip install cfgnet
 
 You can also build it locally with [poetry](https://python-poetry.org/).
 Please refer to the documentation of poetry for further details.
 
 ## Basic Usage
```


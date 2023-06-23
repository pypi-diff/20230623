# Comparing `tmp/vxci-0.0.8.tar.gz` & `tmp/vxci-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vxci-0.0.8.tar", last modified: Fri Sep  9 16:20:01 2022, max compression
+gzip compressed data, was "vxci-0.0.9.tar", last modified: Mon Sep 12 14:29:12 2022, max compression
```

## Comparing `vxci-0.0.8.tar` & `vxci-0.0.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-09 16:20:01.467304 vxci-0.0.8/
--rw-rw-rw-   0 root         (0) root         (0)      193 2022-09-09 16:19:53.000000 vxci-0.0.8/.bumpversion.cfg
--rw-rw-rw-   0 root         (0) root         (0)      179 2022-09-09 16:19:53.000000 vxci-0.0.8/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)      215 2022-09-09 16:19:53.000000 vxci-0.0.8/.editorconfig
--rw-rw-rw-   0 root         (0) root         (0)       52 2022-09-09 16:19:53.000000 vxci-0.0.8/AUTHORS.rst
--rw-rw-rw-   0 root         (0) root         (0)      109 2022-09-09 16:19:53.000000 vxci-0.0.8/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     2718 2022-09-09 16:19:53.000000 vxci-0.0.8/CONTRIBUTING.rst
--rw-rw-rw-   0 root         (0) root         (0)     1285 2022-09-09 16:19:53.000000 vxci-0.0.8/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      364 2022-09-09 16:19:53.000000 vxci-0.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1937 2022-09-09 16:20:01.467304 vxci-0.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2252 2022-09-09 16:19:53.000000 vxci-0.0.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-09 16:20:01.463304 vxci-0.0.8/ci/
--rwxrwxrwx   0 root         (0) root         (0)     2053 2022-09-09 16:19:53.000000 vxci-0.0.8/ci/bootstrap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-09 16:20:01.463304 vxci-0.0.8/docs/
--rw-rw-rw-   0 root         (0) root         (0)       28 2022-09-09 16:19:53.000000 vxci-0.0.8/docs/authors.rst
--rw-rw-rw-   0 root         (0) root         (0)       30 2022-09-09 16:19:53.000000 vxci-0.0.8/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     1358 2022-09-09 16:19:53.000000 vxci-0.0.8/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-09-09 16:19:53.000000 vxci-0.0.8/docs/contributing.rst
--rw-rw-rw-   0 root         (0) root         (0)      245 2022-09-09 16:19:53.000000 vxci-0.0.8/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)       84 2022-09-09 16:19:53.000000 vxci-0.0.8/docs/installation.rst
--rw-rw-rw-   0 root         (0) root         (0)       27 2022-09-09 16:19:53.000000 vxci-0.0.8/docs/readme.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-09 16:20:01.463304 vxci-0.0.8/docs/reference/
--rw-rw-rw-   0 root         (0) root         (0)       56 2022-09-09 16:19:53.000000 vxci-0.0.8/docs/reference/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      108 2022-09-09 16:19:53.000000 vxci-0.0.8/docs/reference/vxci.rst
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-09-09 16:19:53.000000 vxci-0.0.8/docs/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      109 2022-09-09 16:19:53.000000 vxci-0.0.8/docs/spelling_wordlist.txt
--rw-rw-rw-   0 root         (0) root         (0)       56 2022-09-09 16:19:53.000000 vxci-0.0.8/docs/usage.rst
--rw-rw-rw-   0 root         (0) root         (0)      566 2022-09-09 16:20:01.467304 vxci-0.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2766 2022-09-09 16:19:53.000000 vxci-0.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-09 16:20:01.467304 vxci-0.0.8/tests/
--rw-rw-rw-   0 root         (0) root         (0)      187 2022-09-09 16:19:53.000000 vxci-0.0.8/tests/test_vxci.py
--rw-rw-rw-   0 root         (0) root         (0)     1975 2022-09-09 16:19:53.000000 vxci-0.0.8/tox.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-09 16:20:01.467304 vxci-0.0.8/vxci/
--rw-rw-rw-   0 root         (0) root         (0)       22 2022-09-09 16:19:53.000000 vxci-0.0.8/vxci/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3818 2022-09-09 16:19:53.000000 vxci-0.0.8/vxci/checkers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-09 16:20:01.467304 vxci-0.0.8/vxci/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-09 16:19:53.000000 vxci-0.0.8/vxci/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15542 2022-09-09 16:19:53.000000 vxci-0.0.8/vxci/commands/command.py
--rwxrwxrwx   0 root         (0) root         (0)     4548 2022-09-09 16:19:53.000000 vxci-0.0.8/vxci/commands/deployv_tests.py
--rw-rw-rw-   0 root         (0) root         (0)    28590 2022-09-09 16:19:53.000000 vxci-0.0.8/vxci/common.py
--rw-rw-rw-   0 root         (0) root         (0)     3066 2022-09-09 16:19:53.000000 vxci-0.0.8/vxci/coverage.py
--rw-rw-rw-   0 root         (0) root         (0)     4390 2022-09-09 16:19:53.000000 vxci-0.0.8/vxci/get_addons.py
--rw-rw-rw-   0 root         (0) root         (0)     1499 2022-09-09 16:19:53.000000 vxci-0.0.8/vxci/image.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-09 16:20:01.467304 vxci-0.0.8/vxci.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1937 2022-09-09 16:20:01.000000 vxci-0.0.8/vxci.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      793 2022-09-09 16:20:01.000000 vxci-0.0.8/vxci.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-09 16:20:01.000000 vxci-0.0.8/vxci.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2022-09-09 16:20:01.000000 vxci-0.0.8/vxci.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-09 16:20:01.000000 vxci-0.0.8/vxci.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      151 2022-09-09 16:20:01.000000 vxci-0.0.8/vxci.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2022-09-09 16:20:01.000000 vxci-0.0.8/vxci.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-12 14:29:12.795421 vxci-0.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)      193 2022-09-12 14:28:40.000000 vxci-0.0.9/.bumpversion.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      179 2022-09-12 14:26:43.000000 vxci-0.0.9/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)      215 2022-09-12 14:26:43.000000 vxci-0.0.9/.editorconfig
+-rw-rw-rw-   0 root         (0) root         (0)       52 2022-09-12 14:26:43.000000 vxci-0.0.9/AUTHORS.rst
+-rw-rw-rw-   0 root         (0) root         (0)      109 2022-09-12 14:26:43.000000 vxci-0.0.9/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2718 2022-09-12 14:26:43.000000 vxci-0.0.9/CONTRIBUTING.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1285 2022-09-12 14:26:43.000000 vxci-0.0.9/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      364 2022-09-12 14:26:43.000000 vxci-0.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1937 2022-09-12 14:29:12.795421 vxci-0.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2252 2022-09-12 14:28:40.000000 vxci-0.0.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-12 14:29:12.791421 vxci-0.0.9/ci/
+-rwxrwxrwx   0 root         (0) root         (0)     2053 2022-09-12 14:26:43.000000 vxci-0.0.9/ci/bootstrap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-12 14:29:12.791421 vxci-0.0.9/docs/
+-rw-rw-rw-   0 root         (0) root         (0)       28 2022-09-12 14:26:43.000000 vxci-0.0.9/docs/authors.rst
+-rw-rw-rw-   0 root         (0) root         (0)       30 2022-09-12 14:26:43.000000 vxci-0.0.9/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1358 2022-09-12 14:28:40.000000 vxci-0.0.9/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2022-09-12 14:26:43.000000 vxci-0.0.9/docs/contributing.rst
+-rw-rw-rw-   0 root         (0) root         (0)      245 2022-09-12 14:26:43.000000 vxci-0.0.9/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)       84 2022-09-12 14:26:43.000000 vxci-0.0.9/docs/installation.rst
+-rw-rw-rw-   0 root         (0) root         (0)       27 2022-09-12 14:26:43.000000 vxci-0.0.9/docs/readme.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-12 14:29:12.791421 vxci-0.0.9/docs/reference/
+-rw-rw-rw-   0 root         (0) root         (0)       56 2022-09-12 14:26:43.000000 vxci-0.0.9/docs/reference/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      108 2022-09-12 14:26:43.000000 vxci-0.0.9/docs/reference/vxci.rst
+-rw-rw-rw-   0 root         (0) root         (0)       34 2022-09-12 14:26:43.000000 vxci-0.0.9/docs/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      109 2022-09-12 14:26:43.000000 vxci-0.0.9/docs/spelling_wordlist.txt
+-rw-rw-rw-   0 root         (0) root         (0)       56 2022-09-12 14:26:43.000000 vxci-0.0.9/docs/usage.rst
+-rw-rw-rw-   0 root         (0) root         (0)      566 2022-09-12 14:29:12.795421 vxci-0.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2766 2022-09-12 14:28:40.000000 vxci-0.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-12 14:29:12.791421 vxci-0.0.9/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      187 2022-09-12 14:26:43.000000 vxci-0.0.9/tests/test_vxci.py
+-rw-rw-rw-   0 root         (0) root         (0)     1975 2022-09-12 14:26:43.000000 vxci-0.0.9/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-12 14:29:12.791421 vxci-0.0.9/vxci/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2022-09-12 14:28:40.000000 vxci-0.0.9/vxci/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3818 2022-09-12 14:26:43.000000 vxci-0.0.9/vxci/checkers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-12 14:29:12.795421 vxci-0.0.9/vxci/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-12 14:26:43.000000 vxci-0.0.9/vxci/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15905 2022-09-12 14:26:43.000000 vxci-0.0.9/vxci/commands/command.py
+-rwxrwxrwx   0 root         (0) root         (0)     4548 2022-09-12 14:26:43.000000 vxci-0.0.9/vxci/commands/deployv_tests.py
+-rw-rw-rw-   0 root         (0) root         (0)    28759 2022-09-12 14:26:43.000000 vxci-0.0.9/vxci/common.py
+-rw-rw-rw-   0 root         (0) root         (0)     3066 2022-09-12 14:26:43.000000 vxci-0.0.9/vxci/coverage.py
+-rw-rw-rw-   0 root         (0) root         (0)     4390 2022-09-12 14:26:43.000000 vxci-0.0.9/vxci/get_addons.py
+-rw-rw-rw-   0 root         (0) root         (0)     1499 2022-09-12 14:26:43.000000 vxci-0.0.9/vxci/image.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-12 14:29:12.795421 vxci-0.0.9/vxci.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1937 2022-09-12 14:29:12.000000 vxci-0.0.9/vxci.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      793 2022-09-12 14:29:12.000000 vxci-0.0.9/vxci.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-12 14:29:12.000000 vxci-0.0.9/vxci.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2022-09-12 14:29:12.000000 vxci-0.0.9/vxci.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-09-12 14:29:12.000000 vxci-0.0.9/vxci.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      151 2022-09-12 14:29:12.000000 vxci-0.0.9/vxci.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2022-09-12 14:29:12.000000 vxci-0.0.9/vxci.egg-info/top_level.txt
```

### Comparing `vxci-0.0.8/CONTRIBUTING.rst` & `vxci-0.0.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `vxci-0.0.8/LICENSE` & `vxci-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vxci-0.0.8/PKG-INFO` & `vxci-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vxci
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tool created to help with Odoo in the CI environment
 Home-page: https://git.vauxoo.com/devops/vxci
 Author: Vauxoo
 Author-email: info@vauxoo.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `vxci-0.0.8/README.rst` & `vxci-0.0.9/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 .. |version| image:: https://img.shields.io/pypi/v/vxci.svg
     :alt: PyPI Package latest release
     :target: https://pypi.python.org/pypi/vxci
 
 .. |commits-since| image:: https://img.shields.io/github/commits-since/Vauxoo/vxci/v0.2.45.svg
     :alt: Commits since latest release
-    :target: https://github.com/Vauxoo/vxci/compare/v0.0.8...master
+    :target: https://github.com/Vauxoo/vxci/compare/v0.0.9...master
 
 .. |downloads| image:: https://img.shields.io/pypi/dm/vxci.svg
     :alt: PyPI Package monthly downloads
     :target: https://pypi.python.org/pypi/vxci
 
 .. |wheel| image:: https://img.shields.io/pypi/wheel/vxci.svg
     :alt: PyPI Wheel
```

### Comparing `vxci-0.0.8/ci/bootstrap.py` & `vxci-0.0.9/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `vxci-0.0.8/docs/conf.py` & `vxci-0.0.9/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 source_suffix = '.rst'
 master_doc = 'index'
 project = u'Vauxoo Ci Tools'
 year = '2022'
 author = u'Vauxoo'
 copyright = '{0}, {1}'.format(year, author)
-version = release = u'0.0.8'
+version = release = u'0.0.9'
 
 pygments_style = 'trac'
 templates_path = ['.']
 extlinks = {
     'issue': ('https://git.vauxoo.com/devops/vxci/issues/%s', '#'),
     'pr': ('https://git.vauxoo.com/devops/vxci/pull/%s', 'PR #'),
 }
```

### Comparing `vxci-0.0.8/setup.cfg` & `vxci-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `vxci-0.0.8/setup.py` & `vxci-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 
 requirements = open('requirements.txt').readlines()
 
 
 setup(
     name='vxci',
-    version='0.0.8',
+    version='0.0.9',
     license='BSD',
     description='Tool created to help with Odoo in the CI environment',
     long_description='%s\n%s' % (
         re.compile('^.. start-badges.*^.. end-badges', re.M | re.S).sub('', read('README.rst')),
         re.sub(':[a-z]+:`~?(.*?)`', r'``\1``', read('CHANGELOG.rst'))
     ),
     author='Vauxoo',
```

### Comparing `vxci-0.0.8/tox.ini` & `vxci-0.0.9/tox.ini`

 * *Files identical despite different names*

### Comparing `vxci-0.0.8/vxci/checkers.py` & `vxci-0.0.9/vxci/checkers.py`

 * *Files identical despite different names*

### Comparing `vxci-0.0.8/vxci/commands/command.py` & `vxci-0.0.9/vxci/commands/command.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import logging
 import click
 from os import environ, path
+
+from vxbase import logger
+
 from vxci import __version__, common
 from vxci.checkers import check_all
 from vxci.common import check_credentials, prepare, resume_log, notify_orchest
 from vxci.coverage import push_coverage_result
 from vxci.image import push_image
 import signal
 import sys
@@ -13,18 +16,23 @@
 
 signal.signal(signal.SIGTERM, common.reciveSignal)
 signal.signal(signal.SIGINT, common.reciveSignal)
 
 
 @click.group()
 @click.pass_context
-def cli(ctx):
+@click.option('--log_level', default="INFO",
+              help='Set the log level, default to INFO, possible values: INFO, DEBUG, WARNING, ERROR')
+@click.option('--log_file', default=None,
+              help='File where the los will be stored, default to None')
+def cli(ctx, log_level, log_file):
     # ctx.command.config = ctx.parent.command.config
     # parent = ctx.parent.params
-    _logger.info("VxCi: (ver: %d).", __version__)
+    logger.setup_logger("vxci", log_level, log_file)
+    _logger.info("VxCi: (ver: %s).", __version__)
     if not ctx.invoked_subcommand:
         click.echo(ctx.get_help())
 
 
 @cli.command()
 @click.option('--private_deploy_key',
               default=environ.get('PRIVATE_DEPLOY_KEY', False),
@@ -284,15 +292,15 @@
 
 
 @cli.command()
 def push_coverage():
     push_coverage_result()
 
 
-@click.command()
+@cli.command()
 @click.option('--ci_project_name', default=environ.get('CI_PROJECT_NAME'),
               help=("The project name that is currently being built."
                     " Env var: CI_PROJECT_NAME."))
 @click.option('--CI_COMMIT_SHA', default=environ.get('CI_COMMIT_SHA'),
               help=("The commit revision for which project is built."
                     " Env var: CI_COMMIT_SHA."))
 @click.option('--CI_COMMIT_REF_NAME', default=environ.get('CI_COMMIT_REF_NAME'),
```

### Comparing `vxci-0.0.8/vxci/commands/deployv_tests.py` & `vxci-0.0.9/vxci/commands/deployv_tests.py`

 * *Files identical despite different names*

### Comparing `vxci-0.0.8/vxci/common.py` & `vxci-0.0.9/vxci/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -636,15 +636,24 @@
     # Don't complain about null context checking
     if context is None:
     # Don't check obviously not implemented
     raise NotImplementedError
     # We don't really care what happens if fail
     except ImportError:
 
-    """.format(main_app=config_main_app, workdir='/tmp', exclude_var='${EXCLUDE_COVERAGE}')
+fail_under = {min_var}
+precision = {precision_var}
+
+    """.format(
+        main_app=config_main_app,
+        workdir='/tmp',
+        exclude_var='${EXCLUDE_COVERAGE}',
+        min_var='${COVERAGE_MIN-0}',
+        precision_var='${COVERAGE_PRECISION-0}',
+    )
     return coveragerc_content
 
 def show_log(log, title, config):
     _logger.info('='*50)
     _logger.info('%s', title)
     if config['allow_deprecated']:
         _logger.warning('+++ Deprecated methods allowed')
```

### Comparing `vxci-0.0.8/vxci/coverage.py` & `vxci-0.0.9/vxci/coverage.py`

 * *Files identical despite different names*

### Comparing `vxci-0.0.8/vxci/get_addons.py` & `vxci-0.0.9/vxci/get_addons.py`

 * *Files identical despite different names*

### Comparing `vxci-0.0.8/vxci/image.py` & `vxci-0.0.9/vxci/image.py`

 * *Files identical despite different names*

### Comparing `vxci-0.0.8/vxci.egg-info/PKG-INFO` & `vxci-0.0.9/vxci.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vxci
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tool created to help with Odoo in the CI environment
 Home-page: https://git.vauxoo.com/devops/vxci
 Author: Vauxoo
 Author-email: info@vauxoo.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `vxci-0.0.8/vxci.egg-info/SOURCES.txt` & `vxci-0.0.9/vxci.egg-info/SOURCES.txt`

 * *Files identical despite different names*


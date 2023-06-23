# Comparing `tmp/estout-0.0.1.tar.gz` & `tmp/estout-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "estout-0.0.1.tar", last modified: Fri Jun 23 16:25:23 2023, max compression
+gzip compressed data, was "estout-0.0.2.tar", last modified: Fri Jun 23 16:38:18 2023, max compression
```

## Comparing `estout-0.0.1.tar` & `estout-0.0.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-06-23 16:25:23.041069 estout-0.0.1/
-drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-06-23 16:25:23.037069 estout-0.0.1/.github/
-drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-06-23 16:25:23.037069 estout-0.0.1/.github/workflows/
--rw-r--r--   0 imb       (1000) imb       (1000)      242 2023-04-27 10:12:58.000000 estout-0.0.1/.github/workflows/deploy.yaml
--rw-r--r--   0 imb       (1000) imb       (1000)      148 2023-04-27 10:12:58.000000 estout-0.0.1/.github/workflows/test.yaml
--rw-r--r--   0 imb       (1000) imb       (1000)     1618 2023-06-23 13:21:54.000000 estout-0.0.1/.gitignore
--rw-r--r--   0 imb       (1000) imb       (1000)    11337 2023-04-27 10:12:58.000000 estout-0.0.1/LICENSE
--rw-r--r--   0 imb       (1000) imb       (1000)      111 2023-04-27 10:12:58.000000 estout-0.0.1/MANIFEST.in
--rw-rw-r--   0 imb       (1000) imb       (1000)    11311 2023-06-23 16:25:23.041069 estout-0.0.1/PKG-INFO
--rw-r--r--   0 imb       (1000) imb       (1000)    10513 2023-06-23 14:10:11.000000 estout-0.0.1/README.md
-drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-06-23 16:25:23.037069 estout-0.0.1/estout/
--rw-r--r--   0 imb       (1000) imb       (1000)       41 2023-06-22 23:30:00.000000 estout-0.0.1/estout/__init__.py
--rw-r--r--   0 imb       (1000) imb       (1000)     5834 2023-06-23 14:01:27.000000 estout-0.0.1/estout/_modidx.py
--rw-r--r--   0 imb       (1000) imb       (1000)     7659 2023-06-23 14:01:27.000000 estout-0.0.1/estout/core.py
--rw-r--r--   0 imb       (1000) imb       (1000)     1070 2023-06-22 23:30:00.000000 estout-0.0.1/estout/linearmodels_results.py
--rw-r--r--   0 imb       (1000) imb       (1000)     1606 2023-06-22 23:30:00.000000 estout-0.0.1/estout/statsmodels_results.py
--rw-r--r--   0 imb       (1000) imb       (1000)     6836 2023-06-23 13:16:06.000000 estout-0.0.1/estout/utils.py
-drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-06-23 16:25:23.037069 estout-0.0.1/estout.egg-info/
--rw-r--r--   0 imb       (1000) imb       (1000)    11311 2023-06-23 16:25:22.000000 estout-0.0.1/estout.egg-info/PKG-INFO
--rw-r--r--   0 imb       (1000) imb       (1000)      558 2023-06-23 16:25:22.000000 estout-0.0.1/estout.egg-info/SOURCES.txt
--rw-r--r--   0 imb       (1000) imb       (1000)        1 2023-06-23 16:25:22.000000 estout-0.0.1/estout.egg-info/dependency_links.txt
--rw-r--r--   0 imb       (1000) imb       (1000)       34 2023-06-23 16:25:22.000000 estout-0.0.1/estout.egg-info/entry_points.txt
--rw-r--r--   0 imb       (1000) imb       (1000)        1 2023-06-19 18:55:50.000000 estout-0.0.1/estout.egg-info/not-zip-safe
--rw-r--r--   0 imb       (1000) imb       (1000)       61 2023-06-23 16:25:22.000000 estout-0.0.1/estout.egg-info/requires.txt
--rw-r--r--   0 imb       (1000) imb       (1000)        7 2023-06-23 16:25:22.000000 estout-0.0.1/estout.egg-info/top_level.txt
-drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-06-23 16:25:23.041069 estout-0.0.1/nbs/
--rw-r--r--   0 imb       (1000) imb       (1000)    18957 2023-06-23 14:09:35.000000 estout-0.0.1/nbs/00_core.ipynb
--rw-r--r--   0 imb       (1000) imb       (1000)    16776 2023-06-23 13:24:02.000000 estout-0.0.1/nbs/01_utils.ipynb
--rw-r--r--   0 imb       (1000) imb       (1000)      345 2023-06-20 10:59:14.000000 estout-0.0.1/nbs/_quarto.yml
--rw-r--r--   0 imb       (1000) imb       (1000)    31097 2023-06-23 14:09:35.000000 estout-0.0.1/nbs/index.ipynb
--rw-r--r--   0 imb       (1000) imb       (1000)      251 2023-06-22 23:30:01.000000 estout-0.0.1/nbs/nbdev.yml
--rw-r--r--   0 imb       (1000) imb       (1000)      599 2023-06-21 22:34:59.000000 estout-0.0.1/nbs/styles.css
--rw-r--r--   0 imb       (1000) imb       (1000)     1039 2023-06-21 23:01:47.000000 estout-0.0.1/settings.ini
--rw-rw-r--   0 imb       (1000) imb       (1000)       38 2023-06-23 16:25:23.041069 estout-0.0.1/setup.cfg
--rw-r--r--   0 imb       (1000) imb       (1000)     2596 2023-04-27 10:12:58.000000 estout-0.0.1/setup.py
+drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-06-23 16:38:18.601401 estout-0.0.2/
+drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-06-23 16:38:18.597401 estout-0.0.2/.github/
+drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-06-23 16:38:18.597401 estout-0.0.2/.github/workflows/
+-rw-r--r--   0 imb       (1000) imb       (1000)      242 2023-04-27 10:12:58.000000 estout-0.0.2/.github/workflows/deploy.yaml
+-rw-r--r--   0 imb       (1000) imb       (1000)      148 2023-04-27 10:12:58.000000 estout-0.0.2/.github/workflows/test.yaml
+-rw-r--r--   0 imb       (1000) imb       (1000)     1618 2023-06-23 13:21:54.000000 estout-0.0.2/.gitignore
+-rw-r--r--   0 imb       (1000) imb       (1000)    11337 2023-04-27 10:12:58.000000 estout-0.0.2/LICENSE
+-rw-r--r--   0 imb       (1000) imb       (1000)      111 2023-04-27 10:12:58.000000 estout-0.0.2/MANIFEST.in
+-rw-rw-r--   0 imb       (1000) imb       (1000)    11234 2023-06-23 16:38:18.601401 estout-0.0.2/PKG-INFO
+-rw-rw-r--   0 imb       (1000) imb       (1000)    10436 2023-06-23 16:28:14.000000 estout-0.0.2/README.md
+drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-06-23 16:38:18.597401 estout-0.0.2/estout/
+-rw-r--r--   0 imb       (1000) imb       (1000)       41 2023-06-23 16:37:26.000000 estout-0.0.2/estout/__init__.py
+-rw-rw-r--   0 imb       (1000) imb       (1000)     5834 2023-06-23 16:37:26.000000 estout-0.0.2/estout/_modidx.py
+-rw-r--r--   0 imb       (1000) imb       (1000)     7659 2023-06-23 16:37:26.000000 estout-0.0.2/estout/core.py
+-rw-r--r--   0 imb       (1000) imb       (1000)     1070 2023-06-23 16:37:26.000000 estout-0.0.2/estout/linearmodels_results.py
+-rw-r--r--   0 imb       (1000) imb       (1000)     1606 2023-06-23 16:37:26.000000 estout-0.0.2/estout/statsmodels_results.py
+-rw-r--r--   0 imb       (1000) imb       (1000)     6836 2023-06-23 16:37:26.000000 estout-0.0.2/estout/utils.py
+drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-06-23 16:38:18.597401 estout-0.0.2/estout.egg-info/
+-rw-r--r--   0 imb       (1000) imb       (1000)    11234 2023-06-23 16:38:18.000000 estout-0.0.2/estout.egg-info/PKG-INFO
+-rw-r--r--   0 imb       (1000) imb       (1000)      558 2023-06-23 16:38:18.000000 estout-0.0.2/estout.egg-info/SOURCES.txt
+-rw-r--r--   0 imb       (1000) imb       (1000)        1 2023-06-23 16:38:18.000000 estout-0.0.2/estout.egg-info/dependency_links.txt
+-rw-r--r--   0 imb       (1000) imb       (1000)       34 2023-06-23 16:38:18.000000 estout-0.0.2/estout.egg-info/entry_points.txt
+-rw-r--r--   0 imb       (1000) imb       (1000)        1 2023-06-19 18:55:50.000000 estout-0.0.2/estout.egg-info/not-zip-safe
+-rw-r--r--   0 imb       (1000) imb       (1000)       61 2023-06-23 16:38:18.000000 estout-0.0.2/estout.egg-info/requires.txt
+-rw-r--r--   0 imb       (1000) imb       (1000)        7 2023-06-23 16:38:18.000000 estout-0.0.2/estout.egg-info/top_level.txt
+drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-06-23 16:38:18.601401 estout-0.0.2/nbs/
+-rw-r--r--   0 imb       (1000) imb       (1000)    18957 2023-06-23 14:09:35.000000 estout-0.0.2/nbs/00_core.ipynb
+-rw-r--r--   0 imb       (1000) imb       (1000)    16776 2023-06-23 13:24:02.000000 estout-0.0.2/nbs/01_utils.ipynb
+-rw-r--r--   0 imb       (1000) imb       (1000)      345 2023-06-20 10:59:14.000000 estout-0.0.2/nbs/_quarto.yml
+-rw-r--r--   0 imb       (1000) imb       (1000)    30917 2023-06-23 16:27:57.000000 estout-0.0.2/nbs/index.ipynb
+-rw-r--r--   0 imb       (1000) imb       (1000)      251 2023-06-23 16:27:57.000000 estout-0.0.2/nbs/nbdev.yml
+-rw-r--r--   0 imb       (1000) imb       (1000)      599 2023-06-21 22:34:59.000000 estout-0.0.2/nbs/styles.css
+-rw-r--r--   0 imb       (1000) imb       (1000)      898 2023-06-23 16:37:26.000000 estout-0.0.2/settings.ini
+-rw-rw-r--   0 imb       (1000) imb       (1000)       38 2023-06-23 16:38:18.601401 estout-0.0.2/setup.cfg
+-rw-r--r--   0 imb       (1000) imb       (1000)     2596 2023-04-27 10:12:58.000000 estout-0.0.2/setup.py
```

### Comparing `estout-0.0.1/.gitignore` & `estout-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `estout-0.0.1/LICENSE` & `estout-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `estout-0.0.1/PKG-INFO` & `estout-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: estout
-Version: 0.0.1
+Version: 0.0.2
 Summary: Collect regression results and export them to LaTex and pdf
 Home-page: https://github.com/ionmihai/estout
 Author: Mihai Ion
 Author-email: mihaiion@email.arizona.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -20,17 +20,14 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # estout
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
-This file will become your README and also the index of your
-documentation.
-
 ## Install
 
 ``` sh
 pip install estout
 ```
 
 ## How to use
```

### Comparing `estout-0.0.1/README.md` & `estout-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 # estout
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
-This file will become your README and also the index of your
-documentation.
-
 ## Install
 
 ``` sh
 pip install estout
 ```
 
 ## How to use
```

### Comparing `estout-0.0.1/estout/_modidx.py` & `estout-0.0.2/estout/_modidx.py`

 * *Files identical despite different names*

### Comparing `estout-0.0.1/estout/core.py` & `estout-0.0.2/estout/core.py`

 * *Files identical despite different names*

### Comparing `estout-0.0.1/estout/linearmodels_results.py` & `estout-0.0.2/estout/linearmodels_results.py`

 * *Files identical despite different names*

### Comparing `estout-0.0.1/estout/statsmodels_results.py` & `estout-0.0.2/estout/statsmodels_results.py`

 * *Files identical despite different names*

### Comparing `estout-0.0.1/estout/utils.py` & `estout-0.0.2/estout/utils.py`

 * *Files identical despite different names*

### Comparing `estout-0.0.1/estout.egg-info/PKG-INFO` & `estout-0.0.2/estout.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: estout
-Version: 0.0.1
+Version: 0.0.2
 Summary: Collect regression results and export them to LaTex and pdf
 Home-page: https://github.com/ionmihai/estout
 Author: Mihai Ion
 Author-email: mihaiion@email.arizona.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -20,17 +20,14 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 # estout
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
-This file will become your README and also the index of your
-documentation.
-
 ## Install
 
 ``` sh
 pip install estout
 ```
 
 ## How to use
```

### Comparing `estout-0.0.1/estout.egg-info/SOURCES.txt` & `estout-0.0.2/estout.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `estout-0.0.1/nbs/00_core.ipynb` & `estout-0.0.2/nbs/00_core.ipynb`

 * *Files identical despite different names*

### Comparing `estout-0.0.1/nbs/01_utils.ipynb` & `estout-0.0.2/nbs/01_utils.ipynb`

 * *Files identical despite different names*

### Comparing `estout-0.0.1/nbs/index.ipynb` & `estout-0.0.2/nbs/index.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9970238095238095%*

 * *Differences: {"'cells'": '{delete: [2]}'}*

```diff
@@ -22,22 +22,14 @@
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "This file will become your README and also the index of your documentation."
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
                 "## Install"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
```

### Comparing `estout-0.0.1/nbs/styles.css` & `estout-0.0.2/nbs/styles.css`

 * *Files identical despite different names*

### Comparing `estout-0.0.1/settings.ini` & `estout-0.0.2/settings.ini`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,37 @@
 [DEFAULT]
-# All sections below are required unless otherwise specified.
-# See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
-
-### Python library ###
 repo = estout
-lib_name = %(repo)s
-version = 0.0.1
+lib_name = estout
+version = 0.0.2
 min_python = 3.7
 license = apache2
 black_formatting = False
-
-### nbdev ###
 doc_path = _docs
 lib_path = estout
 nbs_path = nbs
 recursive = True
 tst_flags = notest
 put_version_in_init = True
-
-### Docs ###
 branch = main
 custom_sidebar = False
 custom_quarto_yml = True
-doc_host = https://%(user)s.github.io
-doc_baseurl = /%(repo)s
-git_url = https://github.com/%(user)s/%(repo)s
-title = %(lib_name)s
-
-### PyPI ###
+doc_host = https://ionmihai.github.io
+doc_baseurl = /estout
+git_url = https://github.com/ionmihai/estout
+title = estout
 audience = Developers
 author = Mihai Ion
 author_email = mihaiion@email.arizona.edu
-copyright = 2023 onwards, %(author)s
+copyright = 2023 onwards, Mihai Ion
 description = Collect regression results and export them to LaTex and pdf
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = ionmihai
-
-### Optional ###
 requirements = fastcore pandas numpy linearmodels statsmodels jinja2
-#dev_requirements = 
-# console_scripts =
+readme_nb = index.ipynb
+allowed_metadata_keys = 
+allowed_cell_metadata_keys = 
+jupyter_hooks = True
+clean_ids = True
+clear_all = False
+
```

### Comparing `estout-0.0.1/setup.py` & `estout-0.0.2/setup.py`

 * *Files identical despite different names*


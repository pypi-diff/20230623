# Comparing `tmp/pix2vec-0.1.0.tar.gz` & `tmp/pix2vec-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pix2vec-0.1.0.tar", last modified: Wed Jun 21 10:09:43 2023, max compression
+gzip compressed data, was "dist/pix2vec-0.1.1.tar", last modified: Fri Jun 23 19:47:44 2023, max compression
```

## Comparing `pix2vec-0.1.0.tar` & `pix2vec-0.1.1.tar`

### file list

```diff
@@ -1,38 +1,52 @@
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-21 10:09:43.648749 pix2vec-0.1.0/
--rw-r--r--   0 alf        (501) staff       (20)      212 2023-06-21 09:38:53.000000 pix2vec-0.1.0/AUTHORS.rst
--rw-r--r--   0 alf        (501) staff       (20)     3540 2023-06-21 09:12:34.000000 pix2vec-0.1.0/CONTRIBUTING.rst
--rw-r--r--   0 alf        (501) staff       (20)       89 2023-06-21 09:12:34.000000 pix2vec-0.1.0/HISTORY.rst
--rw-r--r--   0 alf        (501) staff       (20)     1564 2023-06-21 09:12:34.000000 pix2vec-0.1.0/LICENSE
--rw-r--r--   0 alf        (501) staff       (20)      262 2023-06-21 09:12:34.000000 pix2vec-0.1.0/MANIFEST.in
--rw-r--r--   0 alf        (501) staff       (20)     2295 2023-06-21 09:12:34.000000 pix2vec-0.1.0/Makefile
--rw-r--r--   0 alf        (501) staff       (20)     2248 2023-06-21 10:09:43.648918 pix2vec-0.1.0/PKG-INFO
--rw-r--r--   0 alf        (501) staff       (20)     1402 2023-06-21 09:57:30.000000 pix2vec-0.1.0/README.rst
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-21 10:09:43.643408 pix2vec-0.1.0/docs/
--rw-r--r--   0 alf        (501) staff       (20)      608 2023-06-21 09:12:34.000000 pix2vec-0.1.0/docs/Makefile
--rw-r--r--   0 alf        (501) staff       (20)       28 2023-06-21 09:12:34.000000 pix2vec-0.1.0/docs/authors.rst
--rwxr-xr-x   0 alf        (501) staff       (20)     4828 2023-06-21 09:12:34.000000 pix2vec-0.1.0/docs/conf.py
--rw-r--r--   0 alf        (501) staff       (20)       33 2023-06-21 09:12:34.000000 pix2vec-0.1.0/docs/contributing.rst
--rw-r--r--   0 alf        (501) staff       (20)       28 2023-06-21 09:12:34.000000 pix2vec-0.1.0/docs/history.rst
--rw-r--r--   0 alf        (501) staff       (20)      312 2023-06-21 09:12:34.000000 pix2vec-0.1.0/docs/index.rst
--rw-r--r--   0 alf        (501) staff       (20)     1138 2023-06-21 09:12:34.000000 pix2vec-0.1.0/docs/installation.rst
--rw-r--r--   0 alf        (501) staff       (20)      805 2023-06-21 09:12:34.000000 pix2vec-0.1.0/docs/make.bat
--rw-r--r--   0 alf        (501) staff       (20)       27 2023-06-21 09:12:34.000000 pix2vec-0.1.0/docs/readme.rst
--rw-r--r--   0 alf        (501) staff       (20)       77 2023-06-21 09:12:34.000000 pix2vec-0.1.0/docs/usage.rst
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-21 10:09:43.645063 pix2vec-0.1.0/pix2vec/
--rw-r--r--   0 alf        (501) staff       (20)      147 2023-06-21 09:12:34.000000 pix2vec-0.1.0/pix2vec/__init__.py
--rw-r--r--   0 alf        (501) staff       (20)      757 2023-06-21 09:35:00.000000 pix2vec-0.1.0/pix2vec/cli.py
--rw-r--r--   0 alf        (501) staff       (20)     6683 2023-06-21 09:32:22.000000 pix2vec-0.1.0/pix2vec/pix2vec.py
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-21 10:09:43.647369 pix2vec-0.1.0/pix2vec.egg-info/
--rw-r--r--   0 alf        (501) staff       (20)     2248 2023-06-21 10:09:43.000000 pix2vec-0.1.0/pix2vec.egg-info/PKG-INFO
--rw-r--r--   0 alf        (501) staff       (20)      575 2023-06-21 10:09:43.000000 pix2vec-0.1.0/pix2vec.egg-info/SOURCES.txt
--rw-r--r--   0 alf        (501) staff       (20)        1 2023-06-21 10:09:43.000000 pix2vec-0.1.0/pix2vec.egg-info/dependency_links.txt
--rw-r--r--   0 alf        (501) staff       (20)       45 2023-06-21 10:09:43.000000 pix2vec-0.1.0/pix2vec.egg-info/entry_points.txt
--rw-r--r--   0 alf        (501) staff       (20)        1 2023-06-21 09:26:55.000000 pix2vec-0.1.0/pix2vec.egg-info/not-zip-safe
--rw-r--r--   0 alf        (501) staff       (20)        8 2023-06-21 10:09:43.000000 pix2vec-0.1.0/pix2vec.egg-info/top_level.txt
--rw-r--r--   0 alf        (501) staff       (20)      145 2023-06-21 09:42:07.000000 pix2vec-0.1.0/requirements_dev.txt
--rw-r--r--   0 alf        (501) staff       (20)      379 2023-06-21 10:09:43.649516 pix2vec-0.1.0/setup.cfg
--rw-r--r--   0 alf        (501) staff       (20)     1413 2023-06-21 09:12:34.000000 pix2vec-0.1.0/setup.py
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-21 10:09:43.648241 pix2vec-0.1.0/tests/
--rw-r--r--   0 alf        (501) staff       (20)       37 2023-06-21 09:12:34.000000 pix2vec-0.1.0/tests/__init__.py
--rw-r--r--   0 alf        (501) staff       (20)      387 2023-06-21 09:12:34.000000 pix2vec-0.1.0/tests/test_pix2vec.py
--rw-r--r--   0 alf        (501) staff       (20)      268 2023-06-21 09:12:34.000000 pix2vec-0.1.0/tox.ini
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-23 19:47:44.000000 pix2vec-0.1.1/
+-rw-r--r--   0 alf        (501) staff       (20)     5394 2023-06-23 19:47:44.000000 pix2vec-0.1.1/PKG-INFO
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-23 19:47:44.000000 pix2vec-0.1.1/pix2vec.egg-info/
+-rw-r--r--   0 alf        (501) staff       (20)     5394 2023-06-23 19:47:44.000000 pix2vec-0.1.1/pix2vec.egg-info/PKG-INFO
+-rw-r--r--   0 alf        (501) staff       (20)        1 2023-06-21 09:26:55.000000 pix2vec-0.1.1/pix2vec.egg-info/not-zip-safe
+-rw-r--r--   0 alf        (501) staff       (20)      818 2023-06-23 19:47:44.000000 pix2vec-0.1.1/pix2vec.egg-info/SOURCES.txt
+-rw-r--r--   0 alf        (501) staff       (20)       46 2023-06-23 19:47:44.000000 pix2vec-0.1.1/pix2vec.egg-info/entry_points.txt
+-rw-r--r--   0 alf        (501) staff       (20)        8 2023-06-23 19:47:44.000000 pix2vec-0.1.1/pix2vec.egg-info/top_level.txt
+-rw-r--r--   0 alf        (501) staff       (20)        1 2023-06-23 19:47:44.000000 pix2vec-0.1.1/pix2vec.egg-info/dependency_links.txt
+-rw-r--r--   0 alf        (501) staff       (20)     1564 2023-06-21 09:12:34.000000 pix2vec-0.1.1/LICENSE
+-rw-r--r--   0 alf        (501) staff       (20)     3524 2023-06-22 08:52:00.000000 pix2vec-0.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 alf        (501) staff       (20)     2295 2023-06-21 09:12:34.000000 pix2vec-0.1.1/Makefile
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-23 19:47:44.000000 pix2vec-0.1.1/tests/
+-rw-r--r--   0 alf        (501) staff       (20)       37 2023-06-21 09:12:34.000000 pix2vec-0.1.1/tests/__init__.py
+-rw-r--r--   0 alf        (501) staff       (20)      387 2023-06-21 09:12:34.000000 pix2vec-0.1.1/tests/test_pix2vec.py
+-rw-r--r--   0 alf        (501) staff       (20)      262 2023-06-21 09:12:34.000000 pix2vec-0.1.1/MANIFEST.in
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-23 19:47:44.000000 pix2vec-0.1.1/docs/
+-rw-r--r--   0 alf        (501) staff       (20)      551 2023-06-22 16:49:30.000000 pix2vec-0.1.1/docs/index.rst
+-rw-r--r--   0 alf        (501) staff       (20)       33 2023-06-21 09:12:34.000000 pix2vec-0.1.1/docs/contributing.rst
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-23 19:47:44.000000 pix2vec-0.1.1/docs/images/
+-rw-r--r--   0 alf        (501) staff       (20)   948490 2023-06-23 18:50:51.000000 pix2vec-0.1.1/docs/images/m3cube-c.png
+-rw-r--r--   0 alf        (501) staff       (20)   530877 2023-06-21 13:49:17.000000 pix2vec-0.1.1/docs/images/m3cube-a.png
+-rw-r--r--   0 alf        (501) staff       (20)      608 2023-06-21 09:12:34.000000 pix2vec-0.1.1/docs/Makefile
+-rwxr-xr-x   0 alf        (501) staff       (20)     4876 2023-06-21 10:42:06.000000 pix2vec-0.1.1/docs/conf.py
+-rw-r--r--   0 alf        (501) staff       (20)       58 2023-06-23 19:26:42.000000 pix2vec-0.1.1/docs/modules.rst
+-rw-r--r--   0 alf        (501) staff       (20)      181 2023-06-21 14:04:55.000000 pix2vec-0.1.1/docs/usage.rst
+-rw-r--r--   0 alf        (501) staff       (20)      805 2023-06-21 09:12:34.000000 pix2vec-0.1.1/docs/make.bat
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-23 19:47:44.000000 pix2vec-0.1.1/docs/_build/
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-23 19:47:44.000000 pix2vec-0.1.1/docs/_build/html/
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-23 19:47:44.000000 pix2vec-0.1.1/docs/_build/html/_static/
+-rw-r--r--   0 alf        (501) staff       (20)       90 2023-06-23 19:26:02.000000 pix2vec-0.1.1/docs/_build/html/_static/plus.png
+-rw-r--r--   0 alf        (501) staff       (20)      286 2023-06-23 19:26:02.000000 pix2vec-0.1.1/docs/_build/html/_static/file.png
+-rw-r--r--   0 alf        (501) staff       (20)       90 2023-06-23 19:26:02.000000 pix2vec-0.1.1/docs/_build/html/_static/minus.png
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-23 19:47:44.000000 pix2vec-0.1.1/docs/_build/html/_images/
+-rw-r--r--   0 alf        (501) staff       (20)   530877 2023-06-21 13:49:17.000000 pix2vec-0.1.1/docs/_build/html/_images/m3cube-a.png
+-rw-r--r--   0 alf        (501) staff       (20)       28 2023-06-21 09:12:34.000000 pix2vec-0.1.1/docs/history.rst
+-rw-r--r--   0 alf        (501) staff       (20)     1114 2023-06-22 08:51:18.000000 pix2vec-0.1.1/docs/installation.rst
+-rw-r--r--   0 alf        (501) staff       (20)       28 2023-06-21 09:12:34.000000 pix2vec-0.1.1/docs/authors.rst
+-rw-r--r--   0 alf        (501) staff       (20)       27 2023-06-21 09:12:34.000000 pix2vec-0.1.1/docs/readme.rst
+-rw-r--r--   0 alf        (501) staff       (20)      423 2023-06-23 19:26:42.000000 pix2vec-0.1.1/docs/pix2vec.rst
+-rw-r--r--   0 alf        (501) staff       (20)     1413 2023-06-23 19:46:19.000000 pix2vec-0.1.1/setup.py
+-rw-r--r--   0 alf        (501) staff       (20)       89 2023-06-21 09:12:34.000000 pix2vec-0.1.1/HISTORY.rst
+-rw-r--r--   0 alf        (501) staff       (20)      268 2023-06-21 09:12:34.000000 pix2vec-0.1.1/tox.ini
+-rw-r--r--   0 alf        (501) staff       (20)      212 2023-06-21 09:38:53.000000 pix2vec-0.1.1/AUTHORS.rst
+-rw-r--r--   0 alf        (501) staff       (20)      379 2023-06-23 19:47:44.000000 pix2vec-0.1.1/setup.cfg
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-23 19:47:44.000000 pix2vec-0.1.1/pix2vec/
+-rw-r--r--   0 alf        (501) staff       (20)     2180 2023-06-22 16:05:48.000000 pix2vec-0.1.1/pix2vec/__init__.py
+-rw-r--r--   0 alf        (501) staff       (20)     1785 2023-06-21 13:22:16.000000 pix2vec-0.1.1/pix2vec/cli.py
+-rw-r--r--   0 alf        (501) staff       (20)     6857 2023-06-22 16:17:11.000000 pix2vec-0.1.1/pix2vec/pix2vec.py
+-rw-r--r--   0 alf        (501) staff       (20)     3605 2023-06-23 19:15:56.000000 pix2vec-0.1.1/README.rst
+-rw-r--r--   0 alf        (501) staff       (20)      205 2023-06-21 10:32:57.000000 pix2vec-0.1.1/.readthedocs.yaml
+-rw-r--r--   0 alf        (501) staff       (20)      185 2023-06-23 19:30:11.000000 pix2vec-0.1.1/requirements_dev.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pix2vec-0.1.0/CONTRIBUTING.rst` & `pix2vec-0.1.1/CONTRIBUTING.rst`

 * *Files 3% similar despite different names*

```diff
@@ -34,16 +34,16 @@
 
 Look through the GitHub issues for features. Anything tagged with "enhancement"
 and "help wanted" is open to whoever wants to implement it.
 
 Write Documentation
 ~~~~~~~~~~~~~~~~~~~
 
-Pixel to Vector could always use more documentation, whether as part of the
-official Pixel to Vector docs, in docstrings, or even on the web in blog posts,
+pix2vec could always use more documentation, whether as part of the
+official pix2vec docs, in docstrings, or even on the web in blog posts,
 articles, and such.
 
 Submit Feedback
 ~~~~~~~~~~~~~~~
 
 The best way to send feedback is to file an issue at https://github.com/afrigeri/pix2vec/issues.
```

### Comparing `pix2vec-0.1.0/LICENSE` & `pix2vec-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.0/Makefile` & `pix2vec-0.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.0/docs/Makefile` & `pix2vec-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.0/docs/conf.py` & `pix2vec-0.1.1/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 source_suffix = '.rst'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
 project = 'Pixel to Vector'
-copyright = "2023, Alessandro Frigeri"
+copyright = "2023, Alessandro Frigeri - Istituto Nazionale di Astrofisica INAF"
 author = "Alessandro Frigeri"
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The short X.Y version.
@@ -79,15 +79,15 @@
 
 
 # -- Options for HTML output -------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = 'alabaster'
+html_theme = 'sphinx_rtd_theme'
 
 # Theme options are theme-specific and customize the look and feel of a
 # theme further.  For a list of options available for each theme, see the
 # documentation.
 #
 # html_theme_options = {}
```

### Comparing `pix2vec-0.1.0/docs/installation.rst` & `pix2vec-0.1.1/docs/installation.rst`

 * *Files 13% similar despite different names*

```diff
@@ -4,33 +4,33 @@
 Installation
 ============
 
 
 Stable release
 --------------
 
-To install Pixel to Vector, run this command in your terminal:
+To install pix2vec, run this command in your terminal:
 
 .. code-block:: console
 
     $ pip install pix2vec
 
-This is the preferred method to install Pixel to Vector, as it will always install the most recent stable release.
+This is the preferred method to install pix2vec, as it will always install the most recent stable release.
 
 If you don't have `pip`_ installed, this `Python installation guide`_ can guide
 you through the process.
 
 .. _pip: https://pip.pypa.io
 .. _Python installation guide: http://docs.python-guide.org/en/latest/starting/installation/
 
 
 From sources
 ------------
 
-The sources for Pixel to Vector can be downloaded from the `Github repo`_.
+The sources for pix2vec can be downloaded from the `Github repo`_.
 
 You can either clone the public repository:
 
 .. code-block:: console
 
     $ git clone git://github.com/afrigeri/pix2vec
```

### Comparing `pix2vec-0.1.0/docs/make.bat` & `pix2vec-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.0/setup.py` & `pix2vec-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,10 +40,10 @@
     include_package_data=True,
     keywords='pix2vec',
     name='pix2vec',
     packages=find_packages(include=['pix2vec', 'pix2vec.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/afrigeri/pix2vec',
-    version='0.1.0',
+    version='0.1.1',
     zip_safe=False,
 )
```


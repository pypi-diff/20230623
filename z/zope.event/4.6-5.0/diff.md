# Comparing `tmp/zope.event-4.6.tar.gz` & `tmp/zope.event-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zope.event-4.6.tar", last modified: Thu Dec 15 07:21:11 2022, max compression
+gzip compressed data, was "zope.event-5.0.tar", last modified: Fri Jun 23 06:28:27 2023, max compression
```

## Comparing `zope.event-4.6.tar` & `zope.event-5.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-12-15 07:21:11.386721 zope.event-4.6/
--rw-r--r--   0 mac        (513) staff       (20)     1913 2022-12-15 07:21:08.000000 zope.event-4.6/CHANGES.rst
--rw-r--r--   0 mac        (513) staff       (20)      804 2022-12-15 07:21:08.000000 zope.event-4.6/CONTRIBUTING.md
--rw-r--r--   0 mac        (513) staff       (20)       32 2022-12-15 07:21:08.000000 zope.event-4.6/COPYRIGHT.txt
--rw-r--r--   0 mac        (513) staff       (20)     2070 2022-12-15 07:21:08.000000 zope.event-4.6/LICENSE.txt
--rw-r--r--   0 mac        (513) staff       (20)      344 2022-12-15 07:21:08.000000 zope.event-4.6/MANIFEST.in
--rw-r--r--   0 mac        (513) staff       (20)     4440 2022-12-15 07:21:11.386886 zope.event-4.6/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)     1075 2022-12-15 07:21:08.000000 zope.event-4.6/README.rst
--rw-r--r--   0 mac        (513) staff       (20)       96 2022-12-15 07:21:08.000000 zope.event-4.6/buildout.cfg
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-12-15 07:21:11.380865 zope.event-4.6/docs/
--rw-r--r--   0 mac        (513) staff       (20)     3132 2022-12-15 07:21:08.000000 zope.event-4.6/docs/Makefile
--rw-r--r--   0 mac        (513) staff       (20)      272 2022-12-15 07:21:08.000000 zope.event-4.6/docs/api.rst
--rw-r--r--   0 mac        (513) staff       (20)      195 2022-12-15 07:21:08.000000 zope.event-4.6/docs/classhandler.rst
--rw-r--r--   0 mac        (513) staff       (20)     6908 2022-12-15 07:21:08.000000 zope.event-4.6/docs/conf.py
--rw-r--r--   0 mac        (513) staff       (20)     8545 2022-12-15 07:21:08.000000 zope.event-4.6/docs/hacking.rst
--rw-r--r--   0 mac        (513) staff       (20)      994 2022-12-15 07:21:08.000000 zope.event-4.6/docs/index.rst
--rw-r--r--   0 mac        (513) staff       (20)     3077 2022-12-15 07:21:08.000000 zope.event-4.6/docs/make.bat
--rw-r--r--   0 mac        (513) staff       (20)      493 2022-12-15 07:21:08.000000 zope.event-4.6/docs/theory.rst
--rw-r--r--   0 mac        (513) staff       (20)     3189 2022-12-15 07:21:08.000000 zope.event-4.6/docs/usage.rst
--rw-r--r--   0 mac        (513) staff       (20)      469 2022-12-15 07:21:11.387738 zope.event-4.6/setup.cfg
--rw-r--r--   0 mac        (513) staff       (20)     3064 2022-12-15 07:21:08.000000 zope.event-4.6/setup.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-12-15 07:21:11.370383 zope.event-4.6/src/
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-12-15 07:21:11.381444 zope.event-4.6/src/zope/
--rw-r--r--   0 mac        (513) staff       (20)       76 2022-12-15 07:21:08.000000 zope.event-4.6/src/zope/__init__.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-12-15 07:21:11.386407 zope.event-4.6/src/zope/event/
--rw-r--r--   0 mac        (513) staff       (20)     1142 2022-12-15 07:21:08.000000 zope.event-4.6/src/zope/event/__init__.py
--rw-r--r--   0 mac        (513) staff       (20)     1820 2022-12-15 07:21:08.000000 zope.event-4.6/src/zope/event/classhandler.py
--rw-r--r--   0 mac        (513) staff       (20)     1871 2022-12-15 07:21:08.000000 zope.event-4.6/src/zope/event/tests.py
-drwxr-xr-x   0 mac        (513) staff       (20)        0 2022-12-15 07:21:11.384949 zope.event-4.6/src/zope.event.egg-info/
--rw-r--r--   0 mac        (513) staff       (20)     4440 2022-12-15 07:21:10.000000 zope.event-4.6/src/zope.event.egg-info/PKG-INFO
--rw-r--r--   0 mac        (513) staff       (20)      631 2022-12-15 07:21:11.000000 zope.event-4.6/src/zope.event.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2022-12-15 07:21:10.000000 zope.event-4.6/src/zope.event.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2022-12-15 07:21:10.000000 zope.event-4.6/src/zope.event.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (513) staff       (20)        1 2022-12-15 07:21:10.000000 zope.event-4.6/src/zope.event.egg-info/not-zip-safe
--rw-r--r--   0 mac        (513) staff       (20)       50 2022-12-15 07:21:10.000000 zope.event-4.6/src/zope.event.egg-info/requires.txt
--rw-r--r--   0 mac        (513) staff       (20)        5 2022-12-15 07:21:10.000000 zope.event-4.6/src/zope.event.egg-info/top_level.txt
--rw-r--r--   0 mac        (513) staff       (20)     1934 2022-12-15 07:21:08.000000 zope.event-4.6/tox.ini
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-06-23 06:28:27.769002 zope.event-5.0/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1991 2023-06-23 06:28:27.000000 zope.event-5.0/CHANGES.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      804 2023-06-23 06:28:27.000000 zope.event-5.0/CONTRIBUTING.md
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2023-06-23 06:28:27.000000 zope.event-5.0/COPYRIGHT.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2023-06-23 06:28:27.000000 zope.event-5.0/LICENSE.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      344 2023-06-23 06:28:27.000000 zope.event-5.0/MANIFEST.in
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4323 2023-06-23 06:28:27.769069 zope.event-5.0/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1075 2023-06-23 06:28:27.000000 zope.event-5.0/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)       96 2023-06-23 06:28:27.000000 zope.event-5.0/buildout.cfg
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-06-23 06:28:27.767232 zope.event-5.0/docs/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3132 2023-06-23 06:28:27.000000 zope.event-5.0/docs/Makefile
+-rw-r--r--   0 m.howitz   (502) staff       (20)      272 2023-06-23 06:28:27.000000 zope.event-5.0/docs/api.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      195 2023-06-23 06:28:27.000000 zope.event-5.0/docs/classhandler.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     6908 2023-06-23 06:28:27.000000 zope.event-5.0/docs/conf.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     8545 2023-06-23 06:28:27.000000 zope.event-5.0/docs/hacking.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      994 2023-06-23 06:28:27.000000 zope.event-5.0/docs/index.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3077 2023-06-23 06:28:27.000000 zope.event-5.0/docs/make.bat
+-rw-r--r--   0 m.howitz   (502) staff       (20)      493 2023-06-23 06:28:27.000000 zope.event-5.0/docs/theory.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3189 2023-06-23 06:28:27.000000 zope.event-5.0/docs/usage.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      470 2023-06-23 06:28:27.769314 zope.event-5.0/setup.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2856 2023-06-23 06:28:27.000000 zope.event-5.0/setup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-06-23 06:28:27.764446 zope.event-5.0/src/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-06-23 06:28:27.767380 zope.event-5.0/src/zope/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       76 2023-06-23 06:28:27.000000 zope.event-5.0/src/zope/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-06-23 06:28:27.768864 zope.event-5.0/src/zope/event/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1142 2023-06-23 06:28:27.000000 zope.event-5.0/src/zope/event/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1820 2023-06-23 06:28:27.000000 zope.event-5.0/src/zope/event/classhandler.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1871 2023-06-23 06:28:27.000000 zope.event-5.0/src/zope/event/tests.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-06-23 06:28:27.768429 zope.event-5.0/src/zope.event.egg-info/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4323 2023-06-23 06:28:27.000000 zope.event-5.0/src/zope.event.egg-info/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)      631 2023-06-23 06:28:27.000000 zope.event-5.0/src/zope.event.egg-info/SOURCES.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-06-23 06:28:27.000000 zope.event-5.0/src/zope.event.egg-info/dependency_links.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        5 2023-06-23 06:28:27.000000 zope.event-5.0/src/zope.event.egg-info/namespace_packages.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-06-23 06:28:27.000000 zope.event-5.0/src/zope.event.egg-info/not-zip-safe
+-rw-r--r--   0 m.howitz   (502) staff       (20)       50 2023-06-23 06:28:27.000000 zope.event-5.0/src/zope.event.egg-info/requires.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        5 2023-06-23 06:28:27.000000 zope.event-5.0/src/zope.event.egg-info/top_level.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1823 2023-06-23 06:28:27.000000 zope.event-5.0/tox.ini
```

### Comparing `zope.event-4.6/CHANGES.rst` & `zope.event-5.0/CHANGES.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 ==========================
  ``zope.event`` Changelog
 ==========================
 
+5.0 (2023-06-23)
+================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+
 4.6 (2022-12-15)
 ================
 
 - Port documentation to Python 3.
 
 - Add support for Python 3.10, 3.11.
```

### Comparing `zope.event-4.6/CONTRIBUTING.md` & `zope.event-5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `zope.event-4.6/LICENSE.txt` & `zope.event-5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zope.event-4.6/PKG-INFO` & `zope.event-5.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 Metadata-Version: 2.1
 Name: zope.event
-Version: 4.6
+Version: 5.0
 Summary: Very basic event publishing system
 Home-page: https://github.com/zopefoundation/zope.event
 Author: Zope Foundation and Contributors
-Author-email: zope-dev@zope.org
+Author-email: zope-dev@zope.dev
 License: ZPL-2.1
 Keywords: event framework dispatch subscribe publish
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: Jython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Framework :: Zope :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.7
 Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE.txt
 
 =======================
  ``zope.event`` README
 =======================
@@ -59,14 +55,20 @@
 
 Please see http://zopeevent.readthedocs.io/ for the documentation.
 
 ==========================
  ``zope.event`` Changelog
 ==========================
 
+5.0 (2023-06-23)
+================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+
 4.6 (2022-12-15)
 ================
 
 - Port documentation to Python 3.
 
 - Add support for Python 3.10, 3.11.
 
@@ -175,9 +177,7 @@
 - A few minor cleanups.
 
 
 3.4.0 (2007-07-14)
 ==================
 
 - Initial release as a separate project.
-
-
```

### Comparing `zope.event-4.6/README.rst` & `zope.event-5.0/README.rst`

 * *Files identical despite different names*

### Comparing `zope.event-4.6/docs/Makefile` & `zope.event-5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zope.event-4.6/docs/conf.py` & `zope.event-5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `zope.event-4.6/docs/hacking.rst` & `zope.event-5.0/docs/hacking.rst`

 * *Files identical despite different names*

### Comparing `zope.event-4.6/docs/index.rst` & `zope.event-5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `zope.event-4.6/docs/make.bat` & `zope.event-5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `zope.event-4.6/docs/usage.rst` & `zope.event-5.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `zope.event-4.6/setup.py` & `zope.event-5.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 # This package is developed by the Zope Toolkit project, documented here:
-# http://docs.zope.org/zopetoolkit
+# https://zopetoolkit.readthedocs.io/
 # When developing and releasing this package, please follow the documented
 # Zope Toolkit policies as described by this documentation.
 ##############################################################################
 """Setup for zope.event package
 """
 
 import os
@@ -28,37 +28,33 @@
 def read(*rnames):
     with open(os.path.join(os.path.dirname(__file__), *rnames)) as f:
         return f.read()
 
 
 setup(
     name='zope.event',
-    version='4.6',
+    version='5.0',
     url='https://github.com/zopefoundation/zope.event',
     license='ZPL-2.1',
     description='Very basic event publishing system',
     author='Zope Foundation and Contributors',
-    author_email='zope-dev@zope.org',
+    author_email='zope-dev@zope.dev',
     long_description=(
         read('README.rst')
         + '\n' +
         read('CHANGES.rst')
     ),
     keywords="event framework dispatch subscribe publish",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Zope Public License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: Jython",
@@ -66,17 +62,17 @@
         "Framework :: Zope :: 3",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     packages=find_packages('src'),
     package_dir={'': 'src'},
     namespace_packages=['zope', ],
     include_package_data=True,
+    python_requires='>=3.7',
     install_requires=['setuptools'],
     zip_safe=False,
-    test_suite='zope.event.tests.test_suite',
     extras_require={
         'docs': [
             'Sphinx',
         ],
         'test': [
             'zope.testrunner',
         ],
```

### Comparing `zope.event-4.6/src/zope/event/__init__.py` & `zope.event-5.0/src/zope/event/__init__.py`

 * *Files identical despite different names*

### Comparing `zope.event-4.6/src/zope/event/classhandler.py` & `zope.event-5.0/src/zope/event/classhandler.py`

 * *Files identical despite different names*

### Comparing `zope.event-4.6/src/zope/event/tests.py` & `zope.event-5.0/src/zope/event/tests.py`

 * *Files identical despite different names*

### Comparing `zope.event-4.6/src/zope.event.egg-info/PKG-INFO` & `zope.event-5.0/src/zope.event.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 Metadata-Version: 2.1
 Name: zope.event
-Version: 4.6
+Version: 5.0
 Summary: Very basic event publishing system
 Home-page: https://github.com/zopefoundation/zope.event
 Author: Zope Foundation and Contributors
-Author-email: zope-dev@zope.org
+Author-email: zope-dev@zope.dev
 License: ZPL-2.1
 Keywords: event framework dispatch subscribe publish
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Zope Public License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: Jython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Framework :: Zope :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.7
 Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE.txt
 
 =======================
  ``zope.event`` README
 =======================
@@ -59,14 +55,20 @@
 
 Please see http://zopeevent.readthedocs.io/ for the documentation.
 
 ==========================
  ``zope.event`` Changelog
 ==========================
 
+5.0 (2023-06-23)
+================
+
+- Drop support for Python 2.7, 3.5, 3.6.
+
+
 4.6 (2022-12-15)
 ================
 
 - Port documentation to Python 3.
 
 - Add support for Python 3.10, 3.11.
 
@@ -175,9 +177,7 @@
 - A few minor cleanups.
 
 
 3.4.0 (2007-07-14)
 ==================
 
 - Initial release as a separate project.
-
-
```

### Comparing `zope.event-4.6/src/zope.event.egg-info/SOURCES.txt` & `zope.event-5.0/src/zope.event.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zope.event-4.6/tox.ini` & `zope.event-5.0/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 # Generated from:
 # https://github.com/zopefoundation/meta/tree/master/config/pure-python
 [tox]
 minversion = 3.18
 envlist =
     lint
-    py27
-    py35
-    py36
     py37
     py38
     py39
     py310
     py311
-    pypy
     pypy3
     docs
     coverage
 
 [testenv]
 usedevelop = true
 deps =
 commands =
     zope-testrunner --test-path=src {posargs:-vc}
-    !py27-!pypy: sphinx-build -b doctest -d {envdir}/.cache/doctrees docs {envdir}/.cache/doctest
+    sphinx-build -b doctest -d {envdir}/.cache/doctrees docs {envdir}/.cache/doctest
 extras =
     test
     docs
 
 [testenv:lint]
 basepython = python3
 skip_install = true
@@ -61,25 +57,23 @@
 
 [testenv:coverage]
 basepython = python3
 allowlist_externals =
     mkdir
 deps =
     coverage
-    coverage-python-version
 commands =
     mkdir -p {toxinidir}/parts/htmlcov
     coverage run -m zope.testrunner --test-path=src {posargs:-vc}
     coverage run -a -m sphinx -b doctest -d {envdir}/.cache/doctrees docs {envdir}/.cache/doctest
     coverage html --ignore-errors
     coverage report --ignore-errors --show-missing --fail-under=100
 
 [coverage:run]
 branch = True
-plugins = coverage_python_version
 source = zope.event
 
 [coverage:report]
 precision = 2
 exclude_lines =
     pragma: no cover
     pragma: nocover
```


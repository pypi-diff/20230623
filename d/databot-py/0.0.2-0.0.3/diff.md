# Comparing `tmp/databot-py-0.0.2.tar.gz` & `tmp/databot-py-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databot-py-0.0.2.tar", last modified: Thu Feb 16 15:27:17 2023, max compression
+gzip compressed data, was "databot-py-0.0.3.tar", last modified: Fri Jun 23 18:52:45 2023, max compression
```

## Comparing `databot-py-0.0.2.tar` & `databot-py-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-02-16 15:27:17.064272 databot-py-0.0.2/
--rw-rw-rw-   0        0        0     1092 2023-02-14 16:33:12.000000 databot-py-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      342 2023-02-16 15:27:17.063273 databot-py-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       64 2023-02-14 16:33:12.000000 databot-py-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-02-16 15:27:17.045274 databot-py-0.0.2/databot/
--rw-rw-rw-   0        0        0        0 2023-02-15 22:49:54.000000 databot-py-0.0.2/databot/__init__.py
--rw-rw-rw-   0        0        0     3499 2023-02-15 18:39:49.000000 databot-py-0.0.2/databot/databot.py
-drwxrwxrwx   0        0        0        0 2023-02-16 15:27:17.061272 databot-py-0.0.2/databot_py.egg-info/
--rw-rw-rw-   0        0        0      342 2023-02-16 15:27:17.000000 databot-py-0.0.2/databot_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-02-16 15:27:17.000000 databot-py-0.0.2/databot_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-16 15:27:17.000000 databot-py-0.0.2/databot_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-02-16 15:27:17.000000 databot-py-0.0.2/databot_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-02-16 15:27:17.000000 databot-py-0.0.2/databot_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2023-02-15 22:48:54.000000 databot-py-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-16 15:27:17.064272 databot-py-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      731 2023-02-16 15:26:55.000000 databot-py-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 18:52:45.877489 databot-py-0.0.3/
+-rw-rw-rw-   0        0        0     1092 2023-02-14 16:33:12.000000 databot-py-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2249 2023-06-23 18:52:45.875479 databot-py-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1937 2023-06-23 18:24:34.000000 databot-py-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 18:52:45.852479 databot-py-0.0.3/databot/
+-rw-rw-rw-   0        0        0    10969 2023-06-23 18:24:34.000000 databot-py-0.0.3/databot/PyDatabot.py
+-rw-rw-rw-   0        0        0        0 2023-06-18 13:23:36.000000 databot-py-0.0.3/databot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 18:52:45.873479 databot-py-0.0.3/databot_py.egg-info/
+-rw-rw-rw-   0        0        0     2249 2023-06-23 18:52:45.000000 databot-py-0.0.3/databot_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-06-23 18:52:45.000000 databot-py-0.0.3/databot_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 18:52:45.000000 databot-py-0.0.3/databot_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-23 18:52:45.000000 databot-py-0.0.3/databot_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-23 18:52:45.000000 databot-py-0.0.3/databot_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2023-06-23 18:24:07.000000 databot-py-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-23 18:52:45.879483 databot-py-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      765 2023-06-23 18:51:59.000000 databot-py-0.0.3/setup.py
```

### Comparing `databot-py-0.0.2/LICENSE` & `databot-py-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `databot-py-0.0.2/setup.py` & `databot-py-0.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 from glob import glob
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='databot-py',
-    version='0.0.2',
+    version='0.0.3',
     packages=['databot'],
     include_package_data=True,
     package_data={
         'media': glob('media/*'),
         'data': glob('data/*'),
         'web': glob('web/*')
     },
     url='https://github.com/dbaldwin/databot-py',
     license='MIT',
-    author='Dennis Baldwin',
-    author_email='db@droneblocks.io',
+    author='Pat Ryan, Dennis Baldwin',
+    author_email='theyoungsoul@gmail.com, db@droneblocks.io',
     description='databot Python Library',
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
         'bleak==0.19.1'
     ]
 )
```


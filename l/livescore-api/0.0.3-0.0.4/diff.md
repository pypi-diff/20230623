# Comparing `tmp/livescore-api-0.0.3.tar.gz` & `tmp/livescore-api-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livescore-api-0.0.3.tar", last modified: Fri Jun 16 13:09:43 2023, max compression
+gzip compressed data, was "livescore-api-0.0.4.tar", last modified: Fri Jun 23 12:52:30 2023, max compression
```

## Comparing `livescore-api-0.0.3.tar` & `livescore-api-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-16 13:09:43.810335 livescore-api-0.0.3/
--rw-rw----   0 root         (0) everybody  (9997)     1064 2023-06-13 16:33:10.000000 livescore-api-0.0.3/LICENSE
--rw-rw----   0 root         (0) everybody  (9997)     8566 2023-06-16 13:09:43.774335 livescore-api-0.0.3/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)     7460 2023-06-16 13:09:23.000000 livescore-api-0.0.3/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-16 13:09:43.554335 livescore-api-0.0.3/livescore_api/
--rw-rw----   0 root         (0) everybody  (9997)      323 2023-06-16 13:08:43.000000 livescore-api-0.0.3/livescore_api/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)       34 2023-06-12 02:52:21.000000 livescore-api-0.0.3/livescore_api/__main__.py
--rw-rw----   0 root         (0) everybody  (9997)     8243 2023-06-13 21:47:47.000000 livescore-api-0.0.3/livescore_api/console.py
--rw-rw----   0 root         (0) everybody  (9997)    12716 2023-06-13 22:03:30.000000 livescore-api-0.0.3/livescore_api/main.py
--rw-rw----   0 root         (0) everybody  (9997)     5186 2023-06-13 22:03:29.000000 livescore-api-0.0.3/livescore_api/predictor.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-16 13:09:43.754335 livescore-api-0.0.3/livescore_api.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)     8566 2023-06-16 13:09:42.000000 livescore-api-0.0.3/livescore_api.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      376 2023-06-16 13:09:42.000000 livescore-api-0.0.3/livescore_api.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-16 13:09:42.000000 livescore-api-0.0.3/livescore_api.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       61 2023-06-16 13:09:42.000000 livescore-api-0.0.3/livescore_api.egg-info/entry_points.txt
--rw-rw----   0 root         (0) everybody  (9997)      109 2023-06-16 13:09:42.000000 livescore-api-0.0.3/livescore_api.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)       14 2023-06-16 13:09:42.000000 livescore-api-0.0.3/livescore_api.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-16 13:09:43.810335 livescore-api-0.0.3/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)     1566 2023-06-16 13:08:57.000000 livescore-api-0.0.3/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-23 12:52:30.126000 livescore-api-0.0.4/
+-rw-rw----   0 root         (0) everybody  (9997)     1064 2023-06-13 16:33:10.000000 livescore-api-0.0.4/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)     8566 2023-06-23 12:52:30.054000 livescore-api-0.0.4/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)     7460 2023-06-23 12:51:08.000000 livescore-api-0.0.4/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-23 12:52:29.846000 livescore-api-0.0.4/livescore_api/
+-rw-rw----   0 root         (0) everybody  (9997)      323 2023-06-23 12:50:14.000000 livescore-api-0.0.4/livescore_api/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)       34 2023-06-12 02:52:21.000000 livescore-api-0.0.4/livescore_api/__main__.py
+-rw-rw----   0 root         (0) everybody  (9997)     8243 2023-06-13 21:47:47.000000 livescore-api-0.0.4/livescore_api/console.py
+-rw-rw----   0 root         (0) everybody  (9997)    12716 2023-06-13 22:03:30.000000 livescore-api-0.0.4/livescore_api/main.py
+-rw-rw----   0 root         (0) everybody  (9997)     5186 2023-06-13 22:03:29.000000 livescore-api-0.0.4/livescore_api/predictor.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-23 12:52:30.034000 livescore-api-0.0.4/livescore_api.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     8566 2023-06-23 12:52:28.000000 livescore-api-0.0.4/livescore_api.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      376 2023-06-23 12:52:29.000000 livescore-api-0.0.4/livescore_api.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-23 12:52:28.000000 livescore-api-0.0.4/livescore_api.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       61 2023-06-23 12:52:28.000000 livescore-api-0.0.4/livescore_api.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) everybody  (9997)      109 2023-06-23 12:52:28.000000 livescore-api-0.0.4/livescore_api.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)       14 2023-06-23 12:52:28.000000 livescore-api-0.0.4/livescore_api.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-23 12:52:30.126000 livescore-api-0.0.4/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     1646 2023-06-23 12:51:32.000000 livescore-api-0.0.4/setup.py
```

### Comparing `livescore-api-0.0.3/LICENSE` & `livescore-api-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `livescore-api-0.0.3/PKG-INFO` & `livescore-api-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livescore-api
-Version: 0.0.3
+Version: 0.0.4
 Summary: Access and manipulate matches from Livescore.com
 Home-page: https://github.com/Simatwa/livescore-api
 Author: Smartwa
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/livescore-api/issues/new
@@ -26,15 +26,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Livescore-api
 <p align="center">
 <a href="https://github.com/Simatwa/livescore-api"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a>
 <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=MIT&label=License"/></a>
-<a href="https://pypi.org/project/livescore-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.3&color=green"/></a>
+<a href="https://pypi.org/project/livescore-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.4&color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a>
 <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a>
 <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=60%&color=yellowgreen"/></a>
 <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>
 <a href="https://pepy.tech/project/livescore-api"><img src="https://static.pepy.tech/personalized-badge/livescore-api?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="Downloads"></a>
 </p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: livescore-api Version: 0.0.3 Summary: Access and
+Metadata-Version: 2.1 Name: livescore-api Version: 0.0.4 Summary: Access and
 manipulate matches from Livescore.com Home-page: https://github.com/Simatwa/
 livescore-api Author: Smartwa Author-email: smartwacaleb@gmail.com Maintainer:
 Smartwa License: MIT Project-URL: Bug Report, https://github.com/Simatwa/
 livescore-api/issues/new Keywords: livescore,football,livescore-api,api
 Classifier: License :: OSI Approved :: MIT License Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
 Natural Language :: English Classifier: License :: Free For Home Use
```

### Comparing `livescore-api-0.0.3/README.md` & `livescore-api-0.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Livescore-api
 <p align="center">
 <a href="https://github.com/Simatwa/livescore-api"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a>
 <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=MIT&label=License"/></a>
-<a href="https://pypi.org/project/livescore-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.3&color=green"/></a>
+<a href="https://pypi.org/project/livescore-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.4&color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a>
 <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a>
 <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=60%&color=yellowgreen"/></a>
 <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>
 <a href="https://pepy.tech/project/livescore-api"><img src="https://static.pepy.tech/personalized-badge/livescore-api?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="Downloads"></a>
 </p>
```

### Comparing `livescore-api-0.0.3/livescore_api/console.py` & `livescore-api-0.0.4/livescore_api/console.py`

 * *Files identical despite different names*

### Comparing `livescore-api-0.0.3/livescore_api/main.py` & `livescore-api-0.0.4/livescore_api/main.py`

 * *Files identical despite different names*

### Comparing `livescore-api-0.0.3/livescore_api/predictor.py` & `livescore-api-0.0.4/livescore_api/predictor.py`

 * *Files identical despite different names*

### Comparing `livescore-api-0.0.3/livescore_api.egg-info/PKG-INFO` & `livescore-api-0.0.4/livescore_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livescore-api
-Version: 0.0.3
+Version: 0.0.4
 Summary: Access and manipulate matches from Livescore.com
 Home-page: https://github.com/Simatwa/livescore-api
 Author: Smartwa
 Author-email: smartwacaleb@gmail.com
 Maintainer: Smartwa
 License: MIT
 Project-URL: Bug Report, https://github.com/Simatwa/livescore-api/issues/new
@@ -26,15 +26,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Livescore-api
 <p align="center">
 <a href="https://github.com/Simatwa/livescore-api"><img alt="Github" src="https://img.shields.io/static/v1?logo=github&color=blueviolet&label=Test&message=Passing"/></a>
 <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=MIT&label=License"/></a>
-<a href="https://pypi.org/project/livescore-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.3&color=green"/></a>
+<a href="https://pypi.org/project/livescore-api"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.0.4&color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a>
 <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a>
 <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=60%&color=yellowgreen"/></a>
 <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>
 <a href="https://pepy.tech/project/livescore-api"><img src="https://static.pepy.tech/personalized-badge/livescore-api?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads" alt="Downloads"></a>
 </p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: livescore-api Version: 0.0.3 Summary: Access and
+Metadata-Version: 2.1 Name: livescore-api Version: 0.0.4 Summary: Access and
 manipulate matches from Livescore.com Home-page: https://github.com/Simatwa/
 livescore-api Author: Smartwa Author-email: smartwacaleb@gmail.com Maintainer:
 Smartwa License: MIT Project-URL: Bug Report, https://github.com/Simatwa/
 livescore-api/issues/new Keywords: livescore,football,livescore-api,api
 Classifier: License :: OSI Approved :: MIT License Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
 Natural Language :: English Classifier: License :: Free For Home Use
```

### Comparing `livescore-api-0.0.3/setup.py` & `livescore-api-0.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 from setuptools import setup
-from livescore_api import __version__, __author__, __repo__, __info__
+
+version = "0.0.4"
+repo = "https://github.com/Simatwa/livescore-api"
+info = "Access and manipulate matches from Livescore.com"
+author = "Smartwa"
 
 setup(
     name="livescore-api",
     packages=["livescore_api"],
-    version=__version__,
+    version=version,
     license="MIT",
-    author=__author__,
-    maintainer=__author__,
+    author=author,
+    maintainer=author,
     author_email="smartwacaleb@gmail.com",
-    description=__info__,
-    url=__repo__,
-    project_urls={"Bug Report": f"{__repo__}/issues/new"},
+    description=info,
+    url=repo,
+    project_urls={"Bug Report": f"{repo}/issues/new"},
     install_requires=[
-    "argparse>=1.1",
-    "requests>=2.0.2",
-    "pandas>=1.3.3",
-    "tabulate==0.9.0",
-    "smartbetsAPI==1.1.4",
-    "tqdm==4.65.0",
-    "colorama==0.4.6",
+        "argparse>=1.1",
+        "requests>=2.0.2",
+        "pandas>=1.3.3",
+        "tabulate==0.9.0",
+        "smartbetsAPI==1.1.4",
+        "tqdm==4.65.0",
+        "colorama==0.4.6",
     ],
     python_requires=">=3.8",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Development Status :: 4 - Beta",
```


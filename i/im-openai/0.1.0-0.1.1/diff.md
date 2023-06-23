# Comparing `tmp/im_openai-0.1.0.tar.gz` & `tmp/im_openai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "im_openai-0.1.0.tar", last modified: Thu Jun 22 22:05:32 2023, max compression
+gzip compressed data, was "im_openai-0.1.1.tar", last modified: Fri Jun 23 21:34:05 2023, max compression
```

## Comparing `im_openai-0.1.0.tar` & `im_openai-0.1.1.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-22 22:05:32.596734 im_openai-0.1.0/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      150 2023-06-20 23:30:14.000000 im_openai-0.1.0/AUTHORS.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3560 2023-06-22 20:28:17.000000 im_openai-0.1.0/CONTRIBUTING.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)       89 2023-06-20 23:30:14.000000 im_openai-0.1.0/HISTORY.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1069 2023-06-20 23:30:14.000000 im_openai-0.1.0/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)      261 2023-06-22 20:24:41.000000 im_openai-0.1.0/MANIFEST.in
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2408 2023-06-22 22:05:32.597268 im_openai-0.1.0/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1560 2023-06-21 23:37:53.000000 im_openai-0.1.0/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-22 22:05:32.555216 im_openai-0.1.0/docs/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      610 2023-06-20 23:30:14.000000 im_openai-0.1.0/docs/Makefile
--rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-06-20 23:30:14.000000 im_openai-0.1.0/docs/authors.rst
--rwxr-xr-x   0 vscode    (1000) vscode    (1000)     4874 2023-06-20 23:30:14.000000 im_openai-0.1.0/docs/conf.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)       33 2023-06-20 23:30:14.000000 im_openai-0.1.0/docs/contributing.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-06-20 23:30:14.000000 im_openai-0.1.0/docs/history.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)      325 2023-06-20 23:30:14.000000 im_openai-0.1.0/docs/index.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1175 2023-06-20 23:30:14.000000 im_openai-0.1.0/docs/installation.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)      807 2023-06-20 23:30:14.000000 im_openai-0.1.0/docs/make.bat
--rw-r--r--   0 vscode    (1000) vscode    (1000)       26 2023-06-22 20:24:52.000000 im_openai-0.1.0/docs/readme.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)       92 2023-06-20 23:30:14.000000 im_openai-0.1.0/docs/usage.rst
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-22 22:05:32.563542 im_openai-0.1.0/im_openai/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      218 2023-06-21 23:21:30.000000 im_openai-0.1.0/im_openai/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1448 2023-06-21 23:22:38.000000 im_openai-0.1.0/im_openai/client.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1755 2023-06-21 23:21:08.000000 im_openai-0.1.0/im_openai/patch.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-22 22:05:32.588925 im_openai-0.1.0/im_openai.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2408 2023-06-22 22:05:32.000000 im_openai-0.1.0/im_openai.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      521 2023-06-22 22:05:32.000000 im_openai-0.1.0/im_openai.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-22 22:05:32.000000 im_openai-0.1.0/im_openai.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-22 22:05:32.000000 im_openai-0.1.0/im_openai.egg-info/not-zip-safe
--rw-r--r--   0 vscode    (1000) vscode    (1000)       10 2023-06-22 22:05:32.000000 im_openai-0.1.0/im_openai.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      426 2023-06-22 22:05:32.598786 im_openai-0.1.0/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1335 2023-06-22 22:04:20.000000 im_openai-0.1.0/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-22 22:05:32.595049 im_openai-0.1.0/tests/
--rw-r--r--   0 vscode    (1000) vscode    (1000)       39 2023-06-20 23:30:14.000000 im_openai-0.1.0/tests/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      559 2023-06-20 23:30:14.000000 im_openai-0.1.0/tests/test_im_openai.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-23 21:34:05.370837 im_openai-0.1.1/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      150 2023-06-20 23:30:14.000000 im_openai-0.1.1/AUTHORS.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3560 2023-06-22 20:28:17.000000 im_openai-0.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       89 2023-06-20 23:30:14.000000 im_openai-0.1.1/HISTORY.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1069 2023-06-20 23:30:14.000000 im_openai-0.1.1/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      261 2023-06-22 20:24:41.000000 im_openai-0.1.1/MANIFEST.in
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2420 2023-06-23 21:34:05.371521 im_openai-0.1.1/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1560 2023-06-21 23:37:53.000000 im_openai-0.1.1/README.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-23 21:34:05.307278 im_openai-0.1.1/docs/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      610 2023-06-20 23:30:14.000000 im_openai-0.1.1/docs/Makefile
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-06-20 23:30:14.000000 im_openai-0.1.1/docs/authors.rst
+-rwxr-xr-x   0 vscode    (1000) vscode    (1000)     4874 2023-06-20 23:30:14.000000 im_openai-0.1.1/docs/conf.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       33 2023-06-20 23:30:14.000000 im_openai-0.1.1/docs/contributing.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-06-20 23:30:14.000000 im_openai-0.1.1/docs/history.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      325 2023-06-20 23:30:14.000000 im_openai-0.1.1/docs/index.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1175 2023-06-20 23:30:14.000000 im_openai-0.1.1/docs/installation.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      807 2023-06-20 23:30:14.000000 im_openai-0.1.1/docs/make.bat
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       26 2023-06-22 20:24:52.000000 im_openai-0.1.1/docs/readme.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       92 2023-06-20 23:30:14.000000 im_openai-0.1.1/docs/usage.rst
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-23 21:34:05.330614 im_openai-0.1.1/im_openai/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      255 2023-06-23 16:59:08.000000 im_openai-0.1.1/im_openai/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1610 2023-06-23 21:03:40.000000 im_openai-0.1.1/im_openai/client.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1755 2023-06-21 23:21:08.000000 im_openai-0.1.1/im_openai/patch.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      390 2023-06-23 16:58:54.000000 im_openai-0.1.1/im_openai/template.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-23 21:34:05.361307 im_openai-0.1.1/im_openai.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2420 2023-06-23 21:34:05.000000 im_openai-0.1.1/im_openai.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      543 2023-06-23 21:34:05.000000 im_openai-0.1.1/im_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-23 21:34:05.000000 im_openai-0.1.1/im_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-23 21:34:05.000000 im_openai-0.1.1/im_openai.egg-info/not-zip-safe
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       10 2023-06-23 21:34:05.000000 im_openai-0.1.1/im_openai.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      426 2023-06-23 21:34:05.376457 im_openai-0.1.1/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1351 2023-06-23 21:33:09.000000 im_openai-0.1.1/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-23 21:34:05.368318 im_openai-0.1.1/tests/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       39 2023-06-20 23:30:14.000000 im_openai-0.1.1/tests/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      559 2023-06-20 23:30:14.000000 im_openai-0.1.1/tests/test_im_openai.py
```

### Comparing `im_openai-0.1.0/CONTRIBUTING.rst` & `im_openai-0.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `im_openai-0.1.0/LICENSE` & `im_openai-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `im_openai-0.1.0/PKG-INFO` & `im_openai-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: im_openai
-Version: 0.1.0
+Version: 0.1.1
 Summary: Wrapper library for openai to send events to the Imaginary Programming monitor
 Home-page: https://github.com/alecf/im_openai
 Author: Alec Flett
 Author-email: alec@thegp.com
 License: MIT license
 Keywords: im_openai
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -12,15 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
-Description-Content-Type: m
+Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 # Imaginary Dev OpenAI wrapper
 
 [![image](https://img.shields.io/pypi/v/im_openai.svg)](https://pypi.python.org/pypi/im_openai)
```

### Comparing `im_openai-0.1.0/README.md` & `im_openai-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `im_openai-0.1.0/docs/Makefile` & `im_openai-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `im_openai-0.1.0/docs/conf.py` & `im_openai-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `im_openai-0.1.0/docs/installation.rst` & `im_openai-0.1.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `im_openai-0.1.0/docs/make.bat` & `im_openai-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `im_openai-0.1.0/im_openai/client.py` & `im_openai-0.1.1/im_openai/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,27 +3,35 @@
 import uuid
 from contextlib import contextmanager
 
 import requests
 
 
 def send_event(
-    project_key: str, prompt_event_id: str, response=None, response_time: float = None
+    project_key: str,
+    prompt_event_id: str,
+    prompt_text: str = None,
+    response: str = None,
+    response_time: float = None,
 ):
     PROMPT_REPORTING_URL = os.environ.get(
         "PROMPT_REPORTING_URL", "https://app.imaginary.dev/api/event"
     )
     event = {
         "params": {},
-        "prompt": {
-            # funcName, funcComment, parameterTypes, returnSchema, isImaginary, serviceParameters
-        },
+        "prompt": {},
         "projectKey": project_key,
         "promptEventId": prompt_event_id,
     }
+    if prompt_text is not None:
+        event["prompt"]["text"] = prompt_text
+        if hasattr(prompt_text, "params"):
+            # Can be TemplateString or any other
+            event["params"] = prompt_text.params
+
     if response is not None:
         event["response"] = response
     if response_time is not None:
         event["responseTime"] = response_time
 
     response = requests.post(PROMPT_REPORTING_URL, json=event)
     response.raise_for_status()
```

### Comparing `im_openai-0.1.0/im_openai/patch.py` & `im_openai-0.1.1/im_openai/patch.py`

 * *Files identical despite different names*

### Comparing `im_openai-0.1.0/im_openai.egg-info/PKG-INFO` & `im_openai-0.1.1/im_openai.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: im-openai
-Version: 0.1.0
+Version: 0.1.1
 Summary: Wrapper library for openai to send events to the Imaginary Programming monitor
 Home-page: https://github.com/alecf/im_openai
 Author: Alec Flett
 Author-email: alec@thegp.com
 License: MIT license
 Keywords: im_openai
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -12,15 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
-Description-Content-Type: m
+Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 # Imaginary Dev OpenAI wrapper
 
 [![image](https://img.shields.io/pypi/v/im_openai.svg)](https://pypi.python.org/pypi/im_openai)
```

### Comparing `im_openai-0.1.0/im_openai.egg-info/SOURCES.txt` & `im_openai-0.1.1/im_openai.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 docs/installation.rst
 docs/make.bat
 docs/readme.rst
 docs/usage.rst
 im_openai/__init__.py
 im_openai/client.py
 im_openai/patch.py
+im_openai/template.py
 im_openai.egg-info/PKG-INFO
 im_openai.egg-info/SOURCES.txt
 im_openai.egg-info/dependency_links.txt
 im_openai.egg-info/not-zip-safe
 im_openai.egg-info/top_level.txt
 tests/__init__.py
 tests/test_im_openai.py
```

### Comparing `im_openai-0.1.0/setup.py` & `im_openai-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 #!/usr/bin/env python
 
 """The setup script."""
 
 from setuptools import setup, find_packages
 
-with open('README.md') as readme_file:
+with open("README.md") as readme_file:
     readme = readme_file.read()
 
-with open('HISTORY.rst') as history_file:
+with open("HISTORY.rst") as history_file:
     history = history_file.read()
 
-requirements = [ ]
+requirements = []
 
-test_requirements = ['pytest>=3', ]
+test_requirements = [
+    "pytest>=3",
+]
 
 setup(
     author="Alec Flett",
-    author_email='alec@thegp.com',
-    python_requires='>=3.6',
+    author_email="alec@thegp.com",
+    python_requires=">=3.6",
     classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Natural Language :: English',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
+        "Development Status :: 2 - Pre-Alpha",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Natural Language :: English",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
     ],
     description="Wrapper library for openai to send events to the Imaginary Programming monitor",
     install_requires=requirements,
     license="MIT license",
-    long_description=readme + '\n\n' + history,
-    long_description_content_type='m',
+    long_description=readme + "\n\n" + history,
+    long_description_content_type="text/markdown",
     include_package_data=True,
-    keywords='im_openai',
-    name='im_openai',
-    packages=find_packages(include=['im_openai', 'im_openai.*']),
-    test_suite='tests',
+    keywords="im_openai",
+    name="im_openai",
+    packages=find_packages(include=["im_openai", "im_openai.*"]),
+    test_suite="tests",
     tests_require=test_requirements,
-    url='https://github.com/alecf/im_openai',
-    version='0.1.0',
+    url="https://github.com/alecf/im_openai",
+    version="0.1.1",
     zip_safe=False,
 )
```

### Comparing `im_openai-0.1.0/tests/test_im_openai.py` & `im_openai-0.1.1/tests/test_im_openai.py`

 * *Files identical despite different names*


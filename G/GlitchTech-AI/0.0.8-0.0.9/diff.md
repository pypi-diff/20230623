# Comparing `tmp/GlitchTech-AI-0.0.8.tar.gz` & `tmp/GlitchTech-AI-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GlitchTech-AI-0.0.8.tar", last modified: Tue Jun 13 19:23:21 2023, max compression
+gzip compressed data, was "GlitchTech-AI-0.0.9.tar", last modified: Tue Jun 13 19:29:55 2023, max compression
```

## Comparing `GlitchTech-AI-0.0.8.tar` & `GlitchTech-AI-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 19:23:21.311390 GlitchTech-AI-0.0.8/
-drwxrwxrwx   0        0        0        0 2023-06-13 19:23:21.309396 GlitchTech-AI-0.0.8/GlitchTech_AI.egg-info/
--rw-rw-rw-   0        0        0      525 2023-06-13 19:23:21.000000 GlitchTech-AI-0.0.8/GlitchTech_AI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      406 2023-06-13 19:23:21.000000 GlitchTech-AI-0.0.8/GlitchTech_AI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 19:23:21.000000 GlitchTech-AI-0.0.8/GlitchTech_AI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-06-13 19:23:21.000000 GlitchTech-AI-0.0.8/GlitchTech_AI.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-06-13 17:49:37.000000 GlitchTech-AI-0.0.8/GlitchTech_AI.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       23 2023-06-13 19:23:21.000000 GlitchTech-AI-0.0.8/GlitchTech_AI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-13 19:23:21.000000 GlitchTech-AI-0.0.8/GlitchTech_AI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35823 2023-06-13 17:46:59.000000 GlitchTech-AI-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      525 2023-06-13 19:23:21.311390 GlitchTech-AI-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       83 2023-06-13 17:46:59.000000 GlitchTech-AI-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 19:23:21.309396 GlitchTech-AI-0.0.8/glitchtech_ai/
--rw-rw-rw-   0        0        0       33 2023-06-13 19:20:19.000000 GlitchTech-AI-0.0.8/glitchtech_ai/__init__.py
--rw-rw-rw-   0        0        0      513 2023-06-13 17:46:59.000000 GlitchTech-AI-0.0.8/glitchtech_ai/glitchtech_ai.py
-drwxrwxrwx   0        0        0        0 2023-06-13 19:23:21.310395 GlitchTech-AI-0.0.8/glitchtech_ai/tools/
--rw-rw-rw-   0        0        0       29 2023-06-13 19:21:47.000000 GlitchTech-AI-0.0.8/glitchtech_ai/tools/__init__.py
--rw-rw-rw-   0        0        0     1875 2023-06-13 17:46:59.000000 GlitchTech-AI-0.0.8/glitchtech_ai/tools/adapter.py
--rw-rw-rw-   0        0        0       42 2023-06-13 19:23:21.311390 GlitchTech-AI-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1002 2023-06-13 19:23:18.000000 GlitchTech-AI-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 19:29:55.758904 GlitchTech-AI-0.0.9/
+drwxrwxrwx   0        0        0        0 2023-06-13 19:29:55.756909 GlitchTech-AI-0.0.9/GlitchTech_AI.egg-info/
+-rw-rw-rw-   0        0        0      525 2023-06-13 19:29:55.000000 GlitchTech-AI-0.0.9/GlitchTech_AI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      375 2023-06-13 19:29:55.000000 GlitchTech-AI-0.0.9/GlitchTech_AI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 19:29:55.000000 GlitchTech-AI-0.0.9/GlitchTech_AI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 19:29:55.000000 GlitchTech-AI-0.0.9/GlitchTech_AI.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-13 17:49:37.000000 GlitchTech-AI-0.0.9/GlitchTech_AI.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       23 2023-06-13 19:29:55.000000 GlitchTech-AI-0.0.9/GlitchTech_AI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-13 19:29:55.000000 GlitchTech-AI-0.0.9/GlitchTech_AI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35823 2023-06-13 17:46:59.000000 GlitchTech-AI-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      525 2023-06-13 19:29:55.758904 GlitchTech-AI-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       83 2023-06-13 17:46:59.000000 GlitchTech-AI-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 19:29:55.757907 GlitchTech-AI-0.0.9/glitchtech_ai/
+-rw-rw-rw-   0        0        0       40 2023-06-13 19:26:28.000000 GlitchTech-AI-0.0.9/glitchtech_ai/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 19:29:55.758904 GlitchTech-AI-0.0.9/glitchtech_ai/tools/
+-rw-rw-rw-   0        0        0       29 2023-06-13 19:21:47.000000 GlitchTech-AI-0.0.9/glitchtech_ai/tools/__init__.py
+-rw-rw-rw-   0        0        0     1875 2023-06-13 17:46:59.000000 GlitchTech-AI-0.0.9/glitchtech_ai/tools/adapter.py
+-rw-rw-rw-   0        0        0       42 2023-06-13 19:29:55.759901 GlitchTech-AI-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      991 2023-06-13 19:29:54.000000 GlitchTech-AI-0.0.9/setup.py
```

### Comparing `GlitchTech-AI-0.0.8/GlitchTech_AI.egg-info/PKG-INFO` & `GlitchTech-AI-0.0.9/GlitchTech_AI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GlitchTech-AI
-Version: 0.0.8
+Version: 0.0.9
 Summary: Basic utility to interface with OpenAI via command line or terminal.
 Author: Clutch_Reboot
 Author-email: clutchshadow26@gmail.com
 License: GNU General Public License v3.0
 Project-URL: Source, https://github.com/ClutchReboot/openai-cli
 Keywords: openai cli terminal glitchtech
 Requires-Python: >=3.10
```

### Comparing `GlitchTech-AI-0.0.8/LICENSE` & `GlitchTech-AI-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `GlitchTech-AI-0.0.8/PKG-INFO` & `GlitchTech-AI-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GlitchTech-AI
-Version: 0.0.8
+Version: 0.0.9
 Summary: Basic utility to interface with OpenAI via command line or terminal.
 Author: Clutch_Reboot
 Author-email: clutchshadow26@gmail.com
 License: GNU General Public License v3.0
 Project-URL: Source, https://github.com/ClutchReboot/openai-cli
 Keywords: openai cli terminal glitchtech
 Requires-Python: >=3.10
```

### Comparing `GlitchTech-AI-0.0.8/glitchtech_ai/tools/adapter.py` & `GlitchTech-AI-0.0.9/glitchtech_ai/tools/adapter.py`

 * *Files identical despite different names*

### Comparing `GlitchTech-AI-0.0.8/setup.py` & `GlitchTech-AI-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup
 
 # python setup.py sdist
 # twine upload dist/*
 
 setup(name='GlitchTech-AI',
-      version='0.0.8',
+      version='0.0.9',
       description='Basic utility to interface with OpenAI via command line or terminal.',
       keywords='openai cli terminal glitchtech',
       author='Clutch_Reboot',
       author_email='clutchshadow26@gmail.com',
       license='GNU General Public License v3.0',
       packages=[
             'glitchtech_ai',
             'glitchtech_ai.tools',
       ],
       entry_points={
             'console_scripts': [
-                  'glitchtech-ai = glitchtech_ai:main'
+                  'glitchtech-ai = src:cli'
             ]
       },
       zip_safe=False,
       long_description=open('README.md', 'rt').read(),
       long_description_content_type='text/markdown',
       python_requires='>=3.10',
       install_requires=[
```


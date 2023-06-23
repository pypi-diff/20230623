# Comparing `tmp/verysimplemodule_lais-0.0.1.tar.gz` & `tmp/verysimplemodule_lais-0.0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verysimplemodule_lais-0.0.1.tar", last modified: Fri Jun 23 19:24:30 2023, max compression
+gzip compressed data, was "verysimplemodule_lais-0.0.1.2.tar", last modified: Fri Jun 23 19:46:30 2023, max compression
```

## Comparing `verysimplemodule_lais-0.0.1.tar` & `verysimplemodule_lais-0.0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 19:24:30.876932 verysimplemodule_lais-0.0.1/
--rw-rw-rw-   0        0        0      542 2023-06-23 19:24:30.876932 verysimplemodule_lais-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-23 19:24:30.876932 verysimplemodule_lais-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1075 2023-06-23 19:22:35.000000 verysimplemodule_lais-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-23 19:24:30.830014 verysimplemodule_lais-0.0.1/verysimplemodule_lais/
--rw-rw-rw-   0        0        0       43 2023-06-23 19:00:28.000000 verysimplemodule_lais-0.0.1/verysimplemodule_lais/__init__.py
--rw-rw-rw-   0        0        0      374 2023-06-23 19:00:35.000000 verysimplemodule_lais-0.0.1/verysimplemodule_lais/baixar_arquivo.py
-drwxrwxrwx   0        0        0        0 2023-06-23 19:24:30.861277 verysimplemodule_lais-0.0.1/verysimplemodule_lais.egg-info/
--rw-rw-rw-   0        0        0      542 2023-06-23 19:24:30.000000 verysimplemodule_lais-0.0.1/verysimplemodule_lais.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-06-23 19:24:30.000000 verysimplemodule_lais-0.0.1/verysimplemodule_lais.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 19:24:30.000000 verysimplemodule_lais-0.0.1/verysimplemodule_lais.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-23 19:24:30.000000 verysimplemodule_lais-0.0.1/verysimplemodule_lais.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-23 19:24:30.000000 verysimplemodule_lais-0.0.1/verysimplemodule_lais.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 19:46:30.513112 verysimplemodule_lais-0.0.1.2/
+-rw-rw-rw-   0        0        0      544 2023-06-23 19:46:30.497491 verysimplemodule_lais-0.0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-23 19:46:30.513112 verysimplemodule_lais-0.0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1107 2023-06-23 19:44:37.000000 verysimplemodule_lais-0.0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 19:46:30.481878 verysimplemodule_lais-0.0.1.2/verysimplemodule_lais/
+-rw-rw-rw-   0        0        0       43 2023-06-23 19:00:28.000000 verysimplemodule_lais-0.0.1.2/verysimplemodule_lais/__init__.py
+-rw-rw-rw-   0        0        0      374 2023-06-23 19:00:35.000000 verysimplemodule_lais-0.0.1.2/verysimplemodule_lais/baixar_arquivo.py
+drwxrwxrwx   0        0        0        0 2023-06-23 19:46:30.497491 verysimplemodule_lais-0.0.1.2/verysimplemodule_lais.egg-info/
+-rw-rw-rw-   0        0        0      544 2023-06-23 19:46:30.000000 verysimplemodule_lais-0.0.1.2/verysimplemodule_lais.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-06-23 19:46:30.000000 verysimplemodule_lais-0.0.1.2/verysimplemodule_lais.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 19:46:30.000000 verysimplemodule_lais-0.0.1.2/verysimplemodule_lais.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-23 19:46:30.000000 verysimplemodule_lais-0.0.1.2/verysimplemodule_lais.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       37 2023-06-23 19:46:30.000000 verysimplemodule_lais-0.0.1.2/verysimplemodule_lais.egg-info/top_level.txt
```

### Comparing `verysimplemodule_lais-0.0.1/PKG-INFO` & `verysimplemodule_lais-0.0.1.2/verysimplemodule_lais.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: verysimplemodule_lais
-Version: 0.0.1
+Name: verysimplemodule-lais
+Version: 0.0.1.2
 Summary: Meu primeiro pacote em Python
 Author: Lais Sousa
 Author-email: <laissouroch@gmail.com>
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `verysimplemodule_lais-0.0.1/setup.py` & `verysimplemodule_lais-0.0.1.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1' 
+VERSION = '0.0.1.2' 
 DESCRIPTION = 'Meu primeiro pacote em Python'
 LONG_DESCRIPTION = 'Meu primeiro pacote em Python para baixar um PDF'
 
 # Setting up
 setup(
        # 'name' deve corresponder ao nome da pasta 'verysimplemodule'
         name="verysimplemodule_lais", 
@@ -12,15 +12,15 @@
         author="Lais Sousa",
         author_email="<laissouroch@gmail.com>",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(),
         install_requires=['requests'], # adicione outros pacotes que 
         # precisem ser instalados com o seu pacote. Ex: 'caer'
-        
+        py_modules=['baixar_arquivo'],
         keywords=['python', 'first package'],
         classifiers= [
             "Development Status :: 3 - Alpha",
             "Intended Audience :: Education",
             "Programming Language :: Python :: 2",
             "Programming Language :: Python :: 3",
             "Operating System :: MacOS :: MacOS X",
```

### Comparing `verysimplemodule_lais-0.0.1/verysimplemodule_lais.egg-info/PKG-INFO` & `verysimplemodule_lais-0.0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: verysimplemodule-lais
-Version: 0.0.1
+Name: verysimplemodule_lais
+Version: 0.0.1.2
 Summary: Meu primeiro pacote em Python
 Author: Lais Sousa
 Author-email: <laissouroch@gmail.com>
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```


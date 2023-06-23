# Comparing `tmp/exem-logs-1.1.1.tar.gz` & `tmp/exem-logs-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exem-logs-1.1.1.tar", last modified: Fri Jun 23 09:18:44 2023, max compression
+gzip compressed data, was "exem-logs-1.1.2.tar", last modified: Fri Jun 23 09:31:09 2023, max compression
```

## Comparing `exem-logs-1.1.1.tar` & `exem-logs-1.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 09:18:44.134878 exem-logs-1.1.1/
--rw-rw-rw-   0        0        0     5467 2023-06-23 09:06:36.000000 exem-logs-1.1.1/Log.py
--rw-rw-rw-   0        0        0      359 2023-06-23 09:18:44.133906 exem-logs-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     7651 2023-06-23 09:06:16.000000 exem-logs-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 09:18:44.096758 exem-logs-1.1.1/exem_logs.egg-info/
--rw-rw-rw-   0        0        0      359 2023-06-23 09:18:44.000000 exem-logs-1.1.1/exem_logs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      618 2023-06-23 09:18:44.000000 exem-logs-1.1.1/exem_logs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 09:18:44.000000 exem-logs-1.1.1/exem_logs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-06-23 09:18:44.000000 exem-logs-1.1.1/exem_logs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-23 09:18:44.000000 exem-logs-1.1.1/exem_logs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 09:18:44.135876 exem-logs-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      630 2023-06-23 09:18:22.000000 exem-logs-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-23 09:18:44.078995 exem-logs-1.1.1/venv10/
-drwxrwxrwx   0        0        0        0 2023-06-23 09:18:44.131878 exem-logs-1.1.1/venv10/Scripts/
--rw-rw-rw-   0        0        0     1169 2023-06-23 07:53:35.000000 exem-logs-1.1.1/venv10/Scripts/activate_this.py
--rw-rw-rw-   0        0        0     6456 2023-06-23 08:01:20.000000 exem-logs-1.1.1/venv10/Scripts/fixup_errorreporting_v1beta1_keywords.py
--rw-rw-rw-   0        0        0      664 2023-06-23 07:54:36.000000 exem-logs-1.1.1/venv10/Scripts/rst2html.py
--rw-rw-rw-   0        0        0      786 2023-06-23 07:54:36.000000 exem-logs-1.1.1/venv10/Scripts/rst2html4.py
--rw-rw-rw-   0        0        0     1121 2023-06-23 07:54:36.000000 exem-logs-1.1.1/venv10/Scripts/rst2html5.py
--rw-rw-rw-   0        0        0      863 2023-06-23 07:54:36.000000 exem-logs-1.1.1/venv10/Scripts/rst2latex.py
--rw-rw-rw-   0        0        0      686 2023-06-23 07:54:36.000000 exem-logs-1.1.1/venv10/Scripts/rst2man.py
--rw-rw-rw-   0        0        0      852 2023-06-23 07:54:36.000000 exem-logs-1.1.1/venv10/Scripts/rst2odt.py
--rw-rw-rw-   0        0        0      658 2023-06-23 07:54:36.000000 exem-logs-1.1.1/venv10/Scripts/rst2odt_prepstyles.py
--rw-rw-rw-   0        0        0      671 2023-06-23 07:54:36.000000 exem-logs-1.1.1/venv10/Scripts/rst2pseudoxml.py
--rw-rw-rw-   0        0        0      707 2023-06-23 07:54:36.000000 exem-logs-1.1.1/venv10/Scripts/rst2s5.py
--rw-rw-rw-   0        0        0      943 2023-06-23 07:54:36.000000 exem-logs-1.1.1/venv10/Scripts/rst2xetex.py
--rw-rw-rw-   0        0        0      672 2023-06-23 07:54:36.000000 exem-logs-1.1.1/venv10/Scripts/rst2xml.py
--rw-rw-rw-   0        0        0      740 2023-06-23 07:54:36.000000 exem-logs-1.1.1/venv10/Scripts/rstpep2html.py
+drwxrwxrwx   0        0        0        0 2023-06-23 09:31:09.658043 exem-logs-1.1.2/
+-rw-rw-rw-   0        0        0     5467 2023-06-23 09:06:36.000000 exem-logs-1.1.2/Log.py
+-rw-rw-rw-   0        0        0     8054 2023-06-23 09:31:09.658043 exem-logs-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7651 2023-06-23 09:06:16.000000 exem-logs-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 09:31:09.597620 exem-logs-1.1.2/exem_logs.egg-info/
+-rw-rw-rw-   0        0        0     8054 2023-06-23 09:31:09.000000 exem-logs-1.1.2/exem_logs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      618 2023-06-23 09:31:09.000000 exem-logs-1.1.2/exem_logs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 09:31:09.000000 exem-logs-1.1.2/exem_logs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-06-23 09:31:09.000000 exem-logs-1.1.2/exem_logs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-23 09:31:09.000000 exem-logs-1.1.2/exem_logs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 09:31:09.658043 exem-logs-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      731 2023-06-23 09:30:30.000000 exem-logs-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 09:31:09.577449 exem-logs-1.1.2/venv10/
+drwxrwxrwx   0        0        0        0 2023-06-23 09:31:09.658043 exem-logs-1.1.2/venv10/Scripts/
+-rw-rw-rw-   0        0        0     1169 2023-06-23 07:53:35.000000 exem-logs-1.1.2/venv10/Scripts/activate_this.py
+-rw-rw-rw-   0        0        0     6456 2023-06-23 08:01:20.000000 exem-logs-1.1.2/venv10/Scripts/fixup_errorreporting_v1beta1_keywords.py
+-rw-rw-rw-   0        0        0      664 2023-06-23 07:54:36.000000 exem-logs-1.1.2/venv10/Scripts/rst2html.py
+-rw-rw-rw-   0        0        0      786 2023-06-23 07:54:36.000000 exem-logs-1.1.2/venv10/Scripts/rst2html4.py
+-rw-rw-rw-   0        0        0     1121 2023-06-23 07:54:36.000000 exem-logs-1.1.2/venv10/Scripts/rst2html5.py
+-rw-rw-rw-   0        0        0      863 2023-06-23 07:54:36.000000 exem-logs-1.1.2/venv10/Scripts/rst2latex.py
+-rw-rw-rw-   0        0        0      686 2023-06-23 07:54:36.000000 exem-logs-1.1.2/venv10/Scripts/rst2man.py
+-rw-rw-rw-   0        0        0      852 2023-06-23 07:54:36.000000 exem-logs-1.1.2/venv10/Scripts/rst2odt.py
+-rw-rw-rw-   0        0        0      658 2023-06-23 07:54:36.000000 exem-logs-1.1.2/venv10/Scripts/rst2odt_prepstyles.py
+-rw-rw-rw-   0        0        0      671 2023-06-23 07:54:36.000000 exem-logs-1.1.2/venv10/Scripts/rst2pseudoxml.py
+-rw-rw-rw-   0        0        0      707 2023-06-23 07:54:36.000000 exem-logs-1.1.2/venv10/Scripts/rst2s5.py
+-rw-rw-rw-   0        0        0      943 2023-06-23 07:54:36.000000 exem-logs-1.1.2/venv10/Scripts/rst2xetex.py
+-rw-rw-rw-   0        0        0      672 2023-06-23 07:54:36.000000 exem-logs-1.1.2/venv10/Scripts/rst2xml.py
+-rw-rw-rw-   0        0        0      740 2023-06-23 07:54:36.000000 exem-logs-1.1.2/venv10/Scripts/rstpep2html.py
```

### Comparing `exem-logs-1.1.1/Log.py` & `exem-logs-1.1.2/Log.py`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.1/README.md` & `exem-logs-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.1/exem_logs.egg-info/SOURCES.txt` & `exem-logs-1.1.2/exem_logs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.1/setup.py` & `exem-logs-1.1.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name='exem-logs',
-    version='1.1.1',
-    description='Powerfull but simplest way to log your python application',
+    version='1.1.2',
+    description='Powerfull but simplest way to log your python application.',
+    long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
     url='https://gitlab.com/exem2/libraries/logs',
     author='Félix BOULE--REIFF',
     author_email='boulereiff@exem.fr',
     license='BSD 2-clause',
     install_requires=[
         'google-cloud',
         'google-cloud-logging',
```

### Comparing `exem-logs-1.1.1/venv10/Scripts/activate_this.py` & `exem-logs-1.1.2/venv10/Scripts/activate_this.py`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.1/venv10/Scripts/fixup_errorreporting_v1beta1_keywords.py` & `exem-logs-1.1.2/venv10/Scripts/fixup_errorreporting_v1beta1_keywords.py`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.1/venv10/Scripts/rst2html.py` & `exem-logs-1.1.2/venv10/Scripts/rst2html.py`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.1/venv10/Scripts/rst2html4.py` & `exem-logs-1.1.2/venv10/Scripts/rst2html4.py`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.1/venv10/Scripts/rst2html5.py` & `exem-logs-1.1.2/venv10/Scripts/rst2html5.py`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.1/venv10/Scripts/rst2latex.py` & `exem-logs-1.1.2/venv10/Scripts/rst2latex.py`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.1/venv10/Scripts/rst2man.py` & `exem-logs-1.1.2/venv10/Scripts/rst2man.py`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.1/venv10/Scripts/rst2odt.py` & `exem-logs-1.1.2/venv10/Scripts/rst2odt.py`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.1/venv10/Scripts/rst2odt_prepstyles.py` & `exem-logs-1.1.2/venv10/Scripts/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.1/venv10/Scripts/rst2pseudoxml.py` & `exem-logs-1.1.2/venv10/Scripts/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.1/venv10/Scripts/rst2s5.py` & `exem-logs-1.1.2/venv10/Scripts/rst2s5.py`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.1/venv10/Scripts/rst2xetex.py` & `exem-logs-1.1.2/venv10/Scripts/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.1/venv10/Scripts/rst2xml.py` & `exem-logs-1.1.2/venv10/Scripts/rst2xml.py`

 * *Files identical despite different names*

### Comparing `exem-logs-1.1.1/venv10/Scripts/rstpep2html.py` & `exem-logs-1.1.2/venv10/Scripts/rstpep2html.py`

 * *Files identical despite different names*


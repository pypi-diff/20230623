# Comparing `tmp/material-va-lighthouse-1.1.0.tar.gz` & `tmp/material-va-lighthouse-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "material-va-lighthouse-1.1.0.tar", last modified: Wed May 10 19:27:22 2023, max compression
+gzip compressed data, was "material-va-lighthouse-1.1.2.tar", last modified: Fri Jun 23 20:14:12 2023, max compression
```

## Comparing `material-va-lighthouse-1.1.0.tar` & `material-va-lighthouse-1.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 alastair   (501) staff       (20)        0 2023-05-10 19:27:22.430939 material-va-lighthouse-1.1.0/
--rw-r--r--   0 alastair   (501) staff       (20)     1327 2023-05-10 19:02:44.000000 material-va-lighthouse-1.1.0/LICENSE
--rw-r--r--   0 alastair   (501) staff       (20)      267 2023-05-10 19:27:22.430666 material-va-lighthouse-1.1.0/PKG-INFO
--rw-r--r--   0 alastair   (501) staff       (20)      877 2023-05-10 19:02:44.000000 material-va-lighthouse-1.1.0/README.md
-drwxr-xr-x   0 alastair   (501) staff       (20)        0 2023-05-10 19:27:22.399261 material-va-lighthouse-1.1.0/material_va_lighthouse/
--rw-r--r--   0 alastair   (501) staff       (20)        0 2023-05-10 19:02:44.000000 material-va-lighthouse-1.1.0/material_va_lighthouse/__init__.py
--rw-r--r--   0 alastair   (501) staff       (20)      915 2023-05-10 19:02:44.000000 material-va-lighthouse-1.1.0/material_va_lighthouse/plugin.py
--rw-r--r--   0 alastair   (501) staff       (20)     1099 2023-05-10 19:02:44.000000 material-va-lighthouse-1.1.0/material_va_lighthouse/va_lighthouse.css
--rw-r--r--   0 alastair   (501) staff       (20)     3180 2023-05-10 19:02:44.000000 material-va-lighthouse-1.1.0/material_va_lighthouse/va_lighthouse_logo.png
-drwxr-xr-x   0 alastair   (501) staff       (20)        0 2023-05-10 19:27:22.430154 material-va-lighthouse-1.1.0/material_va_lighthouse.egg-info/
--rw-r--r--   0 alastair   (501) staff       (20)      267 2023-05-10 19:27:22.000000 material-va-lighthouse-1.1.0/material_va_lighthouse.egg-info/PKG-INFO
--rw-r--r--   0 alastair   (501) staff       (20)      459 2023-05-10 19:27:22.000000 material-va-lighthouse-1.1.0/material_va_lighthouse.egg-info/SOURCES.txt
--rw-r--r--   0 alastair   (501) staff       (20)        1 2023-05-10 19:27:22.000000 material-va-lighthouse-1.1.0/material_va_lighthouse.egg-info/dependency_links.txt
--rw-r--r--   0 alastair   (501) staff       (20)       99 2023-05-10 19:27:22.000000 material-va-lighthouse-1.1.0/material_va_lighthouse.egg-info/entry_points.txt
--rw-r--r--   0 alastair   (501) staff       (20)       44 2023-05-10 19:27:22.000000 material-va-lighthouse-1.1.0/material_va_lighthouse.egg-info/requires.txt
--rw-r--r--   0 alastair   (501) staff       (20)       23 2023-05-10 19:27:22.000000 material-va-lighthouse-1.1.0/material_va_lighthouse.egg-info/top_level.txt
--rw-r--r--   0 alastair   (501) staff       (20)       38 2023-05-10 19:27:22.431022 material-va-lighthouse-1.1.0/setup.cfg
--rw-r--r--   0 alastair   (501) staff       (20)      740 2023-05-10 19:26:33.000000 material-va-lighthouse-1.1.0/setup.py
+drwxr-xr-x   0 alastairdawson   (501) staff       (20)        0 2023-06-23 20:14:12.053723 material-va-lighthouse-1.1.2/
+-rw-r--r--   0 alastairdawson   (501) staff       (20)     1327 2023-05-19 16:12:29.000000 material-va-lighthouse-1.1.2/LICENSE
+-rw-r--r--   0 alastairdawson   (501) staff       (20)      267 2023-06-23 20:14:12.053574 material-va-lighthouse-1.1.2/PKG-INFO
+-rw-r--r--   0 alastairdawson   (501) staff       (20)      877 2023-05-19 16:12:29.000000 material-va-lighthouse-1.1.2/README.md
+drwxr-xr-x   0 alastairdawson   (501) staff       (20)        0 2023-06-23 20:14:12.052088 material-va-lighthouse-1.1.2/material_va_lighthouse/
+-rw-r--r--   0 alastairdawson   (501) staff       (20)        0 2023-05-19 16:12:29.000000 material-va-lighthouse-1.1.2/material_va_lighthouse/__init__.py
+-rw-r--r--   0 alastairdawson   (501) staff       (20)      915 2023-05-19 16:12:29.000000 material-va-lighthouse-1.1.2/material_va_lighthouse/plugin.py
+-rw-r--r--   0 alastairdawson   (501) staff       (20)     1099 2023-05-19 16:12:29.000000 material-va-lighthouse-1.1.2/material_va_lighthouse/va_lighthouse.css
+-rw-r--r--   0 alastairdawson   (501) staff       (20)     3180 2023-05-19 16:12:29.000000 material-va-lighthouse-1.1.2/material_va_lighthouse/va_lighthouse_logo.png
+drwxr-xr-x   0 alastairdawson   (501) staff       (20)        0 2023-06-23 20:14:12.053276 material-va-lighthouse-1.1.2/material_va_lighthouse.egg-info/
+-rw-r--r--   0 alastairdawson   (501) staff       (20)      267 2023-06-23 20:14:12.000000 material-va-lighthouse-1.1.2/material_va_lighthouse.egg-info/PKG-INFO
+-rw-r--r--   0 alastairdawson   (501) staff       (20)      459 2023-06-23 20:14:12.000000 material-va-lighthouse-1.1.2/material_va_lighthouse.egg-info/SOURCES.txt
+-rw-r--r--   0 alastairdawson   (501) staff       (20)        1 2023-06-23 20:14:12.000000 material-va-lighthouse-1.1.2/material_va_lighthouse.egg-info/dependency_links.txt
+-rw-r--r--   0 alastairdawson   (501) staff       (20)       99 2023-06-23 20:14:12.000000 material-va-lighthouse-1.1.2/material_va_lighthouse.egg-info/entry_points.txt
+-rw-r--r--   0 alastairdawson   (501) staff       (20)       66 2023-06-23 20:14:12.000000 material-va-lighthouse-1.1.2/material_va_lighthouse.egg-info/requires.txt
+-rw-r--r--   0 alastairdawson   (501) staff       (20)       23 2023-06-23 20:14:12.000000 material-va-lighthouse-1.1.2/material_va_lighthouse.egg-info/top_level.txt
+-rw-r--r--   0 alastairdawson   (501) staff       (20)       38 2023-06-23 20:14:12.053882 material-va-lighthouse-1.1.2/setup.cfg
+-rw-r--r--   0 alastairdawson   (501) staff       (20)      762 2023-06-23 20:09:18.000000 material-va-lighthouse-1.1.2/setup.py
```

### Comparing `material-va-lighthouse-1.1.0/LICENSE` & `material-va-lighthouse-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `material-va-lighthouse-1.1.0/README.md` & `material-va-lighthouse-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `material-va-lighthouse-1.1.0/material_va_lighthouse/plugin.py` & `material-va-lighthouse-1.1.2/material_va_lighthouse/plugin.py`

 * *Files identical despite different names*

### Comparing `material-va-lighthouse-1.1.0/material_va_lighthouse/va_lighthouse.css` & `material-va-lighthouse-1.1.2/material_va_lighthouse/va_lighthouse.css`

 * *Files identical despite different names*

### Comparing `material-va-lighthouse-1.1.0/material_va_lighthouse/va_lighthouse_logo.png` & `material-va-lighthouse-1.1.2/material_va_lighthouse/va_lighthouse_logo.png`

 * *Files identical despite different names*

### Comparing `material-va-lighthouse-1.1.0/setup.py` & `material-va-lighthouse-1.1.2/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name="material-va-lighthouse",
-    version="1.1.0",
+    version="1.1.2",
     description="A MKDocs plugin which extends the material theme with styles from the VA design system",
     author="Alastair Dawson",
     author_email="alastair.j.dawson@gmail.com",
     license="CC0 1.0",
     packages=find_packages(),
     include_package_data=True,
     package_data={"material_va_lighthouse": ["va_lighthouse.css", "va_lighthouse_logo.png"]},
     install_requires=[
-        "mkdocs",
-        "mkdocs-material",
-        "mkdocs-techdocs-core",
+        "mkdocs==1.4.3",
+        "mkdocs-material==8.1.11",
+        "mkdocs-techdocs-core==1.1.7",
     ],
     entry_points={
         "mkdocs.plugins": [
             "material-va-lighthouse = material_va_lighthouse.plugin:MaterialVALighthousePlugin"
         ],
     },
 )
```


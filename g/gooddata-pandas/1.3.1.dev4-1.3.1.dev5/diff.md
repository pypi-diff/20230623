# Comparing `tmp/gooddata-pandas-1.3.1.dev4.tar.gz` & `tmp/gooddata-pandas-1.3.1.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gooddata-pandas-1.3.1.dev4.tar", last modified: Mon Jun  5 07:30:33 2023, max compression
+gzip compressed data, was "gooddata-pandas-1.3.1.dev5.tar", last modified: Fri Jun 23 15:18:30 2023, max compression
```

## Comparing `gooddata-pandas-1.3.1.dev4.tar` & `gooddata-pandas-1.3.1.dev5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:30:33.107484 gooddata-pandas-1.3.1.dev4/
--rw-r--r--   0 runner    (1001) docker     (123)    78103 2023-06-05 07:30:18.000000 gooddata-pandas-1.3.1.dev4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-05 07:30:18.000000 gooddata-pandas-1.3.1.dev4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-05 07:30:33.107484 gooddata-pandas-1.3.1.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-05 07:30:18.000000 gooddata-pandas-1.3.1.dev4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:30:33.107484 gooddata-pandas-1.3.1.dev4/gooddata_pandas/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-05 07:30:18.000000 gooddata-pandas-1.3.1.dev4/gooddata_pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-05 07:30:18.000000 gooddata-pandas-1.3.1.dev4/gooddata_pandas/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13090 2023-06-05 07:30:18.000000 gooddata-pandas-1.3.1.dev4/gooddata_pandas/data_access.py
--rw-r--r--   0 runner    (1001) docker     (123)    16321 2023-06-05 07:30:18.000000 gooddata-pandas-1.3.1.dev4/gooddata_pandas/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-05 07:30:18.000000 gooddata-pandas-1.3.1.dev4/gooddata_pandas/good_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-05 07:30:18.000000 gooddata-pandas-1.3.1.dev4/gooddata_pandas/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17729 2023-06-05 07:30:18.000000 gooddata-pandas-1.3.1.dev4/gooddata_pandas/result_convertor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-06-05 07:30:18.000000 gooddata-pandas-1.3.1.dev4/gooddata_pandas/series.py
--rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-06-05 07:30:18.000000 gooddata-pandas-1.3.1.dev4/gooddata_pandas/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 07:30:33.107484 gooddata-pandas-1.3.1.dev4/gooddata_pandas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-05 07:30:33.000000 gooddata-pandas-1.3.1.dev4/gooddata_pandas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-05 07:30:33.000000 gooddata-pandas-1.3.1.dev4/gooddata_pandas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 07:30:33.000000 gooddata-pandas-1.3.1.dev4/gooddata_pandas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-05 07:30:33.000000 gooddata-pandas-1.3.1.dev4/gooddata_pandas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-05 07:30:33.000000 gooddata-pandas-1.3.1.dev4/gooddata_pandas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 07:30:33.107484 gooddata-pandas-1.3.1.dev4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-05 07:30:25.000000 gooddata-pandas-1.3.1.dev4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:30.481857 gooddata-pandas-1.3.1.dev5/
+-rw-r--r--   0 runner    (1001) docker     (123)    78103 2023-06-23 15:18:15.000000 gooddata-pandas-1.3.1.dev5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-23 15:18:15.000000 gooddata-pandas-1.3.1.dev5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-23 15:18:30.481857 gooddata-pandas-1.3.1.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-23 15:18:15.000000 gooddata-pandas-1.3.1.dev5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:30.481857 gooddata-pandas-1.3.1.dev5/gooddata_pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-23 15:18:15.000000 gooddata-pandas-1.3.1.dev5/gooddata_pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-23 15:18:15.000000 gooddata-pandas-1.3.1.dev5/gooddata_pandas/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13090 2023-06-23 15:18:15.000000 gooddata-pandas-1.3.1.dev5/gooddata_pandas/data_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16321 2023-06-23 15:18:15.000000 gooddata-pandas-1.3.1.dev5/gooddata_pandas/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-23 15:18:15.000000 gooddata-pandas-1.3.1.dev5/gooddata_pandas/good_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-23 15:18:15.000000 gooddata-pandas-1.3.1.dev5/gooddata_pandas/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17729 2023-06-23 15:18:15.000000 gooddata-pandas-1.3.1.dev5/gooddata_pandas/result_convertor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-06-23 15:18:15.000000 gooddata-pandas-1.3.1.dev5/gooddata_pandas/series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-06-23 15:18:15.000000 gooddata-pandas-1.3.1.dev5/gooddata_pandas/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:30.481857 gooddata-pandas-1.3.1.dev5/gooddata_pandas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-23 15:18:30.000000 gooddata-pandas-1.3.1.dev5/gooddata_pandas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-23 15:18:30.000000 gooddata-pandas-1.3.1.dev5/gooddata_pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 15:18:30.000000 gooddata-pandas-1.3.1.dev5/gooddata_pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-23 15:18:30.000000 gooddata-pandas-1.3.1.dev5/gooddata_pandas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-23 15:18:30.000000 gooddata-pandas-1.3.1.dev5/gooddata_pandas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 15:18:30.481857 gooddata-pandas-1.3.1.dev5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-23 15:18:22.000000 gooddata-pandas-1.3.1.dev5/setup.py
```

### Comparing `gooddata-pandas-1.3.1.dev4/LICENSE.txt` & `gooddata-pandas-1.3.1.dev5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gooddata-pandas-1.3.1.dev4/PKG-INFO` & `gooddata-pandas-1.3.1.dev5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: gooddata-pandas
-Version: 1.3.1.dev4
+Version: 1.3.1.dev5
 Summary: GoodData.CN to pandas
 Author: GoodData
 Author-email: support@gooddata.com
 License: MIT
-Project-URL: Documentation, https://gooddata-pandas.readthedocs.io/en/v1.3.1.dev4
+Project-URL: Documentation, https://gooddata-pandas.readthedocs.io/en/v1.3.1.dev5
 Project-URL: Source, https://github.com/gooddata/gooddata-python-sdk
 Keywords: gooddata,pandas,series,data,frame,data_frame,analytics,headless,business,intelligence,headless-bi,cloud,native,semantic,layer,sql,metrics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `gooddata-pandas-1.3.1.dev4/README.md` & `gooddata-pandas-1.3.1.dev5/README.md`

 * *Files identical despite different names*

### Comparing `gooddata-pandas-1.3.1.dev4/gooddata_pandas/data_access.py` & `gooddata-pandas-1.3.1.dev5/gooddata_pandas/data_access.py`

 * *Files identical despite different names*

### Comparing `gooddata-pandas-1.3.1.dev4/gooddata_pandas/dataframe.py` & `gooddata-pandas-1.3.1.dev5/gooddata_pandas/dataframe.py`

 * *Files identical despite different names*

### Comparing `gooddata-pandas-1.3.1.dev4/gooddata_pandas/good_pandas.py` & `gooddata-pandas-1.3.1.dev5/gooddata_pandas/good_pandas.py`

 * *Files identical despite different names*

### Comparing `gooddata-pandas-1.3.1.dev4/gooddata_pandas/result_convertor.py` & `gooddata-pandas-1.3.1.dev5/gooddata_pandas/result_convertor.py`

 * *Files identical despite different names*

### Comparing `gooddata-pandas-1.3.1.dev4/gooddata_pandas/series.py` & `gooddata-pandas-1.3.1.dev5/gooddata_pandas/series.py`

 * *Files identical despite different names*

### Comparing `gooddata-pandas-1.3.1.dev4/gooddata_pandas/utils.py` & `gooddata-pandas-1.3.1.dev5/gooddata_pandas/utils.py`

 * *Files identical despite different names*

### Comparing `gooddata-pandas-1.3.1.dev4/gooddata_pandas.egg-info/PKG-INFO` & `gooddata-pandas-1.3.1.dev5/gooddata_pandas.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: gooddata-pandas
-Version: 1.3.1.dev4
+Version: 1.3.1.dev5
 Summary: GoodData.CN to pandas
 Author: GoodData
 Author-email: support@gooddata.com
 License: MIT
-Project-URL: Documentation, https://gooddata-pandas.readthedocs.io/en/v1.3.1.dev4
+Project-URL: Documentation, https://gooddata-pandas.readthedocs.io/en/v1.3.1.dev5
 Project-URL: Source, https://github.com/gooddata/gooddata-python-sdk
 Keywords: gooddata,pandas,series,data,frame,data_frame,analytics,headless,business,intelligence,headless-bi,cloud,native,semantic,layer,sql,metrics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `gooddata-pandas-1.3.1.dev4/setup.py` & `gooddata-pandas-1.3.1.dev5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,35 +3,35 @@
 
 from setuptools import find_packages, setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding="utf-8")
 
 REQUIRES = [
-    "gooddata-sdk~=1.3.1.dev4",
+    "gooddata-sdk~=1.3.1.dev5",
     "pandas>=1.0.0,<2.0.0",
     'importlib-metadata >= 1.0 ; python_version >= "3.7"',
 ]
 
 setup(
     name="gooddata-pandas",
     description="GoodData.CN to pandas",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="1.3.1.dev4",
+    version="1.3.1.dev5",
     author="GoodData",
     author_email="support@gooddata.com",
     license="MIT",
     license_file="LICENSE.txt",
     license_files=("LICENSE.txt",),
     install_requires=REQUIRES,
     packages=find_packages(exclude=["tests*"]),
     python_requires=">=3.7.0",
     project_urls={
-        "Documentation": "https://gooddata-pandas.readthedocs.io/en/v1.3.1.dev4",
+        "Documentation": "https://gooddata-pandas.readthedocs.io/en/v1.3.1.dev5",
         "Source": "https://github.com/gooddata/gooddata-python-sdk",
     },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.7",
```


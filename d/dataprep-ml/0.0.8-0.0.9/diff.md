# Comparing `tmp/dataprep_ml-0.0.8.tar.gz` & `tmp/dataprep_ml-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataprep_ml-0.0.8.tar", max compression
+gzip compressed data, was "dataprep_ml-0.0.9.tar", max compression
```

## Comparing `dataprep_ml-0.0.8.tar` & `dataprep_ml-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35104 2023-01-19 16:36:07.841508 dataprep_ml-0.0.8/LICENSE
--rw-r--r--   0        0        0      130 2023-01-19 16:36:07.841508 dataprep_ml-0.0.8/README.md
--rw-r--r--   0        0        0      190 2023-01-19 16:36:07.841508 dataprep_ml-0.0.8/dataprep_ml/__init__.py
--rw-r--r--   0        0        0     1984 2023-01-19 16:36:07.841508 dataprep_ml-0.0.8/dataprep_ml/base.py
--rw-r--r--   0        0        0    13732 2023-01-19 16:36:07.841508 dataprep_ml-0.0.8/dataprep_ml/cleaners.py
--rw-r--r--   0        0        0     1191 2023-01-19 16:36:07.841508 dataprep_ml-0.0.8/dataprep_ml/helpers.py
--rw-r--r--   0        0        0     3342 2023-01-19 16:36:07.841508 dataprep_ml-0.0.8/dataprep_ml/imputers.py
--rw-r--r--   0        0        0     9213 2023-01-19 16:36:07.841508 dataprep_ml-0.0.8/dataprep_ml/insights.py
--rw-r--r--   0        0        0     6531 2023-01-19 16:36:07.845509 dataprep_ml-0.0.8/dataprep_ml/splitters.py
--rw-r--r--   0        0        0      558 2023-01-19 16:36:07.845509 dataprep_ml-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      950 1970-01-01 00:00:00.000000 dataprep_ml-0.0.8/setup.py
--rw-r--r--   0        0        0      965 1970-01-01 00:00:00.000000 dataprep_ml-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    35104 2023-02-22 04:59:45.199893 dataprep_ml-0.0.9/LICENSE
+-rw-r--r--   0        0        0      130 2023-02-22 04:59:45.199893 dataprep_ml-0.0.9/README.md
+-rw-r--r--   0        0        0      190 2023-02-22 04:59:45.199893 dataprep_ml-0.0.9/dataprep_ml/__init__.py
+-rw-r--r--   0        0        0     1984 2023-02-22 04:59:45.199893 dataprep_ml-0.0.9/dataprep_ml/base.py
+-rw-r--r--   0        0        0    13732 2023-02-22 04:59:45.199893 dataprep_ml-0.0.9/dataprep_ml/cleaners.py
+-rw-r--r--   0        0        0     1191 2023-02-22 04:59:45.199893 dataprep_ml-0.0.9/dataprep_ml/helpers.py
+-rw-r--r--   0        0        0     3342 2023-02-22 04:59:45.199893 dataprep_ml-0.0.9/dataprep_ml/imputers.py
+-rw-r--r--   0        0        0     9213 2023-02-22 04:59:45.199893 dataprep_ml-0.0.9/dataprep_ml/insights.py
+-rw-r--r--   0        0        0     6549 2023-02-22 04:59:45.199893 dataprep_ml-0.0.9/dataprep_ml/splitters.py
+-rw-r--r--   0        0        0      558 2023-02-22 04:59:45.203893 dataprep_ml-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      950 1970-01-01 00:00:00.000000 dataprep_ml-0.0.9/setup.py
+-rw-r--r--   0        0        0      965 1970-01-01 00:00:00.000000 dataprep_ml-0.0.9/PKG-INFO
```

### Comparing `dataprep_ml-0.0.8/LICENSE` & `dataprep_ml-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dataprep_ml-0.0.8/dataprep_ml/base.py` & `dataprep_ml-0.0.9/dataprep_ml/base.py`

 * *Files identical despite different names*

### Comparing `dataprep_ml-0.0.8/dataprep_ml/cleaners.py` & `dataprep_ml-0.0.9/dataprep_ml/cleaners.py`

 * *Files identical despite different names*

### Comparing `dataprep_ml-0.0.8/dataprep_ml/helpers.py` & `dataprep_ml-0.0.9/dataprep_ml/helpers.py`

 * *Files identical despite different names*

### Comparing `dataprep_ml-0.0.8/dataprep_ml/imputers.py` & `dataprep_ml-0.0.9/dataprep_ml/imputers.py`

 * *Files identical despite different names*

### Comparing `dataprep_ml-0.0.8/dataprep_ml/insights.py` & `dataprep_ml-0.0.9/dataprep_ml/insights.py`

 * *Files identical despite different names*

### Comparing `dataprep_ml-0.0.8/dataprep_ml/splitters.py` & `dataprep_ml-0.0.9/dataprep_ml/splitters.py`

 * *Files 5% similar despite different names*

```diff
@@ -124,17 +124,17 @@
         for idx, col in enumerate(stratify_on):
             df = df[df[col] == group[idx]]
 
         train_cutoff = round(df.shape[0] * pct_train)
         dev_cutoff = round(df.shape[0] * pct_dev) + train_cutoff
         test_cutoff = round(df.shape[0] * pct_test) + dev_cutoff
 
-        train_st = train_st.append(df[:train_cutoff])
-        dev_st = dev_st.append(df[train_cutoff:dev_cutoff])
-        test_st = test_st.append(df[dev_cutoff:test_cutoff])
+        train_st = pd.concat([train_st, df[:train_cutoff]])
+        dev_st = pd.concat([dev_st, df[train_cutoff:dev_cutoff]])
+        test_st = pd.concat([test_st, df[dev_cutoff:test_cutoff]])
 
     if reshuffle:
         train_st, dev_st, test_st = [df.sample(frac=1, random_state=seed).reset_index(drop=True)
                                      for df in [train_st, dev_st, test_st]]
 
     # check that stratified lengths conform to expected percentages
     emp_tr = len(train_st) / len(data)
```

### Comparing `dataprep_ml-0.0.8/pyproject.toml` & `dataprep_ml-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataprep-ml"
-version = "0.0.8"
+version = "0.0.9"
 description = "Automated dataframe analysis for Machine Learning pipelines."
 authors = ["MindsDB Inc. <hello@mindsdb.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 packages = [{include = "dataprep_ml"}]
 
 [tool.poetry.dependencies]
```

### Comparing `dataprep_ml-0.0.8/setup.py` & `dataprep_ml-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'pydateinfer==0.3.0',
  'python-dateutil>=2.1',
  'scipy>=1.5.4',
  'type-infer>=0.0.7']
 
 setup_kwargs = {
     'name': 'dataprep-ml',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'Automated dataframe analysis for Machine Learning pipelines.',
     'long_description': '# dataprep_ml\nData utilities for Machine Learning pipelines.\n\n\n## Submodules\n\n1. Data cleaning\n2. Data analysis\n3. Data splitting\n',
     'author': 'MindsDB Inc.',
     'author_email': 'hello@mindsdb.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `dataprep_ml-0.0.8/PKG-INFO` & `dataprep_ml-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataprep-ml
-Version: 0.0.8
+Version: 0.0.9
 Summary: Automated dataframe analysis for Machine Learning pipelines.
 License: GPL-3.0
 Author: MindsDB Inc.
 Author-email: hello@mindsdb.com
 Requires-Python: >=3.7,<3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```


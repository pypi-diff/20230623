# Comparing `tmp/quiffen-2.0.7.tar.gz` & `tmp/quiffen-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quiffen-2.0.7.tar", max compression
+gzip compressed data, was "quiffen-2.0.8.tar", max compression
```

## Comparing `quiffen-2.0.7.tar` & `quiffen-2.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    35148 2023-04-02 10:05:40.430967 quiffen-2.0.7/LICENSE
--rw-r--r--   0        0        0     4192 2023-04-02 10:05:40.430967 quiffen-2.0.7/README.rst
--rw-r--r--   0        0        0     1285 2023-04-02 10:36:46.640692 quiffen-2.0.7/pyproject.toml
--rw-r--r--   0        0        0      837 2023-04-02 10:05:40.480967 quiffen-2.0.7/quiffen/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 10:05:40.480967 quiffen-2.0.7/quiffen/core/__init__.py
--rw-r--r--   0        0        0     8684 2023-04-02 10:05:40.480967 quiffen-2.0.7/quiffen/core/account.py
--rw-r--r--   0        0        0     3189 2023-04-02 10:05:40.480967 quiffen-2.0.7/quiffen/core/base.py
--rw-r--r--   0        0        0    17647 2023-04-02 10:05:40.480967 quiffen-2.0.7/quiffen/core/category.py
--rw-r--r--   0        0        0     3027 2023-04-02 10:05:40.480967 quiffen-2.0.7/quiffen/core/class_type.py
--rw-r--r--   0        0        0     7288 2023-04-02 10:05:40.480967 quiffen-2.0.7/quiffen/core/investment.py
--rw-r--r--   0        0        0    20088 2023-04-02 10:36:46.640692 quiffen-2.0.7/quiffen/core/qif.py
--rw-r--r--   0        0        0     4487 2023-04-02 10:05:40.480967 quiffen-2.0.7/quiffen/core/security.py
--rw-r--r--   0        0        0     4147 2023-04-02 10:05:40.480967 quiffen-2.0.7/quiffen/core/split.py
--rw-r--r--   0        0        0    20693 2023-04-02 10:05:40.480967 quiffen-2.0.7/quiffen/core/transaction.py
--rw-r--r--   0        0        0     4517 2023-04-02 10:05:40.480967 quiffen-2.0.7/quiffen/utils.py
--rw-r--r--   0        0        0     5361 1970-01-01 00:00:00.000000 quiffen-2.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-08 20:15:13.884314 quiffen-2.0.8/LICENSE
+-rw-r--r--   0        0        0     4192 2023-04-02 10:05:40.430967 quiffen-2.0.8/README.rst
+-rw-r--r--   0        0        0     1275 2023-06-23 18:54:34.887773 quiffen-2.0.8/pyproject.toml
+-rw-r--r--   0        0        0      837 2023-04-02 10:05:40.480967 quiffen-2.0.8/quiffen/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 10:05:40.480967 quiffen-2.0.8/quiffen/core/__init__.py
+-rw-r--r--   0        0        0     8684 2023-04-02 10:05:40.480967 quiffen-2.0.8/quiffen/core/account.py
+-rw-r--r--   0        0        0     3189 2023-04-02 10:05:40.480967 quiffen-2.0.8/quiffen/core/base.py
+-rw-r--r--   0        0        0    17647 2023-04-02 10:05:40.480967 quiffen-2.0.8/quiffen/core/category.py
+-rw-r--r--   0        0        0     3027 2023-04-02 10:05:40.480967 quiffen-2.0.8/quiffen/core/class_type.py
+-rw-r--r--   0        0        0     7288 2023-04-02 10:05:40.480967 quiffen-2.0.8/quiffen/core/investment.py
+-rw-r--r--   0        0        0    20096 2023-06-23 18:54:18.217776 quiffen-2.0.8/quiffen/core/qif.py
+-rw-r--r--   0        0        0     4487 2023-04-02 10:05:40.480967 quiffen-2.0.8/quiffen/core/security.py
+-rw-r--r--   0        0        0     4147 2023-04-02 10:05:40.480967 quiffen-2.0.8/quiffen/core/split.py
+-rw-r--r--   0        0        0    20693 2023-04-02 10:05:40.480967 quiffen-2.0.8/quiffen/core/transaction.py
+-rw-r--r--   0        0        0     4517 2023-04-02 10:05:40.480967 quiffen-2.0.8/quiffen/utils.py
+-rw-r--r--   0        0        0     5313 1970-01-01 00:00:00.000000 quiffen-2.0.8/PKG-INFO
```

### Comparing `quiffen-2.0.7/README.rst` & `quiffen-2.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `quiffen-2.0.7/pyproject.toml` & `quiffen-2.0.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "quiffen"
-version = "2.0.7"
+version = "2.0.8"
 description = "Quiffen"
 authors = ["Isaac Harris-Holt <isaac@harris-holt.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.rst"
 homepage = "https://github.com/isaacharrisholt/quiffen"
 repository = "https://github.com/isaacharrisholt/quiffen"
 documentation = "https://quiffen.readthedocs.io/en/latest/"
 keywords = ['qif', 'finance', 'data processing']
 classifiers = [
-    "Development Status :: 5 - Production/Stable",
-    "Intended Audience :: Developers",
-    "Programming Language :: Python :: 3",
-    "Operating System :: MacOS :: MacOS X",
-    "Operating System :: Microsoft :: Windows"
+  "Development Status :: 5 - Production/Stable",
+  "Intended Audience :: Developers",
+  "Programming Language :: Python :: 3",
+  "Operating System :: MacOS :: MacOS X",
+  "Operating System :: Microsoft :: Windows",
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.10.2"
 pandas = "^1.5.1"
@@ -43,14 +43,14 @@
 profile = "black"
 include_trailing_comma = true
 
 [tool.ruff]
 line-length = 88
 
 [tool.ruff.per-file-ignores]
-"__init__.py" = ["F401"]  # Ignore unused imports in __init__.py
+"__init__.py" = ["F401"] # Ignore unused imports in __init__.py
 
 [tool.pyright]
 pythonVersion = "3.8"
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
```

### Comparing `quiffen-2.0.7/quiffen/__init__.py` & `quiffen-2.0.8/quiffen/__init__.py`

 * *Files identical despite different names*

### Comparing `quiffen-2.0.7/quiffen/core/account.py` & `quiffen-2.0.8/quiffen/core/account.py`

 * *Files identical despite different names*

### Comparing `quiffen-2.0.7/quiffen/core/base.py` & `quiffen-2.0.8/quiffen/core/base.py`

 * *Files identical despite different names*

### Comparing `quiffen-2.0.7/quiffen/core/category.py` & `quiffen-2.0.8/quiffen/core/category.py`

 * *Files identical despite different names*

### Comparing `quiffen-2.0.7/quiffen/core/class_type.py` & `quiffen-2.0.8/quiffen/core/class_type.py`

 * *Files identical despite different names*

### Comparing `quiffen-2.0.7/quiffen/core/investment.py` & `quiffen-2.0.8/quiffen/core/investment.py`

 * *Files identical despite different names*

### Comparing `quiffen-2.0.7/quiffen/core/qif.py` & `quiffen-2.0.8/quiffen/core/qif.py`

 * *Files 0% similar despite different names*

```diff
@@ -268,15 +268,15 @@
                         f"Line {line_number}: "
                         "No account found before transactions. "
                         "This should not happen."
                     )
 
                 accounts[last_account].add_transaction(
                     new_transaction,
-                    AccountType(header_line.split(":")[1]),
+                    AccountType(header_line.split(":")[1].strip()),
                 )
 
                 if new_transaction.category:
                     root = new_transaction.category.traverse_up()[-1]
                     if root.name in categories:
                         categories[root.name].merge(root)
                     else:
```

### Comparing `quiffen-2.0.7/quiffen/core/security.py` & `quiffen-2.0.8/quiffen/core/security.py`

 * *Files identical despite different names*

### Comparing `quiffen-2.0.7/quiffen/core/split.py` & `quiffen-2.0.8/quiffen/core/split.py`

 * *Files identical despite different names*

### Comparing `quiffen-2.0.7/quiffen/core/transaction.py` & `quiffen-2.0.8/quiffen/core/transaction.py`

 * *Files identical despite different names*

### Comparing `quiffen-2.0.7/quiffen/utils.py` & `quiffen-2.0.8/quiffen/utils.py`

 * *Files identical despite different names*

### Comparing `quiffen-2.0.7/PKG-INFO` & `quiffen-2.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quiffen
-Version: 2.0.7
+Version: 2.0.8
 Summary: Quiffen
 Home-page: https://github.com/isaacharrisholt/quiffen
 License: GPL-3.0-or-later
 Keywords: qif,finance,data processing
 Author: Isaac Harris-Holt
 Author-email: isaac@harris-holt.com
 Requires-Python: >=3.8,<4.0
@@ -14,15 +14,14 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Requires-Dist: pandas (>=1.5.1,<2.0.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Project-URL: Documentation, https://quiffen.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/isaacharrisholt/quiffen
 Description-Content-Type: text/x-rst
```


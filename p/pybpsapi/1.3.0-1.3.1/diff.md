# Comparing `tmp/pybpsapi-1.3.0.tar.gz` & `tmp/pybpsapi-1.3.1.tar.gz`

## Comparing `pybpsapi-1.3.0.tar` & `pybpsapi-1.3.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 pybpsapi-1.3.0/CHANGELOG.MD
--rw-r--r--   0        0        0    10930 2020-02-02 00:00:00.000000 pybpsapi-1.3.0/pybpsapi.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 pybpsapi-1.3.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pybpsapi-1.3.0/.gitignore
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 pybpsapi-1.3.0/LICENSE
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 pybpsapi-1.3.0/README.md
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 pybpsapi-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 pybpsapi-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 pybpsapi-1.3.1/CHANGELOG.MD
+-rw-r--r--   0        0        0    10930 2020-02-02 00:00:00.000000 pybpsapi-1.3.1/pybpsapi.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 pybpsapi-1.3.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pybpsapi-1.3.1/.gitignore
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 pybpsapi-1.3.1/LICENSE
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 pybpsapi-1.3.1/README.md
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 pybpsapi-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 pybpsapi-1.3.1/PKG-INFO
```

### Comparing `pybpsapi-1.3.0/CHANGELOG.MD` & `pybpsapi-1.3.1/CHANGELOG.MD`

 * *Files 4% similar despite different names*

```diff
@@ -59,8 +59,13 @@
 ### Added
 - Dynamic categories support
 
 ### Removed
 - `cached` option in latest circular
 
 ### Improved
-- `CircularChecker` class now returns a sorted dict of new circulars
+- `CircularChecker` class now returns a sorted dict of new circulars
+
+# v1.3.1 - 23/6/2023
+
+### Fixed
+- Changed the param name of /search to `query` from `title` to match API change
```

### Comparing `pybpsapi-1.3.0/pybpsapi.py` & `pybpsapi-1.3.1/pybpsapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     def search(self, query: str or int, amount: int = 1) -> dict or None:
         """The `/search` endpoint lets you search for a circular by its name or ID"""
         if query.isdigit() and len(query) == 4:
             query = int(query)
         elif type(query) != str:
             raise ValueError("Invalid Query")
 
-        params = {'title': query, 'amount': amount}
+        params = {'query': query, 'amount': amount}
 
         request = requests.get(self.url + "search", params=params)
         json = request.json()
 
         try:
             json['http_status']
```

### Comparing `pybpsapi-1.3.0/.github/workflows/python-publish.yml` & `pybpsapi-1.3.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pybpsapi-1.3.0/LICENSE` & `pybpsapi-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pybpsapi-1.3.0/README.md` & `pybpsapi-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pybpsapi-1.3.0/pyproject.toml` & `pybpsapi-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pybpsapi"
-version = "1.3.0"
+version = "1.3.1"
 description = "This package is a Python wrapper for the BPS API. It supports all the five endpoints of the API, and also contains a good circular-checking system."
 author = "Raj Dave"
 author-email = "rajdave8002@gmail.com"
 homepage = "https://bpsapi.rajtech.me/"
 license = "MIT"
 keywords = ["bpsapi", "bps", "api", "wrapper", "python", "python3"]
 requires-python = ">=3.6"
```

### Comparing `pybpsapi-1.3.0/PKG-INFO` & `pybpsapi-1.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybpsapi
-Version: 1.3.0
+Version: 1.3.1
 Summary: This package is a Python wrapper for the BPS API. It supports all the five endpoints of the API, and also contains a good circular-checking system.
 License-Expression: MIT
 License-File: LICENSE
 Keywords: api,bps,bpsapi,python,python3,wrapper
 Requires-Python: >=3.6
 Requires-Dist: requests
 Description-Content-Type: text/markdown
```


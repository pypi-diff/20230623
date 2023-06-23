# Comparing `tmp/jam_ai-0.1.4.tar.gz` & `tmp/jam_ai-0.1.5.tar.gz`

## Comparing `jam_ai-0.1.4.tar` & `jam_ai-0.1.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.4/cmd/__init__.py
--rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 jam_ai-0.1.4/cmd/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.4/example/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.4/example/personnel/__init__.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 jam_ai-0.1.4/example/personnel/albert-einstein.json
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 jam_ai-0.1.4/example/personnel/homer-simpson.json
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 jam_ai-0.1.4/example/personnel/marie-curie.json
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 jam_ai-0.1.4/example/personnel/walter-white.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jam_ai-0.1.4/jam/__init__.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 jam_ai-0.1.4/jam/base.py
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 jam_ai-0.1.4/jam/core.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 jam_ai-0.1.4/jam/version.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 jam_ai-0.1.4/jam/instrument/__init__.py
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 jam_ai-0.1.4/jam/instrument/base.py
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 jam_ai-0.1.4/jam/instrument/image.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.4/jam/instrument/text.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 jam_ai-0.1.4/jam/interface/__init__.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 jam_ai-0.1.4/jam/interface/base.py
--rw-r--r--   0        0        0     3546 2020-02-02 00:00:00.000000 jam_ai-0.1.4/jam/interface/openai.py
--rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 jam_ai-0.1.4/jam/interface/stability_ai.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 jam_ai-0.1.4/jam/persistence/__init__.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 jam_ai-0.1.4/jam/persistence/base.py
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 jam_ai-0.1.4/jam/persistence/memory.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 jam_ai-0.1.4/jam/persistence/model.py
--rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 jam_ai-0.1.4/jam/persistence/sqlite.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jam_ai-0.1.4/jam/personnel/__init__.py
--rw-r--r--   0        0        0     6950 2020-02-02 00:00:00.000000 jam_ai-0.1.4/jam/personnel/base.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jam_ai-0.1.4/jam/personnel/personnel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.4/jam/util/__init__.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 jam_ai-0.1.4/jam/util/generate.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 jam_ai-0.1.4/jam/util/search.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.4/tests/instrument/__init__.py
--rw-r--r--   0        0        0    10211 2020-02-02 00:00:00.000000 jam_ai-0.1.4/tests/instrument/test_base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.4/tests/interface/__init__.py
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 jam_ai-0.1.4/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 jam_ai-0.1.4/LICENSE
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 jam_ai-0.1.4/README.md
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 jam_ai-0.1.4/pyproject.toml
--rw-r--r--   0        0        0    15914 2020-02-02 00:00:00.000000 jam_ai-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.5/cmd/__init__.py
+-rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 jam_ai-0.1.5/cmd/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.5/example/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.5/example/personnel/__init__.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 jam_ai-0.1.5/example/personnel/albert-einstein.json
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 jam_ai-0.1.5/example/personnel/homer-simpson.json
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 jam_ai-0.1.5/example/personnel/marie-curie.json
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 jam_ai-0.1.5/example/personnel/walter-white.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/__init__.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/base.py
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/core.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/version.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/instrument/__init__.py
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/instrument/base.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/instrument/image.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/instrument/text.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/interface/__init__.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/interface/base.py
+-rw-r--r--   0        0        0     3546 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/interface/openai.py
+-rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/interface/stability_ai.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/persistence/__init__.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/persistence/base.py
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/persistence/memory.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/persistence/model.py
+-rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/persistence/sqlite.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/personnel/__init__.py
+-rw-r--r--   0        0        0     6950 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/personnel/base.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/personnel/personnel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/util/__init__.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/util/generate.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 jam_ai-0.1.5/jam/util/search.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.5/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.5/tests/instrument/__init__.py
+-rw-r--r--   0        0        0    10211 2020-02-02 00:00:00.000000 jam_ai-0.1.5/tests/instrument/test_base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.5/tests/interface/__init__.py
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 jam_ai-0.1.5/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 jam_ai-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 jam_ai-0.1.5/README.md
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 jam_ai-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0    15915 2020-02-02 00:00:00.000000 jam_ai-0.1.5/PKG-INFO
```

### Comparing `jam_ai-0.1.4/cmd/main.py` & `jam_ai-0.1.5/cmd/main.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.4/example/personnel/albert-einstein.json` & `jam_ai-0.1.5/example/personnel/albert-einstein.json`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.4/example/personnel/homer-simpson.json` & `jam_ai-0.1.5/example/personnel/homer-simpson.json`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.4/example/personnel/marie-curie.json` & `jam_ai-0.1.5/example/personnel/marie-curie.json`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.4/example/personnel/walter-white.json` & `jam_ai-0.1.5/example/personnel/walter-white.json`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.4/jam/base.py` & `jam_ai-0.1.5/jam/base.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.4/jam/core.py` & `jam_ai-0.1.5/jam/core.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.4/jam/instrument/base.py` & `jam_ai-0.1.5/jam/instrument/base.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.4/jam/instrument/image.py` & `jam_ai-0.1.5/jam/instrument/image.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.4/jam/interface/base.py` & `jam_ai-0.1.5/jam/interface/base.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.4/jam/interface/openai.py` & `jam_ai-0.1.5/jam/interface/openai.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.4/jam/interface/stability_ai.py` & `jam_ai-0.1.5/jam/interface/stability_ai.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.4/jam/persistence/base.py` & `jam_ai-0.1.5/jam/persistence/base.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.4/jam/persistence/memory.py` & `jam_ai-0.1.5/jam/persistence/memory.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.4/jam/persistence/model.py` & `jam_ai-0.1.5/jam/persistence/model.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.4/jam/persistence/sqlite.py` & `jam_ai-0.1.5/jam/persistence/sqlite.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.4/jam/personnel/base.py` & `jam_ai-0.1.5/jam/personnel/base.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.4/tests/instrument/test_base.py` & `jam_ai-0.1.5/tests/instrument/test_base.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.4/.gitignore` & `jam_ai-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.4/LICENSE` & `jam_ai-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.4/README.md` & `jam_ai-0.1.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 )
 
 ```
 
 ## Installation
 
 ```bash
-~ pip install jam --upgrade
+pip install jam-ai --upgrade
 ```
 You need to use Pip to install jam. Conda package is currently unavailable.
 
 ### Requirements
 * Python >= 3.8
 * OpenAI
```

### Comparing `jam_ai-0.1.4/pyproject.toml` & `jam_ai-0.1.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jam-ai"
-version = "0.1.4"
+version = "0.1.5"
 version_pattern = "MAJOR.MINOR.PATCH"
 authors = [
   { name="Abhishta Gatya", email="abhishtagatya@yahoo.com" },
 ]
 description = "Experimental collaboration tool to use multiple AI personnel together equipped with instructed function calls."
 keywords = ["openai", "multi agent", "chat engine", "collaboration", "machine learning", "data science"]
 readme = "README.md"
```

### Comparing `jam_ai-0.1.4/PKG-INFO` & `jam_ai-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jam-ai
-Version: 0.1.4
+Version: 0.1.5
 Summary: Experimental collaboration tool to use multiple AI personnel together equipped with instructed function calls.
 Project-URL: homepage, https://github.com/abhishtagatya/jam
 Project-URL: documentation, https://github.com/abhishtagatya/jam
 Project-URL: changelog, https://github.com/abhishtagatya/jam/blob/master/CHANGELOG.md
 Author-email: Abhishta Gatya <abhishtagatya@yahoo.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
@@ -272,15 +272,15 @@
 )
 
 ```
 
 ## Installation
 
 ```bash
-~ pip install jam --upgrade
+pip install jam-ai --upgrade
 ```
 You need to use Pip to install jam. Conda package is currently unavailable.
 
 ### Requirements
 * Python >= 3.8
 * OpenAI
```


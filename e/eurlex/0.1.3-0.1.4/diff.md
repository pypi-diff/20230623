# Comparing `tmp/eurlex-0.1.3.tar.gz` & `tmp/eurlex-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eurlex-0.1.3.tar", last modified: Wed Jul  6 15:57:14 2022, max compression
+gzip compressed data, was "eurlex-0.1.4.tar", last modified: Fri Jun 23 09:50:34 2023, max compression
```

## Comparing `eurlex-0.1.3.tar` & `eurlex-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 15:57:14.135106 eurlex-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (121)     3413 2022-07-06 15:57:14.135106 eurlex-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2629 2022-07-06 15:56:44.000000 eurlex-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 15:57:14.135106 eurlex-0.1.3/eurlex/
--rw-r--r--   0 runner    (1001) docker     (121)    26094 2022-07-06 15:56:44.000000 eurlex-0.1.3/eurlex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 15:57:14.135106 eurlex-0.1.3/eurlex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3413 2022-07-06 15:57:14.000000 eurlex-0.1.3/eurlex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-07-06 15:57:14.000000 eurlex-0.1.3/eurlex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-06 15:57:14.000000 eurlex-0.1.3/eurlex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-07-06 15:57:14.000000 eurlex-0.1.3/eurlex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-07-06 15:57:14.000000 eurlex-0.1.3/eurlex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-06 15:57:14.135106 eurlex-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      770 2022-07-06 15:56:44.000000 eurlex-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 15:57:14.135106 eurlex-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1602 2022-07-06 15:56:44.000000 eurlex-0.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3484 2022-07-06 15:56:44.000000 eurlex-0.1.3/tests/test_parsing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:50:34.793387 eurlex-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-06-23 09:50:34.793387 eurlex-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-06-23 09:49:54.000000 eurlex-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:50:34.793387 eurlex-0.1.4/eurlex/
+-rw-r--r--   0 runner    (1001) docker     (123)    27747 2023-06-23 09:49:54.000000 eurlex-0.1.4/eurlex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:50:34.793387 eurlex-0.1.4/eurlex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-06-23 09:50:34.000000 eurlex-0.1.4/eurlex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-23 09:50:34.000000 eurlex-0.1.4/eurlex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 09:50:34.000000 eurlex-0.1.4/eurlex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-23 09:50:34.000000 eurlex-0.1.4/eurlex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-23 09:50:34.000000 eurlex-0.1.4/eurlex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 09:50:34.793387 eurlex-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-23 09:49:54.000000 eurlex-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:50:34.793387 eurlex-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-06-23 09:49:54.000000 eurlex-0.1.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-06-23 09:49:54.000000 eurlex-0.1.4/tests/test_parsing.py
```

### Comparing `eurlex-0.1.3/PKG-INFO` & `eurlex-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: eurlex
-Version: 0.1.3
+Version: 0.1.4
 Summary: An EUR-Lex parser for Python.
 Home-page: https://github.com/kevin91nl/eurlex
 Author: K.M.J. Jacobs
-Author-email: mail@kevinjacobs.nl
+Author-email: kmj.jacobs@maastrichtuniversity.nl
 License: UNKNOWN
 Description: # EUR-Lex Parser
         
         <p>
             <a href="https://github.com/kevin91nl/eurlex/actions/workflows/building.yaml"><img src="https://github.com/kevin91nl/eurlex/actions/workflows/building.yaml/badge.svg" alt="Building" height="18"></a>
             <a href="https://badge.fury.io/py/eurlex"><img src="https://badge.fury.io/py/eurlex.svg" alt="PyPI version" height="18"></a>
             <a href=https://github.com/ambv/black><img src="https://img.shields.io/badge/code%20style-black-000000.svg" height="18"></a>
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: eurlex Version: 0.1.3 Summary: An EUR-Lex parser
+Metadata-Version: 2.1 Name: eurlex Version: 0.1.4 Summary: An EUR-Lex parser
 for Python. Home-page: https://github.com/kevin91nl/eurlex Author: K.M.J.
-Jacobs Author-email: mail@kevinjacobs.nl License: UNKNOWN Description: # EUR-
-Lex Parser
+Jacobs Author-email: kmj.jacobs@maastrichtuniversity.nl License: UNKNOWN
+Description: # EUR-Lex Parser
 [Building] [PyPI_version] [https://img.shields.io/badge/code%20style-black-
 000000.svg]
 An EUR-Lex parser for Python. ## Usage You can install this package as follows:
 ```bash pip install -U eurlex ``` After installing this package, you can
 download and parse any document from EUR-Lex. For example, the [32019R0947
 regulation](https://eur-lex.europa.eu/legal-content/EN/TXT/
 ?uri=CELEX%3A32019R0947): ```python from eurlex import get_html_by_celex_id,
```

### Comparing `eurlex-0.1.3/README.md` & `eurlex-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `eurlex-0.1.3/eurlex/__init__.py` & `eurlex-0.1.4/eurlex/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 import rdflib
 import requests
 from SPARQLWrapper import SPARQLWrapper, JSON
 import pandas as pd
 import datetime
 from xml.etree import ElementTree as ETree
-
+from typing import List, Dict
 
 def get_prefixes() -> dict:
     """Get a mapping from prefixes to URLs.
 
     Returns
     -------
     dict
@@ -733,14 +733,54 @@
     )  # pragma: no cover
     results = run_query(prepend_prefixes(query))  # pragma: no cover
     cellar_ids = []  # pragma: no cover
     for result in results["results"]["bindings"]:  # pragma: no cover
         cellar_ids.append(result["doc"]["value"].split("/")[-1])  # pragma: no cover
     return cellar_ids  # pragma: no cover
 
+def get_documents(types: List[str] = ["REG"], limit: int = -1) -> List[Dict[str, str]]:
+    """Retrieve a list of of documents of specified types from EUR-Lex that have a CELEX-number, as a list of dicts.
+
+    Parameters
+    ----------
+    types : List[str]
+        The by the SparQL-API recognized type of documents to return
+        Examples: ["DIR", "DIR_IMPL", "DIR_DEL", "REG", "REG_IMPL", "REG_FINANC", "REG_DEL"]
+    limit : int
+        The maximum number of regulations to retrieve. (default: no limit).
+
+    Returns
+    -------
+    List[dict]
+        A list of dicts, containing publication date, publication url, celex number and type of document.
+    """
+    query  = "select distinct ?doc ?type ?celex ?date\n"
+    query += "where{ ?doc cdm:work_has_resource-type ?type.\n"
+    query += "  FILTER(\n    "
+    query += " ||\n    ".join(map(lambda type: f"?type=<http://publications.europa.eu/resource/authority/resource-type/{type}>", types)) 
+    query += "\n  )\n"
+    query += "  FILTER(BOUND(?celex))\n"
+    query += "  OPTIONAL{?doc cdm:resource_legal_id_celex ?celex.}\n"
+    query += "  OPTIONAL{?doc cdm:work_date_document ?date.}\n"
+    query += "}\n"
+    if (limit > 0):
+        query += "limit " + str(limit)
+
+    results = []
+    query_results = run_query(prepend_prefixes(query))
+        
+    for result in query_results["results"]["bindings"]:
+        results.append({
+            "celex": result["celex"]["value"],
+            "date": result["date"]["value"],
+            "link": result["doc"]["value"],
+            "type": result["type"]["value"].split("/")[-1]
+        })
+
+    return results    
 
 def process_paragraphs(paragraphs: list) -> pd.DataFrame:
     """Process the paragraphs.
 
     Parameters
     ----------
     paragraphs : list
```

### Comparing `eurlex-0.1.3/eurlex.egg-info/PKG-INFO` & `eurlex-0.1.4/eurlex.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: eurlex
-Version: 0.1.3
+Version: 0.1.4
 Summary: An EUR-Lex parser for Python.
 Home-page: https://github.com/kevin91nl/eurlex
 Author: K.M.J. Jacobs
-Author-email: mail@kevinjacobs.nl
+Author-email: kmj.jacobs@maastrichtuniversity.nl
 License: UNKNOWN
 Description: # EUR-Lex Parser
         
         <p>
             <a href="https://github.com/kevin91nl/eurlex/actions/workflows/building.yaml"><img src="https://github.com/kevin91nl/eurlex/actions/workflows/building.yaml/badge.svg" alt="Building" height="18"></a>
             <a href="https://badge.fury.io/py/eurlex"><img src="https://badge.fury.io/py/eurlex.svg" alt="PyPI version" height="18"></a>
             <a href=https://github.com/ambv/black><img src="https://img.shields.io/badge/code%20style-black-000000.svg" height="18"></a>
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: eurlex Version: 0.1.3 Summary: An EUR-Lex parser
+Metadata-Version: 2.1 Name: eurlex Version: 0.1.4 Summary: An EUR-Lex parser
 for Python. Home-page: https://github.com/kevin91nl/eurlex Author: K.M.J.
-Jacobs Author-email: mail@kevinjacobs.nl License: UNKNOWN Description: # EUR-
-Lex Parser
+Jacobs Author-email: kmj.jacobs@maastrichtuniversity.nl License: UNKNOWN
+Description: # EUR-Lex Parser
 [Building] [PyPI_version] [https://img.shields.io/badge/code%20style-black-
 000000.svg]
 An EUR-Lex parser for Python. ## Usage You can install this package as follows:
 ```bash pip install -U eurlex ``` After installing this package, you can
 download and parse any document from EUR-Lex. For example, the [32019R0947
 regulation](https://eur-lex.europa.eu/legal-content/EN/TXT/
 ?uri=CELEX%3A32019R0947): ```python from eurlex import get_html_by_celex_id,
```

### Comparing `eurlex-0.1.3/setup.py` & `eurlex-0.1.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="eurlex",
-    version="0.1.3",
+    version="0.1.4",
     author="K.M.J. Jacobs",
-    author_email="mail@kevinjacobs.nl",
+    author_email="kmj.jacobs@maastrichtuniversity.nl",
     description="An EUR-Lex parser for Python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kevin91nl/eurlex",
     packages=setuptools.find_packages(),
     include_package_data=True,
     classifiers=[],
```

### Comparing `eurlex-0.1.3/tests/__init__.py` & `eurlex-0.1.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `eurlex-0.1.3/tests/test_parsing.py` & `eurlex-0.1.4/tests/test_parsing.py`

 * *Files identical despite different names*


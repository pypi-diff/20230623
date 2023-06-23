# Comparing `tmp/unpywall-0.2.tar.gz` & `tmp/unpywall-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unpywall-0.2.tar", last modified: Wed Dec 16 20:16:42 2020, max compression
+gzip compressed data, was "unpywall-0.2.1.tar", last modified: Fri Jun 23 09:19:23 2023, max compression
```

## Comparing `unpywall-0.2.tar` & `unpywall-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,26 @@
-drwxr-xr-x   0 naustica   (501) staff       (20)        0 2020-12-16 20:16:42.000000 unpywall-0.2/
--rw-r--r--   0 naustica   (501) staff       (20)     1092 2020-12-11 16:16:23.000000 unpywall-0.2/LICENSE.txt
--rw-r--r--   0 naustica   (501) staff       (20)       27 2020-12-11 16:16:23.000000 unpywall-0.2/MANIFEST.in
--rw-r--r--   0 naustica   (501) staff       (20)     8256 2020-12-16 20:16:42.000000 unpywall-0.2/PKG-INFO
--rw-r--r--   0 naustica   (501) staff       (20)     5939 2020-12-16 20:05:50.000000 unpywall-0.2/README.md
--rw-r--r--   0 naustica   (501) staff       (20)       38 2020-12-16 20:16:42.000000 unpywall-0.2/setup.cfg
--rw-r--r--   0 naustica   (501) staff       (20)     1583 2020-12-11 16:32:02.000000 unpywall-0.2/setup.py
-drwxr-xr-x   0 naustica   (501) staff       (20)        0 2020-12-16 20:16:42.000000 unpywall-0.2/unpywall/
--rw-r--r--   0 naustica   (501) staff       (20)    15286 2020-12-14 17:14:04.000000 unpywall-0.2/unpywall/__init__.py
--rw-r--r--   0 naustica   (501) staff       (20)     7720 2020-12-11 16:16:23.000000 unpywall-0.2/unpywall/__main__.py
--rw-r--r--   0 naustica   (501) staff       (20)     5777 2020-12-11 18:36:11.000000 unpywall-0.2/unpywall/cache.py
--rw-r--r--   0 naustica   (501) staff       (20)     3151 2020-12-14 17:20:14.000000 unpywall-0.2/unpywall/utils.py
-drwxr-xr-x   0 naustica   (501) staff       (20)        0 2020-12-16 20:16:42.000000 unpywall-0.2/unpywall.egg-info/
--rw-r--r--   0 naustica   (501) staff       (20)     8256 2020-12-16 20:16:42.000000 unpywall-0.2/unpywall.egg-info/PKG-INFO
--rw-r--r--   0 naustica   (501) staff       (20)      345 2020-12-16 20:16:42.000000 unpywall-0.2/unpywall.egg-info/SOURCES.txt
--rw-r--r--   0 naustica   (501) staff       (20)        1 2020-12-16 20:16:42.000000 unpywall-0.2/unpywall.egg-info/dependency_links.txt
--rw-r--r--   0 naustica   (501) staff       (20)       53 2020-12-16 20:16:42.000000 unpywall-0.2/unpywall.egg-info/entry_points.txt
--rw-r--r--   0 naustica   (501) staff       (20)        1 2020-12-16 20:16:42.000000 unpywall-0.2/unpywall.egg-info/not-zip-safe
--rw-r--r--   0 naustica   (501) staff       (20)       67 2020-12-16 20:16:42.000000 unpywall-0.2/unpywall.egg-info/requires.txt
--rw-r--r--   0 naustica   (501) staff       (20)        9 2020-12-16 20:16:42.000000 unpywall-0.2/unpywall.egg-info/top_level.txt
+drwxr-xr-x   0 naustica   (501) staff       (20)        0 2023-06-23 09:19:23.931768 unpywall-0.2.1/
+-rw-r--r--   0 naustica   (501) staff       (20)     1092 2023-06-23 08:32:38.000000 unpywall-0.2.1/LICENSE.txt
+-rw-r--r--   0 naustica   (501) staff       (20)       27 2023-06-23 08:24:23.000000 unpywall-0.2.1/MANIFEST.in
+-rw-r--r--   0 naustica   (501) staff       (20)     6827 2023-06-23 09:19:23.931637 unpywall-0.2.1/PKG-INFO
+-rw-r--r--   0 naustica   (501) staff       (20)     5953 2023-06-23 09:17:13.000000 unpywall-0.2.1/README.md
+-rw-r--r--   0 naustica   (501) staff       (20)       67 2023-06-23 09:07:16.000000 unpywall-0.2.1/requirements.txt
+-rw-r--r--   0 naustica   (501) staff       (20)       38 2023-06-23 09:19:23.931806 unpywall-0.2.1/setup.cfg
+-rw-r--r--   0 naustica   (501) staff       (20)     1590 2023-06-23 09:08:49.000000 unpywall-0.2.1/setup.py
+drwxr-xr-x   0 naustica   (501) staff       (20)        0 2023-06-23 09:19:23.929871 unpywall-0.2.1/tests/
+-rw-r--r--   0 naustica   (501) staff       (20)     3222 2023-06-23 08:24:23.000000 unpywall-0.2.1/tests/test_cache.py
+-rw-r--r--   0 naustica   (501) staff       (20)     1566 2023-06-23 08:24:23.000000 unpywall-0.2.1/tests/test_cli.py
+-rw-r--r--   0 naustica   (501) staff       (20)     5591 2023-06-23 08:24:23.000000 unpywall-0.2.1/tests/test_unpywall.py
+-rw-r--r--   0 naustica   (501) staff       (20)     1464 2023-06-23 08:24:23.000000 unpywall-0.2.1/tests/test_utils.py
+drwxr-xr-x   0 naustica   (501) staff       (20)        0 2023-06-23 09:19:23.930366 unpywall-0.2.1/unpywall/
+-rw-r--r--   0 naustica   (501) staff       (20)    15316 2023-06-23 09:12:54.000000 unpywall-0.2.1/unpywall/__init__.py
+-rw-r--r--   0 naustica   (501) staff       (20)     7720 2023-06-23 08:24:23.000000 unpywall-0.2.1/unpywall/__main__.py
+-rw-r--r--   0 naustica   (501) staff       (20)     5777 2023-06-23 08:24:23.000000 unpywall-0.2.1/unpywall/cache.py
+-rw-r--r--   0 naustica   (501) staff       (20)     3151 2023-06-23 08:24:23.000000 unpywall-0.2.1/unpywall/utils.py
+drwxr-xr-x   0 naustica   (501) staff       (20)        0 2023-06-23 09:19:23.931420 unpywall-0.2.1/unpywall.egg-info/
+-rw-r--r--   0 naustica   (501) staff       (20)     6827 2023-06-23 09:19:23.000000 unpywall-0.2.1/unpywall.egg-info/PKG-INFO
+-rw-r--r--   0 naustica   (501) staff       (20)      443 2023-06-23 09:19:23.000000 unpywall-0.2.1/unpywall.egg-info/SOURCES.txt
+-rw-r--r--   0 naustica   (501) staff       (20)        1 2023-06-23 09:19:23.000000 unpywall-0.2.1/unpywall.egg-info/dependency_links.txt
+-rw-r--r--   0 naustica   (501) staff       (20)       52 2023-06-23 09:19:23.000000 unpywall-0.2.1/unpywall.egg-info/entry_points.txt
+-rw-r--r--   0 naustica   (501) staff       (20)        1 2023-06-23 08:26:01.000000 unpywall-0.2.1/unpywall.egg-info/not-zip-safe
+-rw-r--r--   0 naustica   (501) staff       (20)       72 2023-06-23 09:19:23.000000 unpywall-0.2.1/unpywall.egg-info/requires.txt
+-rw-r--r--   0 naustica   (501) staff       (20)        9 2023-06-23 09:19:23.000000 unpywall-0.2.1/unpywall.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `unpywall-0.2/LICENSE.txt` & `unpywall-0.2.1/LICENSE.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
-Copyright (c) 2020 Nick Haupka
-Copyright (c) 2020 bganglia
+Copyright (c) 2023 Nick Haupka
+Copyright (c) 2023 bganglia
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 The above copyright notice and this permission notice shall be included in all
```

### Comparing `unpywall-0.2/PKG-INFO` & `unpywall-0.2.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,202 +1,202 @@
 Metadata-Version: 2.1
 Name: unpywall
-Version: 0.2
+Version: 0.2.1
 Summary: Interfacing the Unpaywall Database with Python
 Home-page: https://github.com/unpywall/unpywall
 Author: Nick Haupka, bganglia
 Author-email: nick.haupka@gmail.com, bganglia892@gmail.com
 License: MIT
 Project-URL: Documentation, https://unpywall.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/unpywall/unpywall
 Project-URL: Tracker, https://github.com/unpywall/unpywall/issues
-Description: # unpywall - Interfacing the Unpaywall API with Python
-        
-        [![Build Status](https://travis-ci.org/unpywall/unpywall.svg?branch=master)](https://travis-ci.org/github/unpywall/unpywall)
-        [![codecov.io](https://codecov.io/gh/unpywall/unpywall/branch/master/graph/badge.svg)](https://codecov.io/gh/unpywall/unpywall?branch=master)
-        [![PyPI - Downloads](https://img.shields.io/pypi/dm/unpywall)](https://pypi.org/project/unpywall/)
-        [![License](https://img.shields.io/github/license/unpywall/unpywall)](https://github.com/unpywall/unpywall/blob/master/LICENSE.txt)
-        [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4085415.svg)](https://doi.org/10.5281/zenodo.4085415)
-        [![PyPI - Version](https://img.shields.io/pypi/v/unpywall)](https://pypi.org/project/unpywall/)
-        [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/unpywall)](https://pypi.org/project/unpywall/)
-        [![Documentation Status](https://readthedocs.org/projects/unpywall/badge/?version=latest)](https://unpywall.readthedocs.io/en/latest/?badge=latest)
-        
-        ## Introduction
-        
-        unpywall is a Python client that utilizes the [Unpaywall REST API](https://unpaywall.org/products/api) for scholarly analysis with [pandas](https://pandas.pydata.org/). This package is influenced by [roadoi](https://github.com/ropensci/roadoi), a R client that interacts with the Unpaywall API.
-        
-        You can find more about the Unpaywall service here: https://unpaywall.org/.
-        
-        The documentation about the Unpaywall REST API is located here: https://unpaywall.org/products/api.
-        
-        
-        ## Install
-        
-        Install from [pypi](https://pypi.org/project/unpywall/) using pip:
-        ```bash
-        pip install unpywall
-        ```
-        
-        ## Use
-        
-        ### Authentication
-        
-        An authentification is required to use the Unpaywall Service. For that, unpywall offers two options for authorizing the client. You can either import `UnpywallCredentials` which generates an environment variable or you can set the environment variable by yourself. Both methods require an email.
-        
-        ```python
-        from unpywall.utils import UnpywallCredentials
-        
-        UnpywallCredentials('nick.haupka@gmail.com')
-        ```
-        
-        Notice that the environment variable for authentication needs to be called `UNPAYWALL_EMAIL`.
-        
-        ```bash
-        export UNPAYWALL_EMAIL=nick.haupka@gmail.com
-        ```
-        
-        ### Query Unpaywall by DOI
-        
-        If you want to search articles by a given DOI use the method `doi`. The result is a [pandas DataFrame](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html).
-        
-        ```python
-        from unpywall import Unpywall
-        
-        Unpywall.doi(dois=['10.1038/nature12373', '10.1093/nar/gkr1047'])
-        
-        #   data_standard  ... best_oa_location.version
-        #0              2  ...         publishedVersion
-        #1              2  ...         publishedVersion
-        
-        #[2 rows x 32 columns]
-        ```
-        
-        You can track the progress of your API call by setting the parameter `progress` to True. This is especially useful for estimating the time required.
-        
-        ```python
-        Unpywall.doi(dois=['10.1038/nature12373', '10.1093/nar/gkr1047'],
-                     progress=True)
-        
-        #|=========================                        | 50%
-        ```
-        
-        This method also allows two options for catching errors (`raise` and `ignore`)
-        
-        ```python
-        Unpywall.doi(dois=['10.1038/nature12373', '10.1093/nar/gkr1047'],
-                     errors='ignore')
-        ```
-        
-        ### Query Unpaywall by text search
-        
-        If you want to search articles by a given term use the method `query`. The result is a [pandas DataFrame](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html)
-        
-        ```python
-        Unpywall.query(query='sea lion',
-                       is_oa=True)
-        #   data_standard  ... first_oa_location.version
-        #0              2  ...          publishedVersion
-        #1              2  ...          publishedVersion
-        #2              2  ...          publishedVersion
-        ```
-        
-        ### Conveniently obtain full text
-        
-        If you are using Unpaywall to obtain full-text copies of papers for literature mining, you may benefit from the following functions:
-        
-        You can use the `download_pdf_handle` method to return a PDF handle for the given DOI.
-        
-        ```python
-        Unpywall.download_pdf_handle(doi='10.1038/nature12373')
-        
-        #<http.client.HTTPResponse object at 0x7fd08ef677c0>
-        ```
-        
-        To return an URL to a PDF for the given DOI, use `get_pdf_link`.
-        
-        ```python
-        Unpywall.get_pdf_link(doi='10.1038/nature12373')
-        
-        #'https://dash.harvard.edu/bitstream/1/12285462/1/Nanometer-Scale%20Thermometry.pdf'
-        ```
-        
-        To return an URL to the best available OA copy, regardless of the format, use `get_doc_link`.
-        
-        ```python
-        Unpywall.get_doc_link(doi='10.1016/j.envint.2020.105730')
-        
-        #'https://doi.org/10.1016/j.envint.2020.105730'
-        ```
-        To return a list of all URLS to OA copies, use `get_all_links`.
-        
-        ```python
-        Unpywall.get_all_links(doi='10.1038/nature12373')
-        
-        #['https://dash.harvard.edu/bitstream/1/12285462/1/Nanometer-Scale%20Thermometry.pdf']
-        ```
-        
-        You can also directly access all data provided by unpaywall in json format using `get_json`.
-        
-        ```python
-        Unpywall.get_json(doi='10.1038/nature12373')
-        
-        #{'best_oa_location': {'endpoint_id': '8c9d8ba370a84253deb', 'evidence': 'oa repository (via OAI-PMH doi match)', 'host_type': ...
-        ```
-        
-        ## Command-Line-Interface
-        
-        unpywall comes with a command-line-interface that can be used to quickly look up a PDF or to download free full-text articles to your device.
-        
-        ### Obtain a PDF URL
-        
-        Retrieve the URL of a PDF for a given DOI with the following command.
-        
-        ```bash
-        unpywall link 10.1038/nature12373
-        ```
-        
-        ### View a PDF
-        
-        If you want to view a PDF in your Browser or on your system use `view`.
-        
-        ```bash
-        unpywall view 10.1038/nature12373 -m browser
-        ```
-        
-        ### PDF Download
-        
-        Use `download` if you want to store a PDF on your machine.
-        
-        ```bash
-        unpywall download 10.1038/nature12373 -f article.pdf -p ./documents
-        ```
-        
-        ### Help
-        
-        You can always use `help` to open a description for the provided functions.
-        
-        ```bash
-        unpywall -h
-        ```
-        
-        ## Documentation
-        
-        Full documentation is available at https://unpywall.readthedocs.io/.
-        
-        ## Develop
-        
-        To install unpywall, along with dev tools, run:
-        
-        ```bash
-        pip install -e '.[dev]'
-        ```
-        
 Keywords: Unpaywall,Open Access,full text
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE.txt
+
+# unpywall - Interfacing the Unpaywall API with Python
+
+[![Build Status](https://circleci.com/gh/unpywall/unpywall.svg?style=shield)](https://app.circleci.com/pipelines/github/unpywall/unpywall)
+[![codecov.io](https://codecov.io/gh/unpywall/unpywall/branch/master/graph/badge.svg)](https://codecov.io/gh/unpywall/unpywall?branch=master)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/unpywall)](https://pypi.org/project/unpywall/)
+[![License](https://img.shields.io/github/license/unpywall/unpywall)](https://github.com/unpywall/unpywall/blob/master/LICENSE.txt)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4085414.svg)](https://doi.org/10.5281/zenodo.4085414)
+[![PyPI - Version](https://img.shields.io/pypi/v/unpywall)](https://pypi.org/project/unpywall/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/unpywall)](https://pypi.org/project/unpywall/)
+[![Documentation Status](https://readthedocs.org/projects/unpywall/badge/?version=latest)](https://unpywall.readthedocs.io/en/latest/?badge=latest)
+
+## Introduction
+
+unpywall is a Python client that utilizes the [Unpaywall REST API](https://unpaywall.org/products/api) for scholarly analysis with [pandas](https://pandas.pydata.org/). This package is influenced by [roadoi](https://github.com/ropensci/roadoi), a R client that interacts with the Unpaywall API.
+
+You can find more about the Unpaywall service here: https://unpaywall.org/.
+
+The documentation about the Unpaywall REST API is located here: https://unpaywall.org/products/api.
+
+
+## Install
+
+Install from [pypi](https://pypi.org/project/unpywall/) using pip:
+```bash
+pip install unpywall
+```
+
+## Use
+
+### Authentication
+
+An authentification is required to use the Unpaywall Service. For that, unpywall offers two options for authorizing the client. You can either import `UnpywallCredentials` which generates an environment variable or you can set the environment variable by yourself. Both methods require an email.
+
+```python
+from unpywall.utils import UnpywallCredentials
+
+UnpywallCredentials('nick.haupka@gmail.com')
+```
+
+Notice that the environment variable for authentication needs to be called `UNPAYWALL_EMAIL`.
+
+```bash
+export UNPAYWALL_EMAIL=nick.haupka@gmail.com
+```
+
+### Query Unpaywall by DOI
+
+If you want to search articles by a given DOI use the method `doi`. The result is a [pandas DataFrame](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html).
+
+```python
+from unpywall import Unpywall
+
+Unpywall.doi(dois=['10.1038/nature12373', '10.1093/nar/gkr1047'])
+
+#   data_standard  ... best_oa_location.version
+#0              2  ...         publishedVersion
+#1              2  ...         publishedVersion
+
+#[2 rows x 32 columns]
+```
+
+You can track the progress of your API call by setting the parameter `progress` to True. This is especially useful for estimating the time required.
+
+```python
+Unpywall.doi(dois=['10.1038/nature12373', '10.1093/nar/gkr1047'],
+             progress=True)
+
+#|=========================                        | 50%
+```
+
+This method also allows two options for catching errors (`raise` and `ignore`)
+
+```python
+Unpywall.doi(dois=['10.1038/nature12373', '10.1093/nar/gkr1047'],
+             errors='ignore')
+```
+
+### Query Unpaywall by text search
+
+If you want to search articles by a given term use the method `query`. The result is a [pandas DataFrame](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html)
+
+```python
+Unpywall.query(query='sea lion',
+               is_oa=True)
+#   data_standard  ... first_oa_location.version
+#0              2  ...          publishedVersion
+#1              2  ...          publishedVersion
+#2              2  ...          publishedVersion
+```
+
+### Conveniently obtain full text
+
+If you are using Unpaywall to obtain full-text copies of papers for literature mining, you may benefit from the following functions:
+
+You can use the `download_pdf_handle` method to return a PDF handle for the given DOI.
+
+```python
+Unpywall.download_pdf_handle(doi='10.1038/nature12373')
+
+#<http.client.HTTPResponse object at 0x7fd08ef677c0>
+```
+
+To return an URL to a PDF for the given DOI, use `get_pdf_link`.
+
+```python
+Unpywall.get_pdf_link(doi='10.1038/nature12373')
+
+#'https://dash.harvard.edu/bitstream/1/12285462/1/Nanometer-Scale%20Thermometry.pdf'
+```
+
+To return an URL to the best available OA copy, regardless of the format, use `get_doc_link`.
+
+```python
+Unpywall.get_doc_link(doi='10.1016/j.envint.2020.105730')
+
+#'https://doi.org/10.1016/j.envint.2020.105730'
+```
+To return a list of all URLS to OA copies, use `get_all_links`.
+
+```python
+Unpywall.get_all_links(doi='10.1038/nature12373')
+
+#['https://dash.harvard.edu/bitstream/1/12285462/1/Nanometer-Scale%20Thermometry.pdf']
+```
+
+You can also directly access all data provided by unpaywall in json format using `get_json`.
+
+```python
+Unpywall.get_json(doi='10.1038/nature12373')
+
+#{'best_oa_location': {'endpoint_id': '8c9d8ba370a84253deb', 'evidence': 'oa repository (via OAI-PMH doi match)', 'host_type': ...
+```
+
+## Command-Line-Interface
+
+unpywall comes with a command-line-interface that can be used to quickly look up a PDF or to download free full-text articles to your device.
+
+### Obtain a PDF URL
+
+Retrieve the URL of a PDF for a given DOI with the following command.
+
+```bash
+unpywall link 10.1038/nature12373
+```
+
+### View a PDF
+
+If you want to view a PDF in your Browser or on your system use `view`.
+
+```bash
+unpywall view 10.1038/nature12373 -m browser
+```
+
+### PDF Download
+
+Use `download` if you want to store a PDF on your machine.
+
+```bash
+unpywall download 10.1038/nature12373 -f article.pdf -p ./documents
+```
+
+### Help
+
+You can always use `help` to open a description for the provided functions.
+
+```bash
+unpywall -h
+```
+
+## Documentation
+
+Full documentation is available at https://unpywall.readthedocs.io/.
+
+## Develop
+
+To install unpywall, along with dev tools, run:
+
+```bash
+pip install -e '.[dev]'
+```
```

### Comparing `unpywall-0.2/README.md` & `unpywall-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # unpywall - Interfacing the Unpaywall API with Python
 
-[![Build Status](https://travis-ci.org/unpywall/unpywall.svg?branch=master)](https://travis-ci.org/github/unpywall/unpywall)
+[![Build Status](https://circleci.com/gh/unpywall/unpywall.svg?style=shield)](https://app.circleci.com/pipelines/github/unpywall/unpywall)
 [![codecov.io](https://codecov.io/gh/unpywall/unpywall/branch/master/graph/badge.svg)](https://codecov.io/gh/unpywall/unpywall?branch=master)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/unpywall)](https://pypi.org/project/unpywall/)
 [![License](https://img.shields.io/github/license/unpywall/unpywall)](https://github.com/unpywall/unpywall/blob/master/LICENSE.txt)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4085415.svg)](https://doi.org/10.5281/zenodo.4085415)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4085414.svg)](https://doi.org/10.5281/zenodo.4085414)
 [![PyPI - Version](https://img.shields.io/pypi/v/unpywall)](https://pypi.org/project/unpywall/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/unpywall)](https://pypi.org/project/unpywall/)
 [![Documentation Status](https://readthedocs.org/projects/unpywall/badge/?version=latest)](https://unpywall.readthedocs.io/en/latest/?badge=latest)
 
 ## Introduction
 
 unpywall is a Python client that utilizes the [Unpaywall REST API](https://unpaywall.org/products/api) for scholarly analysis with [pandas](https://pandas.pydata.org/). This package is influenced by [roadoi](https://github.com/ropensci/roadoi), a R client that interacts with the Unpaywall API.
```

### Comparing `unpywall-0.2/setup.py` & `unpywall-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 dir = path.abspath(path.dirname(__file__))
 with open(path.join(dir, 'README.md'), encoding='utf-8') as file:
     long_description = file.read()
 
 
 setup(name='unpywall',
-      version='0.2',
+      version='0.2.1',
       description='Interfacing the Unpaywall Database with Python',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/unpywall/unpywall',
       author='Nick Haupka, bganglia',
       author_email='nick.haupka@gmail.com, bganglia892@gmail.com',
       license='MIT',
@@ -19,15 +19,15 @@
       keywords=['Unpaywall', 'Open Access', 'full text'],
       project_urls={
         'Documentation': 'https://unpywall.readthedocs.io/en/latest/',
         'Source': 'https://github.com/unpywall/unpywall',
         'Tracker': 'https://github.com/unpywall/unpywall/issues'
       },
       install_requires=[
-        'pandas',
+        'pandas>=2.0',
         'requests'
       ],
       extras_require={
        'dev': [
            'pytest',
            'coverage',
            'pytest-cov',
@@ -40,12 +40,12 @@
             'unpywall = unpywall.__main__:main'
         ]
       },
       classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7'
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9'
       ],
       zip_safe=False)
```

### Comparing `unpywall-0.2/unpywall/__init__.py` & `unpywall-0.2.1/unpywall/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,15 +204,15 @@
 
         df = pd.DataFrame()
 
         for obj in data['results']:
             df2 = Unpywall._get_df(data=obj['response'],
                                    format=format,
                                    errors=errors)
-            df = df.append(df2, ignore_index=True)
+            df = pd.concat([df, df2], ignore_index=True)
 
         if df.empty:
             return None
 
         return df
 
     @staticmethod
@@ -266,15 +266,15 @@
             # check if json is not empty or None due to an faulty DOI
             if not bool(data):
                 continue
 
             df2 = Unpywall._get_df(data=data,
                                    format=format,
                                    errors=errors)
-            df = df.append(df2, ignore_index=True)
+            df = pd.concat([df, df2], ignore_index=True)
 
         if df.empty:
             return None
 
         return df
 
     @staticmethod
@@ -500,11 +500,11 @@
 
         if not os.path.exists(filepath):
             os.makedirs(filepath)
 
         with open(path, 'wb') as file:
             chunk_size = 0
             for chunk in r.iter_content(block_size):
-                if progress:
+                if progress and file_size > 0:
                     chunk_size += len(chunk)
                     Unpywall._progress(chunk_size / file_size)
                 file.write(chunk)
```

### Comparing `unpywall-0.2/unpywall/__main__.py` & `unpywall-0.2.1/unpywall/__main__.py`

 * *Files identical despite different names*

### Comparing `unpywall-0.2/unpywall/cache.py` & `unpywall-0.2.1/unpywall/cache.py`

 * *Files identical despite different names*

### Comparing `unpywall-0.2/unpywall/utils.py` & `unpywall-0.2.1/unpywall/utils.py`

 * *Files identical despite different names*

### Comparing `unpywall-0.2/unpywall.egg-info/PKG-INFO` & `unpywall-0.2.1/unpywall.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,202 +1,202 @@
 Metadata-Version: 2.1
 Name: unpywall
-Version: 0.2
+Version: 0.2.1
 Summary: Interfacing the Unpaywall Database with Python
 Home-page: https://github.com/unpywall/unpywall
 Author: Nick Haupka, bganglia
 Author-email: nick.haupka@gmail.com, bganglia892@gmail.com
 License: MIT
 Project-URL: Documentation, https://unpywall.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/unpywall/unpywall
 Project-URL: Tracker, https://github.com/unpywall/unpywall/issues
-Description: # unpywall - Interfacing the Unpaywall API with Python
-        
-        [![Build Status](https://travis-ci.org/unpywall/unpywall.svg?branch=master)](https://travis-ci.org/github/unpywall/unpywall)
-        [![codecov.io](https://codecov.io/gh/unpywall/unpywall/branch/master/graph/badge.svg)](https://codecov.io/gh/unpywall/unpywall?branch=master)
-        [![PyPI - Downloads](https://img.shields.io/pypi/dm/unpywall)](https://pypi.org/project/unpywall/)
-        [![License](https://img.shields.io/github/license/unpywall/unpywall)](https://github.com/unpywall/unpywall/blob/master/LICENSE.txt)
-        [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4085415.svg)](https://doi.org/10.5281/zenodo.4085415)
-        [![PyPI - Version](https://img.shields.io/pypi/v/unpywall)](https://pypi.org/project/unpywall/)
-        [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/unpywall)](https://pypi.org/project/unpywall/)
-        [![Documentation Status](https://readthedocs.org/projects/unpywall/badge/?version=latest)](https://unpywall.readthedocs.io/en/latest/?badge=latest)
-        
-        ## Introduction
-        
-        unpywall is a Python client that utilizes the [Unpaywall REST API](https://unpaywall.org/products/api) for scholarly analysis with [pandas](https://pandas.pydata.org/). This package is influenced by [roadoi](https://github.com/ropensci/roadoi), a R client that interacts with the Unpaywall API.
-        
-        You can find more about the Unpaywall service here: https://unpaywall.org/.
-        
-        The documentation about the Unpaywall REST API is located here: https://unpaywall.org/products/api.
-        
-        
-        ## Install
-        
-        Install from [pypi](https://pypi.org/project/unpywall/) using pip:
-        ```bash
-        pip install unpywall
-        ```
-        
-        ## Use
-        
-        ### Authentication
-        
-        An authentification is required to use the Unpaywall Service. For that, unpywall offers two options for authorizing the client. You can either import `UnpywallCredentials` which generates an environment variable or you can set the environment variable by yourself. Both methods require an email.
-        
-        ```python
-        from unpywall.utils import UnpywallCredentials
-        
-        UnpywallCredentials('nick.haupka@gmail.com')
-        ```
-        
-        Notice that the environment variable for authentication needs to be called `UNPAYWALL_EMAIL`.
-        
-        ```bash
-        export UNPAYWALL_EMAIL=nick.haupka@gmail.com
-        ```
-        
-        ### Query Unpaywall by DOI
-        
-        If you want to search articles by a given DOI use the method `doi`. The result is a [pandas DataFrame](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html).
-        
-        ```python
-        from unpywall import Unpywall
-        
-        Unpywall.doi(dois=['10.1038/nature12373', '10.1093/nar/gkr1047'])
-        
-        #   data_standard  ... best_oa_location.version
-        #0              2  ...         publishedVersion
-        #1              2  ...         publishedVersion
-        
-        #[2 rows x 32 columns]
-        ```
-        
-        You can track the progress of your API call by setting the parameter `progress` to True. This is especially useful for estimating the time required.
-        
-        ```python
-        Unpywall.doi(dois=['10.1038/nature12373', '10.1093/nar/gkr1047'],
-                     progress=True)
-        
-        #|=========================                        | 50%
-        ```
-        
-        This method also allows two options for catching errors (`raise` and `ignore`)
-        
-        ```python
-        Unpywall.doi(dois=['10.1038/nature12373', '10.1093/nar/gkr1047'],
-                     errors='ignore')
-        ```
-        
-        ### Query Unpaywall by text search
-        
-        If you want to search articles by a given term use the method `query`. The result is a [pandas DataFrame](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html)
-        
-        ```python
-        Unpywall.query(query='sea lion',
-                       is_oa=True)
-        #   data_standard  ... first_oa_location.version
-        #0              2  ...          publishedVersion
-        #1              2  ...          publishedVersion
-        #2              2  ...          publishedVersion
-        ```
-        
-        ### Conveniently obtain full text
-        
-        If you are using Unpaywall to obtain full-text copies of papers for literature mining, you may benefit from the following functions:
-        
-        You can use the `download_pdf_handle` method to return a PDF handle for the given DOI.
-        
-        ```python
-        Unpywall.download_pdf_handle(doi='10.1038/nature12373')
-        
-        #<http.client.HTTPResponse object at 0x7fd08ef677c0>
-        ```
-        
-        To return an URL to a PDF for the given DOI, use `get_pdf_link`.
-        
-        ```python
-        Unpywall.get_pdf_link(doi='10.1038/nature12373')
-        
-        #'https://dash.harvard.edu/bitstream/1/12285462/1/Nanometer-Scale%20Thermometry.pdf'
-        ```
-        
-        To return an URL to the best available OA copy, regardless of the format, use `get_doc_link`.
-        
-        ```python
-        Unpywall.get_doc_link(doi='10.1016/j.envint.2020.105730')
-        
-        #'https://doi.org/10.1016/j.envint.2020.105730'
-        ```
-        To return a list of all URLS to OA copies, use `get_all_links`.
-        
-        ```python
-        Unpywall.get_all_links(doi='10.1038/nature12373')
-        
-        #['https://dash.harvard.edu/bitstream/1/12285462/1/Nanometer-Scale%20Thermometry.pdf']
-        ```
-        
-        You can also directly access all data provided by unpaywall in json format using `get_json`.
-        
-        ```python
-        Unpywall.get_json(doi='10.1038/nature12373')
-        
-        #{'best_oa_location': {'endpoint_id': '8c9d8ba370a84253deb', 'evidence': 'oa repository (via OAI-PMH doi match)', 'host_type': ...
-        ```
-        
-        ## Command-Line-Interface
-        
-        unpywall comes with a command-line-interface that can be used to quickly look up a PDF or to download free full-text articles to your device.
-        
-        ### Obtain a PDF URL
-        
-        Retrieve the URL of a PDF for a given DOI with the following command.
-        
-        ```bash
-        unpywall link 10.1038/nature12373
-        ```
-        
-        ### View a PDF
-        
-        If you want to view a PDF in your Browser or on your system use `view`.
-        
-        ```bash
-        unpywall view 10.1038/nature12373 -m browser
-        ```
-        
-        ### PDF Download
-        
-        Use `download` if you want to store a PDF on your machine.
-        
-        ```bash
-        unpywall download 10.1038/nature12373 -f article.pdf -p ./documents
-        ```
-        
-        ### Help
-        
-        You can always use `help` to open a description for the provided functions.
-        
-        ```bash
-        unpywall -h
-        ```
-        
-        ## Documentation
-        
-        Full documentation is available at https://unpywall.readthedocs.io/.
-        
-        ## Develop
-        
-        To install unpywall, along with dev tools, run:
-        
-        ```bash
-        pip install -e '.[dev]'
-        ```
-        
 Keywords: Unpaywall,Open Access,full text
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE.txt
+
+# unpywall - Interfacing the Unpaywall API with Python
+
+[![Build Status](https://circleci.com/gh/unpywall/unpywall.svg?style=shield)](https://app.circleci.com/pipelines/github/unpywall/unpywall)
+[![codecov.io](https://codecov.io/gh/unpywall/unpywall/branch/master/graph/badge.svg)](https://codecov.io/gh/unpywall/unpywall?branch=master)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/unpywall)](https://pypi.org/project/unpywall/)
+[![License](https://img.shields.io/github/license/unpywall/unpywall)](https://github.com/unpywall/unpywall/blob/master/LICENSE.txt)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4085414.svg)](https://doi.org/10.5281/zenodo.4085414)
+[![PyPI - Version](https://img.shields.io/pypi/v/unpywall)](https://pypi.org/project/unpywall/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/unpywall)](https://pypi.org/project/unpywall/)
+[![Documentation Status](https://readthedocs.org/projects/unpywall/badge/?version=latest)](https://unpywall.readthedocs.io/en/latest/?badge=latest)
+
+## Introduction
+
+unpywall is a Python client that utilizes the [Unpaywall REST API](https://unpaywall.org/products/api) for scholarly analysis with [pandas](https://pandas.pydata.org/). This package is influenced by [roadoi](https://github.com/ropensci/roadoi), a R client that interacts with the Unpaywall API.
+
+You can find more about the Unpaywall service here: https://unpaywall.org/.
+
+The documentation about the Unpaywall REST API is located here: https://unpaywall.org/products/api.
+
+
+## Install
+
+Install from [pypi](https://pypi.org/project/unpywall/) using pip:
+```bash
+pip install unpywall
+```
+
+## Use
+
+### Authentication
+
+An authentification is required to use the Unpaywall Service. For that, unpywall offers two options for authorizing the client. You can either import `UnpywallCredentials` which generates an environment variable or you can set the environment variable by yourself. Both methods require an email.
+
+```python
+from unpywall.utils import UnpywallCredentials
+
+UnpywallCredentials('nick.haupka@gmail.com')
+```
+
+Notice that the environment variable for authentication needs to be called `UNPAYWALL_EMAIL`.
+
+```bash
+export UNPAYWALL_EMAIL=nick.haupka@gmail.com
+```
+
+### Query Unpaywall by DOI
+
+If you want to search articles by a given DOI use the method `doi`. The result is a [pandas DataFrame](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html).
+
+```python
+from unpywall import Unpywall
+
+Unpywall.doi(dois=['10.1038/nature12373', '10.1093/nar/gkr1047'])
+
+#   data_standard  ... best_oa_location.version
+#0              2  ...         publishedVersion
+#1              2  ...         publishedVersion
+
+#[2 rows x 32 columns]
+```
+
+You can track the progress of your API call by setting the parameter `progress` to True. This is especially useful for estimating the time required.
+
+```python
+Unpywall.doi(dois=['10.1038/nature12373', '10.1093/nar/gkr1047'],
+             progress=True)
+
+#|=========================                        | 50%
+```
+
+This method also allows two options for catching errors (`raise` and `ignore`)
+
+```python
+Unpywall.doi(dois=['10.1038/nature12373', '10.1093/nar/gkr1047'],
+             errors='ignore')
+```
+
+### Query Unpaywall by text search
+
+If you want to search articles by a given term use the method `query`. The result is a [pandas DataFrame](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html)
+
+```python
+Unpywall.query(query='sea lion',
+               is_oa=True)
+#   data_standard  ... first_oa_location.version
+#0              2  ...          publishedVersion
+#1              2  ...          publishedVersion
+#2              2  ...          publishedVersion
+```
+
+### Conveniently obtain full text
+
+If you are using Unpaywall to obtain full-text copies of papers for literature mining, you may benefit from the following functions:
+
+You can use the `download_pdf_handle` method to return a PDF handle for the given DOI.
+
+```python
+Unpywall.download_pdf_handle(doi='10.1038/nature12373')
+
+#<http.client.HTTPResponse object at 0x7fd08ef677c0>
+```
+
+To return an URL to a PDF for the given DOI, use `get_pdf_link`.
+
+```python
+Unpywall.get_pdf_link(doi='10.1038/nature12373')
+
+#'https://dash.harvard.edu/bitstream/1/12285462/1/Nanometer-Scale%20Thermometry.pdf'
+```
+
+To return an URL to the best available OA copy, regardless of the format, use `get_doc_link`.
+
+```python
+Unpywall.get_doc_link(doi='10.1016/j.envint.2020.105730')
+
+#'https://doi.org/10.1016/j.envint.2020.105730'
+```
+To return a list of all URLS to OA copies, use `get_all_links`.
+
+```python
+Unpywall.get_all_links(doi='10.1038/nature12373')
+
+#['https://dash.harvard.edu/bitstream/1/12285462/1/Nanometer-Scale%20Thermometry.pdf']
+```
+
+You can also directly access all data provided by unpaywall in json format using `get_json`.
+
+```python
+Unpywall.get_json(doi='10.1038/nature12373')
+
+#{'best_oa_location': {'endpoint_id': '8c9d8ba370a84253deb', 'evidence': 'oa repository (via OAI-PMH doi match)', 'host_type': ...
+```
+
+## Command-Line-Interface
+
+unpywall comes with a command-line-interface that can be used to quickly look up a PDF or to download free full-text articles to your device.
+
+### Obtain a PDF URL
+
+Retrieve the URL of a PDF for a given DOI with the following command.
+
+```bash
+unpywall link 10.1038/nature12373
+```
+
+### View a PDF
+
+If you want to view a PDF in your Browser or on your system use `view`.
+
+```bash
+unpywall view 10.1038/nature12373 -m browser
+```
+
+### PDF Download
+
+Use `download` if you want to store a PDF on your machine.
+
+```bash
+unpywall download 10.1038/nature12373 -f article.pdf -p ./documents
+```
+
+### Help
+
+You can always use `help` to open a description for the provided functions.
+
+```bash
+unpywall -h
+```
+
+## Documentation
+
+Full documentation is available at https://unpywall.readthedocs.io/.
+
+## Develop
+
+To install unpywall, along with dev tools, run:
+
+```bash
+pip install -e '.[dev]'
+```
```


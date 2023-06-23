# Comparing `tmp/zenodoclient-0.5.0.tar.gz` & `tmp/zenodoclient-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zenodoclient-0.5.0.tar", last modified: Tue Dec  6 09:08:35 2022, max compression
+gzip compressed data, was "zenodoclient-0.5.1.tar", last modified: Fri Jun 23 14:33:36 2023, max compression
```

## Comparing `zenodoclient-0.5.0.tar` & `zenodoclient-0.5.1.tar`

### file list

```diff
@@ -1,29 +1,35 @@
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-12-06 09:08:35.699617 zenodoclient-0.5.0/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    11357 2021-03-01 08:52:43.000000 zenodoclient-0.5.0/LICENSE
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       35 2021-03-01 08:52:43.000000 zenodoclient-0.5.0/MANIFEST.in
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     3479 2022-12-06 09:08:35.699617 zenodoclient-0.5.0/PKG-INFO
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1784 2022-12-06 08:44:21.000000 zenodoclient-0.5.0/README.md
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       81 2022-12-06 08:39:17.000000 zenodoclient-0.5.0/pyproject.toml
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1993 2022-12-06 09:08:35.703617 zenodoclient-0.5.0/setup.cfg
--rwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)       39 2022-12-06 08:49:10.000000 zenodoclient-0.5.0/setup.py
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-12-06 09:08:35.699617 zenodoclient-0.5.0/src/
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-12-06 09:08:35.699617 zenodoclient-0.5.0/src/zenodoclient/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       61 2022-12-06 09:07:54.000000 zenodoclient-0.5.0/src/zenodoclient/__init__.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1355 2021-03-01 08:52:43.000000 zenodoclient-0.5.0/src/zenodoclient/__main__.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     9867 2022-12-06 08:56:22.000000 zenodoclient-0.5.0/src/zenodoclient/api.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      711 2021-03-01 08:52:43.000000 zenodoclient-0.5.0/src/zenodoclient/catalog.py
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-12-06 09:08:35.699617 zenodoclient-0.5.0/src/zenodoclient/commands/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        0 2021-03-01 08:52:43.000000 zenodoclient-0.5.0/src/zenodoclient/commands/__init__.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      243 2021-03-01 08:52:43.000000 zenodoclient-0.5.0/src/zenodoclient/commands/refresh.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      773 2021-03-01 08:52:43.000000 zenodoclient-0.5.0/src/zenodoclient/commands/update.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     1384 2021-03-01 08:52:43.000000 zenodoclient-0.5.0/src/zenodoclient/commands/updatepeople.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)    10796 2022-12-06 08:56:22.000000 zenodoclient-0.5.0/src/zenodoclient/models.py
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     3617 2021-03-25 08:50:08.000000 zenodoclient-0.5.0/src/zenodoclient/oai.py
-drwxrwxr-x   0 robert_forkel  (1001) robert_forkel  (1001)        0 2022-12-06 09:08:35.699617 zenodoclient-0.5.0/src/zenodoclient.egg-info/
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)     3479 2022-12-06 09:08:35.000000 zenodoclient-0.5.0/src/zenodoclient.egg-info/PKG-INFO
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      658 2022-12-06 09:08:35.000000 zenodoclient-0.5.0/src/zenodoclient.egg-info/SOURCES.txt
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        1 2022-12-06 09:08:35.000000 zenodoclient-0.5.0/src/zenodoclient.egg-info/dependency_links.txt
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       55 2022-12-06 09:08:35.000000 zenodoclient-0.5.0/src/zenodoclient.egg-info/entry_points.txt
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)        1 2021-03-24 08:41:40.000000 zenodoclient-0.5.0/src/zenodoclient.egg-info/not-zip-safe
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)      139 2022-12-06 09:08:35.000000 zenodoclient-0.5.0/src/zenodoclient.egg-info/requires.txt
--rw-rw-r--   0 robert_forkel  (1001) robert_forkel  (1001)       13 2022-12-06 09:08:35.000000 zenodoclient-0.5.0/src/zenodoclient.egg-info/top_level.txt
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-06-23 14:33:36.217774 zenodoclient-0.5.1/
+-rw-rw-r--   0 robert    (1000) robert    (1000)    11357 2022-12-22 15:23:21.000000 zenodoclient-0.5.1/LICENSE
+-rw-rw-r--   0 robert    (1000) robert    (1000)       35 2022-12-22 15:23:21.000000 zenodoclient-0.5.1/MANIFEST.in
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2969 2023-06-23 14:33:36.217774 zenodoclient-0.5.1/PKG-INFO
+-rw-rw-r--   0 robert    (1000) robert    (1000)     1784 2022-12-22 15:23:21.000000 zenodoclient-0.5.1/README.md
+-rw-rw-r--   0 robert    (1000) robert    (1000)       81 2022-12-22 15:23:21.000000 zenodoclient-0.5.1/pyproject.toml
+-rw-rw-r--   0 robert    (1000) robert    (1000)     1993 2023-06-23 14:33:36.217774 zenodoclient-0.5.1/setup.cfg
+-rwxrwxr-x   0 robert    (1000) robert    (1000)       39 2022-12-22 15:23:21.000000 zenodoclient-0.5.1/setup.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-06-23 14:33:36.217774 zenodoclient-0.5.1/src/
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-06-23 14:33:36.217774 zenodoclient-0.5.1/src/zenodoclient/
+-rw-rw-r--   0 robert    (1000) robert    (1000)       61 2023-06-23 14:32:31.000000 zenodoclient-0.5.1/src/zenodoclient/__init__.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     1355 2022-12-22 15:23:21.000000 zenodoclient-0.5.1/src/zenodoclient/__main__.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     9993 2023-06-23 14:20:35.000000 zenodoclient-0.5.1/src/zenodoclient/api.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      711 2022-12-22 15:23:21.000000 zenodoclient-0.5.1/src/zenodoclient/catalog.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-06-23 14:33:36.217774 zenodoclient-0.5.1/src/zenodoclient/commands/
+-rw-rw-r--   0 robert    (1000) robert    (1000)        0 2022-12-22 15:23:21.000000 zenodoclient-0.5.1/src/zenodoclient/commands/__init__.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      243 2022-12-22 15:23:21.000000 zenodoclient-0.5.1/src/zenodoclient/commands/refresh.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      773 2022-12-22 15:23:21.000000 zenodoclient-0.5.1/src/zenodoclient/commands/update.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     1384 2022-12-22 15:23:21.000000 zenodoclient-0.5.1/src/zenodoclient/commands/updatepeople.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)    10802 2023-06-23 14:25:46.000000 zenodoclient-0.5.1/src/zenodoclient/models.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     3617 2022-12-22 15:23:21.000000 zenodoclient-0.5.1/src/zenodoclient/oai.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-06-23 14:33:36.217774 zenodoclient-0.5.1/src/zenodoclient.egg-info/
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2969 2023-06-23 14:33:36.000000 zenodoclient-0.5.1/src/zenodoclient.egg-info/PKG-INFO
+-rw-rw-r--   0 robert    (1000) robert    (1000)      763 2023-06-23 14:33:36.000000 zenodoclient-0.5.1/src/zenodoclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)        1 2023-06-23 14:33:36.000000 zenodoclient-0.5.1/src/zenodoclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)       54 2023-06-23 14:33:36.000000 zenodoclient-0.5.1/src/zenodoclient.egg-info/entry_points.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)        1 2022-12-22 15:23:21.000000 zenodoclient-0.5.1/src/zenodoclient.egg-info/not-zip-safe
+-rw-rw-r--   0 robert    (1000) robert    (1000)      139 2023-06-23 14:33:36.000000 zenodoclient-0.5.1/src/zenodoclient.egg-info/requires.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)       13 2023-06-23 14:33:36.000000 zenodoclient-0.5.1/src/zenodoclient.egg-info/top_level.txt
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-06-23 14:33:36.217774 zenodoclient-0.5.1/tests/
+-rw-rw-r--   0 robert    (1000) robert    (1000)      804 2022-12-22 15:23:20.000000 zenodoclient-0.5.1/tests/test_api.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      244 2022-12-22 15:23:20.000000 zenodoclient-0.5.1/tests/test_catalog.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     1251 2023-06-23 14:22:54.000000 zenodoclient-0.5.1/tests/test_integration.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     4292 2022-12-22 15:23:20.000000 zenodoclient-0.5.1/tests/test_models.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      869 2022-12-22 15:23:20.000000 zenodoclient-0.5.1/tests/test_oai.py
```

### Comparing `zenodoclient-0.5.0/LICENSE` & `zenodoclient-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zenodoclient-0.5.0/PKG-INFO` & `zenodoclient-0.5.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,82 +1,16 @@
 Metadata-Version: 2.1
 Name: zenodoclient
-Version: 0.5.0
+Version: 0.5.1
 Summary: programmatic access to Zenodo
 Home-page: https://github.com/dlce-eva/zenodoclient
 Author: Robert Forkel
 Author-email: robert_forkel@eva.mpg.de
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/dlce-eva/zenodoclient/issues
-Description: # zenodoclient
-        
-        [![Build Status](https://github.com/dlce-eva/zenodoclient/workflows/tests/badge.svg)](https://github.com/dlce-eva/zenodoclient/actions?query=workflow%3Atests)
-        [![PyPI](https://img.shields.io/pypi/v/zenodoclient.svg)](https://pypi.org/project/zenodoclient)
-        
-        Python package to access the Zenodo API ([REST](http://developers.zenodo.org/) and
-        [OAI-PMH](http://developers.zenodo.org/#oai-pmh)) programmatically and from the command line.
-        
-        
-        # Install
-        
-        To install from pypi
-        ```shell
-        pip install zenodoclient
-        ```
-        
-        Instructions for a development installation can be found in 
-        [`CONTRIBUTING.md`](CONTRIBUTING.md).
-        
-        
-        # Curating deposits
-        
-        To curate deposits on Zenodo, you need an [access token](https://zenodo.org/account/settings/applications/tokens/new/).
-        Then you can use the CLI:
-        ```
-        zenodo --access-token $YOURTOKEN ls
-        ```
-        
-        
-        # Accessing OAI-PMH feeds
-        
-        Zenodo disseminates the metadata for communities via OAI-PMH. This metadata
-        can be accessed programmatically from python as folows:
-        ```python
-        >>> from zenodoclient.oai import Records
-        >>> recs = Records('dictionaria')
-        >>> len(recs)
-        18
-        ```
-        We can list the latest version for each Dictionaria dictionary:
-        ```python
-        >>> import itertools
-        >>> for d, records in itertools.groupby(sorted(recs, key=lambda r: (r.repos.repos, r.version), reverse=True), lambda r: r.repos.repos):
-        ...     print(d, next(records).tag)
-        ...     
-        wersing v1.0
-        tseltal v1.0.1
-        teop v1.0
-        sidaama v1.0
-        sanzhi v1.0
-        palula v1.0
-        nen v1.1
-        medialengua v1.0
-        kalamang v1.0
-        hdi v1.1
-        guarayu v1.0
-        diidxaza v1.0
-        daakaka v1.1.1
-        ```
-        and look at metadata:
-        ```python
-        >>> recs[0].doi
-        '10.5281/zenodo.3066952'
-        >>> recs[0].citation
-        'Henrik Liljegren. (2019). dictionaria/palula: Palula Dictionary (Version v1.0) [Data set]. Zenodo. http://doi.org/10.5281/zenodo.3066952'
-        ```
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -88,7 +22,75 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
+License-File: LICENSE
+
+# zenodoclient
+
+[![Build Status](https://github.com/dlce-eva/zenodoclient/workflows/tests/badge.svg)](https://github.com/dlce-eva/zenodoclient/actions?query=workflow%3Atests)
+[![PyPI](https://img.shields.io/pypi/v/zenodoclient.svg)](https://pypi.org/project/zenodoclient)
+
+Python package to access the Zenodo API ([REST](http://developers.zenodo.org/) and
+[OAI-PMH](http://developers.zenodo.org/#oai-pmh)) programmatically and from the command line.
+
+
+# Install
+
+To install from pypi
+```shell
+pip install zenodoclient
+```
+
+Instructions for a development installation can be found in 
+[`CONTRIBUTING.md`](CONTRIBUTING.md).
+
+
+# Curating deposits
+
+To curate deposits on Zenodo, you need an [access token](https://zenodo.org/account/settings/applications/tokens/new/).
+Then you can use the CLI:
+```
+zenodo --access-token $YOURTOKEN ls
+```
+
+
+# Accessing OAI-PMH feeds
+
+Zenodo disseminates the metadata for communities via OAI-PMH. This metadata
+can be accessed programmatically from python as folows:
+```python
+>>> from zenodoclient.oai import Records
+>>> recs = Records('dictionaria')
+>>> len(recs)
+18
+```
+We can list the latest version for each Dictionaria dictionary:
+```python
+>>> import itertools
+>>> for d, records in itertools.groupby(sorted(recs, key=lambda r: (r.repos.repos, r.version), reverse=True), lambda r: r.repos.repos):
+...     print(d, next(records).tag)
+...     
+wersing v1.0
+tseltal v1.0.1
+teop v1.0
+sidaama v1.0
+sanzhi v1.0
+palula v1.0
+nen v1.1
+medialengua v1.0
+kalamang v1.0
+hdi v1.1
+guarayu v1.0
+diidxaza v1.0
+daakaka v1.1.1
+```
+and look at metadata:
+```python
+>>> recs[0].doi
+'10.5281/zenodo.3066952'
+>>> recs[0].citation
+'Henrik Liljegren. (2019). dictionaria/palula: Palula Dictionary (Version v1.0) [Data set]. Zenodo. http://doi.org/10.5281/zenodo.3066952'
+```
```

### Comparing `zenodoclient-0.5.0/README.md` & `zenodoclient-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `zenodoclient-0.5.0/setup.cfg` & `zenodoclient-0.5.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = zenodoclient
-version = 0.5.0
+version = 0.5.1
 author = Robert Forkel
 author_email = robert_forkel@eva.mpg.de
 description = programmatic access to Zenodo
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Apache 2.0
 license_files = LICENSE
```

### Comparing `zenodoclient-0.5.0/src/zenodoclient/__main__.py` & `zenodoclient-0.5.1/src/zenodoclient/__main__.py`

 * *Files identical despite different names*

### Comparing `zenodoclient-0.5.0/src/zenodoclient/api.py` & `zenodoclient-0.5.1/src/zenodoclient/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,23 +9,28 @@
 import zipfile
 import requests
 import tempfile
 import warnings
 from http.client import responses as http_status
 import urllib.request
 
-from urllib3.exceptions import InsecurePlatformWarning, SNIMissingWarning
+from urllib3.exceptions import InsecurePlatformWarning
+try:
+    from urllib3.exceptions import SNIMissingWarning
+except ImportError:
+    SNIMissingWarning = None
 from bs4 import BeautifulSoup as bs
 from clldutils.path import md5
 
 from zenodoclient.models import Deposition, DepositionFile, PUBLISHED, \
     UNSUBMITTED, Record
 from zenodoclient import oai
 
-warnings.simplefilter('once', SNIMissingWarning)
+if SNIMissingWarning is not None:
+    warnings.simplefilter('once', SNIMissingWarning)
 warnings.simplefilter('once', InsecurePlatformWarning)
 
 API_URL = 'https://zenodo.org/api/'
 API_URL_SANDBOX = 'https://sandbox.zenodo.org/api/'
 ACCESS_TOKEN = os.environ.get('ZENODO_ACCESS_TOKEN')
```

### Comparing `zenodoclient-0.5.0/src/zenodoclient/catalog.py` & `zenodoclient-0.5.1/src/zenodoclient/catalog.py`

 * *Files identical despite different names*

### Comparing `zenodoclient-0.5.0/src/zenodoclient/commands/update.py` & `zenodoclient-0.5.1/src/zenodoclient/commands/update.py`

 * *Files identical despite different names*

### Comparing `zenodoclient-0.5.0/src/zenodoclient/commands/updatepeople.py` & `zenodoclient-0.5.1/src/zenodoclient/commands/updatepeople.py`

 * *Files identical despite different names*

### Comparing `zenodoclient-0.5.0/src/zenodoclient/models.py` & `zenodoclient-0.5.1/src/zenodoclient/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,20 +209,20 @@
     )
     contributors = attr.ib(
         default=attr.Factory(list),
         validator=functools.partial(check_persons, with_type=CONTRIBUTOR_TYPES))
     references = attr.ib(default=attr.Factory(list))
     communities = attr.ib(
         default=attr.Factory(list),
-        converter=lambda l: [{'identifier': d.get('id', d.get('identifier'))} for d in l],
+        converter=lambda ll: [{'identifier': d.get('id', d.get('identifier'))} for d in ll],
         validator=functools.partial(check_list_of_objects, dict(identifier=True))
     )
     grants = attr.ib(
         default=attr.Factory(list),
-        converter=lambda l: [convert_grant(d) for d in l],
+        converter=lambda ll: [convert_grant(d) for d in ll],
         validator=functools.partial(
             check_list_of_objects,
             dict(
                 id=True,
                 code=False,
                 program=False,
                 acronym=False,
@@ -294,15 +294,15 @@
     @property
     def url(self):
         return self.links['self']
 
 
 @attr.s
 class Record(Serializable):
-    files = attr.ib(converter=lambda l: [RecordFile(**f) for f in l])
+    files = attr.ib(converter=lambda ll: [RecordFile(**f) for f in ll])
     owners = attr.ib()
     doi = attr.ib()
     stats = attr.ib()
     links = attr.ib()
     conceptdoi = attr.ib()
     created = attr.ib()
     updated = attr.ib()
```

### Comparing `zenodoclient-0.5.0/src/zenodoclient/oai.py` & `zenodoclient-0.5.1/src/zenodoclient/oai.py`

 * *Files identical despite different names*

### Comparing `zenodoclient-0.5.0/src/zenodoclient.egg-info/PKG-INFO` & `zenodoclient-0.5.1/src/zenodoclient.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,82 +1,16 @@
 Metadata-Version: 2.1
 Name: zenodoclient
-Version: 0.5.0
+Version: 0.5.1
 Summary: programmatic access to Zenodo
 Home-page: https://github.com/dlce-eva/zenodoclient
 Author: Robert Forkel
 Author-email: robert_forkel@eva.mpg.de
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/dlce-eva/zenodoclient/issues
-Description: # zenodoclient
-        
-        [![Build Status](https://github.com/dlce-eva/zenodoclient/workflows/tests/badge.svg)](https://github.com/dlce-eva/zenodoclient/actions?query=workflow%3Atests)
-        [![PyPI](https://img.shields.io/pypi/v/zenodoclient.svg)](https://pypi.org/project/zenodoclient)
-        
-        Python package to access the Zenodo API ([REST](http://developers.zenodo.org/) and
-        [OAI-PMH](http://developers.zenodo.org/#oai-pmh)) programmatically and from the command line.
-        
-        
-        # Install
-        
-        To install from pypi
-        ```shell
-        pip install zenodoclient
-        ```
-        
-        Instructions for a development installation can be found in 
-        [`CONTRIBUTING.md`](CONTRIBUTING.md).
-        
-        
-        # Curating deposits
-        
-        To curate deposits on Zenodo, you need an [access token](https://zenodo.org/account/settings/applications/tokens/new/).
-        Then you can use the CLI:
-        ```
-        zenodo --access-token $YOURTOKEN ls
-        ```
-        
-        
-        # Accessing OAI-PMH feeds
-        
-        Zenodo disseminates the metadata for communities via OAI-PMH. This metadata
-        can be accessed programmatically from python as folows:
-        ```python
-        >>> from zenodoclient.oai import Records
-        >>> recs = Records('dictionaria')
-        >>> len(recs)
-        18
-        ```
-        We can list the latest version for each Dictionaria dictionary:
-        ```python
-        >>> import itertools
-        >>> for d, records in itertools.groupby(sorted(recs, key=lambda r: (r.repos.repos, r.version), reverse=True), lambda r: r.repos.repos):
-        ...     print(d, next(records).tag)
-        ...     
-        wersing v1.0
-        tseltal v1.0.1
-        teop v1.0
-        sidaama v1.0
-        sanzhi v1.0
-        palula v1.0
-        nen v1.1
-        medialengua v1.0
-        kalamang v1.0
-        hdi v1.1
-        guarayu v1.0
-        diidxaza v1.0
-        daakaka v1.1.1
-        ```
-        and look at metadata:
-        ```python
-        >>> recs[0].doi
-        '10.5281/zenodo.3066952'
-        >>> recs[0].citation
-        'Henrik Liljegren. (2019). dictionaria/palula: Palula Dictionary (Version v1.0) [Data set]. Zenodo. http://doi.org/10.5281/zenodo.3066952'
-        ```
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -88,7 +22,75 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
+License-File: LICENSE
+
+# zenodoclient
+
+[![Build Status](https://github.com/dlce-eva/zenodoclient/workflows/tests/badge.svg)](https://github.com/dlce-eva/zenodoclient/actions?query=workflow%3Atests)
+[![PyPI](https://img.shields.io/pypi/v/zenodoclient.svg)](https://pypi.org/project/zenodoclient)
+
+Python package to access the Zenodo API ([REST](http://developers.zenodo.org/) and
+[OAI-PMH](http://developers.zenodo.org/#oai-pmh)) programmatically and from the command line.
+
+
+# Install
+
+To install from pypi
+```shell
+pip install zenodoclient
+```
+
+Instructions for a development installation can be found in 
+[`CONTRIBUTING.md`](CONTRIBUTING.md).
+
+
+# Curating deposits
+
+To curate deposits on Zenodo, you need an [access token](https://zenodo.org/account/settings/applications/tokens/new/).
+Then you can use the CLI:
+```
+zenodo --access-token $YOURTOKEN ls
+```
+
+
+# Accessing OAI-PMH feeds
+
+Zenodo disseminates the metadata for communities via OAI-PMH. This metadata
+can be accessed programmatically from python as folows:
+```python
+>>> from zenodoclient.oai import Records
+>>> recs = Records('dictionaria')
+>>> len(recs)
+18
+```
+We can list the latest version for each Dictionaria dictionary:
+```python
+>>> import itertools
+>>> for d, records in itertools.groupby(sorted(recs, key=lambda r: (r.repos.repos, r.version), reverse=True), lambda r: r.repos.repos):
+...     print(d, next(records).tag)
+...     
+wersing v1.0
+tseltal v1.0.1
+teop v1.0
+sidaama v1.0
+sanzhi v1.0
+palula v1.0
+nen v1.1
+medialengua v1.0
+kalamang v1.0
+hdi v1.1
+guarayu v1.0
+diidxaza v1.0
+daakaka v1.1.1
+```
+and look at metadata:
+```python
+>>> recs[0].doi
+'10.5281/zenodo.3066952'
+>>> recs[0].citation
+'Henrik Liljegren. (2019). dictionaria/palula: Palula Dictionary (Version v1.0) [Data set]. Zenodo. http://doi.org/10.5281/zenodo.3066952'
+```
```


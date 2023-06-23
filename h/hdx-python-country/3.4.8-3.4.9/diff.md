# Comparing `tmp/hdx-python-country-3.4.8.tar.gz` & `tmp/hdx_python_country-3.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdx-python-country-3.4.8.tar", last modified: Thu Apr 13 04:30:58 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `hdx-python-country-3.4.8.tar` & `hdx_python_country-3.4.9.tar`

### file list

```diff
@@ -1,46 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:30:58.259808 hdx-python-country-3.4.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:30:58.255807 hdx-python-country-3.4.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:30:58.255807 hdx-python-country-3.4.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-13 04:30:38.000000 hdx-python-country-3.4.8/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-13 04:30:38.000000 hdx-python-country-3.4.8/.github/workflows/run-python-tests.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1148 2023-04-13 04:30:38.000000 hdx-python-country-3.4.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-13 04:30:38.000000 hdx-python-country-3.4.8/.readthedocs.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1306 2023-04-13 04:30:38.000000 hdx-python-country-3.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-04-13 04:30:58.259808 hdx-python-country-3.4.8/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2292 2023-04-13 04:30:38.000000 hdx-python-country-3.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:30:58.255807 hdx-python-country-3.4.8/doc/
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-04-13 04:30:38.000000 hdx-python-country-3.4.8/doc/main.md
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-04-13 04:30:38.000000 hdx-python-country-3.4.8/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)       60 2023-04-13 04:30:38.000000 hdx-python-country-3.4.8/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1516 2023-04-13 04:30:58.263808 hdx-python-country-3.4.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:30:58.255807 hdx-python-country-3.4.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:30:58.255807 hdx-python-country-3.4.8/src/hdx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:30:58.259808 hdx-python-country-3.4.8/src/hdx/location/
--rw-r--r--   0 runner    (1001) docker     (123)    67466 2023-04-13 04:30:38.000000 hdx-python-country-3.4.8/src/hdx/location/Countries & Territories Taxonomy MVP - C&T Taxonomy with HXL Tags.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)       59 2023-04-13 04:30:38.000000 hdx-python-country-3.4.8/src/hdx/location/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-13 04:30:58.000000 hdx-python-country-3.4.8/src/hdx/location/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12372 2023-04-13 04:30:38.000000 hdx-python-country-3.4.8/src/hdx/location/adminlevel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    32381 2023-04-13 04:30:38.000000 hdx-python-country-3.4.8/src/hdx/location/country.py
--rw-r--r--   0 runner    (1001) docker     (123)    17159 2023-04-13 04:30:38.000000 hdx-python-country-3.4.8/src/hdx/location/currency.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-13 04:30:38.000000 hdx-python-country-3.4.8/src/hdx/location/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-13 04:30:38.000000 hdx-python-country-3.4.8/src/hdx/location/phonetics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:30:58.259808 hdx-python-country-3.4.8/src/hdx_python_country.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-04-13 04:30:58.000000 hdx-python-country-3.4.8/src/hdx_python_country.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-13 04:30:58.000000 hdx-python-country-3.4.8/src/hdx_python_country.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 04:30:58.000000 hdx-python-country-3.4.8/src/hdx_python_country.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-13 04:30:58.000000 hdx-python-country-3.4.8/src/hdx_python_country.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-13 04:30:58.000000 hdx-python-country-3.4.8/src/hdx_python_country.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 04:30:56.000000 hdx-python-country-3.4.8/src/hdx_python_country.egg-info/zip-safe
--rwxr-xr-x   0 runner    (1001) docker     (123)       64 2023-04-13 04:30:38.000000 hdx-python-country-3.4.8/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:30:58.255807 hdx-python-country-3.4.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:30:58.259808 hdx-python-country-3.4.8/tests/fixtures/
--rwxr-xr-x   0 runner    (1001) docker     (123)    22035 2023-04-13 04:30:38.000000 hdx-python-country-3.4.8/tests/fixtures/adminlevel.yml
--rw-r--r--   0 runner    (1001) docker     (123)    33190 2023-04-13 04:30:38.000000 hdx-python-country-3.4.8/tests/fixtures/secondary_historic_rates.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-13 04:30:38.000000 hdx-python-country-3.4.8/tests/fixtures/secondary_rates.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:30:58.255807 hdx-python-country-3.4.8/tests/hdx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:30:58.259808 hdx-python-country-3.4.8/tests/hdx/location/
--rwxr-xr-x   0 runner    (1001) docker     (123)    65717 2023-04-13 04:30:38.000000 hdx-python-country-3.4.8/tests/hdx/location/Countries_UZB_Deleted.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)      177 2023-04-13 04:30:38.000000 hdx-python-country-3.4.8/tests/hdx/location/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4456 2023-04-13 04:30:38.000000 hdx-python-country-3.4.8/tests/hdx/location/test_adminlevel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    30396 2023-04-13 04:30:38.000000 hdx-python-country-3.4.8/tests/hdx/location/test_country.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9462 2023-04-13 04:30:38.000000 hdx-python-country-3.4.8/tests/hdx/location/test_currency.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/CONTRIBUTING.md
+-rwxr-xr-x   0        0        0     3858 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/requirements.txt
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/.config/black.toml
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/.config/coveragerc
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/.config/pre-commit-config.yaml
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/.config/pytest.ini
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/.config/ruff.toml
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/.github/workflows/run-python-tests.yml
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/documentation/.readthedocs.yaml
+-rw-r--r--   0        0        0     8302 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/documentation/main.md
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/documentation/pydoc-markdown.yml
+-rw-r--r--   0        0        0    67466 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/src/hdx/location/Countries & Territories Taxonomy MVP - C&T Taxonomy with HXL Tags.csv
+-rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/src/hdx/location/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/src/hdx/location/_version.py
+-rwxr-xr-x   0        0        0    12372 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/src/hdx/location/adminlevel.py
+-rwxr-xr-x   0        0        0    32382 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/src/hdx/location/country.py
+-rw-r--r--   0        0        0    17159 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/src/hdx/location/currency.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/src/hdx/location/names.py
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/src/hdx/location/phonetics.py
+-rwxr-xr-x   0        0        0    22035 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/tests/fixtures/adminlevel.yml
+-rw-r--r--   0        0        0    33190 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/tests/fixtures/secondary_historic_rates.csv
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/tests/fixtures/secondary_rates.json
+-rwxr-xr-x   0        0        0    65717 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/tests/hdx/location/Countries_UZB_Deleted.csv
+-rwxr-xr-x   0        0        0      177 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/tests/hdx/location/__init__.py
+-rwxr-xr-x   0        0        0     4456 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/tests/hdx/location/test_adminlevel.py
+-rwxr-xr-x   0        0        0    30396 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/tests/hdx/location/test_country.py
+-rwxr-xr-x   0        0        0     9462 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/tests/hdx/location/test_currency.py
+-rwxr-xr-x   0        0        0     1143 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/.gitignore
+-rwxr-xr-x   0        0        0     1306 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/LICENSE
+-rwxr-xr-x   0        0        0     2304 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/README.md
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/pyproject.toml
+-rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 hdx_python_country-3.4.9/PKG-INFO
```

### Comparing `hdx-python-country-3.4.8/.github/workflows/publish.yml` & `hdx_python_country-3.4.9/.github/workflows/publish.yml`

 * *Files 19% similar despite different names*

```diff
@@ -6,25 +6,28 @@
 
 jobs:
   publish:
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v3
-    - name: Get history and tags for SCM versioning to work
+    - name: Get history and tags for versioning to work
       run: |
         git fetch --prune --unshallow
         git fetch --depth=1 origin +refs/tags/*:refs/tags/*
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
         python-version: '3.x'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install --upgrade tox-gh-actions
-    - name: Publish with tox and twine
+        pip install --upgrade hatch
+    - name: Build with hatch
+      run: |
+        hatch build
+    - name: Publish with hatch
       env:
-        TWINE_USERNAME: ${{ secrets.TWINE_USERNAME }}
-        TWINE_PASSWORD: ${{ secrets.TWINE_PASSWORD }}
+        HATCH_INDEX_USER: ${{secrets.HATCH_INDEX_USER}}
+        HATCH_INDEX_AUTH: ${{secrets.HATCH_INDEX_AUTH}}
       run: |
-        tox -e publish
+        hatch publish
```

### Comparing `hdx-python-country-3.4.8/.github/workflows/run-python-tests.yml` & `hdx_python_country-3.4.9/.github/workflows/run-python-tests.yml`

 * *Files 18% similar despite different names*

```diff
@@ -20,20 +20,27 @@
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
         python-version: '3.x'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install --upgrade tox-gh-actions
-    - name: Test with tox/pytest
+        pip install --upgrade hatch
+    - name: Test with hatch/pytest
       run: |
-        tox
+        hatch run test:test
+    - name: Check styling
+      if: always()
+      run: |
+        hatch run lint:style
     - name: Publish Unit Test Results
       uses: EnricoMi/publish-unit-test-result-action@v2
       if: always()
       with:
         github_token: ${{ secrets.GITHUB_TOKEN }}
-        junit_files: .tox/*.xml
-    - name: Upload Coverage Results
-      uses: codecov/codecov-action@v3
-      if: success()
+        junit_files: test-results.xml
+    - name: Publish in Coveralls
+      uses: coverallsapp/github-action@v2
+      with:
+        github-token: ${{ secrets.GITHUB_TOKEN }}
+        flag-name: tests
+        format: lcov
```

### Comparing `hdx-python-country-3.4.8/.gitignore` & `hdx_python_country-3.4.9/.gitignore`

 * *Files 16% similar despite different names*

```diff
@@ -90,9 +90,9 @@
 
 # Rope project settings
 .ropeproject
 
 # IntelliJ
 .idea/
 
-# setuptools_scm
+# hatch-vcs
 _version.py
```

### Comparing `hdx-python-country-3.4.8/LICENSE` & `hdx_python_country-3.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hdx-python-country-3.4.8/PKG-INFO` & `hdx_python_country-3.4.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,46 @@
 Metadata-Version: 2.1
 Name: hdx-python-country
-Version: 3.4.8
+Version: 3.4.9
 Summary: HDX Python country code and exchange rate (fx) utilities
-Home-page: https://github.com/OCHA-DAP/hdx-python-country
-Author: Michael Rans
-Author-email: rans@email.com
+Project-URL: Homepage, https://github.com/OCHA-DAP/hdx-python-country
+Author-email: Michael Rans <rans@email.com>
 License: MIT
-Keywords: HDX,location,country,country code,iso 3166,iso2,iso3,region,fx,currency,currencies,exchange rate,foreign exchange
-Platform: any
+License-File: LICENSE
+Keywords: HDX,country,country code,currencies,currency,exchange rate,foreign exchange,fx,iso 3166,iso2,iso3,location,region
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Microsoft :: Windows
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
-Description-Content-Type: text/markdown; charset=UTF-8
-License-File: LICENSE
+Requires-Dist: hdx-python-utilities>=3.5.9
+Requires-Dist: libhxl
+Requires-Dist: pyphonetics
+Provides-Extra: dev
+Requires-Dist: pre-commit; extra == 'dev'
+Provides-Extra: test
+Requires-Dist: pytest; extra == 'test'
+Requires-Dist: pytest-cov; extra == 'test'
+Description-Content-Type: text/markdown
 
 [![Build Status](https://github.com/OCHA-DAP/hdx-python-country/actions/workflows/run-python-tests.yml/badge.svg)](https://github.com/OCHA-DAP/hdx-python-country/actions/workflows/run-python-tests.yml)
-[![Coverage Status](https://codecov.io/gh/OCHA-DAP/hdx-python-country/branch/main/graph/badge.svg?token=JpWZc5js4y)](https://codecov.io/gh/OCHA-DAP/hdx-python-country)
+[![Coverage Status](https://coveralls.io/repos/github/OCHA-DAP/hdx-python-country/badge.svg?branch=main&ts=1)](https://coveralls.io/github/OCHA-DAP/hdx-python-country?branch=main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![Downloads](https://img.shields.io/pypi/dm/hdx-python-country.svg)](https://pypistats.org/packages/hdx-python-country)
 
 The HDX Python Country Library provides utilities to map between country and region 
 codes and names and to match administrative level names from different sources.
 It also provides utilities for foreign exchange enabling obtaining current and historic
```

### Comparing `hdx-python-country-3.4.8/README.md` & `hdx_python_country-3.4.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [![Build Status](https://github.com/OCHA-DAP/hdx-python-country/actions/workflows/run-python-tests.yml/badge.svg)](https://github.com/OCHA-DAP/hdx-python-country/actions/workflows/run-python-tests.yml)
-[![Coverage Status](https://codecov.io/gh/OCHA-DAP/hdx-python-country/branch/main/graph/badge.svg?token=JpWZc5js4y)](https://codecov.io/gh/OCHA-DAP/hdx-python-country)
+[![Coverage Status](https://coveralls.io/repos/github/OCHA-DAP/hdx-python-country/badge.svg?branch=main&ts=1)](https://coveralls.io/github/OCHA-DAP/hdx-python-country?branch=main)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![Downloads](https://img.shields.io/pypi/dm/hdx-python-country.svg)](https://pypistats.org/packages/hdx-python-country)
 
 The HDX Python Country Library provides utilities to map between country and region 
 codes and names and to match administrative level names from different sources.
 It also provides utilities for foreign exchange enabling obtaining current and historic
```

### Comparing `hdx-python-country-3.4.8/doc/main.md` & `hdx_python_country-3.4.9/documentation/main.md`

 * *Files identical despite different names*

### Comparing `hdx-python-country-3.4.8/src/hdx/location/Countries & Territories Taxonomy MVP - C&T Taxonomy with HXL Tags.csv` & `hdx_python_country-3.4.9/src/hdx/location/Countries & Territories Taxonomy MVP - C&T Taxonomy with HXL Tags.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-country-3.4.8/src/hdx/location/adminlevel.py` & `hdx_python_country-3.4.9/src/hdx/location/adminlevel.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 from typing import Dict, List, Optional, Tuple
 
-from hdx.utilities.text import multiple_replace
 from unidecode import unidecode
 
 from hdx.location.country import Country
 from hdx.location.names import clean_name
 from hdx.location.phonetics import Phonetics
+from hdx.utilities.text import multiple_replace
 
 logger = logging.getLogger(__name__)
 
 
 class AdminLevel:
     """AdminLevel class which takes in pcodes and then maps names to those pcodes with fuzzy matching if necessary. The
     input configuration dictionary, admin_config, requires key admin_info which is a list with values of the form:
```

### Comparing `hdx-python-country-3.4.8/src/hdx/location/country.py` & `hdx_python_country-3.4.9/src/hdx/location/country.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 import copy
 import logging
 import re
 from string import punctuation
 from typing import Dict, List, Optional, Tuple, TypeVar, Union
 
 import hxl
+from hxl import InputOptions
+
 from hdx.utilities.path import script_dir_plus_file
 from hdx.utilities.text import get_words_in_sentence
-from hxl import InputOptions
 
 ExceptionUpperBound = TypeVar("T", bound="Exception")
 
 
 logger = logging.getLogger(__name__)
```

### Comparing `hdx-python-country-3.4.8/src/hdx/location/currency.py` & `hdx_python_country-3.4.9/src/hdx/location/currency.py`

 * *Files identical despite different names*

### Comparing `hdx-python-country-3.4.8/src/hdx/location/names.py` & `hdx_python_country-3.4.9/src/hdx/location/names.py`

 * *Files identical despite different names*

### Comparing `hdx-python-country-3.4.8/src/hdx/location/phonetics.py` & `hdx_python_country-3.4.9/src/hdx/location/phonetics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Callable, Optional
 
 import pyphonetics
+
 from hdx.utilities.typehint import ListTuple
 
 
 class Phonetics(pyphonetics.RefinedSoundex):
     def match(
         self,
         possible_names: ListTuple,
```

### Comparing `hdx-python-country-3.4.8/tests/fixtures/adminlevel.yml` & `hdx_python_country-3.4.9/tests/fixtures/adminlevel.yml`

 * *Files identical despite different names*

### Comparing `hdx-python-country-3.4.8/tests/fixtures/secondary_historic_rates.csv` & `hdx_python_country-3.4.9/tests/fixtures/secondary_historic_rates.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-country-3.4.8/tests/fixtures/secondary_rates.json` & `hdx_python_country-3.4.9/tests/fixtures/secondary_rates.json`

 * *Files identical despite different names*

### Comparing `hdx-python-country-3.4.8/tests/hdx/location/Countries_UZB_Deleted.csv` & `hdx_python_country-3.4.9/tests/hdx/location/Countries_UZB_Deleted.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-country-3.4.8/tests/hdx/location/test_adminlevel.py` & `hdx_python_country-3.4.9/tests/hdx/location/test_adminlevel.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """location Tests"""
 from os.path import join
 
 import pytest
-from hdx.utilities.loader import load_yaml
 
 from hdx.location.adminlevel import AdminLevel
+from hdx.utilities.loader import load_yaml
 
 
 class TestAdminLevel:
     @pytest.fixture(scope="function")
     def config(self):
         return load_yaml(join("tests", "fixtures", "adminlevel.yml"))
```

### Comparing `hdx-python-country-3.4.8/tests/hdx/location/test_country.py` & `hdx_python_country-3.4.9/tests/hdx/location/test_country.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """location Tests"""
 import hxl
 import pytest
-from hdx.utilities.path import script_dir_plus_file
 from hxl import InputOptions
 
 from hdx.location.country import Country
+from hdx.utilities.path import script_dir_plus_file
 
 
 class LocationError(Exception):
     pass
 
 
 # Note that the Country class is set up in __init__.py
```

### Comparing `hdx-python-country-3.4.8/tests/hdx/location/test_currency.py` & `hdx_python_country-3.4.9/tests/hdx/location/test_currency.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Currency Tests"""
 from os.path import join
 
 import pytest
+
+from hdx.location.currency import Currency, CurrencyError
 from hdx.utilities.dateparse import parse_date
 from hdx.utilities.downloader import Download
 from hdx.utilities.path import get_temp_dir
 from hdx.utilities.retriever import Retrieve
 from hdx.utilities.useragent import UserAgent
 
-from hdx.location.currency import Currency, CurrencyError
-
 
 class TestCurrency:
     @pytest.fixture(scope="class")
     def fixtures(self):
         return join("tests", "fixtures")
 
     @pytest.fixture(scope="class")
```


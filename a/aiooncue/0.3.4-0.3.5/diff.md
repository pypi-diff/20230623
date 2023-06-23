# Comparing `tmp/aiooncue-0.3.4.tar.gz` & `tmp/aiooncue-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiooncue-0.3.4.tar", last modified: Tue May  3 17:46:45 2022, max compression
+gzip compressed data, was "aiooncue-0.3.5.tar", last modified: Fri Jun 23 21:24:40 2023, max compression
```

## Comparing `aiooncue-0.3.4.tar` & `aiooncue-0.3.5.tar`

### file list

```diff
@@ -1,48 +1,36 @@
-drwxr-xr-x   0 bdraco     (502) staff       (20)        0 2022-05-03 17:46:45.641068 aiooncue-0.3.4/
--rw-r--r--   0 bdraco     (502) staff       (20)      292 2022-01-01 03:42:46.000000 aiooncue-0.3.4/.editorconfig
-drwxr-xr-x   0 bdraco     (502) staff       (20)        0 2022-05-03 17:46:45.638001 aiooncue-0.3.4/.github/
--rw-r--r--   0 bdraco     (502) staff       (20)      322 2022-01-01 03:42:46.000000 aiooncue-0.3.4/.github/ISSUE_TEMPLATE.md
-drwxr-xr-x   0 bdraco     (502) staff       (20)        0 2022-05-03 17:46:45.638139 aiooncue-0.3.4/.github/workflows/
--rw-r--r--   0 bdraco     (502) staff       (20)      524 2022-01-01 20:20:24.000000 aiooncue-0.3.4/.github/workflows/ci.yaml
--rw-r--r--   0 bdraco     (502) staff       (20)     1214 2022-01-01 03:42:46.000000 aiooncue-0.3.4/.gitignore
--rw-r--r--   0 bdraco     (502) staff       (20)      690 2022-01-01 03:42:46.000000 aiooncue-0.3.4/.travis.yml
--rw-r--r--   0 bdraco     (502) staff       (20)      155 2022-01-01 03:42:46.000000 aiooncue-0.3.4/AUTHORS.rst
--rw-r--r--   0 bdraco     (502) staff       (20)     3520 2022-01-01 03:42:46.000000 aiooncue-0.3.4/CONTRIBUTING.rst
--rw-r--r--   0 bdraco     (502) staff       (20)       89 2022-01-01 03:42:46.000000 aiooncue-0.3.4/HISTORY.rst
--rw-r--r--   0 bdraco     (502) staff       (20)      586 2022-01-01 03:42:46.000000 aiooncue-0.3.4/LICENSE
--rw-r--r--   0 bdraco     (502) staff       (20)      262 2022-01-01 03:42:46.000000 aiooncue-0.3.4/MANIFEST.in
--rw-r--r--   0 bdraco     (502) staff       (20)     2201 2022-01-01 03:42:46.000000 aiooncue-0.3.4/Makefile
--rw-r--r--   0 bdraco     (502) staff       (20)     1720 2022-05-03 17:46:45.641143 aiooncue-0.3.4/PKG-INFO
--rwxr-xr-x   0 bdraco     (502) staff       (20)      629 2022-01-01 03:42:46.000000 aiooncue-0.3.4/README.md
--rw-r--r--   0 bdraco     (502) staff       (20)      862 2022-01-01 03:42:46.000000 aiooncue-0.3.4/README.rst
-drwxr-xr-x   0 bdraco     (502) staff       (20)        0 2022-05-03 17:46:45.638615 aiooncue-0.3.4/aiooncue/
--rw-r--r--   0 bdraco     (502) staff       (20)     8181 2022-05-03 17:45:52.000000 aiooncue-0.3.4/aiooncue/__init__.py
--rw-r--r--   0 bdraco     (502) staff       (20)    10819 2022-01-14 00:07:57.000000 aiooncue-0.3.4/aiooncue/const.py
--rw-r--r--   0 bdraco     (502) staff       (20)        0 2022-01-01 20:20:24.000000 aiooncue-0.3.4/aiooncue/py.typed
-drwxr-xr-x   0 bdraco     (502) staff       (20)        0 2022-05-03 17:46:45.639330 aiooncue-0.3.4/aiooncue.egg-info/
--rw-r--r--   0 bdraco     (502) staff       (20)     1720 2022-05-03 17:46:45.000000 aiooncue-0.3.4/aiooncue.egg-info/PKG-INFO
--rw-r--r--   0 bdraco     (502) staff       (20)      704 2022-05-03 17:46:45.000000 aiooncue-0.3.4/aiooncue.egg-info/SOURCES.txt
--rw-r--r--   0 bdraco     (502) staff       (20)        1 2022-05-03 17:46:45.000000 aiooncue-0.3.4/aiooncue.egg-info/dependency_links.txt
--rw-r--r--   0 bdraco     (502) staff       (20)        1 2022-01-01 03:58:24.000000 aiooncue-0.3.4/aiooncue.egg-info/not-zip-safe
--rw-r--r--   0 bdraco     (502) staff       (20)        8 2022-05-03 17:46:45.000000 aiooncue-0.3.4/aiooncue.egg-info/requires.txt
--rw-r--r--   0 bdraco     (502) staff       (20)        9 2022-05-03 17:46:45.000000 aiooncue-0.3.4/aiooncue.egg-info/top_level.txt
--rwxr-xr-x   0 bdraco     (502) staff       (20)       67 2022-01-01 20:25:24.000000 aiooncue-0.3.4/build.sh
-drwxr-xr-x   0 bdraco     (502) staff       (20)        0 2022-05-03 17:46:45.640694 aiooncue-0.3.4/docs/
--rw-r--r--   0 bdraco     (502) staff       (20)      609 2022-01-01 03:42:46.000000 aiooncue-0.3.4/docs/Makefile
--rw-r--r--   0 bdraco     (502) staff       (20)       28 2022-01-01 03:42:46.000000 aiooncue-0.3.4/docs/authors.rst
--rw-r--r--   0 bdraco     (502) staff       (20)     4809 2022-01-01 03:42:46.000000 aiooncue-0.3.4/docs/conf.py
--rw-r--r--   0 bdraco     (502) staff       (20)       33 2022-01-01 03:42:46.000000 aiooncue-0.3.4/docs/contributing.rst
--rw-r--r--   0 bdraco     (502) staff       (20)       28 2022-01-01 03:42:46.000000 aiooncue-0.3.4/docs/history.rst
--rw-r--r--   0 bdraco     (502) staff       (20)      308 2022-01-01 03:42:46.000000 aiooncue-0.3.4/docs/index.rst
--rw-r--r--   0 bdraco     (502) staff       (20)     1123 2022-01-01 03:42:46.000000 aiooncue-0.3.4/docs/installation.rst
--rw-r--r--   0 bdraco     (502) staff       (20)      770 2022-01-01 03:42:46.000000 aiooncue-0.3.4/docs/make.bat
--rw-r--r--   0 bdraco     (502) staff       (20)       27 2022-01-01 03:42:46.000000 aiooncue-0.3.4/docs/readme.rst
--rw-r--r--   0 bdraco     (502) staff       (20)       74 2022-01-01 03:42:46.000000 aiooncue-0.3.4/docs/usage.rst
--rw-r--r--   0 bdraco     (502) staff       (20)      363 2022-01-01 20:20:24.000000 aiooncue-0.3.4/pyproject.toml
--rw-r--r--   0 bdraco     (502) staff       (20)      166 2022-01-01 03:42:46.000000 aiooncue-0.3.4/requirements_dev.txt
--rw-r--r--   0 bdraco     (502) staff       (20)      683 2022-05-03 17:46:45.641453 aiooncue-0.3.4/setup.cfg
--rw-r--r--   0 bdraco     (502) staff       (20)     1463 2022-05-03 17:45:52.000000 aiooncue-0.3.4/setup.py
-drwxr-xr-x   0 bdraco     (502) staff       (20)        0 2022-05-03 17:46:45.640962 aiooncue-0.3.4/tests/
--rw-r--r--   0 bdraco     (502) staff       (20)       38 2022-01-01 03:42:46.000000 aiooncue-0.3.4/tests/__init__.py
--rw-r--r--   0 bdraco     (502) staff       (20)      556 2022-01-01 03:42:46.000000 aiooncue-0.3.4/tests/test_aiooncue.py
--rw-r--r--   0 bdraco     (502) staff       (20)      539 2022-01-01 03:42:46.000000 aiooncue-0.3.4/tox.ini
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-06-23 21:24:40.704870 aiooncue-0.3.5/
+-rw-r--r--   0 bdraco     (501) staff       (20)      155 2022-10-20 20:30:06.000000 aiooncue-0.3.5/AUTHORS.rst
+-rw-r--r--   0 bdraco     (501) staff       (20)     3520 2022-10-20 20:30:06.000000 aiooncue-0.3.5/CONTRIBUTING.rst
+-rw-r--r--   0 bdraco     (501) staff       (20)       89 2022-10-20 20:30:06.000000 aiooncue-0.3.5/HISTORY.rst
+-rw-r--r--   0 bdraco     (501) staff       (20)      586 2022-10-20 20:30:06.000000 aiooncue-0.3.5/LICENSE
+-rw-r--r--   0 bdraco     (501) staff       (20)      262 2022-10-20 20:30:06.000000 aiooncue-0.3.5/MANIFEST.in
+-rw-r--r--   0 bdraco     (501) staff       (20)     1700 2023-06-23 21:24:40.704924 aiooncue-0.3.5/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)      862 2022-10-20 20:30:06.000000 aiooncue-0.3.5/README.rst
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-06-23 21:24:40.702637 aiooncue-0.3.5/aiooncue/
+-rw-r--r--   0 bdraco     (501) staff       (20)     8689 2023-06-23 21:24:20.000000 aiooncue-0.3.5/aiooncue/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    10819 2022-10-20 20:30:06.000000 aiooncue-0.3.5/aiooncue/const.py
+-rw-r--r--   0 bdraco     (501) staff       (20)        0 2022-10-20 20:30:06.000000 aiooncue-0.3.5/aiooncue/py.typed
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-06-23 21:24:40.703503 aiooncue-0.3.5/aiooncue.egg-info/
+-rw-r--r--   0 bdraco     (501) staff       (20)     1700 2023-06-23 21:24:40.000000 aiooncue-0.3.5/aiooncue.egg-info/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)      558 2023-06-23 21:24:40.000000 aiooncue-0.3.5/aiooncue.egg-info/SOURCES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-06-23 21:24:40.000000 aiooncue-0.3.5/aiooncue.egg-info/dependency_links.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-06-23 21:22:32.000000 aiooncue-0.3.5/aiooncue.egg-info/not-zip-safe
+-rw-r--r--   0 bdraco     (501) staff       (20)        8 2023-06-23 21:24:40.000000 aiooncue-0.3.5/aiooncue.egg-info/requires.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        9 2023-06-23 21:24:40.000000 aiooncue-0.3.5/aiooncue.egg-info/top_level.txt
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-06-23 21:24:40.704574 aiooncue-0.3.5/docs/
+-rw-r--r--   0 bdraco     (501) staff       (20)      609 2022-10-20 20:30:06.000000 aiooncue-0.3.5/docs/Makefile
+-rw-r--r--   0 bdraco     (501) staff       (20)       28 2022-10-20 20:30:06.000000 aiooncue-0.3.5/docs/authors.rst
+-rw-r--r--   0 bdraco     (501) staff       (20)     4809 2022-10-20 20:30:06.000000 aiooncue-0.3.5/docs/conf.py
+-rw-r--r--   0 bdraco     (501) staff       (20)       33 2022-10-20 20:30:06.000000 aiooncue-0.3.5/docs/contributing.rst
+-rw-r--r--   0 bdraco     (501) staff       (20)       28 2022-10-20 20:30:06.000000 aiooncue-0.3.5/docs/history.rst
+-rw-r--r--   0 bdraco     (501) staff       (20)      308 2022-10-20 20:30:06.000000 aiooncue-0.3.5/docs/index.rst
+-rw-r--r--   0 bdraco     (501) staff       (20)     1123 2022-10-20 20:30:06.000000 aiooncue-0.3.5/docs/installation.rst
+-rw-r--r--   0 bdraco     (501) staff       (20)      770 2022-10-20 20:30:06.000000 aiooncue-0.3.5/docs/make.bat
+-rw-r--r--   0 bdraco     (501) staff       (20)       27 2022-10-20 20:30:06.000000 aiooncue-0.3.5/docs/readme.rst
+-rw-r--r--   0 bdraco     (501) staff       (20)       74 2022-10-20 20:30:06.000000 aiooncue-0.3.5/docs/usage.rst
+-rw-r--r--   0 bdraco     (501) staff       (20)      363 2022-10-20 20:30:06.000000 aiooncue-0.3.5/pyproject.toml
+-rw-r--r--   0 bdraco     (501) staff       (20)      683 2023-06-23 21:24:40.705181 aiooncue-0.3.5/setup.cfg
+-rw-r--r--   0 bdraco     (501) staff       (20)     1463 2023-06-23 21:24:20.000000 aiooncue-0.3.5/setup.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-06-23 21:24:40.704776 aiooncue-0.3.5/tests/
+-rw-r--r--   0 bdraco     (501) staff       (20)       38 2022-10-20 20:30:06.000000 aiooncue-0.3.5/tests/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      553 2023-06-23 21:24:12.000000 aiooncue-0.3.5/tests/test_aiooncue.py
```

### Comparing `aiooncue-0.3.4/CONTRIBUTING.rst` & `aiooncue-0.3.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `aiooncue-0.3.4/LICENSE` & `aiooncue-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aiooncue-0.3.4/PKG-INFO` & `aiooncue-0.3.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: aiooncue
-Version: 0.3.4
+Version: 0.3.5
 Summary: Async for Oncue
 Home-page: https://github.com/bdraco/aiooncue
 Author: J. Nick Koston
 Author-email: nick@koston.org
 License: Apache Software License 2.0
 Keywords: aiooncue
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
@@ -64,9 +63,7 @@
 History
 =======
 
 0.1.0 (2021-02-09)
 ------------------
 
 * First release on PyPI.
-
-
```

### Comparing `aiooncue-0.3.4/README.rst` & `aiooncue-0.3.5/README.rst`

 * *Files identical despite different names*

### Comparing `aiooncue-0.3.4/aiooncue/__init__.py` & `aiooncue-0.3.5/aiooncue/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from dataclasses import dataclass
 import json
 
 import aiohttp
 
 __author__ = """J. Nick Koston"""
 __email__ = "nick@koston.org"
-__version__ = "0.3.4"
+__version__ = "0.3.5"
 
 from .const import NAME_TO_SENSOR_ID
 
 REQUIRED_DEVICE_KEYS = {
     "displayname",
     "devicestate",
     "productname",
@@ -74,15 +74,21 @@
     "Latest Firmware",  # 1671
 ]
 
 ALL_DEVICES_PARAMETERS = json.dumps(
     [[NAME_TO_SENSOR_ID[name] for name in ALL_DETAILS_NAMES]], separators=(",", ":")
 )
 
-LOGIN_FAILED_CODES = {0: "Unknown", 1200: "Session Expired", 1207: "Invalid Password"}
+LOGIN_FAILED_CODES = {
+    0: "Unknown",
+    1200: "Session Expired",
+    1202: "Invalid username",
+    1207: "Invalid Password",
+}
+INCORRECT_CREDENTIALS_CODES = {1207, 1202}
 
 LOGIN_ENDPOINT = "/users/connect"
 
 
 @dataclass
 class OncueSensor:
     name: str
@@ -98,18 +104,26 @@
     state: str
     product_name: str
     hardware_version: str
     serial_number: str
     sensors: dict[str, OncueSensor]
 
 
-class LoginFailedException(Exception):
+class OncueException(Exception):
+    """Base oncue exception."""
+
+
+class LoginFailedException(OncueException):
     """Login failed exception."""
 
 
+class ServiceFailedException(OncueException):
+    """Service failed exception."""
+
+
 class Oncue:
     """Async oncue api."""
 
     def __init__(
         self,
         username: str,
         password: str,
@@ -147,17 +161,23 @@
 
     async def async_login(self) -> None:
         """Call api to login"""
         login_data = await self._get(
             LOGIN_ENDPOINT, {"username": self._username, "password": self._password}
         )
 
-        if "sessionkey" not in login_data:
-            self._auth_invalid = f"{login_data['message']} ({login_data.get('code')})"
-            raise LoginFailedException(self._auth_invalid)
+        if "code" in login_data:
+            code = login_data["code"]
+            message = login_data.get("message", "no message")
+            if login_data["code"] in INCORRECT_CREDENTIALS_CODES:
+                self._auth_invalid = f"{message} ({code})"
+                raise LoginFailedException(self._auth_invalid)
+            raise ServiceFailedException(
+                f"Login failed with unknown error code: {code} ({message})"
+            )
 
         self._sessionkey = login_data["sessionkey"]
 
     async def async_fetch_all(self) -> dict[str, OncueDevice]:
         """Fetch all devices."""
         devices = await self.async_list_devices_with_params()
         indexed_devices: dict[str, OncueDevice] = {}
```

### Comparing `aiooncue-0.3.4/aiooncue/const.py` & `aiooncue-0.3.5/aiooncue/const.py`

 * *Files identical despite different names*

### Comparing `aiooncue-0.3.4/aiooncue.egg-info/PKG-INFO` & `aiooncue-0.3.5/aiooncue.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: aiooncue
-Version: 0.3.4
+Version: 0.3.5
 Summary: Async for Oncue
 Home-page: https://github.com/bdraco/aiooncue
 Author: J. Nick Koston
 Author-email: nick@koston.org
 License: Apache Software License 2.0
 Keywords: aiooncue
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
@@ -64,9 +63,7 @@
 History
 =======
 
 0.1.0 (2021-02-09)
 ------------------
 
 * First release on PyPI.
-
-
```

### Comparing `aiooncue-0.3.4/docs/Makefile` & `aiooncue-0.3.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aiooncue-0.3.4/docs/conf.py` & `aiooncue-0.3.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aiooncue-0.3.4/docs/installation.rst` & `aiooncue-0.3.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `aiooncue-0.3.4/docs/make.bat` & `aiooncue-0.3.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aiooncue-0.3.4/setup.cfg` & `aiooncue-0.3.5/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.3.4
+current_version = 0.3.5
 commit = True
 tag = True
 tag_name = {new_version}
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `aiooncue-0.3.4/setup.py` & `aiooncue-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,10 +46,10 @@
     keywords="aiooncue",
     name="aiooncue",
     packages=find_packages(include=["aiooncue", "aiooncue.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/bdraco/aiooncue",
-    version="0.3.4",
+    version="0.3.5",
     zip_safe=False,
 )
```

### Comparing `aiooncue-0.3.4/tests/test_aiooncue.py` & `aiooncue-0.3.5/tests/test_aiooncue.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 """Tests for `aiooncue` package."""
 
 import pytest
 
 
-from aiooncue import aiooncue
+from aiooncue import Oncue
 
 
 @pytest.fixture
 def response():
     """Sample pytest fixture.
 
     See more at: http://doc.pytest.org/en/latest/fixture.html
```


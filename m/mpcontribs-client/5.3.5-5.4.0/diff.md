# Comparing `tmp/mpcontribs-client-5.3.5.tar.gz` & `tmp/mpcontribs-client-5.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpcontribs-client-5.3.5.tar", last modified: Tue May 23 23:51:53 2023, max compression
+gzip compressed data, was "mpcontribs-client-5.4.0.tar", last modified: Fri Jun 23 01:21:03 2023, max compression
```

## Comparing `mpcontribs-client-5.3.5.tar` & `mpcontribs-client-5.4.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:51:53.870851 mpcontribs-client-5.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-23 23:51:41.000000 mpcontribs-client-5.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-23 23:51:53.870851 mpcontribs-client-5.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-23 23:51:41.000000 mpcontribs-client-5.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:51:53.866851 mpcontribs-client-5.3.5/mpcontribs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:51:53.866851 mpcontribs-client-5.3.5/mpcontribs/client/
--rw-r--r--   0 runner    (1001) docker     (123)    86143 2023-05-23 23:51:41.000000 mpcontribs-client-5.3.5/mpcontribs/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:51:53.870851 mpcontribs-client-5.3.5/mpcontribs_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-23 23:51:53.000000 mpcontribs-client-5.3.5/mpcontribs_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-23 23:51:53.000000 mpcontribs-client-5.3.5/mpcontribs_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 23:51:53.000000 mpcontribs-client-5.3.5/mpcontribs_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 23:51:53.000000 mpcontribs-client-5.3.5/mpcontribs_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-23 23:51:53.000000 mpcontribs-client-5.3.5/mpcontribs_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-23 23:51:53.000000 mpcontribs-client-5.3.5/mpcontribs_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:51:53.870851 mpcontribs-client-5.3.5/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-05-23 23:51:41.000000 mpcontribs-client-5.3.5/requirements/deployment.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-05-23 23:51:41.000000 mpcontribs-client-5.3.5/requirements/macos-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-05-23 23:51:41.000000 mpcontribs-client-5.3.5/requirements/macos-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-05-23 23:51:41.000000 mpcontribs-client-5.3.5/requirements/macos-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-05-23 23:51:41.000000 mpcontribs-client-5.3.5/requirements/macos-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-05-23 23:51:41.000000 mpcontribs-client-5.3.5/requirements/macos-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-05-23 23:51:41.000000 mpcontribs-client-5.3.5/requirements/macos-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-05-23 23:51:41.000000 mpcontribs-client-5.3.5/requirements/ubuntu-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-05-23 23:51:41.000000 mpcontribs-client-5.3.5/requirements/ubuntu-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-05-23 23:51:41.000000 mpcontribs-client-5.3.5/requirements/ubuntu-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-05-23 23:51:41.000000 mpcontribs-client-5.3.5/requirements/ubuntu-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-05-23 23:51:41.000000 mpcontribs-client-5.3.5/requirements/ubuntu-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-05-23 23:51:41.000000 mpcontribs-client-5.3.5/requirements/ubuntu-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 23:51:53.870851 mpcontribs-client-5.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-23 23:51:41.000000 mpcontribs-client-5.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 23:51:53.870851 mpcontribs-client-5.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-23 23:51:41.000000 mpcontribs-client-5.3.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-05-23 23:51:41.000000 mpcontribs-client-5.3.5/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:21:03.388965 mpcontribs-client-5.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-23 01:20:45.000000 mpcontribs-client-5.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-23 01:21:03.388965 mpcontribs-client-5.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-23 01:20:45.000000 mpcontribs-client-5.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:21:03.384965 mpcontribs-client-5.4.0/mpcontribs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:21:03.384965 mpcontribs-client-5.4.0/mpcontribs/client/
+-rw-r--r--   0 runner    (1001) docker     (123)    87013 2023-06-23 01:20:45.000000 mpcontribs-client-5.4.0/mpcontribs/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:21:03.384965 mpcontribs-client-5.4.0/mpcontribs_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-23 01:21:02.000000 mpcontribs-client-5.4.0/mpcontribs_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-23 01:21:03.000000 mpcontribs-client-5.4.0/mpcontribs_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 01:21:02.000000 mpcontribs-client-5.4.0/mpcontribs_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 01:21:02.000000 mpcontribs-client-5.4.0/mpcontribs_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-23 01:21:02.000000 mpcontribs-client-5.4.0/mpcontribs_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-23 01:21:02.000000 mpcontribs-client-5.4.0/mpcontribs_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:21:03.388965 mpcontribs-client-5.4.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-06-23 01:20:45.000000 mpcontribs-client-5.4.0/requirements/deployment.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-06-23 01:20:45.000000 mpcontribs-client-5.4.0/requirements/macos-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-06-23 01:20:45.000000 mpcontribs-client-5.4.0/requirements/macos-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-06-23 01:20:45.000000 mpcontribs-client-5.4.0/requirements/macos-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-06-23 01:20:45.000000 mpcontribs-client-5.4.0/requirements/macos-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-06-23 01:20:45.000000 mpcontribs-client-5.4.0/requirements/macos-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-06-23 01:20:45.000000 mpcontribs-client-5.4.0/requirements/macos-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-06-23 01:20:45.000000 mpcontribs-client-5.4.0/requirements/ubuntu-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-06-23 01:20:45.000000 mpcontribs-client-5.4.0/requirements/ubuntu-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-06-23 01:20:45.000000 mpcontribs-client-5.4.0/requirements/ubuntu-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-06-23 01:20:45.000000 mpcontribs-client-5.4.0/requirements/ubuntu-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-06-23 01:20:45.000000 mpcontribs-client-5.4.0/requirements/ubuntu-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-06-23 01:20:45.000000 mpcontribs-client-5.4.0/requirements/ubuntu-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 01:21:03.388965 mpcontribs-client-5.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-23 01:20:45.000000 mpcontribs-client-5.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 01:21:03.388965 mpcontribs-client-5.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-23 01:20:45.000000 mpcontribs-client-5.4.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-06-23 01:20:45.000000 mpcontribs-client-5.4.0/tests/test_client.py
```

### Comparing `mpcontribs-client-5.3.5/LICENSE` & `mpcontribs-client-5.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.3.5/PKG-INFO` & `mpcontribs-client-5.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpcontribs-client
-Version: 5.3.5
+Version: 5.4.0
 Summary: client library for MPContribs API
 Home-page: https://github.com/materialsproject/MPContribs/tree/master/mpcontribs-client
 Author: Patrick Huck
 Author-email: phuck@lbl.gov
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `mpcontribs-client-5.3.5/README.md` & `mpcontribs-client-5.4.0/README.md`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.3.5/mpcontribs/client/__init__.py` & `mpcontribs-client-5.4.0/mpcontribs/client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -442,14 +442,45 @@
         return cls(
             name=filename,
             mime="application/gzip",
             content=b64encode(content).decode("utf-8")
         )
 
     @classmethod
+    def from_textfile(cls, path: Union[Path, str]):
+        """Construct attachment from (uncompressed) text file
+
+        Args:
+            path (pathlib.Path, str): file path
+        """
+        try:
+            path = Path(path)
+        except TypeError:
+            typ = type(path)
+            raise MPContribsClientError(f"use pathlib.Path or str (is: {typ}).")
+
+        content = path.read_bytes()
+
+        try:
+            content = gzip.compress(content)
+        except Exception:
+            raise MPContribsClientError(f"Failed to gzip {path}.")
+
+        size = len(content)
+
+        if size > MAX_BYTES:
+            raise MPContribsClientError(f"{path} too large ({size} > {MAX_BYTES})!")
+
+        return cls(
+            name=path.name,
+            mime="application/gzip",
+            content=b64encode(content).decode("utf-8")
+        )
+
+    @classmethod
     def from_dict(cls, dct: dict):
         """Construct Attachment from dict
 
         Args:
             dct (dict): dictionary format of attachment
         """
         keys = {"id", "name", "md5", "content", "mime"}
```

### Comparing `mpcontribs-client-5.3.5/mpcontribs_client.egg-info/PKG-INFO` & `mpcontribs-client-5.4.0/mpcontribs_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpcontribs-client
-Version: 5.3.5
+Version: 5.4.0
 Summary: client library for MPContribs API
 Home-page: https://github.com/materialsproject/MPContribs/tree/master/mpcontribs-client
 Author: Patrick Huck
 Author-email: phuck@lbl.gov
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `mpcontribs-client-5.3.5/mpcontribs_client.egg-info/SOURCES.txt` & `mpcontribs-client-5.4.0/mpcontribs_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.3.5/requirements/deployment.txt` & `mpcontribs-client-5.4.0/requirements/deployment.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,51 +18,51 @@
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
 bravado-core==5.17.1
     # via bravado
 certifi==2023.5.7
     # via requests
 charset-normalizer==3.1.0
     # via requests
-contourpy==1.0.7
+contourpy==1.1.0
     # via matplotlib
 cycler==0.11.0
     # via matplotlib
 decorator==5.1.1
     # via ipython
 dnspython==2.3.0
     # via
     #   pyisemail
     #   pymongo
-emmet-core==0.55.2
+emmet-core==0.57.2
     # via mp-api
 executing==1.2.0
     # via stack-data
 filetype==1.2.0
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
 flatten-dict==0.4.2
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
-fonttools==4.39.4
+fonttools==4.40.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
     #   jsonschema
     #   requests
-ipython==8.13.2
+ipython==8.14.0
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
 isoduration==20.11.0
     # via jsonschema
 jedi==0.18.2
     # via ipython
 json2html==1.3.0
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
-jsonpointer==2.3
+jsonpointer==2.4
     # via jsonschema
 jsonref==1.1.0
     # via bravado-core
 jsonschema[format]==4.17.3
     # via
     #   bravado-core
     #   swagger-spec-validator
@@ -105,57 +105,57 @@
     #   spglib
 packaging==23.1
     # via
     #   matplotlib
     #   plotly
 palettable==3.3.3
     # via pymatgen
-pandas==2.0.1
+pandas==2.0.2
     # via
     #   -r python/requirements.txt
     #   mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
 pillow==9.5.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
-plotly==5.14.1
+plotly==5.15.0
     # via
     #   mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
     #   pymatgen
 prompt-toolkit==3.0.38
     # via ipython
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
-pydantic==1.10.7
+pydantic==1.10.9
     # via emmet-core
 pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
-pymatgen==2023.5.10
+pymatgen==2023.5.31
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
-pymongo==4.3.3
+pymongo==4.4.0
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
-pyparsing==3.0.9
+pyparsing==3.1.0
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
 python-dateutil==2.8.2
     # via
     #   arrow
     #   bravado
@@ -175,21 +175,21 @@
 requests==2.31.0
     # via
     #   bravado
     #   bravado-core
     #   mp-api
     #   pymatgen
     #   requests-futures
-requests-futures==1.0.0
+requests-futures==1.0.1
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
 rfc3339-validator==0.1.4
     # via jsonschema
 rfc3987==1.3.8
     # via jsonschema
-ruamel-yaml==0.17.26
+ruamel-yaml==0.17.32
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 scipy==1.10.1
     # via
     #   -r python/requirements.txt
     #   pymatgen
@@ -229,30 +229,30 @@
     # via
     #   mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.6.0
+typing-extensions==4.6.3
     # via
     #   bravado
     #   emmet-core
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
 tzdata==2023.3
     # via pandas
-ujson==5.7.0
+ujson==5.8.0
     # via mpcontribs-client (MPContribs/mpcontribs-client/setup.py)
 uncertainties==3.1.7
     # via pymatgen
-uri-template==1.2.0
+uri-template==1.3.0
     # via jsonschema
-urllib3==2.0.2
+urllib3==2.0.3
     # via requests
 wcwidth==0.2.6
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
 
 # The following packages are considered to be unsafe in a requirements file:
```

### Comparing `mpcontribs-client-5.3.5/requirements/macos-latest_py3.10.txt` & `mpcontribs-client-5.4.0/requirements/macos-latest_py3.8.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --output-file=requirements/macos-latest_py3.10.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/macos-latest_py3.8.txt --resolver=backtracking
 #
 appnope==0.1.3
     # via ipython
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
@@ -20,51 +20,55 @@
     # via mpcontribs-client (setup.py)
 bravado-core==5.17.1
     # via bravado
 certifi==2023.5.7
     # via requests
 charset-normalizer==3.1.0
     # via requests
-contourpy==1.0.7
+contourpy==1.1.0
     # via matplotlib
 cycler==0.11.0
     # via matplotlib
 decorator==5.1.1
     # via ipython
 dnspython==2.3.0
     # via
     #   pyisemail
     #   pymongo
-emmet-core==0.55.2
+emmet-core==0.57.2
     # via mp-api
 executing==1.2.0
     # via stack-data
 filetype==1.2.0
     # via mpcontribs-client (setup.py)
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
-fonttools==4.39.4
+fonttools==4.40.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
     #   jsonschema
     #   requests
-ipython==8.13.2
+importlib-resources==5.12.0
+    # via
+    #   jsonschema
+    #   matplotlib
+ipython==8.12.2
     # via mpcontribs-client (setup.py)
 isoduration==20.11.0
     # via jsonschema
 jedi==0.18.2
     # via ipython
 json2html==1.3.0
     # via mpcontribs-client (setup.py)
-jsonpointer==2.3
+jsonpointer==2.4
     # via jsonschema
 jsonref==1.1.0
     # via bravado-core
 jsonschema[format]==4.17.3
     # via
     #   bravado-core
     #   swagger-spec-validator
@@ -104,56 +108,58 @@
     #   spglib
 packaging==23.1
     # via
     #   matplotlib
     #   plotly
 palettable==3.3.3
     # via pymatgen
-pandas==2.0.1
+pandas==2.0.2
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
 pillow==9.5.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
-plotly==5.14.1
+pkgutil-resolve-name==1.3.10
+    # via jsonschema
+plotly==5.15.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 prompt-toolkit==3.0.38
     # via ipython
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
-pydantic==1.10.7
+pydantic==1.10.9
     # via emmet-core
 pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
-pymatgen==2023.5.10
+pymatgen==2023.5.31
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (setup.py)
-pymongo==4.3.3
+pymongo==4.4.0
     # via mpcontribs-client (setup.py)
-pyparsing==3.0.9
+pyparsing==3.1.0
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
 python-dateutil==2.8.2
     # via
     #   arrow
     #   bravado
@@ -173,21 +179,21 @@
 requests==2.31.0
     # via
     #   bravado
     #   bravado-core
     #   mp-api
     #   pymatgen
     #   requests-futures
-requests-futures==1.0.0
+requests-futures==1.0.1
     # via mpcontribs-client (setup.py)
 rfc3339-validator==0.1.4
     # via jsonschema
 rfc3987==1.3.8
     # via jsonschema
-ruamel-yaml==0.17.26
+ruamel-yaml==0.17.32
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 scipy==1.10.1
     # via pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (setup.py)
@@ -225,31 +231,34 @@
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.6.0
+typing-extensions==4.6.3
     # via
     #   bravado
     #   emmet-core
+    #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
 tzdata==2023.3
     # via pandas
-ujson==5.7.0
+ujson==5.8.0
     # via mpcontribs-client (setup.py)
 uncertainties==3.1.7
     # via pymatgen
-uri-template==1.2.0
+uri-template==1.3.0
     # via jsonschema
-urllib3==2.0.2
+urllib3==2.0.3
     # via requests
 wcwidth==0.2.6
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
+zipp==3.15.0
+    # via importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `mpcontribs-client-5.3.5/requirements/macos-latest_py3.10_extras.txt` & `mpcontribs-client-5.4.0/requirements/ubuntu-latest_py3.10_extras.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.10_extras.txt --resolver=backtracking
+#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.10_extras.txt --resolver=backtracking
 #
-appnope==0.1.3
-    # via ipython
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
 attrs==23.1.0
     # via jsonschema
 backcall==0.2.0
@@ -20,61 +18,61 @@
     # via mpcontribs-client (setup.py)
 bravado-core==5.17.1
     # via bravado
 certifi==2023.5.7
     # via requests
 charset-normalizer==3.1.0
     # via requests
-contourpy==1.0.7
+contourpy==1.1.0
     # via matplotlib
-coverage[toml]==7.2.5
+coverage[toml]==7.2.7
     # via pytest-cov
 cycler==0.11.0
     # via matplotlib
 decorator==5.1.1
     # via ipython
 dnspython==2.3.0
     # via
     #   pyisemail
     #   pymongo
-emmet-core==0.55.2
+emmet-core==0.57.2
     # via mp-api
 exceptiongroup==1.1.1
     # via pytest
 executing==1.2.0
     # via stack-data
 filetype==1.2.0
     # via mpcontribs-client (setup.py)
 flake8==6.0.0
     # via
     #   mpcontribs-client (setup.py)
     #   pytest-flake8
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
-fonttools==4.39.4
+fonttools==4.40.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
     #   jsonschema
     #   requests
 iniconfig==2.0.0
     # via pytest
-ipython==8.13.2
+ipython==8.14.0
     # via mpcontribs-client (setup.py)
 isoduration==20.11.0
     # via jsonschema
 jedi==0.18.2
     # via ipython
 json2html==1.3.0
     # via mpcontribs-client (setup.py)
-jsonpointer==2.3
+jsonpointer==2.4
     # via jsonschema
 jsonref==1.1.0
     # via bravado-core
 jsonschema[format]==4.17.3
     # via
     #   bravado-core
     #   swagger-spec-validator
@@ -102,48 +100,48 @@
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
 networkx==3.1
     # via pymatgen
-numpy==1.24.3
+numpy==1.25.0
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
 packaging==23.1
     # via
     #   matplotlib
     #   plotly
     #   pytest
 palettable==3.3.3
     # via pymatgen
-pandas==2.0.1
+pandas==2.0.2
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
 pillow==9.5.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
-plotly==5.14.1
+plotly==5.15.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
-pluggy==1.0.0
+pluggy==1.2.0
     # via pytest
 prompt-toolkit==3.0.38
     # via ipython
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
@@ -155,40 +153,40 @@
     # via
     #   emmet-core
     #   pymatgen
 pycodestyle==2.10.0
     # via
     #   flake8
     #   pytest-pycodestyle
-pydantic==1.10.7
+pydantic==1.10.9
     # via emmet-core
 pyflakes==3.0.1
     # via flake8
 pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
-pymatgen==2023.5.10
+pymatgen==2023.5.31
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (setup.py)
-pymongo==4.3.3
+pymongo==4.4.0
     # via mpcontribs-client (setup.py)
-pyparsing==3.0.9
+pyparsing==3.1.0
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
-pytest==7.3.1
+pytest==7.3.2
     # via
     #   mpcontribs-client (setup.py)
     #   pytest-cov
     #   pytest-flake8
     #   pytest-pycodestyle
-pytest-cov==4.0.0
+pytest-cov==4.1.0
     # via mpcontribs-client (setup.py)
 pytest-flake8==1.1.1
     # via mpcontribs-client (setup.py)
 pytest-pycodestyle==2.3.1
     # via mpcontribs-client (setup.py)
 python-dateutil==2.8.2
     # via
@@ -210,21 +208,21 @@
 requests==2.31.0
     # via
     #   bravado
     #   bravado-core
     #   mp-api
     #   pymatgen
     #   requests-futures
-requests-futures==1.0.0
+requests-futures==1.0.1
     # via mpcontribs-client (setup.py)
 rfc3339-validator==0.1.4
     # via jsonschema
 rfc3987==1.3.8
     # via jsonschema
-ruamel-yaml==0.17.26
+ruamel-yaml==0.17.32
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 scipy==1.10.1
     # via pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (setup.py)
@@ -266,30 +264,30 @@
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.6.0
+typing-extensions==4.6.3
     # via
     #   bravado
     #   emmet-core
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
 tzdata==2023.3
     # via pandas
-ujson==5.7.0
+ujson==5.8.0
     # via mpcontribs-client (setup.py)
 uncertainties==3.1.7
     # via pymatgen
-uri-template==1.2.0
+uri-template==1.3.0
     # via jsonschema
-urllib3==2.0.2
+urllib3==2.0.3
     # via requests
 wcwidth==0.2.6
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
 
 # The following packages are considered to be unsafe in a requirements file:
```

### Comparing `mpcontribs-client-5.3.5/requirements/macos-latest_py3.8.txt` & `mpcontribs-client-5.4.0/requirements/ubuntu-latest_py3.8.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 #
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --output-file=requirements/macos-latest_py3.8.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/ubuntu-latest_py3.8.txt --resolver=backtracking
 #
-appnope==0.1.3
-    # via ipython
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
 attrs==23.1.0
     # via jsonschema
 backcall==0.2.0
@@ -20,33 +18,33 @@
     # via mpcontribs-client (setup.py)
 bravado-core==5.17.1
     # via bravado
 certifi==2023.5.7
     # via requests
 charset-normalizer==3.1.0
     # via requests
-contourpy==1.0.7
+contourpy==1.1.0
     # via matplotlib
 cycler==0.11.0
     # via matplotlib
 decorator==5.1.1
     # via ipython
 dnspython==2.3.0
     # via
     #   pyisemail
     #   pymongo
-emmet-core==0.55.2
+emmet-core==0.57.2
     # via mp-api
 executing==1.2.0
     # via stack-data
 filetype==1.2.0
     # via mpcontribs-client (setup.py)
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
-fonttools==4.39.4
+fonttools==4.40.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
@@ -60,15 +58,15 @@
     # via mpcontribs-client (setup.py)
 isoduration==20.11.0
     # via jsonschema
 jedi==0.18.2
     # via ipython
 json2html==1.3.0
     # via mpcontribs-client (setup.py)
-jsonpointer==2.3
+jsonpointer==2.4
     # via jsonschema
 jsonref==1.1.0
     # via bravado-core
 jsonschema[format]==4.17.3
     # via
     #   bravado-core
     #   swagger-spec-validator
@@ -108,15 +106,15 @@
     #   spglib
 packaging==23.1
     # via
     #   matplotlib
     #   plotly
 palettable==3.3.3
     # via pymatgen
-pandas==2.0.1
+pandas==2.0.2
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
@@ -124,42 +122,42 @@
     # via ipython
 pillow==9.5.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
 pkgutil-resolve-name==1.3.10
     # via jsonschema
-plotly==5.14.1
+plotly==5.15.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 prompt-toolkit==3.0.38
     # via ipython
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
-pydantic==1.10.7
+pydantic==1.10.9
     # via emmet-core
 pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
-pymatgen==2023.5.10
+pymatgen==2023.5.31
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (setup.py)
-pymongo==4.3.3
+pymongo==4.4.0
     # via mpcontribs-client (setup.py)
-pyparsing==3.0.9
+pyparsing==3.1.0
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
 python-dateutil==2.8.2
     # via
     #   arrow
     #   bravado
@@ -179,21 +177,21 @@
 requests==2.31.0
     # via
     #   bravado
     #   bravado-core
     #   mp-api
     #   pymatgen
     #   requests-futures
-requests-futures==1.0.0
+requests-futures==1.0.1
     # via mpcontribs-client (setup.py)
 rfc3339-validator==0.1.4
     # via jsonschema
 rfc3987==1.3.8
     # via jsonschema
-ruamel-yaml==0.17.26
+ruamel-yaml==0.17.32
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 scipy==1.10.1
     # via pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (setup.py)
@@ -231,31 +229,31 @@
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.6.0
+typing-extensions==4.6.3
     # via
     #   bravado
     #   emmet-core
     #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
 tzdata==2023.3
     # via pandas
-ujson==5.7.0
+ujson==5.8.0
     # via mpcontribs-client (setup.py)
 uncertainties==3.1.7
     # via pymatgen
-uri-template==1.2.0
+uri-template==1.3.0
     # via jsonschema
-urllib3==2.0.2
+urllib3==2.0.3
     # via requests
 wcwidth==0.2.6
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
 zipp==3.15.0
     # via importlib-resources
```

### Comparing `mpcontribs-client-5.3.5/requirements/macos-latest_py3.8_extras.txt` & `mpcontribs-client-5.4.0/requirements/ubuntu-latest_py3.8_extras.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 #
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.8_extras.txt --resolver=backtracking
+#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.8_extras.txt --resolver=backtracking
 #
-appnope==0.1.3
-    # via ipython
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
 attrs==23.1.0
     # via jsonschema
 backcall==0.2.0
@@ -20,41 +18,41 @@
     # via mpcontribs-client (setup.py)
 bravado-core==5.17.1
     # via bravado
 certifi==2023.5.7
     # via requests
 charset-normalizer==3.1.0
     # via requests
-contourpy==1.0.7
+contourpy==1.1.0
     # via matplotlib
-coverage[toml]==7.2.5
+coverage[toml]==7.2.7
     # via pytest-cov
 cycler==0.11.0
     # via matplotlib
 decorator==5.1.1
     # via ipython
 dnspython==2.3.0
     # via
     #   pyisemail
     #   pymongo
-emmet-core==0.55.2
+emmet-core==0.57.2
     # via mp-api
 exceptiongroup==1.1.1
     # via pytest
 executing==1.2.0
     # via stack-data
 filetype==1.2.0
     # via mpcontribs-client (setup.py)
 flake8==6.0.0
     # via
     #   mpcontribs-client (setup.py)
     #   pytest-flake8
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
-fonttools==4.39.4
+fonttools==4.40.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
@@ -70,15 +68,15 @@
     # via mpcontribs-client (setup.py)
 isoduration==20.11.0
     # via jsonschema
 jedi==0.18.2
     # via ipython
 json2html==1.3.0
     # via mpcontribs-client (setup.py)
-jsonpointer==2.3
+jsonpointer==2.4
     # via jsonschema
 jsonref==1.1.0
     # via bravado-core
 jsonschema[format]==4.17.3
     # via
     #   bravado-core
     #   swagger-spec-validator
@@ -121,15 +119,15 @@
 packaging==23.1
     # via
     #   matplotlib
     #   plotly
     #   pytest
 palettable==3.3.3
     # via pymatgen
-pandas==2.0.1
+pandas==2.0.2
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
@@ -137,19 +135,19 @@
     # via ipython
 pillow==9.5.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
 pkgutil-resolve-name==1.3.10
     # via jsonschema
-plotly==5.14.1
+plotly==5.15.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
-pluggy==1.0.0
+pluggy==1.2.0
     # via pytest
 prompt-toolkit==3.0.38
     # via ipython
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
@@ -161,40 +159,40 @@
     # via
     #   emmet-core
     #   pymatgen
 pycodestyle==2.10.0
     # via
     #   flake8
     #   pytest-pycodestyle
-pydantic==1.10.7
+pydantic==1.10.9
     # via emmet-core
 pyflakes==3.0.1
     # via flake8
 pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
-pymatgen==2023.5.10
+pymatgen==2023.5.31
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (setup.py)
-pymongo==4.3.3
+pymongo==4.4.0
     # via mpcontribs-client (setup.py)
-pyparsing==3.0.9
+pyparsing==3.1.0
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
-pytest==7.3.1
+pytest==7.3.2
     # via
     #   mpcontribs-client (setup.py)
     #   pytest-cov
     #   pytest-flake8
     #   pytest-pycodestyle
-pytest-cov==4.0.0
+pytest-cov==4.1.0
     # via mpcontribs-client (setup.py)
 pytest-flake8==1.1.1
     # via mpcontribs-client (setup.py)
 pytest-pycodestyle==2.3.1
     # via mpcontribs-client (setup.py)
 python-dateutil==2.8.2
     # via
@@ -216,21 +214,21 @@
 requests==2.31.0
     # via
     #   bravado
     #   bravado-core
     #   mp-api
     #   pymatgen
     #   requests-futures
-requests-futures==1.0.0
+requests-futures==1.0.1
     # via mpcontribs-client (setup.py)
 rfc3339-validator==0.1.4
     # via jsonschema
 rfc3987==1.3.8
     # via jsonschema
-ruamel-yaml==0.17.26
+ruamel-yaml==0.17.32
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 scipy==1.10.1
     # via pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (setup.py)
@@ -272,31 +270,31 @@
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.6.0
+typing-extensions==4.6.3
     # via
     #   bravado
     #   emmet-core
     #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
 tzdata==2023.3
     # via pandas
-ujson==5.7.0
+ujson==5.8.0
     # via mpcontribs-client (setup.py)
 uncertainties==3.1.7
     # via pymatgen
-uri-template==1.2.0
+uri-template==1.3.0
     # via jsonschema
-urllib3==2.0.2
+urllib3==2.0.3
     # via requests
 wcwidth==0.2.6
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
 zipp==3.15.0
     # via importlib-resources
```

### Comparing `mpcontribs-client-5.3.5/requirements/macos-latest_py3.9.txt` & `mpcontribs-client-5.4.0/requirements/macos-latest_py3.9.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,53 +20,53 @@
     # via mpcontribs-client (setup.py)
 bravado-core==5.17.1
     # via bravado
 certifi==2023.5.7
     # via requests
 charset-normalizer==3.1.0
     # via requests
-contourpy==1.0.7
+contourpy==1.1.0
     # via matplotlib
 cycler==0.11.0
     # via matplotlib
 decorator==5.1.1
     # via ipython
 dnspython==2.3.0
     # via
     #   pyisemail
     #   pymongo
-emmet-core==0.55.2
+emmet-core==0.57.2
     # via mp-api
 executing==1.2.0
     # via stack-data
 filetype==1.2.0
     # via mpcontribs-client (setup.py)
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
-fonttools==4.39.4
+fonttools==4.40.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
     #   jsonschema
     #   requests
 importlib-resources==5.12.0
     # via matplotlib
-ipython==8.13.2
+ipython==8.14.0
     # via mpcontribs-client (setup.py)
 isoduration==20.11.0
     # via jsonschema
 jedi==0.18.2
     # via ipython
 json2html==1.3.0
     # via mpcontribs-client (setup.py)
-jsonpointer==2.3
+jsonpointer==2.4
     # via jsonschema
 jsonref==1.1.0
     # via bravado-core
 jsonschema[format]==4.17.3
     # via
     #   bravado-core
     #   swagger-spec-validator
@@ -92,70 +92,70 @@
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
 networkx==3.1
     # via pymatgen
-numpy==1.24.3
+numpy==1.25.0
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
 packaging==23.1
     # via
     #   matplotlib
     #   plotly
 palettable==3.3.3
     # via pymatgen
-pandas==2.0.1
+pandas==2.0.2
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
 pillow==9.5.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
-plotly==5.14.1
+plotly==5.15.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 prompt-toolkit==3.0.38
     # via ipython
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
-pydantic==1.10.7
+pydantic==1.10.9
     # via emmet-core
 pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
-pymatgen==2023.5.10
+pymatgen==2023.5.31
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (setup.py)
-pymongo==4.3.3
+pymongo==4.4.0
     # via mpcontribs-client (setup.py)
-pyparsing==3.0.9
+pyparsing==3.1.0
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
 python-dateutil==2.8.2
     # via
     #   arrow
     #   bravado
@@ -175,21 +175,21 @@
 requests==2.31.0
     # via
     #   bravado
     #   bravado-core
     #   mp-api
     #   pymatgen
     #   requests-futures
-requests-futures==1.0.0
+requests-futures==1.0.1
     # via mpcontribs-client (setup.py)
 rfc3339-validator==0.1.4
     # via jsonschema
 rfc3987==1.3.8
     # via jsonschema
-ruamel-yaml==0.17.26
+ruamel-yaml==0.17.32
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 scipy==1.10.1
     # via pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (setup.py)
@@ -227,31 +227,31 @@
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.6.0
+typing-extensions==4.6.3
     # via
     #   bravado
     #   emmet-core
     #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
 tzdata==2023.3
     # via pandas
-ujson==5.7.0
+ujson==5.8.0
     # via mpcontribs-client (setup.py)
 uncertainties==3.1.7
     # via pymatgen
-uri-template==1.2.0
+uri-template==1.3.0
     # via jsonschema
-urllib3==2.0.2
+urllib3==2.0.3
     # via requests
 wcwidth==0.2.6
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
 zipp==3.15.0
     # via importlib-resources
```

### Comparing `mpcontribs-client-5.3.5/requirements/macos-latest_py3.9_extras.txt` & `mpcontribs-client-5.4.0/requirements/macos-latest_py3.8_extras.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.9_extras.txt --resolver=backtracking
+#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.8_extras.txt --resolver=backtracking
 #
 appnope==0.1.3
     # via ipython
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
@@ -20,63 +20,65 @@
     # via mpcontribs-client (setup.py)
 bravado-core==5.17.1
     # via bravado
 certifi==2023.5.7
     # via requests
 charset-normalizer==3.1.0
     # via requests
-contourpy==1.0.7
+contourpy==1.1.0
     # via matplotlib
-coverage[toml]==7.2.5
+coverage[toml]==7.2.7
     # via pytest-cov
 cycler==0.11.0
     # via matplotlib
 decorator==5.1.1
     # via ipython
 dnspython==2.3.0
     # via
     #   pyisemail
     #   pymongo
-emmet-core==0.55.2
+emmet-core==0.57.2
     # via mp-api
 exceptiongroup==1.1.1
     # via pytest
 executing==1.2.0
     # via stack-data
 filetype==1.2.0
     # via mpcontribs-client (setup.py)
 flake8==6.0.0
     # via
     #   mpcontribs-client (setup.py)
     #   pytest-flake8
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
-fonttools==4.39.4
+fonttools==4.40.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
     #   jsonschema
     #   requests
 importlib-resources==5.12.0
-    # via matplotlib
+    # via
+    #   jsonschema
+    #   matplotlib
 iniconfig==2.0.0
     # via pytest
-ipython==8.13.2
+ipython==8.12.2
     # via mpcontribs-client (setup.py)
 isoduration==20.11.0
     # via jsonschema
 jedi==0.18.2
     # via ipython
 json2html==1.3.0
     # via mpcontribs-client (setup.py)
-jsonpointer==2.3
+jsonpointer==2.4
     # via jsonschema
 jsonref==1.1.0
     # via bravado-core
 jsonschema[format]==4.17.3
     # via
     #   bravado-core
     #   swagger-spec-validator
@@ -119,33 +121,35 @@
 packaging==23.1
     # via
     #   matplotlib
     #   plotly
     #   pytest
 palettable==3.3.3
     # via pymatgen
-pandas==2.0.1
+pandas==2.0.2
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
 pillow==9.5.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
-plotly==5.14.1
+pkgutil-resolve-name==1.3.10
+    # via jsonschema
+plotly==5.15.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
-pluggy==1.0.0
+pluggy==1.2.0
     # via pytest
 prompt-toolkit==3.0.38
     # via ipython
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
@@ -157,40 +161,40 @@
     # via
     #   emmet-core
     #   pymatgen
 pycodestyle==2.10.0
     # via
     #   flake8
     #   pytest-pycodestyle
-pydantic==1.10.7
+pydantic==1.10.9
     # via emmet-core
 pyflakes==3.0.1
     # via flake8
 pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
-pymatgen==2023.5.10
+pymatgen==2023.5.31
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (setup.py)
-pymongo==4.3.3
+pymongo==4.4.0
     # via mpcontribs-client (setup.py)
-pyparsing==3.0.9
+pyparsing==3.1.0
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
-pytest==7.3.1
+pytest==7.3.2
     # via
     #   mpcontribs-client (setup.py)
     #   pytest-cov
     #   pytest-flake8
     #   pytest-pycodestyle
-pytest-cov==4.0.0
+pytest-cov==4.1.0
     # via mpcontribs-client (setup.py)
 pytest-flake8==1.1.1
     # via mpcontribs-client (setup.py)
 pytest-pycodestyle==2.3.1
     # via mpcontribs-client (setup.py)
 python-dateutil==2.8.2
     # via
@@ -212,21 +216,21 @@
 requests==2.31.0
     # via
     #   bravado
     #   bravado-core
     #   mp-api
     #   pymatgen
     #   requests-futures
-requests-futures==1.0.0
+requests-futures==1.0.1
     # via mpcontribs-client (setup.py)
 rfc3339-validator==0.1.4
     # via jsonschema
 rfc3987==1.3.8
     # via jsonschema
-ruamel-yaml==0.17.26
+ruamel-yaml==0.17.32
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 scipy==1.10.1
     # via pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (setup.py)
@@ -268,31 +272,31 @@
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.6.0
+typing-extensions==4.6.3
     # via
     #   bravado
     #   emmet-core
     #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
 tzdata==2023.3
     # via pandas
-ujson==5.7.0
+ujson==5.8.0
     # via mpcontribs-client (setup.py)
 uncertainties==3.1.7
     # via pymatgen
-uri-template==1.2.0
+uri-template==1.3.0
     # via jsonschema
-urllib3==2.0.2
+urllib3==2.0.3
     # via requests
 wcwidth==0.2.6
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
 zipp==3.15.0
     # via importlib-resources
```

### Comparing `mpcontribs-client-5.3.5/requirements/ubuntu-latest_py3.10.txt` & `mpcontribs-client-5.4.0/requirements/ubuntu-latest_py3.10.txt`

 * *Files 3% similar despite different names*

```diff
@@ -18,51 +18,51 @@
     # via mpcontribs-client (setup.py)
 bravado-core==5.17.1
     # via bravado
 certifi==2023.5.7
     # via requests
 charset-normalizer==3.1.0
     # via requests
-contourpy==1.0.7
+contourpy==1.1.0
     # via matplotlib
 cycler==0.11.0
     # via matplotlib
 decorator==5.1.1
     # via ipython
 dnspython==2.3.0
     # via
     #   pyisemail
     #   pymongo
-emmet-core==0.55.2
+emmet-core==0.57.2
     # via mp-api
 executing==1.2.0
     # via stack-data
 filetype==1.2.0
     # via mpcontribs-client (setup.py)
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
-fonttools==4.39.4
+fonttools==4.40.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
     #   jsonschema
     #   requests
-ipython==8.13.2
+ipython==8.14.0
     # via mpcontribs-client (setup.py)
 isoduration==20.11.0
     # via jsonschema
 jedi==0.18.2
     # via ipython
 json2html==1.3.0
     # via mpcontribs-client (setup.py)
-jsonpointer==2.3
+jsonpointer==2.4
     # via jsonschema
 jsonref==1.1.0
     # via bravado-core
 jsonschema[format]==4.17.3
     # via
     #   bravado-core
     #   swagger-spec-validator
@@ -88,70 +88,70 @@
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
 networkx==3.1
     # via pymatgen
-numpy==1.24.3
+numpy==1.25.0
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
 packaging==23.1
     # via
     #   matplotlib
     #   plotly
 palettable==3.3.3
     # via pymatgen
-pandas==2.0.1
+pandas==2.0.2
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
 pillow==9.5.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
-plotly==5.14.1
+plotly==5.15.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 prompt-toolkit==3.0.38
     # via ipython
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
-pydantic==1.10.7
+pydantic==1.10.9
     # via emmet-core
 pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
-pymatgen==2023.5.10
+pymatgen==2023.5.31
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (setup.py)
-pymongo==4.3.3
+pymongo==4.4.0
     # via mpcontribs-client (setup.py)
-pyparsing==3.0.9
+pyparsing==3.1.0
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
 python-dateutil==2.8.2
     # via
     #   arrow
     #   bravado
@@ -171,21 +171,21 @@
 requests==2.31.0
     # via
     #   bravado
     #   bravado-core
     #   mp-api
     #   pymatgen
     #   requests-futures
-requests-futures==1.0.0
+requests-futures==1.0.1
     # via mpcontribs-client (setup.py)
 rfc3339-validator==0.1.4
     # via jsonschema
 rfc3987==1.3.8
     # via jsonschema
-ruamel-yaml==0.17.26
+ruamel-yaml==0.17.32
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 scipy==1.10.1
     # via pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (setup.py)
@@ -223,30 +223,30 @@
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.6.0
+typing-extensions==4.6.3
     # via
     #   bravado
     #   emmet-core
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
 tzdata==2023.3
     # via pandas
-ujson==5.7.0
+ujson==5.8.0
     # via mpcontribs-client (setup.py)
 uncertainties==3.1.7
     # via pymatgen
-uri-template==1.2.0
+uri-template==1.3.0
     # via jsonschema
-urllib3==2.0.2
+urllib3==2.0.3
     # via requests
 wcwidth==0.2.6
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
 
 # The following packages are considered to be unsafe in a requirements file:
```

### Comparing `mpcontribs-client-5.3.5/requirements/ubuntu-latest_py3.10_extras.txt` & `mpcontribs-client-5.4.0/requirements/macos-latest_py3.10_extras.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.10_extras.txt --resolver=backtracking
+#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.10_extras.txt --resolver=backtracking
 #
+appnope==0.1.3
+    # via ipython
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
 attrs==23.1.0
     # via jsonschema
 backcall==0.2.0
@@ -18,61 +20,61 @@
     # via mpcontribs-client (setup.py)
 bravado-core==5.17.1
     # via bravado
 certifi==2023.5.7
     # via requests
 charset-normalizer==3.1.0
     # via requests
-contourpy==1.0.7
+contourpy==1.1.0
     # via matplotlib
-coverage[toml]==7.2.5
+coverage[toml]==7.2.7
     # via pytest-cov
 cycler==0.11.0
     # via matplotlib
 decorator==5.1.1
     # via ipython
 dnspython==2.3.0
     # via
     #   pyisemail
     #   pymongo
-emmet-core==0.55.2
+emmet-core==0.57.2
     # via mp-api
 exceptiongroup==1.1.1
     # via pytest
 executing==1.2.0
     # via stack-data
 filetype==1.2.0
     # via mpcontribs-client (setup.py)
 flake8==6.0.0
     # via
     #   mpcontribs-client (setup.py)
     #   pytest-flake8
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
-fonttools==4.39.4
+fonttools==4.40.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
     #   jsonschema
     #   requests
 iniconfig==2.0.0
     # via pytest
-ipython==8.13.2
+ipython==8.14.0
     # via mpcontribs-client (setup.py)
 isoduration==20.11.0
     # via jsonschema
 jedi==0.18.2
     # via ipython
 json2html==1.3.0
     # via mpcontribs-client (setup.py)
-jsonpointer==2.3
+jsonpointer==2.4
     # via jsonschema
 jsonref==1.1.0
     # via bravado-core
 jsonschema[format]==4.17.3
     # via
     #   bravado-core
     #   swagger-spec-validator
@@ -100,48 +102,48 @@
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
 networkx==3.1
     # via pymatgen
-numpy==1.24.3
+numpy==1.25.0
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
 packaging==23.1
     # via
     #   matplotlib
     #   plotly
     #   pytest
 palettable==3.3.3
     # via pymatgen
-pandas==2.0.1
+pandas==2.0.2
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
 pillow==9.5.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
-plotly==5.14.1
+plotly==5.15.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
-pluggy==1.0.0
+pluggy==1.2.0
     # via pytest
 prompt-toolkit==3.0.38
     # via ipython
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
@@ -153,40 +155,40 @@
     # via
     #   emmet-core
     #   pymatgen
 pycodestyle==2.10.0
     # via
     #   flake8
     #   pytest-pycodestyle
-pydantic==1.10.7
+pydantic==1.10.9
     # via emmet-core
 pyflakes==3.0.1
     # via flake8
 pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
-pymatgen==2023.5.10
+pymatgen==2023.5.31
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (setup.py)
-pymongo==4.3.3
+pymongo==4.4.0
     # via mpcontribs-client (setup.py)
-pyparsing==3.0.9
+pyparsing==3.1.0
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
-pytest==7.3.1
+pytest==7.3.2
     # via
     #   mpcontribs-client (setup.py)
     #   pytest-cov
     #   pytest-flake8
     #   pytest-pycodestyle
-pytest-cov==4.0.0
+pytest-cov==4.1.0
     # via mpcontribs-client (setup.py)
 pytest-flake8==1.1.1
     # via mpcontribs-client (setup.py)
 pytest-pycodestyle==2.3.1
     # via mpcontribs-client (setup.py)
 python-dateutil==2.8.2
     # via
@@ -208,21 +210,21 @@
 requests==2.31.0
     # via
     #   bravado
     #   bravado-core
     #   mp-api
     #   pymatgen
     #   requests-futures
-requests-futures==1.0.0
+requests-futures==1.0.1
     # via mpcontribs-client (setup.py)
 rfc3339-validator==0.1.4
     # via jsonschema
 rfc3987==1.3.8
     # via jsonschema
-ruamel-yaml==0.17.26
+ruamel-yaml==0.17.32
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 scipy==1.10.1
     # via pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (setup.py)
@@ -264,30 +266,30 @@
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.6.0
+typing-extensions==4.6.3
     # via
     #   bravado
     #   emmet-core
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
 tzdata==2023.3
     # via pandas
-ujson==5.7.0
+ujson==5.8.0
     # via mpcontribs-client (setup.py)
 uncertainties==3.1.7
     # via pymatgen
-uri-template==1.2.0
+uri-template==1.3.0
     # via jsonschema
-urllib3==2.0.2
+urllib3==2.0.3
     # via requests
 wcwidth==0.2.6
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
 
 # The following packages are considered to be unsafe in a requirements file:
```

### Comparing `mpcontribs-client-5.3.5/requirements/ubuntu-latest_py3.8.txt` & `mpcontribs-client-5.4.0/requirements/macos-latest_py3.10.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --output-file=requirements/ubuntu-latest_py3.8.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/macos-latest_py3.10.txt --resolver=backtracking
 #
+appnope==0.1.3
+    # via ipython
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
 attrs==23.1.0
     # via jsonschema
 backcall==0.2.0
@@ -18,55 +20,51 @@
     # via mpcontribs-client (setup.py)
 bravado-core==5.17.1
     # via bravado
 certifi==2023.5.7
     # via requests
 charset-normalizer==3.1.0
     # via requests
-contourpy==1.0.7
+contourpy==1.1.0
     # via matplotlib
 cycler==0.11.0
     # via matplotlib
 decorator==5.1.1
     # via ipython
 dnspython==2.3.0
     # via
     #   pyisemail
     #   pymongo
-emmet-core==0.55.2
+emmet-core==0.57.2
     # via mp-api
 executing==1.2.0
     # via stack-data
 filetype==1.2.0
     # via mpcontribs-client (setup.py)
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
-fonttools==4.39.4
+fonttools==4.40.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
     #   jsonschema
     #   requests
-importlib-resources==5.12.0
-    # via
-    #   jsonschema
-    #   matplotlib
-ipython==8.12.2
+ipython==8.14.0
     # via mpcontribs-client (setup.py)
 isoduration==20.11.0
     # via jsonschema
 jedi==0.18.2
     # via ipython
 json2html==1.3.0
     # via mpcontribs-client (setup.py)
-jsonpointer==2.3
+jsonpointer==2.4
     # via jsonschema
 jsonref==1.1.0
     # via bravado-core
 jsonschema[format]==4.17.3
     # via
     #   bravado-core
     #   swagger-spec-validator
@@ -92,72 +90,70 @@
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
 networkx==3.1
     # via pymatgen
-numpy==1.24.3
+numpy==1.25.0
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
 packaging==23.1
     # via
     #   matplotlib
     #   plotly
 palettable==3.3.3
     # via pymatgen
-pandas==2.0.1
+pandas==2.0.2
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
 pillow==9.5.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
-pkgutil-resolve-name==1.3.10
-    # via jsonschema
-plotly==5.14.1
+plotly==5.15.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 prompt-toolkit==3.0.38
     # via ipython
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
-pydantic==1.10.7
+pydantic==1.10.9
     # via emmet-core
 pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
-pymatgen==2023.5.10
+pymatgen==2023.5.31
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (setup.py)
-pymongo==4.3.3
+pymongo==4.4.0
     # via mpcontribs-client (setup.py)
-pyparsing==3.0.9
+pyparsing==3.1.0
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
 python-dateutil==2.8.2
     # via
     #   arrow
     #   bravado
@@ -177,21 +173,21 @@
 requests==2.31.0
     # via
     #   bravado
     #   bravado-core
     #   mp-api
     #   pymatgen
     #   requests-futures
-requests-futures==1.0.0
+requests-futures==1.0.1
     # via mpcontribs-client (setup.py)
 rfc3339-validator==0.1.4
     # via jsonschema
 rfc3987==1.3.8
     # via jsonschema
-ruamel-yaml==0.17.26
+ruamel-yaml==0.17.32
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 scipy==1.10.1
     # via pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (setup.py)
@@ -229,34 +225,31 @@
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.6.0
+typing-extensions==4.6.3
     # via
     #   bravado
     #   emmet-core
-    #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
 tzdata==2023.3
     # via pandas
-ujson==5.7.0
+ujson==5.8.0
     # via mpcontribs-client (setup.py)
 uncertainties==3.1.7
     # via pymatgen
-uri-template==1.2.0
+uri-template==1.3.0
     # via jsonschema
-urllib3==2.0.2
+urllib3==2.0.3
     # via requests
 wcwidth==0.2.6
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
-zipp==3.15.0
-    # via importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `mpcontribs-client-5.3.5/requirements/ubuntu-latest_py3.8_extras.txt` & `mpcontribs-client-5.4.0/requirements/ubuntu-latest_py3.9.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.8_extras.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/ubuntu-latest_py3.9.txt --resolver=backtracking
 #
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
 attrs==23.1.0
     # via jsonschema
@@ -18,65 +18,53 @@
     # via mpcontribs-client (setup.py)
 bravado-core==5.17.1
     # via bravado
 certifi==2023.5.7
     # via requests
 charset-normalizer==3.1.0
     # via requests
-contourpy==1.0.7
+contourpy==1.1.0
     # via matplotlib
-coverage[toml]==7.2.5
-    # via pytest-cov
 cycler==0.11.0
     # via matplotlib
 decorator==5.1.1
     # via ipython
 dnspython==2.3.0
     # via
     #   pyisemail
     #   pymongo
-emmet-core==0.55.2
+emmet-core==0.57.2
     # via mp-api
-exceptiongroup==1.1.1
-    # via pytest
 executing==1.2.0
     # via stack-data
 filetype==1.2.0
     # via mpcontribs-client (setup.py)
-flake8==6.0.0
-    # via
-    #   mpcontribs-client (setup.py)
-    #   pytest-flake8
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
-fonttools==4.39.4
+fonttools==4.40.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
     #   jsonschema
     #   requests
 importlib-resources==5.12.0
-    # via
-    #   jsonschema
-    #   matplotlib
-iniconfig==2.0.0
-    # via pytest
-ipython==8.12.2
+    # via matplotlib
+ipython==8.14.0
     # via mpcontribs-client (setup.py)
 isoduration==20.11.0
     # via jsonschema
 jedi==0.18.2
     # via ipython
 json2html==1.3.0
     # via mpcontribs-client (setup.py)
-jsonpointer==2.3
+jsonpointer==2.4
     # via jsonschema
 jsonref==1.1.0
     # via bravado-core
 jsonschema[format]==4.17.3
     # via
     #   bravado-core
     #   swagger-spec-validator
@@ -84,16 +72,14 @@
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 matplotlib==3.7.1
     # via pymatgen
 matplotlib-inline==0.1.6
     # via ipython
-mccabe==0.7.0
-    # via flake8
 monotonic==1.6
     # via bravado
 monty==2023.5.8
     # via
     #   emmet-core
     #   mp-api
     #   pymatgen
@@ -104,100 +90,73 @@
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
 networkx==3.1
     # via pymatgen
-numpy==1.24.3
+numpy==1.25.0
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
 packaging==23.1
     # via
     #   matplotlib
     #   plotly
-    #   pytest
 palettable==3.3.3
     # via pymatgen
-pandas==2.0.1
+pandas==2.0.2
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
 pillow==9.5.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
-pkgutil-resolve-name==1.3.10
-    # via jsonschema
-plotly==5.14.1
+plotly==5.15.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
-pluggy==1.0.0
-    # via pytest
 prompt-toolkit==3.0.38
     # via ipython
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
-py==1.11.0
-    # via
-    #   mpcontribs-client (setup.py)
-    #   pytest-pycodestyle
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
-pycodestyle==2.10.0
-    # via
-    #   flake8
-    #   pytest-pycodestyle
-pydantic==1.10.7
+pydantic==1.10.9
     # via emmet-core
-pyflakes==3.0.1
-    # via flake8
 pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
-pymatgen==2023.5.10
+pymatgen==2023.5.31
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (setup.py)
-pymongo==4.3.3
+pymongo==4.4.0
     # via mpcontribs-client (setup.py)
-pyparsing==3.0.9
+pyparsing==3.1.0
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
-pytest==7.3.1
-    # via
-    #   mpcontribs-client (setup.py)
-    #   pytest-cov
-    #   pytest-flake8
-    #   pytest-pycodestyle
-pytest-cov==4.0.0
-    # via mpcontribs-client (setup.py)
-pytest-flake8==1.1.1
-    # via mpcontribs-client (setup.py)
-pytest-pycodestyle==2.3.1
-    # via mpcontribs-client (setup.py)
 python-dateutil==2.8.2
     # via
     #   arrow
     #   bravado
     #   bravado-core
     #   matplotlib
     #   pandas
@@ -214,21 +173,21 @@
 requests==2.31.0
     # via
     #   bravado
     #   bravado-core
     #   mp-api
     #   pymatgen
     #   requests-futures
-requests-futures==1.0.0
+requests-futures==1.0.1
     # via mpcontribs-client (setup.py)
 rfc3339-validator==0.1.4
     # via jsonschema
 rfc3987==1.3.8
     # via jsonschema
-ruamel-yaml==0.17.26
+ruamel-yaml==0.17.32
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 scipy==1.10.1
     # via pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (setup.py)
@@ -258,43 +217,39 @@
     #   mpcontribs-client (setup.py)
 sympy==1.12
     # via pymatgen
 tabulate==0.9.0
     # via pymatgen
 tenacity==8.2.2
     # via plotly
-tomli==2.0.1
-    # via
-    #   coverage
-    #   pytest
 tqdm==4.65.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.6.0
+typing-extensions==4.6.3
     # via
     #   bravado
     #   emmet-core
     #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
 tzdata==2023.3
     # via pandas
-ujson==5.7.0
+ujson==5.8.0
     # via mpcontribs-client (setup.py)
 uncertainties==3.1.7
     # via pymatgen
-uri-template==1.2.0
+uri-template==1.3.0
     # via jsonschema
-urllib3==2.0.2
+urllib3==2.0.3
     # via requests
 wcwidth==0.2.6
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
 zipp==3.15.0
     # via importlib-resources
```

### Comparing `mpcontribs-client-5.3.5/requirements/ubuntu-latest_py3.9.txt` & `mpcontribs-client-5.4.0/requirements/macos-latest_py3.9_extras.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --output-file=requirements/ubuntu-latest_py3.9.txt --resolver=backtracking
+#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.9_extras.txt --resolver=backtracking
 #
+appnope==0.1.3
+    # via ipython
 arrow==1.2.3
     # via isoduration
 asttokens==2.2.1
     # via stack-data
 attrs==23.1.0
     # via jsonschema
 backcall==0.2.0
@@ -18,53 +20,63 @@
     # via mpcontribs-client (setup.py)
 bravado-core==5.17.1
     # via bravado
 certifi==2023.5.7
     # via requests
 charset-normalizer==3.1.0
     # via requests
-contourpy==1.0.7
+contourpy==1.1.0
     # via matplotlib
+coverage[toml]==7.2.7
+    # via pytest-cov
 cycler==0.11.0
     # via matplotlib
 decorator==5.1.1
     # via ipython
 dnspython==2.3.0
     # via
     #   pyisemail
     #   pymongo
-emmet-core==0.55.2
+emmet-core==0.57.2
     # via mp-api
+exceptiongroup==1.1.1
+    # via pytest
 executing==1.2.0
     # via stack-data
 filetype==1.2.0
     # via mpcontribs-client (setup.py)
+flake8==6.0.0
+    # via
+    #   mpcontribs-client (setup.py)
+    #   pytest-flake8
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
-fonttools==4.39.4
+fonttools==4.40.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
     #   jsonschema
     #   requests
 importlib-resources==5.12.0
     # via matplotlib
-ipython==8.13.2
+iniconfig==2.0.0
+    # via pytest
+ipython==8.14.0
     # via mpcontribs-client (setup.py)
 isoduration==20.11.0
     # via jsonschema
 jedi==0.18.2
     # via ipython
 json2html==1.3.0
     # via mpcontribs-client (setup.py)
-jsonpointer==2.3
+jsonpointer==2.4
     # via jsonschema
 jsonref==1.1.0
     # via bravado-core
 jsonschema[format]==4.17.3
     # via
     #   bravado-core
     #   swagger-spec-validator
@@ -72,14 +84,16 @@
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 matplotlib==3.7.1
     # via pymatgen
 matplotlib-inline==0.1.6
     # via ipython
+mccabe==0.7.0
+    # via flake8
 monotonic==1.6
     # via bravado
 monty==2023.5.8
     # via
     #   emmet-core
     #   mp-api
     #   pymatgen
@@ -90,73 +104,98 @@
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
 networkx==3.1
     # via pymatgen
-numpy==1.24.3
+numpy==1.25.0
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
 packaging==23.1
     # via
     #   matplotlib
     #   plotly
+    #   pytest
 palettable==3.3.3
     # via pymatgen
-pandas==2.0.1
+pandas==2.0.2
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
 pillow==9.5.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
-plotly==5.14.1
+plotly==5.15.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
+pluggy==1.2.0
+    # via pytest
 prompt-toolkit==3.0.38
     # via ipython
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
+py==1.11.0
+    # via
+    #   mpcontribs-client (setup.py)
+    #   pytest-pycodestyle
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
-pydantic==1.10.7
+pycodestyle==2.10.0
+    # via
+    #   flake8
+    #   pytest-pycodestyle
+pydantic==1.10.9
     # via emmet-core
+pyflakes==3.0.1
+    # via flake8
 pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
-pymatgen==2023.5.10
+pymatgen==2023.5.31
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (setup.py)
-pymongo==4.3.3
+pymongo==4.4.0
     # via mpcontribs-client (setup.py)
-pyparsing==3.0.9
+pyparsing==3.1.0
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
+pytest==7.3.2
+    # via
+    #   mpcontribs-client (setup.py)
+    #   pytest-cov
+    #   pytest-flake8
+    #   pytest-pycodestyle
+pytest-cov==4.1.0
+    # via mpcontribs-client (setup.py)
+pytest-flake8==1.1.1
+    # via mpcontribs-client (setup.py)
+pytest-pycodestyle==2.3.1
+    # via mpcontribs-client (setup.py)
 python-dateutil==2.8.2
     # via
     #   arrow
     #   bravado
     #   bravado-core
     #   matplotlib
     #   pandas
@@ -173,21 +212,21 @@
 requests==2.31.0
     # via
     #   bravado
     #   bravado-core
     #   mp-api
     #   pymatgen
     #   requests-futures
-requests-futures==1.0.0
+requests-futures==1.0.1
     # via mpcontribs-client (setup.py)
 rfc3339-validator==0.1.4
     # via jsonschema
 rfc3987==1.3.8
     # via jsonschema
-ruamel-yaml==0.17.26
+ruamel-yaml==0.17.32
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 scipy==1.10.1
     # via pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (setup.py)
@@ -217,39 +256,43 @@
     #   mpcontribs-client (setup.py)
 sympy==1.12
     # via pymatgen
 tabulate==0.9.0
     # via pymatgen
 tenacity==8.2.2
     # via plotly
+tomli==2.0.1
+    # via
+    #   coverage
+    #   pytest
 tqdm==4.65.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.6.0
+typing-extensions==4.6.3
     # via
     #   bravado
     #   emmet-core
     #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
 tzdata==2023.3
     # via pandas
-ujson==5.7.0
+ujson==5.8.0
     # via mpcontribs-client (setup.py)
 uncertainties==3.1.7
     # via pymatgen
-uri-template==1.2.0
+uri-template==1.3.0
     # via jsonschema
-urllib3==2.0.2
+urllib3==2.0.3
     # via requests
 wcwidth==0.2.6
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
 zipp==3.15.0
     # via importlib-resources
```

### Comparing `mpcontribs-client-5.3.5/requirements/ubuntu-latest_py3.9_extras.txt` & `mpcontribs-client-5.4.0/requirements/ubuntu-latest_py3.9_extras.txt`

 * *Files 4% similar despite different names*

```diff
@@ -18,63 +18,63 @@
     # via mpcontribs-client (setup.py)
 bravado-core==5.17.1
     # via bravado
 certifi==2023.5.7
     # via requests
 charset-normalizer==3.1.0
     # via requests
-contourpy==1.0.7
+contourpy==1.1.0
     # via matplotlib
-coverage[toml]==7.2.5
+coverage[toml]==7.2.7
     # via pytest-cov
 cycler==0.11.0
     # via matplotlib
 decorator==5.1.1
     # via ipython
 dnspython==2.3.0
     # via
     #   pyisemail
     #   pymongo
-emmet-core==0.55.2
+emmet-core==0.57.2
     # via mp-api
 exceptiongroup==1.1.1
     # via pytest
 executing==1.2.0
     # via stack-data
 filetype==1.2.0
     # via mpcontribs-client (setup.py)
 flake8==6.0.0
     # via
     #   mpcontribs-client (setup.py)
     #   pytest-flake8
 flatten-dict==0.4.2
     # via mpcontribs-client (setup.py)
-fonttools==4.39.4
+fonttools==4.40.0
     # via matplotlib
 fqdn==1.5.1
     # via jsonschema
 future==0.18.3
     # via uncertainties
 idna==3.4
     # via
     #   jsonschema
     #   requests
 importlib-resources==5.12.0
     # via matplotlib
 iniconfig==2.0.0
     # via pytest
-ipython==8.13.2
+ipython==8.14.0
     # via mpcontribs-client (setup.py)
 isoduration==20.11.0
     # via jsonschema
 jedi==0.18.2
     # via ipython
 json2html==1.3.0
     # via mpcontribs-client (setup.py)
-jsonpointer==2.3
+jsonpointer==2.4
     # via jsonschema
 jsonref==1.1.0
     # via bravado-core
 jsonschema[format]==4.17.3
     # via
     #   bravado-core
     #   swagger-spec-validator
@@ -102,48 +102,48 @@
 msgpack==1.0.5
     # via
     #   bravado
     #   bravado-core
     #   mp-api
 networkx==3.1
     # via pymatgen
-numpy==1.24.3
+numpy==1.25.0
     # via
     #   contourpy
     #   matplotlib
     #   pandas
     #   pymatgen
     #   scipy
     #   spglib
 packaging==23.1
     # via
     #   matplotlib
     #   plotly
     #   pytest
 palettable==3.3.3
     # via pymatgen
-pandas==2.0.1
+pandas==2.0.2
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
     # via ipython
 pickleshare==0.7.5
     # via ipython
 pillow==9.5.0
     # via matplotlib
 pint==0.19.2
     # via mpcontribs-client (setup.py)
-plotly==5.14.1
+plotly==5.15.0
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
-pluggy==1.0.0
+pluggy==1.2.0
     # via pytest
 prompt-toolkit==3.0.38
     # via ipython
 ptyprocess==0.7.0
     # via pexpect
 pure-eval==0.2.2
     # via stack-data
@@ -155,40 +155,40 @@
     # via
     #   emmet-core
     #   pymatgen
 pycodestyle==2.10.0
     # via
     #   flake8
     #   pytest-pycodestyle
-pydantic==1.10.7
+pydantic==1.10.9
     # via emmet-core
 pyflakes==3.0.1
     # via flake8
 pygments==2.15.1
     # via ipython
 pyisemail==2.0.1
     # via mpcontribs-client (setup.py)
-pymatgen==2023.5.10
+pymatgen==2023.5.31
     # via
     #   emmet-core
     #   mp-api
     #   mpcontribs-client (setup.py)
-pymongo==4.3.3
+pymongo==4.4.0
     # via mpcontribs-client (setup.py)
-pyparsing==3.0.9
+pyparsing==3.1.0
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
-pytest==7.3.1
+pytest==7.3.2
     # via
     #   mpcontribs-client (setup.py)
     #   pytest-cov
     #   pytest-flake8
     #   pytest-pycodestyle
-pytest-cov==4.0.0
+pytest-cov==4.1.0
     # via mpcontribs-client (setup.py)
 pytest-flake8==1.1.1
     # via mpcontribs-client (setup.py)
 pytest-pycodestyle==2.3.1
     # via mpcontribs-client (setup.py)
 python-dateutil==2.8.2
     # via
@@ -210,21 +210,21 @@
 requests==2.31.0
     # via
     #   bravado
     #   bravado-core
     #   mp-api
     #   pymatgen
     #   requests-futures
-requests-futures==1.0.0
+requests-futures==1.0.1
     # via mpcontribs-client (setup.py)
 rfc3339-validator==0.1.4
     # via jsonschema
 rfc3987==1.3.8
     # via jsonschema
-ruamel-yaml==0.17.26
+ruamel-yaml==0.17.32
     # via pymatgen
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 scipy==1.10.1
     # via pymatgen
 semantic-version==2.10.0
     # via mpcontribs-client (setup.py)
@@ -266,31 +266,31 @@
     # via
     #   mpcontribs-client (setup.py)
     #   pymatgen
 traitlets==5.9.0
     # via
     #   ipython
     #   matplotlib-inline
-typing-extensions==4.6.0
+typing-extensions==4.6.3
     # via
     #   bravado
     #   emmet-core
     #   ipython
     #   mp-api
     #   pydantic
     #   swagger-spec-validator
 tzdata==2023.3
     # via pandas
-ujson==5.7.0
+ujson==5.8.0
     # via mpcontribs-client (setup.py)
 uncertainties==3.1.7
     # via pymatgen
-uri-template==1.2.0
+uri-template==1.3.0
     # via jsonschema
-urllib3==2.0.2
+urllib3==2.0.3
     # via requests
 wcwidth==0.2.6
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
 zipp==3.15.0
     # via importlib-resources
```

### Comparing `mpcontribs-client-5.3.5/setup.py` & `mpcontribs-client-5.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `mpcontribs-client-5.3.5/tests/test_client.py` & `mpcontribs-client-5.4.0/tests/test_client.py`

 * *Files identical despite different names*


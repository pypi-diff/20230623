# Comparing `tmp/erddapy-2.0.1.tar.gz` & `tmp/erddapy-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erddapy-2.0.1.tar", last modified: Thu Apr 20 17:50:17 2023, max compression
+gzip compressed data, was "erddapy-2.0.2.tar", last modified: Fri Jun 23 16:34:44 2023, max compression
```

## Comparing `erddapy-2.0.1.tar` & `erddapy-2.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:50:17.469162 erddapy-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-04-20 17:50:03.000000 erddapy-2.0.1/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-20 17:50:03.000000 erddapy-2.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-20 17:50:03.000000 erddapy-2.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-04-20 17:50:17.469162 erddapy-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-20 17:50:03.000000 erddapy-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:50:17.469162 erddapy-2.0.1/erddapy/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-20 17:50:03.000000 erddapy-2.0.1/erddapy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:50:17.469162 erddapy-2.0.1/erddapy/core/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-20 17:50:03.000000 erddapy-2.0.1/erddapy/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-20 17:50:03.000000 erddapy-2.0.1/erddapy/core/griddap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-04-20 17:50:03.000000 erddapy-2.0.1/erddapy/core/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-20 17:50:03.000000 erddapy-2.0.1/erddapy/core/netcdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    14312 2023-04-20 17:50:03.000000 erddapy-2.0.1/erddapy/core/url.py
--rw-r--r--   0 runner    (1001) docker     (123)    16215 2023-04-20 17:50:03.000000 erddapy-2.0.1/erddapy/erddapy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-04-20 17:50:03.000000 erddapy-2.0.1/erddapy/multiple_server_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:50:17.469162 erddapy-2.0.1/erddapy/servers/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-20 17:50:03.000000 erddapy-2.0.1/erddapy/servers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-04-20 17:50:03.000000 erddapy-2.0.1/erddapy/servers/erddaps.json
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-20 17:50:03.000000 erddapy-2.0.1/erddapy/servers/servers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:50:17.469162 erddapy-2.0.1/erddapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-20 17:50:17.000000 erddapy-2.0.1/erddapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-04-20 17:50:03.000000 erddapy-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-20 17:50:03.000000 erddapy-2.0.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-20 17:50:03.000000 erddapy-2.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 17:50:17.469162 erddapy-2.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:34:44.591858 erddapy-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-06-23 16:34:30.000000 erddapy-2.0.2/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-23 16:34:30.000000 erddapy-2.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-23 16:34:30.000000 erddapy-2.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-06-23 16:34:44.591858 erddapy-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-06-23 16:34:30.000000 erddapy-2.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:34:44.591858 erddapy-2.0.2/erddapy/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-23 16:34:30.000000 erddapy-2.0.2/erddapy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:34:44.591858 erddapy-2.0.2/erddapy/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-23 16:34:30.000000 erddapy-2.0.2/erddapy/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-23 16:34:30.000000 erddapy-2.0.2/erddapy/core/griddap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-06-23 16:34:30.000000 erddapy-2.0.2/erddapy/core/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-23 16:34:30.000000 erddapy-2.0.2/erddapy/core/netcdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14281 2023-06-23 16:34:30.000000 erddapy-2.0.2/erddapy/core/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16853 2023-06-23 16:34:30.000000 erddapy-2.0.2/erddapy/erddapy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-06-23 16:34:30.000000 erddapy-2.0.2/erddapy/multiple_server_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:34:44.591858 erddapy-2.0.2/erddapy/servers/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-23 16:34:30.000000 erddapy-2.0.2/erddapy/servers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-06-23 16:34:30.000000 erddapy-2.0.2/erddapy/servers/erddaps.json
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-23 16:34:30.000000 erddapy-2.0.2/erddapy/servers/servers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:34:44.591858 erddapy-2.0.2/erddapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-23 16:34:44.000000 erddapy-2.0.2/erddapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-06-23 16:34:30.000000 erddapy-2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-23 16:34:30.000000 erddapy-2.0.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-23 16:34:30.000000 erddapy-2.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 16:34:44.591858 erddapy-2.0.2/setup.cfg
```

### Comparing `erddapy-2.0.1/CHANGES.txt` & `erddapy-2.0.2/CHANGES.txt`

 * *Files identical despite different names*

### Comparing `erddapy-2.0.1/LICENSE.txt` & `erddapy-2.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `erddapy-2.0.1/PKG-INFO` & `erddapy-2.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erddapy
-Version: 2.0.1
+Version: 2.0.2
 Summary: Python interface for ERDDAP
 Author-email: Filipe Fernandes <ocefpaf+erddapy@gmail.com>
 License: Copyright 2017 Filipe Fernandes
         
         
         Redistribution and use in source and binary forms,
         with or without modification,
@@ -31,14 +31,19 @@
         HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT,
         STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY
         WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: documentation, https://ioos.github.io/erddapy
 Project-URL: homepage, https://github.com/ioos/erddapy
 Project-URL: repository, https://github.com/ioos/erddapy
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 <h1 align="center" style="margin:1em;">
   <a href="https://ioos.github.io/erddapy/">erddapy</a>
 </h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: erddapy Version: 2.0.1 Summary: Python interface
+Metadata-Version: 2.1 Name: erddapy Version: 2.0.2 Summary: Python interface
 for ERDDAP Author-email: Filipe Fernandes
 erddapy@gmail.com> License: Copyright 2017 Filipe Fernandes Redistribution and
 use in source and binary forms, with or without modification, are permitted
 provided that the following conditions are met: 1. Redistributions of source
 code must retain the above copyright notice, this list of conditions and the
 following disclaimer. 2. Redistributions in binary form must reproduce the
 above copyright notice, this list of conditions and the following disclaimer in
@@ -17,16 +17,20 @@
 INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
 LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR
 PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
 OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 ADVISED OF THE POSSIBILITY OF SUCH DAMAGE. Project-URL: documentation, https://
 ioos.github.io/erddapy Project-URL: homepage, https://github.com/ioos/erddapy
-Project-URL: repository, https://github.com/ioos/erddapy Requires-Python: >=3.8
-Description-Content-Type: text/markdown License-File: LICENSE.txt
+Project-URL: repository, https://github.com/ioos/erddapy Classifier:
+Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Requires-Python: >=3.8 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
                              ****** erddapy ******
                        *** erddapy: ERDDAP + Python. ***
    [conda-forge_downloads] [Latest_version] [Commits_since_last_release] [#
       contributors] [zenodo] [zenodo] [pre-commit.ci_status] [GHA-tests]
 
 # Table of contents  - [Overview](#overview) - [Example](#example) - [Get in
 touch](#get-in-touch) - [License and copyright](#license-and-copyright)  ##
```

### Comparing `erddapy-2.0.1/README.md` & `erddapy-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `erddapy-2.0.1/erddapy/core/__init__.py` & `erddapy-2.0.2/erddapy/core/__init__.py`

 * *Files identical despite different names*

### Comparing `erddapy-2.0.1/erddapy/core/griddap.py` & `erddapy-2.0.2/erddapy/core/griddap.py`

 * *Files identical despite different names*

### Comparing `erddapy-2.0.1/erddapy/core/interfaces.py` & `erddapy-2.0.2/erddapy/core/interfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     """
     Convert a URL to Pandas DataFrame.
 
     url: URL to request data from.
     requests_kwargs: arguments to be passed to urlopen method.
     **pandas_kwargs: kwargs to be passed to third-party library (pandas).
     """
-    data = urlopen(url, **(requests_kwargs or {}))
+    data = urlopen(url, requests_kwargs or {})
     try:
         return pd.read_csv(data, **(pandas_kwargs or {}))
     except Exception as e:
         raise ValueError(f"Could not read url {url} with Pandas.read_csv.") from e
 
 
 def to_ncCF(
```

### Comparing `erddapy-2.0.1/erddapy/core/netcdf.py` & `erddapy-2.0.2/erddapy/core/netcdf.py`

 * *Files identical despite different names*

### Comparing `erddapy-2.0.1/erddapy/core/url.py` & `erddapy-2.0.2/erddapy/core/url.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,30 +52,29 @@
 
     """
     r = httpx.head(url, **kwargs)
     r.raise_for_status()
     return url
 
 
-def _distinct(url: str, **kwargs: Dict) -> str:
+def _distinct(url: str, distinct: Optional[bool] = False) -> str:
     """
     Sort all of the rows in the results table.
 
     Starting with the first requested variable,
     then using the second requested variable if the first variable has a tie, ...,
     then remove all non-unique rows of data.
 
     For example, a query for the variables ["stationType", "stationID"] with `distinct=True`
     will return a sorted list of "stationIDs" associated with each "stationType".
 
     See http://erddap.ioos.us/erddap/tabledap/documentation.html#distinct
 
     """
-    distinct = kwargs.pop("distinct", False)
-    if distinct is True:
+    if distinct:
         return f"{url}&distinct()"
     return url
 
 
 def _format_search_string(server: str, query: str) -> str:
     """Generate a search string for an erddap server with user defined query."""
     return f'{server}search/index.csv?page=1&itemsPerPage=100000&searchFor="{query}"'
@@ -106,15 +105,15 @@
     """Join the constraint variables with separator '&' to add to the download link."""
     return "".join([f"&{k}{v}" for k, v in kwargs.items()])
 
 
 def _check_substrings(constraint):
     """Extend the OPeNDAP with extra strings."""
     substrings = ["now", "min", "max"]
-    return any([True for substring in substrings if substring in str(constraint)])
+    return any(True for substring in substrings if substring in str(constraint))
 
 
 def parse_dates(
     date_time: Union[datetime, str],
     dayfirst=False,
     yearfirst=False,
 ) -> float:
@@ -338,15 +337,15 @@
     server: str,
     dataset_id: OptionalStr = None,
     protocol: OptionalStr = None,
     variables: Optional[ListLike] = None,
     dim_names: Optional[ListLike] = None,
     response=None,
     constraints=None,
-    **kwargs,
+    distinct=False,
 ) -> str:
     """
     Build the download URL for the `server` endpoint.
 
     Args:
         dataset_id: a dataset unique id.
         protocol: tabledap or griddap.
@@ -432,9 +431,9 @@
             if k.startswith(valid_time_constraints):
                 _constraints.update({k: parse_dates(v)})
         _constraints = _quote_string_constraints(_constraints)
         _constraints_url = _format_constraints_url(_constraints)
 
         url += f"{_constraints_url}"
 
-    url = _distinct(url, **kwargs)
+    url = _distinct(url, distinct)
     return url
```

### Comparing `erddapy-2.0.1/erddapy/erddapy.py` & `erddapy-2.0.2/erddapy/erddapy.py`

 * *Files 19% similar despite different names*

```diff
@@ -154,14 +154,18 @@
         dataset_id = dataset_id if dataset_id else self.dataset_id
         if self.protocol != "griddap":
             raise ValueError(
                 f"Method only valid using griddap protocol, got {self.protocol}",
             )
         if dataset_id is None:
             raise ValueError(f"Must set a valid dataset_id, got {self.dataset_id}")
+        # Return the opendap URL without any slicing so the user can do it later.
+        if self.response == "opendap":
+            return
+
         metadata_url = f"{self.server}/griddap/{self.dataset_id}"
         (
             self.constraints,
             self.dim_names,
             self.variables,
         ) = _griddap_get_constraints(metadata_url, step)
         self._constraints_original = self.constraints.copy()
@@ -269,15 +273,15 @@
         self,
         dataset_id: OptionalStr = None,
         protocol: OptionalStr = None,
         variables: Optional[ListLike] = None,
         dim_names: Optional[ListLike] = None,
         response=None,
         constraints=None,
-        **kwargs,
+        distinct=False,
     ) -> str:
         """
         Build the download URL for the `server` endpoint.
 
         Args:
             dataset_id: a dataset unique id.
             protocol: tabledap or griddap.
@@ -327,60 +331,70 @@
             self.server,
             dataset_id,
             protocol,
             variables,
             dim_names,
             response,
             constraints,
-            **kwargs,
+            distinct,
         )
 
-    def to_pandas(self, **kw):
+    def to_pandas(
+        self,
+        requests_kwargs: Optional[Dict] = None,
+        **kw,
+    ) -> "pd.DataFrame":
         """Save a data request to a pandas.DataFrame.
 
         Accepts any `pandas.read_csv` keyword arguments, passed as a dictionary to pandas_kwargs.
 
         This method uses the .csvp [1] response as the default for simplicity,
         please check ERDDAP's documentation for the other csv options available.
 
         [1] Download a ISO-8859-1 .csv file with line 1: name (units). Times are ISO 8601 strings.
 
+        requests_kwargs: kwargs to be passed to urlopen method.
+        **kw: kwargs to be passed to third-party library (pandas).
         """
         response = kw.pop("response", "csvp")
-        url = self.get_download_url(response=response, **kw)
-        return to_pandas(url, pandas_kwargs=dict(**kw))
+        distinct = kw.pop("distinct", False)
+        url = self.get_download_url(response=response, distinct=distinct)
+        return to_pandas(url, requests_kwargs=requests_kwargs, pandas_kwargs=dict(**kw))
 
     def to_ncCF(self, protocol: str = None, **kw):
         """Load the data request into a Climate and Forecast compliant netCDF4-python object."""
+        distinct = kw.pop("distinct", False)
         protocol = protocol if protocol else self.protocol
-        url = self.get_download_url(response="ncCF", **kw)
+        url = self.get_download_url(response="ncCF", distinct=distinct)
         return to_ncCF(url, protocol=protocol, requests_kwargs=dict(**kw))
 
     def to_xarray(self, **kw):
         """Load the data request into a xarray.Dataset.
 
         Accepts any `xr.open_dataset` keyword arguments.
         """
         if self.response == "opendap":
             response = "opendap"
         elif self.protocol == "griddap":
             response = "nc"
         else:
             response = "ncCF"
-        url = self.get_download_url(response=response)
+        distinct = kw.pop("distinct", False)
+        url = self.get_download_url(response=response, distinct=distinct)
         requests_kwargs = {"auth": self.auth}
         return to_xarray(url, response, requests_kwargs, xarray_kwargs=dict(**kw))
 
     def to_iris(self, **kw):
         """Load the data request into an iris.CubeList.
 
         Accepts any `iris.load_raw` keyword arguments.
         """
         response = "nc" if self.protocol == "griddap" else "ncCF"
-        url = self.get_download_url(response=response, **kw)
+        distinct = kw.pop("distinct", False)
+        url = self.get_download_url(response=response, distinct=distinct)
         return to_iris(url, iris_kwargs=dict(**kw))
 
     def _get_variables_uncached(self, dataset_id: OptionalStr = None) -> Dict:
         if not dataset_id:
             dataset_id = self.dataset_id
 
         if dataset_id is None:
```

### Comparing `erddapy-2.0.1/erddapy/multiple_server_search.py` & `erddapy-2.0.2/erddapy/multiple_server_search.py`

 * *Files identical despite different names*

### Comparing `erddapy-2.0.1/erddapy/servers/erddaps.json` & `erddapy-2.0.2/erddapy/servers/erddaps.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7182539682539683%*

 * *Differences: {'14': "{'url': 'https://sccoos.org/erddap/'}",*

 * * '19': "{'url': 'https://erddap.dataexplorer.oceanobservatories.org/erddap/'}",*

 * * '22': "{'name': 'Regional Ocean Modelling System'}",*

 * * '26': "{'name': 'GCOOS Atmospheric and Oceanographic: Historical Data', 'url': "*

 * *       "'https://gcoos5.geos.tamu.edu/erddap/'}",*

 * * '27': "{'name': 'GCOOS Biological and Socioeconomics', 'url': 'https://gcoos4.tamu.edu/erddap/'}",*

 * * '34': "{'url': 'https://www.ifremer.fr/erddap/'}",*

 * * '38': "{'name': 'Hakai Institute', 'short_nam […]*

```diff
@@ -1,9 +1,15 @@
 [
     {
+        "name": "St. Lawrence Global Observatory - CIOOS | Observatoire global du Saint-Laurent - SIOOC",
+        "public": true,
+        "short_name": "SLGO-OGSL",
+        "url": "https://erddap.ogsl.ca/erddap/"
+    },
+    {
         "name": "CoastWatch West Coast Node",
         "public": true,
         "short_name": "CSWC",
         "url": "https://coastwatch.pfeg.noaa.gov/erddap/"
     },
     {
         "name": "ERDDAP at the Asia-Pacific Data-Research Center",
@@ -41,21 +47,27 @@
         "short_name": "CSCGOM",
         "url": "https://cwcgom.aoml.noaa.gov/erddap/"
     },
     {
         "name": "NOAA IOOS Sensors ERDDAP",
         "public": true,
         "short_name": "IOOS-Sensors",
-        "url": "http://erddap.sensors.ioos.us/erddap/"
+        "url": "https://erddap.sensors.ioos.us/erddap/"
     },
     {
         "name": "NOAA IOOS CeNCOOS (Central and Northern California Ocean Observing System)",
         "public": true,
         "short_name": "CeNCOOS",
-        "url": "http://erddap.axiomdatascience.com/erddap/"
+        "url": "https://erddap.axiomdatascience.com/erddap/"
+    },
+    {
+        "name": "CeNCOOS (Central and Northern California Ocean Observing System) ERDDAP",
+        "public": true,
+        "short_name": "CeNCOOS ERDDAP",
+        "url": "http://erddap.cencoos.org/erddap/"
     },
     {
         "name": "NOAA IOOS NERACOOS (Northeastern Regional Association of Coastal and Ocean Observing Systems)",
         "public": true,
         "short_name": "NERACOOS",
         "url": "http://www.neracoos.org/erddap/"
     },
@@ -71,29 +83,23 @@
         "short_name": "PacIOOS",
         "url": "https://pae-paha.pacioos.hawaii.edu/erddap/"
     },
     {
         "name": "Southern California Coastal Ocean Observing System (SCCOOS)",
         "public": true,
         "short_name": "SCCOOS",
-        "url": "http://sccoos.org/erddap/"
+        "url": "https://sccoos.org/erddap/"
     },
     {
         "name": "NOAA IOOS SECOORA (Southeast Coastal Ocean Observing Regional Association)",
         "public": true,
         "short_name": "SECOORA",
         "url": "http://erddap.secoora.org/erddap/"
     },
     {
-        "name": "NOAA NCEI (National Centers for Environmental Information) / NCDDC",
-        "public": true,
-        "short_name": "NCDDC",
-        "url": "https://ecowatch.ncddc.noaa.gov/erddap/"
-    },
-    {
         "name": "NOAA OSMC (Observing System Monitoring Center)",
         "public": true,
         "short_name": "OSMC",
         "url": "http://osmc.noaa.gov/erddap/"
     },
     {
         "name": "ONC (Ocean Networks Canada)",
@@ -107,24 +113,30 @@
         "short_name": "PIFSC",
         "url": "https://oceanwatch.pifsc.noaa.gov/erddap/"
     },
     {
         "name": "Ocean Observatories Initiative (OOI)",
         "public": true,
         "short_name": "OOI",
-        "url": "https://erddap-uncabled.oceanobservatories.org/uncabled/erddap/"
+        "url": "https://erddap.dataexplorer.oceanobservatories.org/erddap/"
+    },
+    {
+        "name": "Ocean Observatories Initiative (OOI) Goldcopy",
+        "public": true,
+        "short_name": "OOI Goldcopy",
+        "url": "https://erddap-goldcopy.dataexplorer.oceanobservatories.org/erddap/"
     },
     {
         "name": "Ocean Tracking Network",
         "public": true,
         "short_name": "OTN",
         "url": "https://members.oceantrack.org/erddap/"
     },
     {
-        "name": "",
+        "name": "Regional Ocean Modelling System",
         "public": false,
         "short_name": "MYROMS",
         "url": "http://www.myroms.org:8080/erddap/"
     },
     {
         "name": "Department of Marine and Coastal Sciences, School of Environmental and Biological Sciences, Rutgers, The State University of New Jersey",
         "public": true,
@@ -140,38 +152,32 @@
     {
         "name": "NOAA's Center for Operational Oceanographic Products and Services",
         "public": true,
         "short_name": "COOPS-NOS",
         "url": "https://opendap.co-ops.nos.noaa.gov/erddap/"
     },
     {
-        "name": "",
+        "name": "GCOOS Atmospheric and Oceanographic: Historical Data",
         "public": false,
         "short_name": "GCOO5-TAMU",
-        "url": "http://gcoos5.geos.tamu.edu:6060/erddap/"
+        "url": "https://gcoos5.geos.tamu.edu/erddap/"
     },
     {
-        "name": "",
+        "name": "GCOOS Biological and Socioeconomics",
         "public": false,
         "short_name": "GCOO4-TAMU",
-        "url": "http://gcoos4.tamu.edu:8080/erddap/"
+        "url": "https://gcoos4.tamu.edu/erddap/"
     },
     {
         "name": "NOAA CoastWatch Great Lakes Node",
         "public": true,
         "short_name": "GLERL",
         "url": "https://coastwatch.glerl.noaa.gov/erddap/"
     },
     {
-        "name": "",
-        "public": false,
-        "short_name": "SFEI",
-        "url": "http://sfbaynutrients.sfei.org/erddap/"
-    },
-    {
         "name": "Spray Underwater Glider data from Instrument Development Group, Scripps Institute of Oceanography, University of California, San Diego",
         "public": true,
         "short_name": "UCSD",
         "url": "https://spraydata.ucsd.edu/erddap/"
     },
     {
         "name": "UBC Earth, Ocean & Atmospheric Sciences SalishSeaCast Project",
@@ -194,24 +200,18 @@
     {
         "name": "Marine Domain Awareness (MDA) - Italy",
         "public": true,
         "short_name": "MDA",
         "url": "https://bluehub.jrc.ec.europa.eu/erddap/"
     },
     {
-        "name": "R.Tech Engineering",
-        "public": true,
-        "short_name": "RTECH",
-        "url": "https://meteo.rtech.fr/erddap/"
-    },
-    {
         "name": "French Research Institute for the Exploitation of the Sea",
         "public": true,
         "short_name": "IFREMER",
-        "url": "http://www.ifremer.fr/erddap/"
+        "url": "https://www.ifremer.fr/erddap/"
     },
     {
         "name": "NOAA PMEL (Pacific Marine Environmental Laboratory)",
         "public": true,
         "short_name": "PMEL",
         "url": "https://ferret.pmel.noaa.gov/pmel/erddap"
     },
@@ -224,27 +224,27 @@
     {
         "name": "SOCAT (Surface Ocean CO2 ATlas)",
         "public": true,
         "short_name": "SOCAT",
         "url": "https://ferret.pmel.noaa.gov/socat/erddap/"
     },
     {
-        "name": "HAKAI Institute",
+        "name": "Hakai Institute",
         "public": true,
-        "short_name": "HAKAI",
+        "short_name": "Hakai",
         "url": "https://catalogue.hakai.org/erddap/"
     },
     {
         "name": "NANOOS (Northwest Association of Networked Ocean Observing Systems)",
         "public": true,
         "short_name": "NANOOS",
         "url": "https://wilson.coas.oregonstate.edu/erddap/"
     },
     {
-        "name": "NOAH Polar Watch",
+        "name": "NOAA Polar Watch",
         "public": true,
         "short_name": "POLARWATCH",
         "url": "https://polarwatch.noaa.gov/erddap/"
     },
     {
         "name": "NCI (National Computational Infrastructure",
         "public": true,
@@ -278,15 +278,15 @@
     {
         "name": "GRIIDC (Gulf of Mexico Research Initiative",
         "public": true,
         "short_name": "GRIIDC",
         "url": "https://erddap.griidc.org/erddap/"
     },
     {
-        "name": "NOAH ATN IOOS (Animal Telemetry Network)",
+        "name": "NOAA ATN IOOS (Animal Telemetry Network)",
         "public": true,
         "short_name": "ATN-IOOS",
         "url": "https://atn.ioos.us/erddap/"
     },
     {
         "name": "DIVER (NOAA Office of Response and Restoration)",
         "public": true,
@@ -294,9 +294,69 @@
         "url": "https://pub-data.diver.orr.noaa.gov/erddap/"
     },
     {
         "name": "JEODPP ERDDAP server",
         "public": true,
         "short_name": "JEOPP",
         "url": "https://jeodpp.jrc.ec.europa.eu/services/erddap/"
+    },
+    {
+        "name": "GCOOS Atmospheric and Oceanographic: Observing System",
+        "public": true,
+        "short_name": "GCOOS",
+        "url": "https://erddap.gcoos.org/erddap/"
+    },
+    {
+        "name": "University of Delaware, College of Earth, Ocean and Environment",
+        "public": true,
+        "short_name": "CEOE",
+        "url": "https://basin.ceoe.udel.edu/erddap/"
+    },
+    {
+        "name": "Canadian Integrated Ocean Observatory System Atlantic",
+        "public": true,
+        "short_name": "CIOOS Atlantic",
+        "url": "https://cioosatlantic.ca/erddap/"
+    },
+    {
+        "name": "Canadian Integrated Ocean Observatory System Pacific",
+        "public": true,
+        "short_name": "CIOOS Pacific",
+        "url": "https://data.cioospacific.ca/erddap/"
+    },
+    {
+        "name": "European Multidisciplinary Seafloor and water column Observatory (EMSO)",
+        "public": true,
+        "short_name": "EMSO ERIC",
+        "url": "http://erddap.emso.eu:8080/erddap/"
+    },
+    {
+        "name": "Southern Ocean Carbon and Heat Imact on Climate (SO-CHIC)",
+        "public": true,
+        "short_name": "SO-CHIC",
+        "url": "http://erddap.sochic-h2020.eu/erddap/"
+    },
+    {
+        "name": "NOAA CoastWatch Central Operations",
+        "public": true,
+        "short_name": "NCCO",
+        "url": "https://coastwatch.noaa.gov/erddap/"
+    },
+    {
+        "name": "The Canadian Watershed Information Network at the University of Manitoba",
+        "public": true,
+        "short_name": "CanWIN",
+        "url": "https://canwinerddap.ad.umanitoba.ca/erddap/index.html"
+    },
+    {
+        "name": "NOAA Oceanview",
+        "public": true,
+        "short_name": "NOAA Oceanview",
+        "url": "https://oceanview.pfeg.noaa.gov/erddap/index.html"
+    },
+    {
+        "name": "UNESCO IOC-IODE Ocean Acidification",
+        "public": true,
+        "short_name": "IOC-IODE-OA",
+        "url": "https://erddap.oa.iode.org/erddap/"
     }
 ]
```

### Comparing `erddapy-2.0.1/erddapy/servers/servers.py` & `erddapy-2.0.2/erddapy/servers/servers.py`

 * *Files identical despite different names*

### Comparing `erddapy-2.0.1/pyproject.toml` & `erddapy-2.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -11,14 +11,21 @@
 description = "Python interface for ERDDAP"
 readme = "README.md"
 license = {file = "LICENSE.txt"}
 authors = [
     {name = "Filipe Fernandes", email = "ocefpaf+erddapy@gmail.com"},
 ]
 requires-python = ">=3.8"
+classifiers = [
+  "Programming Language :: Python :: 3 :: Only",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+]
 dynamic = [
   "dependencies",
   "version",
 ]
 [project.urls]
 documentation = "https://ioos.github.io/erddapy"
 homepage = "https://github.com/ioos/erddapy"
@@ -32,25 +39,14 @@
 dependencies = {file = ["requirements.txt"]}
 
 [tool.setuptools_scm]
 write_to = "erddapy/_version.py"
 write_to_template = "__version__ = '{version}'"
 tag_regex = "^(?P<prefix>v)?(?P<version>[^\\+]+)(?P<suffix>.*)?$"
 
-[tool.pytest.ini_options]
-markers = [
-    "web: marks tests require connection (deselect with '-m \"not web\"')",
-    "serial: marks tests that cannot be run in parallel (deselect with '-m \"not serial\"')",
-]
-filterwarnings = [
-    "error:::erddapy.*",
-    "ignore::UserWarning",
-    "ignore::RuntimeWarning",
-]
-
 [tool.ruff]
 select = [
     "A", # flake8-builtins
     "B", # flake8-bugbear
     "C4", # flake8-comprehensions
     "F", # flakes
     "I", # import sorting
@@ -62,14 +58,25 @@
 
 [tool.ruff.per-file-ignores]
 "docs/source/conf.py" = [
   "E402",
   "A001",
 ]
 
+[tool.pytest.ini_options]
+markers = [
+    "web: marks tests require connection (deselect with '-m \"not web\"')",
+    "serial: marks tests that cannot be run in parallel (deselect with '-m \"not serial\"')",
+]
+filterwarnings = [
+    "error:::erddapy.*",
+    "ignore::UserWarning",
+    "ignore::RuntimeWarning",
+]
+
 [tool.check-manifest]
 ignore = [
     "*.yml",
     ".coveragerc",
     "Makefile",
     "docs",
     "docs/*",
@@ -83,11 +90,11 @@
 ignore-init-method = true
 ignore-init-module = false
 ignore-magic = false
 ignore-semiprivate = false
 ignore-private = false
 ignore-module = false
 fail-under = 85
-exclude = ["setup.py", "docs", "tests"]
+exclude = ["docs", "tests"]
 verbose = 1
 quiet = false
 color = true
```


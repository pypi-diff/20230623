# Comparing `tmp/uddr_client-0.1.0.tar.gz` & `tmp/uddr_client-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uddr_client-0.1.0.tar", last modified: Wed Jun 14 05:06:53 2023, max compression
+gzip compressed data, was "uddr_client-0.2.0.tar", last modified: Thu Jun 22 21:58:34 2023, max compression
```

## Comparing `uddr_client-0.1.0.tar` & `uddr_client-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,25 @@
-drwxr-xr-x   0 shane     (1000) shane     (1000)        0 2023-06-14 05:06:53.519488 uddr_client-0.1.0/
--rw-r--r--   0 shane     (1000) shane     (1000)     1071 2023-06-14 04:19:49.000000 uddr_client-0.1.0/LICENSE.md
--rw-r--r--   0 shane     (1000) shane     (1000)     2105 2023-06-14 05:06:53.519488 uddr_client-0.1.0/PKG-INFO
--rw-r--r--   0 shane     (1000) shane     (1000)     1490 2023-06-14 05:06:26.000000 uddr_client-0.1.0/README.md
--rw-r--r--   0 shane     (1000) shane     (1000)       38 2023-06-14 05:06:53.519488 uddr_client-0.1.0/setup.cfg
--rw-r--r--   0 shane     (1000) shane     (1000)      919 2023-06-14 04:20:53.000000 uddr_client-0.1.0/setup.py
-drwxr-xr-x   0 shane     (1000) shane     (1000)        0 2023-06-14 05:06:53.519488 uddr_client-0.1.0/src/
-drwxr-xr-x   0 shane     (1000) shane     (1000)        0 2023-06-14 05:06:53.519488 uddr_client-0.1.0/src/uddr_client/
--rw-r--r--   0 shane     (1000) shane     (1000)       37 2023-06-09 19:52:19.000000 uddr_client-0.1.0/src/uddr_client/__init__.py
--rw-r--r--   0 shane     (1000) shane     (1000)    19611 2023-06-14 03:49:52.000000 uddr_client-0.1.0/src/uddr_client/client.py
--rw-r--r--   0 shane     (1000) shane     (1000)     1677 2023-06-14 03:52:07.000000 uddr_client-0.1.0/src/uddr_client/connection.py
--rw-r--r--   0 shane     (1000) shane     (1000)     1250 2023-06-14 02:40:35.000000 uddr_client-0.1.0/src/uddr_client/response.py
-drwxr-xr-x   0 shane     (1000) shane     (1000)        0 2023-06-14 05:06:53.519488 uddr_client-0.1.0/src/uddr_client.egg-info/
--rw-r--r--   0 shane     (1000) shane     (1000)     2105 2023-06-14 05:06:53.000000 uddr_client-0.1.0/src/uddr_client.egg-info/PKG-INFO
--rw-r--r--   0 shane     (1000) shane     (1000)      335 2023-06-14 05:06:53.000000 uddr_client-0.1.0/src/uddr_client.egg-info/SOURCES.txt
--rw-r--r--   0 shane     (1000) shane     (1000)        1 2023-06-14 05:06:53.000000 uddr_client-0.1.0/src/uddr_client.egg-info/dependency_links.txt
--rw-r--r--   0 shane     (1000) shane     (1000)       32 2023-06-14 05:06:53.000000 uddr_client-0.1.0/src/uddr_client.egg-info/requires.txt
--rw-r--r--   0 shane     (1000) shane     (1000)       12 2023-06-14 05:06:53.000000 uddr_client-0.1.0/src/uddr_client.egg-info/top_level.txt
+drwxr-xr-x   0 shane     (1000) shane     (1000)        0 2023-06-22 21:58:34.824825 uddr_client-0.2.0/
+-rw-r--r--   0 shane     (1000) shane     (1000)     1071 2023-06-14 04:19:49.000000 uddr_client-0.2.0/LICENSE.md
+-rw-r--r--   0 shane     (1000) shane     (1000)     4191 2023-06-22 21:58:34.824825 uddr_client-0.2.0/PKG-INFO
+-rw-r--r--   0 shane     (1000) shane     (1000)     3576 2023-06-22 21:56:00.000000 uddr_client-0.2.0/README.md
+-rw-r--r--   0 shane     (1000) shane     (1000)       38 2023-06-22 21:58:34.824825 uddr_client-0.2.0/setup.cfg
+-rw-r--r--   0 shane     (1000) shane     (1000)      948 2023-06-22 21:58:18.000000 uddr_client-0.2.0/setup.py
+drwxr-xr-x   0 shane     (1000) shane     (1000)        0 2023-06-22 21:58:34.814825 uddr_client-0.2.0/src/
+drwxr-xr-x   0 shane     (1000) shane     (1000)        0 2023-06-22 21:58:34.814825 uddr_client-0.2.0/src/uddr_client/
+-rw-r--r--   0 shane     (1000) shane     (1000)       37 2023-06-09 19:52:19.000000 uddr_client-0.2.0/src/uddr_client/__init__.py
+drwxr-xr-x   0 shane     (1000) shane     (1000)        0 2023-06-22 21:58:34.814825 uddr_client-0.2.0/src/uddr_client/api/
+-rw-r--r--   0 shane     (1000) shane     (1000)       33 2023-06-22 21:56:00.000000 uddr_client-0.2.0/src/uddr_client/api/__init__.py
+-rw-r--r--   0 shane     (1000) shane     (1000)    18903 2023-06-22 21:56:00.000000 uddr_client-0.2.0/src/uddr_client/api/api_client.py
+-rw-r--r--   0 shane     (1000) shane     (1000)     2593 2023-06-22 21:56:00.000000 uddr_client-0.2.0/src/uddr_client/client.py
+-rw-r--r--   0 shane     (1000) shane     (1000)     3065 2023-06-22 21:56:00.000000 uddr_client-0.2.0/src/uddr_client/connection.py
+drwxr-xr-x   0 shane     (1000) shane     (1000)        0 2023-06-22 21:58:34.814825 uddr_client-0.2.0/src/uddr_client/doh/
+-rw-r--r--   0 shane     (1000) shane     (1000)       33 2023-06-22 21:56:00.000000 uddr_client-0.2.0/src/uddr_client/doh/__init__.py
+-rw-r--r--   0 shane     (1000) shane     (1000)     4886 2023-06-22 21:56:00.000000 uddr_client-0.2.0/src/uddr_client/doh/doh_client.py
+-rw-r--r--   0 shane     (1000) shane     (1000)     1062 2023-06-22 21:56:00.000000 uddr_client-0.2.0/src/uddr_client/doh/ioc_parser.py
+-rw-r--r--   0 shane     (1000) shane     (1000)     1481 2023-06-22 21:56:00.000000 uddr_client-0.2.0/src/uddr_client/response.py
+drwxr-xr-x   0 shane     (1000) shane     (1000)        0 2023-06-22 21:58:34.814825 uddr_client-0.2.0/src/uddr_client.egg-info/
+-rw-r--r--   0 shane     (1000) shane     (1000)     4191 2023-06-22 21:58:34.000000 uddr_client-0.2.0/src/uddr_client.egg-info/PKG-INFO
+-rw-r--r--   0 shane     (1000) shane     (1000)      501 2023-06-22 21:58:34.000000 uddr_client-0.2.0/src/uddr_client.egg-info/SOURCES.txt
+-rw-r--r--   0 shane     (1000) shane     (1000)        1 2023-06-22 21:58:34.000000 uddr_client-0.2.0/src/uddr_client.egg-info/dependency_links.txt
+-rw-r--r--   0 shane     (1000) shane     (1000)       53 2023-06-22 21:58:34.000000 uddr_client-0.2.0/src/uddr_client.egg-info/requires.txt
+-rw-r--r--   0 shane     (1000) shane     (1000)       12 2023-06-22 21:58:34.000000 uddr_client-0.2.0/src/uddr_client.egg-info/top_level.txt
```

### Comparing `uddr_client-0.1.0/LICENSE.md` & `uddr_client-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `uddr_client-0.1.0/PKG-INFO` & `uddr_client-0.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uddr_client
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Python client for the UDDR API.
 Home-page: https://github.com/sbarbett/uddr_client
 Author: Shane Barbetta
 Author-email: shane@barbetta.me
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -16,82 +16,137 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 uddr_client
 ======================
 
-A Python library for the UltraDDR API
+A Python SDK for UltraDDR
 
 ## Installation
 
 The package can be installed using pip
 
 ```bash
 pip install uddr_client
 ```
 
 ## Setup
 
-For ease of use, you can store your API key as an environment variable using the client's "setup" method.
+For ease of use, you can store your API key and client ID in an environment file using the client's "setup" method.
 
 ```python
 import uddr_client
-uddr_client.connect.setup('<your API key>')
+uddr_client.connect.setup()
 ```
 
-Alternatively, you can pass the API key directly to the connection.
+Alternatively, you can pass the key or ID directly to the connection using keyword arguments.
 
 ```python
-c = uddr_client.connect('<your API key>')
+c = uddr_client.connect('api_key=<your API key>, client_id=<your client ID>')
 ```
 
-## Usage
+## API Usage
 
 ```python
 import uddr_client
 
-c = uddr_client.connect() # Instantiates a new instance of the client which, by default, uses the API key
-						  # stored in your environment
+c = uddr_client.connect() # Instantiates a new instance of the client which, by default, uses the API key stored in your .env
 
-resp = c.reports()        # Call an endpoint
-print(response)
+resp = c.api().reports()        # Call an endpoint
+print(resp)
 ```
 
 ### Available methods
 
-The client currently supports the following endpoints:
+The API client currently supports the following endpoints:
 
 * `aggregates()`
 * `bar()`
 * `histogram()`
 * `summary()`
 * `report()`
 * `reports()`
 * `histogram_artifact()`
 * `logs()`
 * `passthrough()`
 
 Use Python's help function for more in-depth documentation on each method.
 
 ```python
-help(c.logs)
+help(c.api().logs)
 ```
 
 ### Response parsing
 
 Aside from the `report()` endpoint (which returns an application/pdf), all methods produce a Response object which handles different outputs.
 
 * `Response.xml()`: Outputs the response in XML
 * `Response.csv()`: Outputs the response in CSV
 
 The default is JSON.
 
+## DoH Usage
+
+The DNS over HTTPS (DoH) client provides an interface for directly querying the UDDR resolvers.
+
+```python
+import uddr_client
+
+c = uddr_client.connect() # Instantiates a new instance of the client
+doh = c.doh('google.com') # Creates a DOHClient instance for google.com
+print(doh)                # This will return the full json response
+```
+
+### Record Types
+
+The client stores the response for various DNS record types as properties. The following are supported.
+
+```python
+doh.A      # For A records
+doh.AAAA   # For AAAA records
+doh.CNAME  # For CNAME records
+doh.NS     # For NS records
+doh.MX     # For MX records
+doh.TXT    # For TXT records
+doh.SOA    # For SOA records
+doh.SRV    # For SRV records
+doh.CAA    # For CAA records
+doh.DS     # For DS records
+doh.DNSKEY # For DNSKEY records
+```
+
+### Reverse Lookups
+
+If you pass an IP to the client, it will automatically perform a reverse lookup (PTR). IPv6 support hasn't been added yet.
+
+### IoC Parsing
+
+This concept is borrowed from Michael Smith's [DDR-IOC-Checker](https://github.com/rybolov/DDR-IOC-Checker).
+
+Indicators of compromise passed to the DOHClient as a positional argument will be run through a parser. The parser accepts the following:
+
+1. Domain names
+2. URLs by means of stripping the protocol and path
+3. "Defanged" URLs which are intentionally obfuscated for security reasons
+4. Emails - the parser will remove the prefix and @
+5. IP addresses (not IPv6 yet)
+
+### Additional Methods
+
+The following methods return information about the DoH query or specific parts of the response.
+
+* `status()` - Returns an object with information about the status of the response. DoH provides a numerical code, this expands with a message and description.
+* `block_info()` - Returns a string stating whether the domain is blocked (by checking if the A record resolves to the UDDR block page).
+* `answer()` - Returns the answer section of the response, if one exists.
+* `authority()` - Returns the authority section of the response, if one exists.
+
 ## Dependencies
 
 * pandas
 * xmltodict
+* python-decouple
 
 ## License
 
 This project is licensed under the terms of the MIT license. See LICENSE.md for more details.
```

### Comparing `uddr_client-0.1.0/setup.py` & `uddr_client-0.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="uddr_client", 
-    version="0.1.0",  
+    version="0.2.0",  
     description="A Python client for the UDDR API.", 
     long_description=open("README.md").read(),
     long_description_content_type='text/markdown', 
     author="Shane Barbetta", 
     author_email="shane@barbetta.me",  
     url="https://github.com/sbarbett/uddr_client", 
     license="MIT", 
@@ -19,10 +19,11 @@
         "Programming Language :: Python :: 3.9",
     ],
     package_dir={"": "src"},  
     packages=find_packages(where="src"),  
     python_requires=">=3.7", 
     install_requires=[
         "pandas>=2.0.2",
-        "xmltodict>=0.13.0"
+        "xmltodict>=0.13.0",
+	"python-decouple>=3.8",
     ],
-)
+)
```

### Comparing `uddr_client-0.1.0/src/uddr_client/client.py` & `uddr_client-0.2.0/src/uddr_client/api/api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,15 @@
-from .connection import Connection
-from .response import Response
 import json, datetime, os
 from typing import Dict, List, Optional
+from ..response import Response
+from ..connection import Connection
 
-class Client:
-    def __init__(self, api_key: Optional[str] = None):
-        """Initialize the client.
-        
-        :param api_key: (Optional) UDDR user's API key if not set in the environment
-        """
-        self.connection = Connection(api_key)
-        
-    @staticmethod
-    def setup(api_key: str):
-        """
-        This method stores the user's API key in their environment for later use.
-
-        :param api_key: The user's UDDR API key.
-        """
-        if 'UDDR_API_KEY' in os.environ:
-            overwrite = input('UDDR_API_KEY is already set. Do you want to overwrite it? (y/n): ')
-            if overwrite.lower() != 'y':
-                print('Aborting...')
-                return
-
-        os.environ['UDDR_API_KEY'] = api_key
-        print('UDDR_API_KEY is set.')
+class APIClient:
+    def __init__(self, connection: Connection):
+        self.connection = connection
         
     def _is_valid_date(self, date: str) -> bool:
         """
         Validate if a string is in 'YYYY-MM-DDTHH:MM:SS.sssZ' or 'YYYY-MM-DD' format.
 
         :param date: The string to validate.
         :return: A boolean value. True if the string is a valid date, False otherwise.
```

### Comparing `uddr_client-0.1.0/src/uddr_client/response.py` & `uddr_client-0.2.0/src/uddr_client/response.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 import json
 import pandas as pd
 import xmltodict as xmltd
 from typing import Any, Union, List
 
 class Response:
-    def __init__(self, data: Any) -> None:
+    def __init__(self, data: Any):
         self.data = data
+        
+    def __json__(self):
+        return self.data
 
     def __str__(self) -> str:
-        return json.dumps(self.data)
+        return json.dumps(self.__json__())
 
     def __repr__(self) -> str:
         return self.__str__()
+        
+    def get(self, key: str, default: Any = None) -> Any:
+        """Get an element from the serialized JSON data"""
+        return self.data.get(key, default)
 
     def xml(self) -> str:
         try:
             return xmltd.unparse({'response': self.data})
         except ValueError as e:
             return str(e)
```


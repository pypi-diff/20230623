# Comparing `tmp/BLEST-0.0.6.tar.gz` & `tmp/BLEST-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BLEST-0.0.6.tar", last modified: Sun Jun 18 23:13:54 2023, max compression
+gzip compressed data, was "BLEST-0.0.7.tar", last modified: Fri Jun 23 01:26:19 2023, max compression
```

## Comparing `BLEST-0.0.6.tar` & `BLEST-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 admin      (501) wheel        (0)        0 2023-06-18 23:13:54.012050 BLEST-0.0.6/
-drwxr-xr-x   0 admin      (501) wheel        (0)        0 2023-06-18 23:13:54.011259 BLEST-0.0.6/BLEST.egg-info/
--rw-r--r--   0 admin      (501) wheel        (0)     4101 2023-06-18 23:13:53.000000 BLEST-0.0.6/BLEST.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) wheel        (0)      170 2023-06-18 23:13:54.000000 BLEST-0.0.6/BLEST.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) wheel        (0)        1 2023-06-18 23:13:53.000000 BLEST-0.0.6/BLEST.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) wheel        (0)       34 2023-06-18 23:13:54.000000 BLEST-0.0.6/BLEST.egg-info/requires.txt
--rw-r--r--   0 admin      (501) wheel        (0)        1 2023-06-18 23:13:54.000000 BLEST-0.0.6/BLEST.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) wheel        (0)     1061 2023-06-11 20:34:38.000000 BLEST-0.0.6/LICENSE
--rw-r--r--   0 admin      (501) wheel        (0)     4101 2023-06-18 23:13:54.011694 BLEST-0.0.6/PKG-INFO
--rw-r--r--   0 admin      (501) wheel        (0)     3508 2023-06-18 23:10:16.000000 BLEST-0.0.6/README.md
--rw-r--r--   0 admin      (501) wheel        (0)       38 2023-06-18 23:13:54.012216 BLEST-0.0.6/setup.cfg
--rw-r--r--   0 admin      (501) wheel        (0)      957 2023-06-18 23:10:57.000000 BLEST-0.0.6/setup.py
+drwxr-xr-x   0 admin      (501) wheel        (0)        0 2023-06-23 01:26:19.250604 BLEST-0.0.7/
+drwxr-xr-x   0 admin      (501) wheel        (0)        0 2023-06-23 01:26:19.249598 BLEST-0.0.7/BLEST.egg-info/
+-rw-r--r--   0 admin      (501) wheel        (0)     4125 2023-06-23 01:26:19.000000 BLEST-0.0.7/BLEST.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) wheel        (0)      170 2023-06-23 01:26:19.000000 BLEST-0.0.7/BLEST.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) wheel        (0)        1 2023-06-23 01:26:19.000000 BLEST-0.0.7/BLEST.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) wheel        (0)       37 2023-06-23 01:26:19.000000 BLEST-0.0.7/BLEST.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) wheel        (0)        1 2023-06-23 01:26:19.000000 BLEST-0.0.7/BLEST.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) wheel        (0)     1061 2023-06-11 20:34:38.000000 BLEST-0.0.7/LICENSE
+-rw-r--r--   0 admin      (501) wheel        (0)     4125 2023-06-23 01:26:19.250124 BLEST-0.0.7/PKG-INFO
+-rw-r--r--   0 admin      (501) wheel        (0)     3369 2023-06-23 01:13:48.000000 BLEST-0.0.7/README.md
+-rw-r--r--   0 admin      (501) wheel        (0)       38 2023-06-23 01:26:19.250715 BLEST-0.0.7/setup.cfg
+-rw-r--r--   0 admin      (501) wheel        (0)     1134 2023-06-23 01:24:58.000000 BLEST-0.0.7/setup.py
```

### Comparing `BLEST-0.0.6/BLEST.egg-info/PKG-INFO` & `BLEST-0.0.7/BLEST.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: BLEST
-Version: 0.0.6
-Summary: The Python reference implementation of BLEST (Batch-able, Lightweight, Encrypted State Transfer)
+Version: 0.0.7
+Summary: The Python reference implementation of BLEST (Batch-able, Lightweight, Encrypted State Transfer), an improved communication protocol for web APIs which leverages JSON, supports request batching and selective returns, and provides a modern alternative to REST.
 Home-page: https://github.com/jhuntdev/blest-py
 Author: JHunt
 Author-email: blest@jhunt.dev
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python :: 3
@@ -38,15 +38,15 @@
 
 ```bash
 python3 -m pip install blest
 ```
 
 ## Usage
 
-Use the `create_request_handler` function to create a request handler suitable for use in an existing Python application. Use the `create_http_server` function to create a standalone HTTP server for your request handler. Use the `create_http_client` to create BLEST HTTP clients to interact with other servers.
+Use the `create_request_handler` function to create a request handler suitable for use in an existing Python application. Use the `create_http_server` function to create a standalone HTTP server for your request handler. Use the `create_http_client` function to create a BLEST HTTP client.
 
 ### create_request_handler
 
 The following example uses Flask, but you can find examples with other frameworks [here](examples).
 
 ```python
 from flask import Flask, make_response, request
@@ -131,14 +131,10 @@
   try:
     result = await request('greet', { 'name': 'Steve' }, ['greeting'])
     # Do something with the result
   except Exception as error:
     # Do something in case of error
 ```
 
-## Contributing
-
-We actively welcome pull requests. Learn how to [contribute](CONTRIBUTING.md) for more information.
-
 ## License
 
 This project is licensed under the [MIT License](LICENSE).
```

### Comparing `BLEST-0.0.6/LICENSE` & `BLEST-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `BLEST-0.0.6/PKG-INFO` & `BLEST-0.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: BLEST
-Version: 0.0.6
-Summary: The Python reference implementation of BLEST (Batch-able, Lightweight, Encrypted State Transfer)
+Version: 0.0.7
+Summary: The Python reference implementation of BLEST (Batch-able, Lightweight, Encrypted State Transfer), an improved communication protocol for web APIs which leverages JSON, supports request batching and selective returns, and provides a modern alternative to REST.
 Home-page: https://github.com/jhuntdev/blest-py
 Author: JHunt
 Author-email: blest@jhunt.dev
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python :: 3
@@ -38,15 +38,15 @@
 
 ```bash
 python3 -m pip install blest
 ```
 
 ## Usage
 
-Use the `create_request_handler` function to create a request handler suitable for use in an existing Python application. Use the `create_http_server` function to create a standalone HTTP server for your request handler. Use the `create_http_client` to create BLEST HTTP clients to interact with other servers.
+Use the `create_request_handler` function to create a request handler suitable for use in an existing Python application. Use the `create_http_server` function to create a standalone HTTP server for your request handler. Use the `create_http_client` function to create a BLEST HTTP client.
 
 ### create_request_handler
 
 The following example uses Flask, but you can find examples with other frameworks [here](examples).
 
 ```python
 from flask import Flask, make_response, request
@@ -131,14 +131,10 @@
   try:
     result = await request('greet', { 'name': 'Steve' }, ['greeting'])
     # Do something with the result
   except Exception as error:
     # Do something in case of error
 ```
 
-## Contributing
-
-We actively welcome pull requests. Learn how to [contribute](CONTRIBUTING.md) for more information.
-
 ## License
 
 This project is licensed under the [MIT License](LICENSE).
```

### Comparing `BLEST-0.0.6/README.md` & `BLEST-0.0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 ```bash
 python3 -m pip install blest
 ```
 
 ## Usage
 
-Use the `create_request_handler` function to create a request handler suitable for use in an existing Python application. Use the `create_http_server` function to create a standalone HTTP server for your request handler. Use the `create_http_client` to create BLEST HTTP clients to interact with other servers.
+Use the `create_request_handler` function to create a request handler suitable for use in an existing Python application. Use the `create_http_server` function to create a standalone HTTP server for your request handler. Use the `create_http_client` function to create a BLEST HTTP client.
 
 ### create_request_handler
 
 The following example uses Flask, but you can find examples with other frameworks [here](examples).
 
 ```python
 from flask import Flask, make_response, request
@@ -114,14 +114,10 @@
   try:
     result = await request('greet', { 'name': 'Steve' }, ['greeting'])
     # Do something with the result
   except Exception as error:
     # Do something in case of error
 ```
 
-## Contributing
-
-We actively welcome pull requests. Learn how to [contribute](CONTRIBUTING.md) for more information.
-
 ## License
 
 This project is licensed under the [MIT License](LICENSE).
```


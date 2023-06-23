# Comparing `tmp/cryptoparser-0.9.0.tar.gz` & `tmp/CryptoParser-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptoparser-0.9.0.tar", last modified: Sat Apr 29 12:09:24 2023, max compression
+gzip compressed data, was "CryptoParser-0.9.1.tar", last modified: Fri Jun 23 13:02:47 2023, max compression
```

## Comparing `cryptoparser-0.9.0.tar` & `CryptoParser-0.9.1.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-04-29 12:09:24.511059 cryptoparser-0.9.0/
--rw-r--r--   0 coroner   (1000) coroner   (1000)     8322 2023-04-29 11:18:56.000000 cryptoparser-0.9.0/CHANGELOG.rst
--rw-r--r--   0 coroner   (1000) coroner   (1000)     8617 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/CONTRIBUTING.rst
--rw-r--r--   0 coroner   (1000) coroner   (1000)    16726 2023-04-06 21:12:48.000000 cryptoparser-0.9.0/LICENSE.txt
--rw-r--r--   0 coroner   (1000) coroner   (1000)       39 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/MANIFEST.in
--rw-r--r--   0 coroner   (1000) coroner   (1000)     3263 2023-04-29 12:09:24.511059 cryptoparser-0.9.0/PKG-INFO
--rw-r--r--   0 coroner   (1000) coroner   (1000)      909 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/README.rst
-drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-04-29 12:09:24.504059 cryptoparser-0.9.0/cryptoparser/
--rw-rw-r--   0 coroner   (1000) coroner   (1000)        0 2022-04-23 18:10:38.000000 cryptoparser-0.9.0/cryptoparser/__init__.py
-drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-04-29 12:09:24.507059 cryptoparser-0.9.0/cryptoparser/common/
--rw-rw-r--   0 coroner   (1000) coroner   (1000)        0 2021-04-28 17:35:12.000000 cryptoparser-0.9.0/cryptoparser/common/__init__.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)    29870 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/cryptoparser/common/base.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)     1714 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/cryptoparser/common/classes.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)      655 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/cryptoparser/common/exception.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)      894 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/cryptoparser/common/key.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)    32485 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/cryptoparser/common/parse.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)     1051 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/cryptoparser/common/utils.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)      583 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/cryptoparser/common/x509.py
-drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-04-29 12:09:24.508059 cryptoparser-0.9.0/cryptoparser/httpx/
--rw-r--r--   0 coroner   (1000) coroner   (1000)        0 2022-09-04 16:33:32.000000 cryptoparser-0.9.0/cryptoparser/httpx/__init__.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)    19581 2023-04-29 07:15:22.000000 cryptoparser-0.9.0/cryptoparser/httpx/header.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)    16124 2023-04-29 07:15:22.000000 cryptoparser-0.9.0/cryptoparser/httpx/parse.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)      700 2022-09-04 16:33:32.000000 cryptoparser-0.9.0/cryptoparser/httpx/version.py
-drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-04-29 12:09:24.509059 cryptoparser-0.9.0/cryptoparser/ssh/
--rw-r--r--   0 coroner   (1000) coroner   (1000)        0 2022-09-04 16:33:32.000000 cryptoparser-0.9.0/cryptoparser/ssh/__init__.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)    33359 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/cryptoparser/ssh/key.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)     2201 2023-04-06 21:12:48.000000 cryptoparser-0.9.0/cryptoparser/ssh/record.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)    20265 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/cryptoparser/ssh/subprotocol.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)     6215 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/cryptoparser/ssh/version.py
-drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-04-29 12:09:24.511059 cryptoparser-0.9.0/cryptoparser/tls/
--rw-rw-r--   0 coroner   (1000) coroner   (1000)        0 2021-04-28 17:35:12.000000 cryptoparser-0.9.0/cryptoparser/tls/__init__.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)      884 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/cryptoparser/tls/algorithm.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)      645 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/cryptoparser/tls/ciphersuite.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)    39461 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/cryptoparser/tls/extension.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)     3166 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/cryptoparser/tls/grease.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)     5802 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/cryptoparser/tls/ldap.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)    16107 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/cryptoparser/tls/mysql.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)     7217 2023-04-29 07:52:48.000000 cryptoparser-0.9.0/cryptoparser/tls/openvpn.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)     1618 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/cryptoparser/tls/postgresql.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)     7009 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/cryptoparser/tls/rdp.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)     3953 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/cryptoparser/tls/record.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)    38089 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/cryptoparser/tls/subprotocol.py
--rw-r--r--   0 coroner   (1000) coroner   (1000)     2369 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/cryptoparser/tls/version.py
-drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-04-29 12:09:24.505059 cryptoparser-0.9.0/cryptoparser.egg-info/
--rw-rw-r--   0 coroner   (1000) coroner   (1000)     3263 2023-04-29 12:09:24.000000 cryptoparser-0.9.0/cryptoparser.egg-info/PKG-INFO
--rw-rw-r--   0 coroner   (1000) coroner   (1000)     1159 2023-04-29 12:09:24.000000 cryptoparser-0.9.0/cryptoparser.egg-info/SOURCES.txt
--rw-rw-r--   0 coroner   (1000) coroner   (1000)        1 2023-04-29 12:09:24.000000 cryptoparser-0.9.0/cryptoparser.egg-info/dependency_links.txt
--rw-rw-r--   0 coroner   (1000) coroner   (1000)      268 2023-04-29 12:09:24.000000 cryptoparser-0.9.0/cryptoparser.egg-info/requires.txt
--rw-rw-r--   0 coroner   (1000) coroner   (1000)       13 2023-04-29 12:09:24.000000 cryptoparser-0.9.0/cryptoparser.egg-info/top_level.txt
--rw-r--r--   0 coroner   (1000) coroner   (1000)      127 2023-04-06 21:14:45.000000 cryptoparser-0.9.0/requirements.txt
--rw-r--r--   0 coroner   (1000) coroner   (1000)       38 2023-04-29 12:09:24.512059 cryptoparser-0.9.0/setup.cfg
--rw-r--r--   0 coroner   (1000) coroner   (1000)     3605 2023-04-29 11:22:50.000000 cryptoparser-0.9.0/setup.py
+drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-06-23 13:02:47.644691 CryptoParser-0.9.1/
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     8535 2023-06-23 10:58:57.000000 CryptoParser-0.9.1/CHANGELOG.rst
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     8617 2023-06-19 13:35:22.000000 CryptoParser-0.9.1/CONTRIBUTING.rst
+drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-06-23 13:02:47.637691 CryptoParser-0.9.1/CryptoParser.egg-info/
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     3466 2023-06-23 13:02:47.000000 CryptoParser-0.9.1/CryptoParser.egg-info/PKG-INFO
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     1185 2023-06-23 13:02:47.000000 CryptoParser-0.9.1/CryptoParser.egg-info/SOURCES.txt
+-rw-r--r--   0 coroner   (1000) coroner   (1000)        1 2023-06-23 13:02:47.000000 CryptoParser-0.9.1/CryptoParser.egg-info/dependency_links.txt
+-rw-r--r--   0 coroner   (1000) coroner   (1000)      284 2023-06-23 13:02:47.000000 CryptoParser-0.9.1/CryptoParser.egg-info/requires.txt
+-rw-r--r--   0 coroner   (1000) coroner   (1000)       13 2023-06-23 13:02:47.000000 CryptoParser-0.9.1/CryptoParser.egg-info/top_level.txt
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    16726 2023-04-06 21:12:48.000000 CryptoParser-0.9.1/LICENSE.txt
+-rw-r--r--   0 coroner   (1000) coroner   (1000)       39 2023-06-19 13:35:22.000000 CryptoParser-0.9.1/MANIFEST.in
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     3466 2023-06-23 13:02:47.644691 CryptoParser-0.9.1/PKG-INFO
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     1112 2023-06-23 10:58:57.000000 CryptoParser-0.9.1/README.rst
+drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-06-23 13:02:47.637691 CryptoParser-0.9.1/cryptoparser/
+-rw-rw-r--   0 coroner   (1000) coroner   (1000)        0 2022-04-23 18:10:38.000000 CryptoParser-0.9.1/cryptoparser/__init__.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)      356 2023-06-23 10:58:57.000000 CryptoParser-0.9.1/cryptoparser/__setup__.py
+drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-06-23 13:02:47.639691 CryptoParser-0.9.1/cryptoparser/common/
+-rw-rw-r--   0 coroner   (1000) coroner   (1000)        0 2021-04-28 17:35:12.000000 CryptoParser-0.9.1/cryptoparser/common/__init__.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    30029 2023-06-22 13:58:19.000000 CryptoParser-0.9.1/cryptoparser/common/base.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     1714 2023-06-19 13:35:22.000000 CryptoParser-0.9.1/cryptoparser/common/classes.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)      655 2023-06-19 13:35:22.000000 CryptoParser-0.9.1/cryptoparser/common/exception.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)      894 2023-06-19 13:35:22.000000 CryptoParser-0.9.1/cryptoparser/common/key.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    32881 2023-06-21 13:56:43.000000 CryptoParser-0.9.1/cryptoparser/common/parse.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     1051 2023-06-19 13:35:22.000000 CryptoParser-0.9.1/cryptoparser/common/utils.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     3276 2023-06-22 16:23:07.000000 CryptoParser-0.9.1/cryptoparser/common/x509.py
+drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-06-23 13:02:47.640691 CryptoParser-0.9.1/cryptoparser/httpx/
+-rw-r--r--   0 coroner   (1000) coroner   (1000)        0 2022-09-04 16:33:32.000000 CryptoParser-0.9.1/cryptoparser/httpx/__init__.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    19581 2023-06-19 13:35:22.000000 CryptoParser-0.9.1/cryptoparser/httpx/header.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    16124 2023-06-19 13:35:22.000000 CryptoParser-0.9.1/cryptoparser/httpx/parse.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)      700 2022-09-04 16:33:32.000000 CryptoParser-0.9.1/cryptoparser/httpx/version.py
+drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-06-23 13:02:47.641691 CryptoParser-0.9.1/cryptoparser/ssh/
+-rw-r--r--   0 coroner   (1000) coroner   (1000)        0 2022-09-04 16:33:32.000000 CryptoParser-0.9.1/cryptoparser/ssh/__init__.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    33359 2023-06-19 13:35:22.000000 CryptoParser-0.9.1/cryptoparser/ssh/key.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     2201 2023-04-06 21:12:48.000000 CryptoParser-0.9.1/cryptoparser/ssh/record.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    20265 2023-06-23 07:49:17.000000 CryptoParser-0.9.1/cryptoparser/ssh/subprotocol.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     6215 2023-06-19 13:35:22.000000 CryptoParser-0.9.1/cryptoparser/ssh/version.py
+drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-06-23 13:02:47.643691 CryptoParser-0.9.1/cryptoparser/tls/
+-rw-rw-r--   0 coroner   (1000) coroner   (1000)        0 2021-04-28 17:35:12.000000 CryptoParser-0.9.1/cryptoparser/tls/__init__.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)      884 2023-06-19 13:35:22.000000 CryptoParser-0.9.1/cryptoparser/tls/algorithm.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)      645 2023-06-19 13:35:22.000000 CryptoParser-0.9.1/cryptoparser/tls/ciphersuite.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    39645 2023-06-21 13:56:43.000000 CryptoParser-0.9.1/cryptoparser/tls/extension.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     3166 2023-06-19 13:35:22.000000 CryptoParser-0.9.1/cryptoparser/tls/grease.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     5802 2023-06-19 13:35:22.000000 CryptoParser-0.9.1/cryptoparser/tls/ldap.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    16107 2023-06-19 13:35:22.000000 CryptoParser-0.9.1/cryptoparser/tls/mysql.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     7217 2023-06-19 13:35:22.000000 CryptoParser-0.9.1/cryptoparser/tls/openvpn.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     1618 2023-06-19 13:35:22.000000 CryptoParser-0.9.1/cryptoparser/tls/postgresql.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     7009 2023-06-19 13:35:22.000000 CryptoParser-0.9.1/cryptoparser/tls/rdp.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     3953 2023-06-19 13:35:22.000000 CryptoParser-0.9.1/cryptoparser/tls/record.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    38089 2023-06-19 13:35:22.000000 CryptoParser-0.9.1/cryptoparser/tls/subprotocol.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     2369 2023-06-19 13:35:22.000000 CryptoParser-0.9.1/cryptoparser/tls/version.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)      147 2023-06-23 10:59:11.000000 CryptoParser-0.9.1/requirements.txt
+-rw-r--r--   0 coroner   (1000) coroner   (1000)       38 2023-06-23 13:02:47.644691 CryptoParser-0.9.1/setup.cfg
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     3570 2023-06-23 10:02:10.000000 CryptoParser-0.9.1/setup.py
```

### Comparing `cryptoparser-0.9.0/CHANGELOG.rst` & `CryptoParser-0.9.1/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 Changelog
 =========
 
+0.9.1 - 2022-06-22
+------------------
+
+-  TLS (``tls``)
+
+   -  Generic
+
+      -  add parser for `signed certificate timestamp <https://www.rfc-editor.org/rfc/rfc6962.html#section-3.3.1>`__
+         entries (#52)
+
 0.9.0 - 2023-04-29
 ------------------
 
 -  TLS (``tls``)
 
    -  Generic
```

### Comparing `cryptoparser-0.9.0/CONTRIBUTING.rst` & `CryptoParser-0.9.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.9.0/LICENSE.txt` & `CryptoParser-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.9.0/PKG-INFO` & `CryptoParser-0.9.1/CryptoParser.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cryptoparser
-Version: 0.9.0
+Name: CryptoParser
+Version: 0.9.1
 Summary: Fast and flexible security protocol parser and generator
 Author: Szilárd Pfeiffer
 Author-email: coroner@pfeifferszilard.hu
 Maintainer: Szilárd Pfeiffer
 Maintainer-email: coroner@pfeifferszilard.hu
 License: MPL-2.0
 Project-URL: Homepage, https://gitlab.com/coroner/cryptoparser
@@ -84,7 +84,13 @@
 License
 -------
 
 The code is available under the terms of Mozilla Public License Version 2.0 (MPL 2.0).
 
 A non-comprehensive, but straightforward description of MPL 2.0 can be found at
 `Choose an open source license <https://choosealicense.com/licenses#mpl-2.0>`__ website.
+
+Credits
+-------
+
+-  `NLnet Foundation <https://nlnet.nl>`__ and `NGI Assure <https://www.assure.ngi.eu>`__, supports the project part of
+   the `Next Generation Internet <https://ngi.eu>`__ initiative.
```

### Comparing `cryptoparser-0.9.0/README.rst` & `CryptoParser-0.9.1/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -32,7 +32,13 @@
 License
 -------
 
 The code is available under the terms of Mozilla Public License Version 2.0 (MPL 2.0).
 
 A non-comprehensive, but straightforward description of MPL 2.0 can be found at
 `Choose an open source license <https://choosealicense.com/licenses#mpl-2.0>`__ website.
+
+Credits
+-------
+
+-  `NLnet Foundation <https://nlnet.nl>`__ and `NGI Assure <https://www.assure.ngi.eu>`__, supports the project part of
+   the `Next Generation Internet <https://ngi.eu>`__ initiative.
```

### Comparing `cryptoparser-0.9.0/cryptoparser/common/base.py` & `CryptoParser-0.9.1/cryptoparser/common/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
             else:
                 keys = sorted(dict_value.keys())
         elif hasattr(dict_value, '__dict__'):
             dict_value = dict_value.__dict__
             keys = sorted(filter(lambda key: not key.startswith('_'), dict_value.keys()))
 
         result = OrderedDict([
-            (str(key), dict_value[key])
+            (key, dict_value[key])
             for key in keys
         ])
 
         return result
 
     @staticmethod
     def _json_result(obj):
@@ -131,20 +131,21 @@
         return 4 * level * ' '
 
     @classmethod
     def _markdown_human_readable_names(cls, obj, dict_value):
         name_dict = {}
         fields_dict = attr.fields_dict(type(obj)) if attr.has(type(obj)) else {}
         for name in dict_value:
-            if name in fields_dict and 'human_readable_name' in fields_dict[name].metadata:
-                human_readable_name = fields_dict[name].metadata['human_readable_name']
+            if isinstance(name, six.string_types):
+                if name in fields_dict and 'human_readable_name' in fields_dict[name].metadata:
+                    human_readable_name = fields_dict[name].metadata['human_readable_name']
+                else:
+                    human_readable_name = ' '.join(name.split('_')).title()
             else:
                 _, human_readable_name = cls._markdown_result(name)
-                if not human_readable_name.isupper():
-                    human_readable_name = ' '.join(name.split('_')).title()
             name_dict[name] = human_readable_name
 
         return name_dict
 
     @classmethod
     def _markdown_result_complex(cls, obj, level=0):
         indent = Serializable._markdown_indent_from_level(level)
@@ -188,15 +189,15 @@
                 newline='' if multiline else '\n',
             )
 
         return True, result
 
     @staticmethod
     def _markdown_is_directly_printable(obj):
-        return isinstance(obj, six.string_types + six.integer_types + (float, ))
+        return not isinstance(obj, enum.Enum) and isinstance(obj, six.string_types + six.integer_types + (float, ))
 
     @classmethod
     def _markdown_result(cls, obj, level=0):
         if obj is None:
             result = False, 'n/a'
         elif isinstance(obj, bool):
             result = False, 'yes' if obj else 'no'
@@ -207,14 +208,16 @@
         elif isinstance(obj, enum.Enum):
             if isinstance(obj.value, Serializable):
                 return obj.value._as_markdown(level)  # pylint: disable=protected-access
             if isinstance(obj.value, CryptoDataParamsBase):
                 return False, str(obj.value)
 
             return False, obj.name
+        elif hasattr(obj, '_asdict'):
+            result = cls._markdown_result(obj._asdict(), level)
         elif hasattr(obj, '__dict__') or isinstance(obj, dict):
             result = cls._markdown_result_complex(obj, level)
         elif isinstance(obj, (list, tuple, set, ArrayBase)):
             result = cls._markdown_result_list(obj, level)
         elif isinstance(obj, (bytes, bytearray)):
             result = False, bytes_to_hex_string(obj, separator=':', lowercase=False)
         else:
```

### Comparing `cryptoparser-0.9.0/cryptoparser/common/classes.py` & `CryptoParser-0.9.1/cryptoparser/common/classes.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.9.0/cryptoparser/common/exception.py` & `CryptoParser-0.9.1/cryptoparser/common/exception.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.9.0/cryptoparser/common/key.py` & `CryptoParser-0.9.1/cryptoparser/common/key.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.9.0/cryptoparser/common/parse.py` & `CryptoParser-0.9.1/cryptoparser/common/parse.py`

 * *Files 1% similar despite different names*

```diff
@@ -453,24 +453,29 @@
         self._parsed_length += parsed_length
 
 
 @attr.s
 class ParserBinary(ParserBase):
     byte_order = attr.ib(default=ByteOrder.NETWORK, validator=attr.validators.in_(ByteOrder))
 
-    def parse_timestamp(self, name):
+    def parse_timestamp(self, name, milliseconds=False):
         value, parsed_length = self._parse_numeric_array(name, 1, 8, int)
 
         self._parsed_length += parsed_length
         if value[0] == 0xffffffffffffffff:
             self._parsed_values[name] = None
         else:
-            self._parsed_values[name] = datetime.datetime.fromtimestamp(
-                0x00000000ffffffff & value[0], dateutil.tz.UTC
-            )
+            value = value[0]
+            if milliseconds:
+                millis = value % 1000
+                value //= 1000
+            value = datetime.datetime.fromtimestamp(0x00000000ffffffff & value, dateutil.tz.UTC)
+            if milliseconds:
+                value += datetime.timedelta(milliseconds=millis)
+            self._parsed_values[name] = value
 
     def _parse_numeric_array(self, name, item_num, item_size, item_numeric_class):
         if self._parsed_length + (item_num * item_size) > len(self._parsable):
             raise NotEnoughData(bytes_needed=(item_num * item_size) - self.unparsed_length)
 
         if item_size in _SIZE_TO_FORMAT:
             value = []
@@ -569,15 +574,15 @@
         except ValueError as e:
             six.raise_from(InvalidValue(value, converter, name), e)
         self._parsed_length += len(parsed_bytes)
 
     def parse_raw(self, name, size):
         parsed_bytes = self._parse_bytes(size)
 
-        self._parsed_values[name] = parsed_bytes
+        self._parsed_values[name] = bytearray(parsed_bytes)
         self._parsed_length += size
 
     def parse_string(self, name, item_size, encoding, converter=str):
         value, parsed_length = self._parse_numeric_array(name, 1, item_size, int)
         value = value[0]
         self._parsed_length += parsed_length
 
@@ -778,21 +783,25 @@
         self.compose_numeric(int(value.total_seconds()))
 
 
 @attr.s
 class ComposerBinary(ComposerBase):
     byte_order = attr.ib(default=ByteOrder.NETWORK, validator=attr.validators.in_(ByteOrder))
 
-    def compose_timestamp(self, value):
+    def compose_timestamp(self, value, milliseconds=False):
         if value is None:
-            value = 0xffffffffffffffff
+            timestamp = 0xffffffffffffffff
         else:
-            value = int(time.mktime(value.timetuple())) - time.timezone
+            timestamp = int(time.mktime(value.timetuple())) - time.timezone
+
+            if milliseconds:
+                timestamp *= 1000
+                timestamp += value.microsecond // 1000
 
-        return self._compose_numeric_array([value, ], 8)
+        return self._compose_numeric_array([timestamp, ], 8)
 
     def _compose_numeric_array(self, values, item_size):
         composed_bytes = bytearray()
 
         for value in values:
             try:
                 packed_bytes = struct.pack(
```

### Comparing `cryptoparser-0.9.0/cryptoparser/common/utils.py` & `CryptoParser-0.9.1/cryptoparser/common/utils.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.9.0/cryptoparser/httpx/header.py` & `CryptoParser-0.9.1/cryptoparser/httpx/header.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.9.0/cryptoparser/httpx/parse.py` & `CryptoParser-0.9.1/cryptoparser/httpx/parse.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.9.0/cryptoparser/httpx/version.py` & `CryptoParser-0.9.1/cryptoparser/httpx/version.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.9.0/cryptoparser/ssh/key.py` & `CryptoParser-0.9.1/cryptoparser/ssh/key.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.9.0/cryptoparser/ssh/record.py` & `CryptoParser-0.9.1/cryptoparser/ssh/record.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.9.0/cryptoparser/ssh/subprotocol.py` & `CryptoParser-0.9.1/cryptoparser/ssh/subprotocol.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.9.0/cryptoparser/ssh/version.py` & `CryptoParser-0.9.1/cryptoparser/ssh/version.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.9.0/cryptoparser/tls/algorithm.py` & `CryptoParser-0.9.1/cryptoparser/tls/algorithm.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.9.0/cryptoparser/tls/ciphersuite.py` & `CryptoParser-0.9.1/cryptoparser/tls/ciphersuite.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.9.0/cryptoparser/tls/extension.py` & `CryptoParser-0.9.1/cryptoparser/tls/extension.py`

 * *Files 1% similar despite different names*

```diff
@@ -681,36 +681,34 @@
         return VectorParamParsable(
             item_class=TlsCertificateStatusRequestResponderId,
             fallback_class=None,
             min_byte_num=0, max_byte_num=2 ** 16 - 1
         )
 
 
-class TlsExtensionCertificateStatusRequest(TlsExtensionParsed):
+class TlsExtensionCertificateStatusRequestClient(TlsExtensionParsed):
     def __init__(self, responder_id_list=(), extensions=()):
-        super(TlsExtensionCertificateStatusRequest, self).__init__()
+        super(TlsExtensionCertificateStatusRequestClient, self).__init__()
 
         self.responder_id_list = TlsCertificateStatusRequestResponderIdList(responder_id_list)
         self.request_extensions = TlsCertificateStatusRequestExtensions(extensions)
 
     @classmethod
     def get_extension_type(cls):
         return TlsExtensionType.STATUS_REQUEST
 
     @classmethod
     def _parse(cls, parsable):
-        parser = super(TlsExtensionCertificateStatusRequest, cls)._parse_header(parsable)
-        if parser['extension_length'] == 0:
-            return TlsExtensionCertificateStatusRequest(), parser.parsed_length
+        parser = super(TlsExtensionCertificateStatusRequestClient, cls)._parse_header(parsable)
 
         parser.parse_numeric('status_type', 1, TlsCertificateStatusType)
         parser.parse_parsable('responder_id_list', TlsCertificateStatusRequestResponderIdList)
         parser.parse_parsable('extensions', TlsCertificateStatusRequestExtensions)
 
-        return TlsExtensionCertificateStatusRequest(
+        return cls(
             parser['responder_id_list'],
             parser['extensions'],
         ), parser.parsed_length
 
     def compose(self):
         payload_composer = ComposerBinary()
 
@@ -719,14 +717,20 @@
         payload_composer.compose_parsable(self.request_extensions)
 
         header_bytes = self._compose_header(payload_composer.composed_length)
 
         return header_bytes + payload_composer.composed_bytes
 
 
+class TlsExtensionCertificateStatusRequestServer(TlsExtensionUnusedData):
+    @classmethod
+    def get_extension_type(cls):
+        return TlsExtensionType.STATUS_REQUEST
+
+
 class TlsRenegotiatedConnection(Opaque):
     @classmethod
     def get_param(cls):
         return OpaqueParam(
             min_byte_num=0,
             max_byte_num=2 ** 8 - 1,
         )
@@ -1076,15 +1080,18 @@
     @classmethod
     def get_extension_type(cls):
         return TlsExtensionType.SIGNED_CERTIFICATE_TIMESTAMP
 
 
 @attr.s
 class TlsExtensionSignedCertificateTimestampServer(TlsExtensionParsed):
-    scts = attr.ib(validator=attr.validators.optional(attr.validators.instance_of(SignedCertificateTimestampList)))
+    scts = attr.ib(
+        converter=SignedCertificateTimestampList,
+        validator=attr.validators.optional(attr.validators.instance_of(SignedCertificateTimestampList))
+    )
 
     @classmethod
     def get_extension_type(cls):
         return TlsExtensionType.SIGNED_CERTIFICATE_TIMESTAMP
 
     @classmethod
     def _parse(cls, parsable):
@@ -1163,15 +1170,15 @@
 
     @classmethod
     def _parse(cls, parsable):
         parser = super(TlsExtensionPadding, cls)._parse_header(parsable)
 
         parser.parse_raw('padding', parser['extension_length'])
         try:
-            non_zero_int = next(byte for byte in six.iterbytes(parser['padding']) if byte != 0)
+            non_zero_int = next(byte for byte in parser['padding'] if byte != 0)
             raise InvalidValue(six.int2byte(non_zero_int), cls)
         except StopIteration:
             pass
 
         return cls(parser['extension_length']), parser.parsed_length
 
     def compose(self):
@@ -1216,15 +1223,15 @@
             (TlsExtensionType.ENCRYPT_THEN_MAC, [TlsExtensionEncryptThenMAC, ]),
             (TlsExtensionType.EXTENDED_MASTER_SECRET, [TlsExtensionExtendedMasterSecret, ]),
             (TlsExtensionType.RENEGOTIATION_INFO, [TlsExtensionRenegotiationInfo, ]),
             (TlsExtensionType.NEXT_PROTOCOL_NEGOTIATION, [TlsExtensionNextProtocolNegotiationClient, ]),
             (TlsExtensionType.PADDING, [TlsExtensionPadding, ]),
             (TlsExtensionType.SERVER_NAME, [TlsExtensionServerNameClient, ]),
             (TlsExtensionType.SESSION_TICKET, [TlsExtensionSessionTicket, ]),
-            (TlsExtensionType.STATUS_REQUEST, [TlsExtensionCertificateStatusRequest, ]),
+            (TlsExtensionType.STATUS_REQUEST, [TlsExtensionCertificateStatusRequestClient, ]),
             (TlsExtensionType.SUPPORTED_GROUPS, [TlsExtensionEllipticCurves, ]),
             (TlsExtensionType.DELEGATED_CREDENTIALS, [TlsExtensionDelegatedCredentials, ]),
             (TlsExtensionType.EC_POINT_FORMATS, [TlsExtensionECPointFormats, ]),
             (TlsExtensionType.KEY_SHARE, [TlsExtensionKeyShareClient, ]),
             (TlsExtensionType.KEY_SHARE_RESERVED, [TlsExtensionKeyShareReservedClient, ]),
             (TlsExtensionType.PSK_KEY_EXCHANGE_MODES, [TlsExtensionPskKeyExchangeModes, ]),
             (TlsExtensionType.RECORD_SIZE_LIMIT, [TlsExtensionRecordSizeLimit, ]),
@@ -1250,9 +1257,10 @@
             (TlsExtensionType.KEY_SHARE, [TlsExtensionKeyShareClientHelloRetry, TlsExtensionKeyShareServer]),
             (TlsExtensionType.NEXT_PROTOCOL_NEGOTIATION, [TlsExtensionNextProtocolNegotiationServer, ]),
             (TlsExtensionType.RECORD_SIZE_LIMIT, [TlsExtensionRecordSizeLimit, ]),
             (TlsExtensionType.RENEGOTIATION_INFO, [TlsExtensionRenegotiationInfo, ]),
             (TlsExtensionType.SERVER_NAME, [TlsExtensionServerNameServer, ]),
             (TlsExtensionType.SESSION_TICKET, [TlsExtensionSessionTicket, ]),
             (TlsExtensionType.SIGNED_CERTIFICATE_TIMESTAMP, [TlsExtensionSignedCertificateTimestampServer, ]),
+            (TlsExtensionType.STATUS_REQUEST, [TlsExtensionCertificateStatusRequestServer, ]),
             (TlsExtensionType.SUPPORTED_VERSIONS, [TlsExtensionSupportedVersionsServer, ]),
         ])
```

### Comparing `cryptoparser-0.9.0/cryptoparser/tls/grease.py` & `CryptoParser-0.9.1/cryptoparser/tls/grease.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.9.0/cryptoparser/tls/ldap.py` & `CryptoParser-0.9.1/cryptoparser/tls/ldap.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.9.0/cryptoparser/tls/mysql.py` & `CryptoParser-0.9.1/cryptoparser/tls/mysql.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.9.0/cryptoparser/tls/openvpn.py` & `CryptoParser-0.9.1/cryptoparser/tls/openvpn.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.9.0/cryptoparser/tls/postgresql.py` & `CryptoParser-0.9.1/cryptoparser/tls/postgresql.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.9.0/cryptoparser/tls/rdp.py` & `CryptoParser-0.9.1/cryptoparser/tls/rdp.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.9.0/cryptoparser/tls/record.py` & `CryptoParser-0.9.1/cryptoparser/tls/record.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.9.0/cryptoparser/tls/subprotocol.py` & `CryptoParser-0.9.1/cryptoparser/tls/subprotocol.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.9.0/cryptoparser/tls/version.py` & `CryptoParser-0.9.1/cryptoparser/tls/version.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.9.0/cryptoparser.egg-info/PKG-INFO` & `CryptoParser-0.9.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cryptoparser
-Version: 0.9.0
+Name: CryptoParser
+Version: 0.9.1
 Summary: Fast and flexible security protocol parser and generator
 Author: Szilárd Pfeiffer
 Author-email: coroner@pfeifferszilard.hu
 Maintainer: Szilárd Pfeiffer
 Maintainer-email: coroner@pfeifferszilard.hu
 License: MPL-2.0
 Project-URL: Homepage, https://gitlab.com/coroner/cryptoparser
@@ -84,7 +84,13 @@
 License
 -------
 
 The code is available under the terms of Mozilla Public License Version 2.0 (MPL 2.0).
 
 A non-comprehensive, but straightforward description of MPL 2.0 can be found at
 `Choose an open source license <https://choosealicense.com/licenses#mpl-2.0>`__ website.
+
+Credits
+-------
+
+-  `NLnet Foundation <https://nlnet.nl>`__ and `NGI Assure <https://www.assure.ngi.eu>`__, supports the project part of
+   the `Next Generation Internet <https://ngi.eu>`__ initiative.
```

### Comparing `cryptoparser-0.9.0/cryptoparser.egg-info/SOURCES.txt` & `CryptoParser-0.9.1/CryptoParser.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 CHANGELOG.rst
 CONTRIBUTING.rst
 LICENSE.txt
 MANIFEST.in
 README.rst
 requirements.txt
 setup.py
+CryptoParser.egg-info/PKG-INFO
+CryptoParser.egg-info/SOURCES.txt
+CryptoParser.egg-info/dependency_links.txt
+CryptoParser.egg-info/requires.txt
+CryptoParser.egg-info/top_level.txt
 cryptoparser/__init__.py
-cryptoparser.egg-info/PKG-INFO
-cryptoparser.egg-info/SOURCES.txt
-cryptoparser.egg-info/dependency_links.txt
-cryptoparser.egg-info/requires.txt
-cryptoparser.egg-info/top_level.txt
+cryptoparser/__setup__.py
 cryptoparser/common/__init__.py
 cryptoparser/common/base.py
 cryptoparser/common/classes.py
 cryptoparser/common/exception.py
 cryptoparser/common/key.py
 cryptoparser/common/parse.py
 cryptoparser/common/utils.py
```

### Comparing `cryptoparser-0.9.0/setup.py` & `CryptoParser-0.9.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,65 +3,61 @@
 
 import codecs
 import os
 import unittest
 
 from setuptools import setup
 
+from cryptoparser import __setup__
+
+
 this_directory = os.getenv('REQUIREMENTS_DIR', '')
 with open(os.path.join(this_directory, 'requirements.txt')) as f:
     install_requirements = f.read().splitlines()
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with codecs.open(os.path.join(this_directory, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 
-test_requirements = [
-    "unittest2",
-    "coverage",
-    "six",
-]
-
-
 def test_discover():
     test_loader = unittest.TestLoader()
     test_suite = test_loader.discover('test', pattern='test_*.py')
     return test_suite
 
 
 setup(
-    name='cryptoparser',
-    version='0.9.0',
-    description='Fast and flexible security protocol parser and generator',
+    name=__setup__.__title__,
+    version=__setup__.__version__,
+    description=__setup__.__description__,
     long_description=long_description,
     long_description_content_type='text/x-rst',
-    author='Szilárd Pfeiffer',
-    author_email='coroner@pfeifferszilard.hu',
-    maintainer='Szilárd Pfeiffer',
-    maintainer_email='coroner@pfeifferszilard.hu',
-    license='MPL-2.0',
+    author=__setup__.__author__,
+    author_email=__setup__.__author_email__,
+    maintainer=__setup__.__author__,
+    maintainer_email=__setup__.__author_email__,
+    license=__setup__.__license__,
     license_files=['LICENSE.txt', ],
     project_urls={
-        'Homepage': 'https://gitlab.com/coroner/cryptoparser',
-        'Changelog': 'https://cryptoparser.readthedocs.io/en/latest/changelog',
-        'Documentation': 'https://cryptoparser.readthedocs.io/en/latest/',
-        'Issues': 'https://gitlab.com/coroner/cryptoparser/-/issues',
-        'Source': 'https://gitlab.com/coroner/cryptoparser',
+        'Homepage': __setup__.__url__,
+        'Changelog': 'https://' + __setup__.__technical_name__ + '.readthedocs.io/en/latest/changelog',
+        'Documentation': 'https://' + __setup__.__technical_name__ + '.readthedocs.io/en/latest/',
+        'Issues': __setup__.__url__ + '/-/issues',
+        'Source': __setup__.__url__,
     },
     keywords='ssl tls gost ja3 ldap rdp ssh hsts',
 
     install_requires=install_requirements,
     extras_require={
         ":python_version < '3'": [
             "enum34==1.1.6",
             "pathlib2==2.3.7.post1",
             "Mock",
+            "unittest2",
         ],
-
-        "test": test_requirements,
+        "test": ["coverage", ],
         "pep8": ["flake8", ],
         "pylint": ["pylint", ],
     },
 
     packages=[
         'cryptoparser',
         'cryptoparser.common',
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```


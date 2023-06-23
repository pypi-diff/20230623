# Comparing `tmp/apigeecli-0.8.3.tar.gz` & `tmp/apigeecli-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apigeecli-0.8.3.tar", last modified: Mon Nov  4 12:11:01 2019, max compression
+gzip compressed data, was "dist/apigeecli-0.9.0.tar", last modified: Tue Nov  5 01:28:09 2019, max compression
```

## Comparing `apigeecli-0.8.3.tar` & `apigeecli-0.9.0.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxr-xr-x   0 mssdyn    (1000) mssdyn    (1000)        0 2019-11-04 12:11:01.000000 apigeecli-0.8.3/
--rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)     1518 2019-11-04 03:39:01.000000 apigeecli-0.8.3/setup.py
-drwxr-xr-x   0 mssdyn    (1000) mssdyn    (1000)        0 2019-11-04 12:11:01.000000 apigeecli-0.8.3/apigee/
-drwxr-xr-x   0 mssdyn    (1000) mssdyn    (1000)        0 2019-11-04 12:11:01.000000 apigeecli-0.8.3/apigee/api/
--rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)     1225 2019-10-15 23:27:05.000000 apigeecli-0.8.3/apigee/api/apps.py
--rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)     3934 2019-11-01 04:23:00.000000 apigeecli-0.8.3/apigee/api/permissions.py
--rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)      958 2019-11-01 02:13:13.000000 apigeecli-0.8.3/apigee/api/deployments.py
--rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)     9231 2019-10-13 22:16:39.000000 apigeecli-0.8.3/apigee/api/deploy.py
--rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)     1437 2019-10-15 23:26:57.000000 apigeecli-0.8.3/apigee/api/apis.py
--rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)      210 2019-09-25 22:49:18.000000 apigeecli-0.8.3/apigee/api/__init__.py
--rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)     1040 2019-10-15 23:28:02.000000 apigeecli-0.8.3/apigee/api/targetservers.py
--rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)     6634 2019-11-04 12:02:26.000000 apigeecli-0.8.3/apigee/api/keyvaluemaps.py
--rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)      670 2019-10-15 23:27:26.000000 apigeecli-0.8.3/apigee/api/developers.py
--rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)     2074 2019-10-31 02:24:25.000000 apigeecli-0.8.3/apigee/api/maskconfigs.py
--rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)     1003 2019-10-15 23:26:50.000000 apigeecli-0.8.3/apigee/api/apiproducts.py
--rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)    26005 2019-11-04 03:49:55.000000 apigeecli-0.8.3/apigee/__main__.py
--rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)      666 2019-11-04 12:08:32.000000 apigeecli-0.8.3/apigee/__init__.py
-drwxr-xr-x   0 mssdyn    (1000) mssdyn    (1000)        0 2019-11-04 12:11:01.000000 apigeecli-0.8.3/apigee/util/
--rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)     1973 2019-10-30 07:30:16.000000 apigeecli-0.8.3/apigee/util/__init__.py
--rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)     1514 2019-10-13 22:16:39.000000 apigeecli-0.8.3/apigee/util/mfa_with_pyotp.py
--rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)      661 2019-10-31 21:50:40.000000 apigeecli-0.8.3/apigee/util/prepend.py
--rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)     2184 2019-10-30 06:58:12.000000 apigeecli-0.8.3/apigee/util/config.py
--rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)      660 2019-10-30 07:10:27.000000 apigeecli-0.8.3/apigee/util/authorization.py
-drwxr-xr-x   0 mssdyn    (1000) mssdyn    (1000)        0 2019-11-04 12:11:01.000000 apigeecli-0.8.3/apigeecli.egg-info/
--rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)       34 2019-11-04 12:11:01.000000 apigeecli-0.8.3/apigeecli.egg-info/requires.txt
--rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)        1 2019-11-04 12:11:01.000000 apigeecli-0.8.3/apigeecli.egg-info/dependency_links.txt
--rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)    20874 2019-11-04 12:11:01.000000 apigeecli-0.8.3/apigeecli.egg-info/PKG-INFO
--rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)        7 2019-11-04 12:11:01.000000 apigeecli-0.8.3/apigeecli.egg-info/top_level.txt
--rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)      651 2019-11-04 12:11:01.000000 apigeecli-0.8.3/apigeecli.egg-info/SOURCES.txt
--rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)       49 2019-11-04 12:11:01.000000 apigeecli-0.8.3/apigeecli.egg-info/entry_points.txt
--rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)    20874 2019-11-04 12:11:01.000000 apigeecli-0.8.3/PKG-INFO
--rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)    16955 2019-11-04 12:01:00.000000 apigeecli-0.8.3/README.rst
--rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)       38 2019-11-04 12:11:01.000000 apigeecli-0.8.3/setup.cfg
+drwxr-xr-x   0 mssdyn    (1000) mssdyn    (1000)        0 2019-11-05 01:28:09.000000 apigeecli-0.9.0/
+-rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)     1518 2019-11-04 03:39:01.000000 apigeecli-0.9.0/setup.py
+drwxr-xr-x   0 mssdyn    (1000) mssdyn    (1000)        0 2019-11-05 01:28:09.000000 apigeecli-0.9.0/apigee/
+drwxr-xr-x   0 mssdyn    (1000) mssdyn    (1000)        0 2019-11-05 01:28:09.000000 apigeecli-0.9.0/apigee/api/
+-rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)     1225 2019-10-15 23:27:05.000000 apigeecli-0.9.0/apigee/api/apps.py
+-rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)     3934 2019-11-01 04:23:00.000000 apigeecli-0.9.0/apigee/api/permissions.py
+-rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)      958 2019-11-01 02:13:13.000000 apigeecli-0.9.0/apigee/api/deployments.py
+-rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)     9231 2019-10-13 22:16:39.000000 apigeecli-0.9.0/apigee/api/deploy.py
+-rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)     1437 2019-10-15 23:26:57.000000 apigeecli-0.9.0/apigee/api/apis.py
+-rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)      210 2019-09-25 22:49:18.000000 apigeecli-0.9.0/apigee/api/__init__.py
+-rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)     2739 2019-11-05 01:20:09.000000 apigeecli-0.9.0/apigee/api/targetservers.py
+-rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)     6623 2019-11-04 23:54:37.000000 apigeecli-0.9.0/apigee/api/keyvaluemaps.py
+-rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)      670 2019-10-15 23:27:26.000000 apigeecli-0.9.0/apigee/api/developers.py
+-rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)     2074 2019-10-31 02:24:25.000000 apigeecli-0.9.0/apigee/api/maskconfigs.py
+-rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)     1003 2019-10-15 23:26:50.000000 apigeecli-0.9.0/apigee/api/apiproducts.py
+drwxr-xr-x   0 mssdyn    (1000) mssdyn    (1000)        0 2019-11-05 01:28:09.000000 apigeecli-0.9.0/apigee/parsers/
+-rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)      210 2019-11-04 20:41:39.000000 apigeecli-0.9.0/apigee/parsers/__init__.py
+-rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)     3179 2019-11-04 23:23:10.000000 apigeecli-0.9.0/apigee/parsers/parent_parser.py
+-rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)    25882 2019-11-05 01:16:40.000000 apigeecli-0.9.0/apigee/__main__.py
+-rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)      666 2019-11-05 01:26:46.000000 apigeecli-0.9.0/apigee/__init__.py
+drwxr-xr-x   0 mssdyn    (1000) mssdyn    (1000)        0 2019-11-05 01:28:09.000000 apigeecli-0.9.0/apigee/util/
+-rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)     1973 2019-10-30 07:30:16.000000 apigeecli-0.9.0/apigee/util/__init__.py
+-rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)     1514 2019-10-13 22:16:39.000000 apigeecli-0.9.0/apigee/util/mfa_with_pyotp.py
+-rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)      661 2019-10-31 21:50:40.000000 apigeecli-0.9.0/apigee/util/prepend.py
+-rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)     2184 2019-10-30 06:58:12.000000 apigeecli-0.9.0/apigee/util/config.py
+-rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)      660 2019-10-30 07:10:27.000000 apigeecli-0.9.0/apigee/util/authorization.py
+drwxr-xr-x   0 mssdyn    (1000) mssdyn    (1000)        0 2019-11-05 01:28:09.000000 apigeecli-0.9.0/apigeecli.egg-info/
+-rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)       34 2019-11-05 01:28:08.000000 apigeecli-0.9.0/apigeecli.egg-info/requires.txt
+-rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)        1 2019-11-05 01:28:08.000000 apigeecli-0.9.0/apigeecli.egg-info/dependency_links.txt
+-rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)    20844 2019-11-05 01:28:08.000000 apigeecli-0.9.0/apigeecli.egg-info/PKG-INFO
+-rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)        7 2019-11-05 01:28:08.000000 apigeecli-0.9.0/apigeecli.egg-info/top_level.txt
+-rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)      710 2019-11-05 01:28:09.000000 apigeecli-0.9.0/apigeecli.egg-info/SOURCES.txt
+-rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)       49 2019-11-05 01:28:08.000000 apigeecli-0.9.0/apigeecli.egg-info/entry_points.txt
+-rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)    20844 2019-11-05 01:28:09.000000 apigeecli-0.9.0/PKG-INFO
+-rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)    16925 2019-11-05 01:24:02.000000 apigeecli-0.9.0/README.rst
+-rw-r--r--   0 mssdyn    (1000) mssdyn    (1000)       38 2019-11-05 01:28:09.000000 apigeecli-0.9.0/setup.cfg
```

### Comparing `apigeecli-0.8.3/setup.py` & `apigeecli-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `apigeecli-0.8.3/apigee/api/apps.py` & `apigeecli-0.9.0/apigee/api/apps.py`

 * *Files identical despite different names*

### Comparing `apigeecli-0.8.3/apigee/api/permissions.py` & `apigeecli-0.9.0/apigee/api/permissions.py`

 * *Files identical despite different names*

### Comparing `apigeecli-0.8.3/apigee/api/deployments.py` & `apigeecli-0.9.0/apigee/api/deployments.py`

 * *Files identical despite different names*

### Comparing `apigeecli-0.8.3/apigee/api/deploy.py` & `apigeecli-0.9.0/apigee/api/deploy.py`

 * *Files identical despite different names*

### Comparing `apigeecli-0.8.3/apigee/api/apis.py` & `apigeecli-0.9.0/apigee/api/apis.py`

 * *Files identical despite different names*

### Comparing `apigeecli-0.8.3/apigee/api/targetservers.py` & `apigeecli-0.9.0/apigee/api/apiproducts.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 #!/usr/bin/env python
-"""https://apidocs.apigee.com/api/api_resources/51-targetservers"""
+"""https://apidocs.apigee.com/api/api-products-1"""
 
 import requests
 import json
 
 from apigee import APIGEE_ADMIN_API_URL
 from apigee.util import authorization
 
-def list_targetservers_in_an_environment(args):
-    uri = '{}/v1/organizations/{}/environments/{}/targetservers'.format(
-        APIGEE_ADMIN_API_URL, args.org, args.environment)
+def get_api_product(args):
+    uri = '{}/v1/organizations/{}/apiproducts/{}'.format(
+        APIGEE_ADMIN_API_URL, args.org, args.name)
     hdrs = authorization.set_header({'Accept': 'application/json'}, args)
     resp = requests.get(uri, headers=hdrs)
     resp.raise_for_status()
     # print(resp.status_code)
-    if args.prefix:
-        return json.dumps([i for i in resp.json() if i.startswith(args.prefix)])
-    return resp.text
+    return resp
 
-def get_targetserver(args):
-    uri = '{}/v1/organizations/{}/environments/{}/targetservers/{}'.format(
-        APIGEE_ADMIN_API_URL, args.org, args.environment, args.name)
+def list_api_products(args):
+    uri = '{}/v1/organizations/{}/apiproducts?expand={}&count={}&startKey={}'.format(
+        APIGEE_ADMIN_API_URL, args.org, args.expand, args.count, args.startkey)
     hdrs = authorization.set_header({'Accept': 'application/json'}, args)
     resp = requests.get(uri, headers=hdrs)
     resp.raise_for_status()
     # print(resp.status_code)
-    return resp
+    if args.prefix:
+        return json.dumps([i for i in resp.json() if i.startswith(args.prefix)])
+    return resp.text
```

### Comparing `apigeecli-0.8.3/apigee/api/keyvaluemaps.py` & `apigeecli-0.9.0/apigee/api/keyvaluemaps.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import progressbar
 
 from apigee import APIGEE_ADMIN_API_URL
 from apigee.util import authorization
 
 def create_keyvaluemap_in_an_environment(args):
     uri = '{}/v1/organizations/{}/environments/{}/keyvaluemaps'.format(
-        APIGEE_ADMIN_API_URL, args.org, args.environment, args.name)
+        APIGEE_ADMIN_API_URL, args.org, args.environment)
     hdrs = authorization.set_header({'Accept': 'application/json', 'Content-Type': 'application/json'}, args)
     body = json.loads(args.body)
     resp = requests.post(uri, headers=hdrs, json=body)
     resp.raise_for_status()
     # print(resp.status_code)
     return resp
```

### Comparing `apigeecli-0.8.3/apigee/api/developers.py` & `apigeecli-0.9.0/apigee/api/developers.py`

 * *Files identical despite different names*

### Comparing `apigeecli-0.8.3/apigee/api/maskconfigs.py` & `apigeecli-0.9.0/apigee/api/maskconfigs.py`

 * *Files identical despite different names*

### Comparing `apigeecli-0.8.3/apigee/__main__.py` & `apigeecli-0.9.0/apigee/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,60 +1,23 @@
 #!/usr/bin/env python
 """apigee"""
 
 import argparse
-import os
-import sys
 
 import apigee
 
-from apigee import APIGEE_CLI_CREDS
 from apigee import APIGEE_CLI_PREFIX
-from apigee import APIGEE_ORG
-from apigee import APIGEE_USERNAME
-from apigee import APIGEE_PASSWORD
-from apigee import APIGEE_MFA_SECRET
 from apigee.api import *
+from apigee.parsers.parent_parser import ParentParser
 from apigee.util import *
 
 @exception_handler
 def main():
-    parent_parser = argparse.ArgumentParser(add_help=False)
-    parent_parser.add_argument('-P', '--profile', action='store', help='name of credentials profile', default='default')
-
-    profile = parent_parser.parse_known_args()[0].profile
-
-    mfa_secret = authorization.get_credential(profile, 'mfa_secret')
-    org = authorization.get_credential(profile, 'org')
-    username = authorization.get_credential(profile, 'username')
-    password = authorization.get_credential(profile, 'password')
-    prefix = authorization.get_credential(profile, 'prefix')
-
-    parent_parser.add_argument('--mfa-secret', action='store', help='apigee mfa secret', required=False, default=APIGEE_MFA_SECRET if mfa_secret is None else mfa_secret)
-
-    if org:
-        parent_parser.add_argument('-o', '--org', action='store', help='apigee org', required=False, default=org)
-    elif APIGEE_ORG:
-        parent_parser.add_argument('-o', '--org', action='store', help='apigee org', required=False, default=APIGEE_ORG)
-    else:
-        parent_parser.add_argument('-o', '--org', action='store', help='apigee org', required=True)
-
-    if username:
-        parent_parser.add_argument('-u', '--username', action='store', help='apigee username', required=False, default=username)
-    elif APIGEE_USERNAME:
-        parent_parser.add_argument('-u', '--username', action='store', help='apigee username', required=False, default=APIGEE_USERNAME)
-    else:
-        parent_parser.add_argument('-u', '--username', action='store', help='apigee username', required=True)
-
-    if password:
-        parent_parser.add_argument('-p', '--password', action='store', help='apigee password', required=False, default=password)
-    elif APIGEE_PASSWORD:
-        parent_parser.add_argument('-p', '--password', action='store', help='apigee password', required=False, default=APIGEE_PASSWORD)
-    else:
-        parent_parser.add_argument('-p', '--password', action='store', help='apigee password', required=True)
+    parent_parser = ParentParser()
+    prefix = authorization.get_credential(parent_parser.profile, 'prefix')
 
     file_parser = argparse.ArgumentParser(add_help=False)
     file_parser.add_argument('-f', '--file', action='store', help='file path', required=True, type=isfile)
 
     dir_parser = argparse.ArgumentParser(add_help=False)
     dir_parser.add_argument('-d', '--directory', action='store', help='directory path', required=True, type=isdir)
 
@@ -67,226 +30,246 @@
     prefix_parser = argparse.ArgumentParser(add_help=False)
     prefix_parser.add_argument('--prefix', help='prefix filter for apigee items', default=APIGEE_CLI_PREFIX if prefix is None else prefix)
 
     parser = argparse.ArgumentParser(prog=apigee.CMD, description=apigee.description)
     parser.add_argument('-V', '--version', action='version', version=apigee.APP + ' ' + apigee.__version__)
     subparsers = parser.add_subparsers()
 
-    parser_test = subparsers.add_parser('test', help='test get access token', parents=[parent_parser])
+    parser_test = subparsers.add_parser('test', help='test get access token', parents=[parent_parser()])
     parser_test.set_defaults(func=test)
 
     parser_configure = subparsers.add_parser('configure', help='configure credentials')
     parser_configure.add_argument('-P', '--profile', help='name of profile to create', default='default')
     parser_configure.set_defaults(func=config.main)
 
     parser_apis = subparsers.add_parser('apis', help='apis').add_subparsers()
     parser_deployments = subparsers.add_parser('deployments', aliases=['deps'], help='see apis that are actively deployed').add_subparsers()
     parser_keyvaluemaps = subparsers.add_parser('kvms', aliases=['keyvaluemaps'], help='keyvaluemaps').add_subparsers()
     parser_developers = subparsers.add_parser('developers', aliases=['devs'], help='developers').add_subparsers()
     parser_apps = subparsers.add_parser('apps', help='developer apps').add_subparsers()
     parser_apiproducts = subparsers.add_parser('products', aliases=['prods'], help='api products').add_subparsers()
     parser_targetservers = subparsers.add_parser('ts', aliases=['targetservers'], help='target servers').add_subparsers()
     parser_maskconfigs = subparsers.add_parser('mask', aliases=['maskconfigs'], help='data masks').add_subparsers()
-    parser_permissions = subparsers.add_parser('perms', aliases=['permissions'], help='set a permission for a role').add_subparsers()
+    parser_permissions = subparsers.add_parser('perms', aliases=['permissions'], help='manage permissions for a role').add_subparsers()
 
     parser_prepend = subparsers.add_parser('prepend', aliases=['prefix'], help='prepend all matching strings with a prefix in all files in the specified directory (rudimentary stream editor). this is potentially VERY DANGEROUS. make sure you have version control such as Git to revert any changes in the target directory.', parents=[dir_parser])
     parser_prepend.add_argument('-P', '--prefix', help='prefix to prepend', required=True)
     parser_prepend.add_argument('-r', '--resource', help='apigee resource to be prepended', required=True)
     parser_prepend.set_defaults(func=prepend.main)
 
-    apis_deploy = parser_apis.add_parser('deploy', help='deploy apis', parents=[parent_parser, dir_parser, environment_parser])
+    apis_deploy = parser_apis.add_parser('deploy', help='deploy apis', parents=[parent_parser(), dir_parser, environment_parser])
     apis_deploy.add_argument('-n', '--name', help='name', required=True)
     # apis_deploy.add_argument('-d', '--directory', help='directory name')
     # apis_deploy.add_argument('-p', '--path', help='base path')
     apis_deploy.add_argument('-i', '--import-only', action='store_true', help='denotes to import only and not actually deploy')
     apis_deploy.add_argument('-s', '--seamless-deploy', action='store_true', help='seamless deploy the bundle')
     apis_deploy.set_defaults(func=deploy.deploy)
 
-    export_api_proxy = parser_apis.add_parser('export', aliases=['export-api-proxy'], parents=[parent_parser],
+    export_api_proxy = parser_apis.add_parser('export', aliases=['export-api-proxy'], parents=[parent_parser()],
         help='Outputs an API proxy revision as a ZIP formatted bundle of code and config files. This enables local configuration and development, including attachment of policies and scripts.')
     export_api_proxy.add_argument('-n', '--name', help='name', required=True)
     export_api_proxy.add_argument('-r', '--revision-number', help='revision number', required=True)
     export_api_proxy.add_argument('-O', '--output-file', help='output file')
     # export_api_proxy.set_defaults(func=lambda args: print(apis.export_api_proxy(args).text))
     export_api_proxy.set_defaults(func=apis.export_api_proxy)
 
-    get_api_proxy = parser_apis.add_parser('get', aliases=['get-api-proxy'], parents=[parent_parser],
+    get_api_proxy = parser_apis.add_parser('get', aliases=['get-api-proxy'], parents=[parent_parser()],
         help='Gets an API proxy by name, including a list of existing revisions of the proxy.')
     get_api_proxy.add_argument('-n', '--name', help='name', required=True)
     get_api_proxy.set_defaults(func=lambda args: print(apis.get_api_proxy(args).text))
 
-    list_api_proxies = parser_apis.add_parser('list', aliases=['list-api-proxies'], parents=[parent_parser, prefix_parser],
+    list_api_proxies = parser_apis.add_parser('list', aliases=['list-api-proxies'], parents=[parent_parser(), prefix_parser],
         help='Gets the names of all API proxies in an organization. The names correspond to the names defined in the configuration files for each API proxy.')
     list_api_proxies.set_defaults(func=lambda args: print(apis.list_api_proxies(args)))
 
-    get_api_proxy_deployment_details = parser_deployments.add_parser('get', aliases=['get-api-proxy-deployment-details'], parents=[parent_parser],
+    get_api_proxy_deployment_details = parser_deployments.add_parser('get', aliases=['get-api-proxy-deployment-details'], parents=[parent_parser()],
         help='Returns detail on all deployments of the API proxy for all environments. All deployments are listed in the test and prod environments, as well as other environments, if they exist.')
     get_api_proxy_deployment_details.add_argument('-n', '--name', help='name', required=True)
     get_api_proxy_deployment_details.add_argument('-r', '--revision-name', action='store_true', help='get revisions only')
     get_api_proxy_deployment_details.add_argument('-j', '--json', action='store_true', help='use json output')
     get_api_proxy_deployment_details.add_argument('--max-colwidth', help='max column width', type=int, default=40)
     get_api_proxy_deployment_details.set_defaults(func=lambda args: print(deployments.get_api_proxy_deployment_details(args)))
 
-    create_keyvaluemap_in_an_environment = parser_keyvaluemaps.add_parser('create', aliases=['create-keyvaluemap-in-an-environment'], parents=[parent_parser, environment_parser],
+    create_keyvaluemap_in_an_environment = parser_keyvaluemaps.add_parser('create', aliases=['create-keyvaluemap-in-an-environment'], parents=[parent_parser(), environment_parser],
         help='Creates a key value map in an environment.')
-    create_keyvaluemap_in_an_environment.add_argument('-n', '--name', help='name', required=True)
     create_keyvaluemap_in_an_environment.add_argument('-b', '--body', help='request body', required=True)
     create_keyvaluemap_in_an_environment.set_defaults(func=lambda args: print(keyvaluemaps.create_keyvaluemap_in_an_environment(args).text))
 
-    delete_keyvaluemap_from_an_environment = parser_keyvaluemaps.add_parser('delete', aliases=['delete-keyvaluemap-from-an-environment'], parents=[parent_parser, environment_parser],
+    delete_keyvaluemap_from_an_environment = parser_keyvaluemaps.add_parser('delete', aliases=['delete-keyvaluemap-from-an-environment'], parents=[parent_parser(), environment_parser],
         help='Deletes a key/value map and all associated entries from an environment.')
     delete_keyvaluemap_from_an_environment.add_argument('-n', '--name', help='name', required=True)
     delete_keyvaluemap_from_an_environment.set_defaults(func=lambda args: print(keyvaluemaps.delete_keyvaluemap_from_an_environment(args).text))
 
-    delete_keyvaluemap_entry_in_an_environment = parser_keyvaluemaps.add_parser('delete-entry', aliases=['delete-keyvaluemap-entry-in-an-environment'], parents=[parent_parser, environment_parser],
+    delete_keyvaluemap_entry_in_an_environment = parser_keyvaluemaps.add_parser('delete-entry', aliases=['delete-keyvaluemap-entry-in-an-environment'], parents=[parent_parser(), environment_parser],
         help='Deletes a specific key/value map entry in an environment by name, along with associated entries.')
     delete_keyvaluemap_entry_in_an_environment.add_argument('-n', '--name', help='name', required=True)
     delete_keyvaluemap_entry_in_an_environment.add_argument('--entry-name', help='entry name', required=True)
     delete_keyvaluemap_entry_in_an_environment.set_defaults(func=lambda args: print(keyvaluemaps.delete_keyvaluemap_entry_in_an_environment(args).text))
 
-    get_keyvaluemap_in_an_environment = parser_keyvaluemaps.add_parser('get', aliases=['get-keyvaluemap-in-an-environment'], parents=[parent_parser, environment_parser],
+    get_keyvaluemap_in_an_environment = parser_keyvaluemaps.add_parser('get', aliases=['get-keyvaluemap-in-an-environment'], parents=[parent_parser(), environment_parser],
         help='Gets a KeyValueMap (KVM) in an environment by name, along with the keys and values.')
     get_keyvaluemap_in_an_environment.add_argument('-n', '--name', help='name', required=True)
     get_keyvaluemap_in_an_environment.set_defaults(func=lambda args: print(keyvaluemaps.get_keyvaluemap_in_an_environment(args).text))
 
-    get_a_keys_value_in_an_environment_scoped_keyvaluemap = parser_keyvaluemaps.add_parser('get-value', aliases=['get-a-keys-value-in-an-environment-scoped-keyvaluemap'], parents=[parent_parser, environment_parser],
+    get_a_keys_value_in_an_environment_scoped_keyvaluemap = parser_keyvaluemaps.add_parser('get-value', aliases=['get-a-keys-value-in-an-environment-scoped-keyvaluemap'], parents=[parent_parser(), environment_parser],
         help='Gets the value of a key in an environment-scoped KeyValueMap (KVM).')
     get_a_keys_value_in_an_environment_scoped_keyvaluemap.add_argument('-n', '--name', help='name', required=True)
     get_a_keys_value_in_an_environment_scoped_keyvaluemap.add_argument('--entry-name', help='entry name', required=True)
     get_a_keys_value_in_an_environment_scoped_keyvaluemap.set_defaults(func=lambda args: print(keyvaluemaps.get_a_keys_value_in_an_environment_scoped_keyvaluemap(args).text))
 
-    list_keyvaluemaps_in_an_environment = parser_keyvaluemaps.add_parser('list', aliases=['list-keyvaluemaps-in-an-environment'], parents=[parent_parser, environment_parser, prefix_parser],
+    list_keyvaluemaps_in_an_environment = parser_keyvaluemaps.add_parser('list', aliases=['list-keyvaluemaps-in-an-environment'], parents=[parent_parser(), environment_parser, prefix_parser],
         help='Lists the name of all key/value maps in an environment and optionally returns an expanded view of all key/value maps for the environment.')
     list_keyvaluemaps_in_an_environment.set_defaults(func=lambda args: print(keyvaluemaps.list_keyvaluemaps_in_an_environment(args)))
 
-    update_keyvaluemap_in_an_environment = parser_keyvaluemaps.add_parser('update', aliases=['update-keyvaluemap-in-an-environment'], parents=[parent_parser, environment_parser],
+    update_keyvaluemap_in_an_environment = parser_keyvaluemaps.add_parser('update', aliases=['update-keyvaluemap-in-an-environment'], parents=[parent_parser(), environment_parser],
         help='Note: This API is supported for Apigee Edge for Private Cloud only. For Apigee Edge for Public Cloud use Update an entry in an environment-scoped KVM. Updates an existing KeyValueMap in an environment. Does not override the existing map. Instead, this method updates the entries if they exist or adds them if not. It can take several minutes before the new value is visible to runtime traffic.')
     update_keyvaluemap_in_an_environment.add_argument('-n', '--name', help='name', required=True)
     update_keyvaluemap_in_an_environment.add_argument('-b', '--body', help='request body', required=True)
     update_keyvaluemap_in_an_environment.set_defaults(func=lambda args: print(keyvaluemaps.update_keyvaluemap_in_an_environment(args).text))
 
-    create_an_entry_in_an_environment_scoped_kvm = parser_keyvaluemaps.add_parser('create-entry', aliases=['create-an-entry-in-an-environment-scoped-kvm'], parents=[parent_parser, environment_parser],
+    create_an_entry_in_an_environment_scoped_kvm = parser_keyvaluemaps.add_parser('create-entry', aliases=['create-an-entry-in-an-environment-scoped-kvm'], parents=[parent_parser(), environment_parser],
         help='Note: This API is supported for Apigee Edge for the Public Cloud only. Creates an entry in an existing KeyValueMap scoped to an environment. A key (name) cannot be larger than 2 KB. KVM names are case sensitive.')
     create_an_entry_in_an_environment_scoped_kvm.add_argument('-n', '--name', help='name', required=True)
     create_an_entry_in_an_environment_scoped_kvm.add_argument('--entry-name', help='entry name', required=True)
     create_an_entry_in_an_environment_scoped_kvm.add_argument('--entry-value', help='entry value', required=True)
     create_an_entry_in_an_environment_scoped_kvm.set_defaults(func=lambda args: print(keyvaluemaps.create_an_entry_in_an_environment_scoped_kvm(args).text))
 
-    update_an_entry_in_an_environment_scoped_kvm = parser_keyvaluemaps.add_parser('update-entry', aliases=['update-an-entry-in-an-environment-scoped-kvm'], parents=[parent_parser, environment_parser],
+    update_an_entry_in_an_environment_scoped_kvm = parser_keyvaluemaps.add_parser('update-entry', aliases=['update-an-entry-in-an-environment-scoped-kvm'], parents=[parent_parser(), environment_parser],
         help='Note: This API is supported for Apigee Edge for the Public Cloud only. Updates an entry in a KeyValueMap scoped to an environment. A key cannot be larger than 2 KB. KVM names are case sensitive. Does not override the existing map. It can take several minutes before the new value is visible to runtime traffic.')
     update_an_entry_in_an_environment_scoped_kvm.add_argument('-n', '--name', help='name', required=True)
     update_an_entry_in_an_environment_scoped_kvm.add_argument('--entry-name', help='entry name', required=True)
     update_an_entry_in_an_environment_scoped_kvm.add_argument('--updated-value', help='updated value', required=True)
     update_an_entry_in_an_environment_scoped_kvm.set_defaults(func=lambda args: print(keyvaluemaps.update_an_entry_in_an_environment_scoped_kvm(args).text))
 
-    list_keys_in_an_environment_scoped_keyvaluemap = parser_keyvaluemaps.add_parser('list-keys', aliases=['list-keys-in-an-environment-scoped-keyvaluemap'], parents=[parent_parser, environment_parser, prefix_parser],
+    list_keys_in_an_environment_scoped_keyvaluemap = parser_keyvaluemaps.add_parser('list-keys', aliases=['list-keys-in-an-environment-scoped-keyvaluemap'], parents=[parent_parser(), environment_parser, prefix_parser],
         help='Note: This API is supported for Apigee Edge for the Public Cloud only. Lists keys in a KeyValueMap scoped to an environment. KVM names are case sensitive.')
     list_keys_in_an_environment_scoped_keyvaluemap.add_argument('-n', '--name', help='name', required=True)
     list_keys_in_an_environment_scoped_keyvaluemap.add_argument('--startkey', default='',
         help='To filter the keys that are returned, enter the name of a key that the list will start with.')
     list_keys_in_an_environment_scoped_keyvaluemap.add_argument('--count', default=100, type=int,
         help='Limits the list of keys to the number you specify, up to a maximum of 100. Use with the startkey parameter to provide more targeted filtering.')
     list_keys_in_an_environment_scoped_keyvaluemap.set_defaults(func=lambda args: print(keyvaluemaps.list_keys_in_an_environment_scoped_keyvaluemap(args)))
 
-    push_keyvaluemap = parser_keyvaluemaps.add_parser('push', aliases=['push-keyvaluemap'], parents=[parent_parser, environment_parser, file_parser],
-        help='Magically Push KeyValueMap to Apigee. This will create KeyValueMap/entries if they do not exist, update existing KeyValueMap/entries, and delete entries on Apigee that are not present in the request body.')
+    push_keyvaluemap = parser_keyvaluemaps.add_parser('push', aliases=['push-keyvaluemap'], parents=[parent_parser(), environment_parser, file_parser],
+        help='Push KeyValueMap to Apigee. This will create KeyValueMap/entries if they do not exist, update existing KeyValueMap/entries, and delete entries on Apigee that are not present in the request body.')
     # push_keyvaluemap.add_argument('-n', '--name', help='name', required=True)
     push_keyvaluemap.set_defaults(func=lambda args: keyvaluemaps.push_keyvaluemap(args))
 
-    list_developers = parser_developers.add_parser('list', aliases=['list-developers'], parents=[parent_parser, prefix_parser],
+    list_developers = parser_developers.add_parser('list', aliases=['list-developers'], parents=[parent_parser(), prefix_parser],
         help='Lists all developers in an organization by email address. This call does not list any company developers who are a part of the designated organization.')
     list_developers.add_argument('--expand', action='store_true',
         help='Set to true to list developers exanded with details.')
     list_developers.add_argument('--count', default=1000, type=int,
         help='Limits the list to the number you specify. Use with the startKey parameter to provide more targeted filtering. The limit is 1000.')
     list_developers.add_argument('--startkey', default='',
         help='To filter the keys that are returned, enter the email of a developer that the list will start with.')
     list_developers.set_defaults(func=lambda args: print(developers.list_developers(args)))
 
-    list_developer_apps = parser_apps.add_parser('list', aliases=['list-developer-apps'], parents=[parent_parser, prefix_parser],
+    list_developer_apps = parser_apps.add_parser('list', aliases=['list-developer-apps'], parents=[parent_parser(), prefix_parser],
         help='Lists all apps created by a developer in an organization, and optionally provides an expanded view of the apps. All time values in the response are UNIX times. You can specify either the developer\'s email address or Edge ID.')
     list_developer_apps.add_argument('-d', '--developer', help='developer email or id', required=True)
     list_developer_apps.add_argument('--expand', action='store_true',
         help='Set to true to expand the results. This query parameter does not work if you use the count or startKey query parameters.')
     list_developer_apps.add_argument('--count', default=100, type=int,
         help='Limits the list to the number you specify. The limit is 100. Use with the startKey parameter to provide more targeted filtering.')
     list_developer_apps.add_argument('--startkey', default='',
         help='To filter the keys that are returned, enter the name of a company app that the list will start with.')
     list_developer_apps.set_defaults(func=lambda args: print(apps.list_developer_apps(args)))
 
-    get_developer_app_details = parser_apps.add_parser('get', aliases=['get-developer-app-details'], parents=[parent_parser],
+    get_developer_app_details = parser_apps.add_parser('get', aliases=['get-developer-app-details'], parents=[parent_parser()],
         help='Get the profile of a specific developer app. All times in the response are UNIX times. Note that the response contains a top-level attribute named accessType that is no longer used by Apigee.')
     get_developer_app_details.add_argument('-d', '--developer', help='developer email or id', required=True)
     get_developer_app_details.add_argument('-n', '--name', help='name', required=True)
     get_developer_app_details.set_defaults(func=lambda args: print(apps.get_developer_app_details(args).text))
 
-    list_api_products = parser_apiproducts.add_parser('list', aliases=['list-api-products'], parents=[parent_parser, prefix_parser],
+    list_api_products = parser_apiproducts.add_parser('list', aliases=['list-api-products'], parents=[parent_parser(), prefix_parser],
         help='Get a list of all API product names for an organization.')
     list_api_products.add_argument('--expand', action='store_true',
         help='Set to \'true\' to get expanded details about each product.')
     list_api_products.add_argument('--count', default=1000, type=int,
         help='Number of API products to return in the API call. The maximum limit is 1000. Use with the startkey to provide more targeted filtering.')
     list_api_products.add_argument('--startkey', default='',
         help='Returns a list of API products starting with the specified API product.')
     list_api_products.set_defaults(func=lambda args: print(apiproducts.list_api_products(args)))
 
-    get_api_product = parser_apiproducts.add_parser('get', aliases=['get-api-product'], parents=[parent_parser],
+    get_api_product = parser_apiproducts.add_parser('get', aliases=['get-api-product'], parents=[parent_parser()],
         help='Gets configuration data for an API product. The API product name required in the request URL is not the "Display Name" value displayed for the API product in the Edge UI. While they may be the same, they are not always the same depending on whether the API product was created via UI or API.')
     get_api_product.add_argument('-n', '--name', help='name', required=True)
     get_api_product.set_defaults(func=lambda args: print(apiproducts.get_api_product(args).text))
 
-    list_targetservers_in_an_environment = parser_targetservers.add_parser('list', aliases=['list-targetservers-in-an-environment'], parents=[parent_parser, environment_parser, prefix_parser],
+    create_a_targetserver = parser_targetservers.add_parser('create', aliases=['create-a-targetserver'], parents=[parent_parser(), environment_parser],
+        help='Create a TargetServer in the specified environment. TargetServers are used to decouple TargetEndpoint HTTPTargetConnections from concrete URLs for backend services.')
+    create_a_targetserver.add_argument('-b', '--body', help='request body', required=True)
+    create_a_targetserver.set_defaults(func=lambda args: print(targetservers.create_a_targetserver(args).text))
+
+    delete_a_targetserver = parser_targetservers.add_parser('delete', aliases=['delete-a-targetserver'], parents=[parent_parser(), environment_parser],
+        help='Delete a TargetServer configuration from an environment. Returns information about the deleted TargetServer.')
+    delete_a_targetserver.add_argument('-n', '--name', help='name', required=True)
+    delete_a_targetserver.set_defaults(func=lambda args: print(targetservers.delete_a_targetserver(args).text))
+
+    list_targetservers_in_an_environment = parser_targetservers.add_parser('list', aliases=['list-targetservers-in-an-environment'], parents=[parent_parser(), environment_parser, prefix_parser],
         help='List all TargetServers in an environment.')
     list_targetservers_in_an_environment.set_defaults(func=lambda args: print(targetservers.list_targetservers_in_an_environment(args)))
 
-    get_targetserver = parser_targetservers.add_parser('get', aliases=['get-targetserver'], parents=[parent_parser, environment_parser],
+    get_targetserver = parser_targetservers.add_parser('get', aliases=['get-targetserver'], parents=[parent_parser(), environment_parser],
         help='Returns a TargetServer definition.')
     get_targetserver.add_argument('-n', '--name', help='name', required=True)
     get_targetserver.set_defaults(func=lambda args: print(targetservers.get_targetserver(args).text))
 
-    create_data_masks_for_an_api_proxy = parser_maskconfigs.add_parser('create-api', aliases=['create-data-masks-for-an-api-proxy'], parents=[parent_parser],
+    update_a_targetserver = parser_targetservers.add_parser('update', aliases=['update-a-targetserver'], parents=[parent_parser(), environment_parser],
+        help='Modifies an existing TargetServer.')
+    update_a_targetserver.add_argument('-n', '--name', help='name', required=True)
+    update_a_targetserver.add_argument('-b', '--body', help='request body', required=True)
+    update_a_targetserver.set_defaults(func=lambda args: print(targetservers.update_a_targetserver(args).text))
+
+    push_targetserver = parser_targetservers.add_parser('push', aliases=['push-targetserver'], parents=[parent_parser(), environment_parser, file_parser],
+        help='Push TargetServer to Apigee. This will create/update a TargetServer.')
+    # push_keyvaluemap.add_argument('-n', '--name', help='name', required=True)
+    push_targetserver.set_defaults(func=lambda args: targetservers.push_targetserver(args))
+
+    create_data_masks_for_an_api_proxy = parser_maskconfigs.add_parser('create-api', aliases=['create-data-masks-for-an-api-proxy'], parents=[parent_parser()],
         help='Create a data mask for an API proxy. You can capture message content to assist in runtime debugging of APIs calls. In many cases, API traffic contains sensitive data, such credit cards or personally identifiable health information (PHI) that needs to filtered out of the captured message content. Data masks enable you to specify data that will be filtered out of trace sessions. Data masking is only enabled when a trace session (also called a \'debug\' session) is enabled for an API proxy. If no trace session are enabled on an API proxy, then the data will not be masked.')
     create_data_masks_for_an_api_proxy.add_argument('-n', '--name', help='name', required=True)
     create_data_masks_for_an_api_proxy.add_argument('-b', '--body', help='request body', required=True)
     create_data_masks_for_an_api_proxy.set_defaults(func=lambda args: print(maskconfigs.create_data_masks_for_an_api_proxy(args).text))
 
-    delete_data_masks_for_an_api_proxy = parser_maskconfigs.add_parser('delete-api', aliases=['delete-data-masks-for-an-api-proxy'], parents=[parent_parser],
+    delete_data_masks_for_an_api_proxy = parser_maskconfigs.add_parser('delete-api', aliases=['delete-data-masks-for-an-api-proxy'], parents=[parent_parser()],
         help='Delete a data mask for an API proxy.')
     delete_data_masks_for_an_api_proxy.add_argument('-n', '--name', help='name', required=True)
     delete_data_masks_for_an_api_proxy.add_argument('--maskconfig-name', help='data mask name', required=True)
     delete_data_masks_for_an_api_proxy.set_defaults(func=lambda args: print(maskconfigs.delete_data_masks_for_an_api_proxy(args).text))
 
-    get_data_mask_details_for_an_api_proxy = parser_maskconfigs.add_parser('get-api', aliases=['get-data-mask-details-for-an-api-proxy'], parents=[parent_parser],
+    get_data_mask_details_for_an_api_proxy = parser_maskconfigs.add_parser('get-api', aliases=['get-data-mask-details-for-an-api-proxy'], parents=[parent_parser()],
         help='Get the details for a data mask for an API proxy.')
     get_data_mask_details_for_an_api_proxy.add_argument('-n', '--name', help='name', required=True)
     get_data_mask_details_for_an_api_proxy.add_argument('--maskconfig-name', help='data mask name', required=True)
     get_data_mask_details_for_an_api_proxy.set_defaults(func=lambda args: print(maskconfigs.get_data_mask_details_for_an_api_proxy(args).text))
 
-    list_data_masks_for_an_api_proxy = parser_maskconfigs.add_parser('list-api', aliases=['list-data-masks-for-an-api-proxy'], parents=[parent_parser],
+    list_data_masks_for_an_api_proxy = parser_maskconfigs.add_parser('list-api', aliases=['list-data-masks-for-an-api-proxy'], parents=[parent_parser()],
         help='List all data masks for an API proxy.')
     list_data_masks_for_an_api_proxy.add_argument('-n', '--name', help='name', required=True)
     list_data_masks_for_an_api_proxy.set_defaults(func=lambda args: print(maskconfigs.list_data_masks_for_an_api_proxy(args).text))
 
-    list_data_masks_for_an_organization = parser_maskconfigs.add_parser('list', aliases=['list-data-masks-for-an-organization'], parents=[parent_parser],
+    list_data_masks_for_an_organization = parser_maskconfigs.add_parser('list', aliases=['list-data-masks-for-an-organization'], parents=[parent_parser()],
         help='List all data masks for an organization.')
     list_data_masks_for_an_organization.set_defaults(func=lambda args: print(maskconfigs.list_data_masks_for_an_organization(args).text))
 
-    create_permissions = parser_permissions.add_parser('create', aliases=['create-permissions'], parents=[parent_parser],
+    create_permissions = parser_permissions.add_parser('create', aliases=['create-permissions'], parents=[parent_parser()],
         help='Create permissions for a role.')
     create_permissions.add_argument('-n', '--name', help='name', required=True)
     create_permissions.add_argument('-b', '--body', help='request body', required=True)
     create_permissions.set_defaults(func=lambda args: print(permissions.create_permissions(args).text))
 
-    team_permissions = parser_permissions.add_parser('team', aliases=['team-permissions'], parents=[parent_parser],
+    team_permissions = parser_permissions.add_parser('team', aliases=['team-permissions'], parents=[parent_parser()],
         help='Create default permissions for a team role based on a template.')
     team_permissions.add_argument('-n', '--name', help='name of user role', required=True)
     team_permissions.add_argument('-t', '--team', help='team prefix/code', required=True)
     team_permissions.set_defaults(func=lambda args: print(permissions.team_permissions(args).text))
 
-    get_permissions = parser_permissions.add_parser('get', aliases=['get-permissions'], parents=[parent_parser],
+    get_permissions = parser_permissions.add_parser('get', aliases=['get-permissions'], parents=[parent_parser()],
         help='Get permissions for a role.')
     get_permissions.add_argument('-n', '--name', help='name', required=True)
     get_permissions.add_argument('-j', '--json', action='store_true', help='use json output')
     get_permissions.add_argument('--max-colwidth', help='max column width', type=int, default=40)
     get_permissions.set_defaults(func=lambda args: print(permissions.get_permissions(args)))
 
     args = parser.parse_args()
```

### Comparing `apigeecli-0.8.3/apigee/__init__.py` & `apigeecli-0.9.0/apigee/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 APP = 'apigeecli'
 CMD = 'apigee'
-__version__ = '0.8.3'
+__version__ = '0.9.0'
 description = 'Apigee Management API command-line interface with easy-to-use OAuth2 authentication'
 
 import json
 from os import getenv
 from pathlib import Path
 
 APIGEE_CLI_DIR = str(Path.home())+'/.apigee'
```

### Comparing `apigeecli-0.8.3/apigee/util/__init__.py` & `apigeecli-0.9.0/apigee/util/__init__.py`

 * *Files identical despite different names*

### Comparing `apigeecli-0.8.3/apigee/util/mfa_with_pyotp.py` & `apigeecli-0.9.0/apigee/util/mfa_with_pyotp.py`

 * *Files identical despite different names*

### Comparing `apigeecli-0.8.3/apigee/util/prepend.py` & `apigeecli-0.9.0/apigee/util/prepend.py`

 * *Files identical despite different names*

### Comparing `apigeecli-0.8.3/apigee/util/config.py` & `apigeecli-0.9.0/apigee/util/config.py`

 * *Files identical despite different names*

### Comparing `apigeecli-0.8.3/apigee/util/authorization.py` & `apigeecli-0.9.0/apigee/util/authorization.py`

 * *Files identical despite different names*

### Comparing `apigeecli-0.8.3/apigeecli.egg-info/PKG-INFO` & `apigeecli-0.9.0/apigeecli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: apigeecli
-Version: 0.8.3
+Version: 0.9.0
 Summary: Apigee Management API command-line interface with easy-to-use OAuth2 authentication
 Home-page: https://github.com/mdelotavo/apigee-cli
 Author: Matthew Delotavo
 Author-email: matthew.t.delotavo@gmail.com
 License: Apache license 2.0
-Download-URL: https://github.com/mdelotavo/apigee-cli/archive/v0.8.3.tar.gz
+Download-URL: https://github.com/mdelotavo/apigee-cli/archive/v0.9.0.tar.gz
 Description: ==========
         apigee-cli
         ==========
         
         This package provides a command-line interface for the Apigee Management API with easy-to-use OAuth2 authentication. ::
         
             usage: apigee [-h] [-V]
@@ -30,15 +30,15 @@
                                     keyvaluemaps
                 developers (devs)   developers
                 apps                developer apps
                 products (prods)    api products
                 ts (targetservers)  target servers
                 mask (maskconfigs)  data masks
                 perms (permissions)
-                                    set a permission for a role
+                                    manage permissions for a role
                 prepend (prefix)    prepend all matching strings with a prefix in all
                                     files in the specified directory (rudimentary stream
                                     editor). this is potentially VERY DANGEROUS. make sure
                                     you have version control such as Git to revert any
                                     changes in the target directory.
         
             optional arguments:
@@ -251,15 +251,15 @@
                                     the existing map. It can take several minutes before
                                     the new value is visible to runtime traffic.
                 list-keys (list-keys-in-an-environment-scoped-keyvaluemap)
                                     Note: This API is supported for Apigee Edge for the
                                     Public Cloud only. Lists keys in a KeyValueMap scoped
                                     to an environment. KVM names are case sensitive.
                 push (push-keyvaluemap)
-                                    Magically Push KeyValueMap to Apigee. This will create
+                                    Push KeyValueMap to Apigee. This will create
                                     KeyValueMap/entries if they do not exist, update
                                     existing KeyValueMap/entries, and delete entries on
                                     Apigee that are not present in the request body.
         
             optional arguments:
               -h, --help            show this help message and exit
         
@@ -283,17 +283,17 @@
                "value" : "value_two"
               }
              ]
             }'
         
         Then run::
         
-            $ apigee kvms create -e [env] -n Map_name -b "$body"
+            $ apigee kvms create -e [env] -b "$body"
         
-        To magically ``push`` a key value map in a file to Apigee Edge, run::
+        To ``push`` a key value map in a file to Apigee Edge, run::
         
             $ apigee kvms push -e dev -f test_kvm.json
         
         This will display a loading bar output like so::
         
             Updating existing entries in test-kvm                                                              |
             100% |#############################################################################################|
```

### Comparing `apigeecli-0.8.3/apigeecli.egg-info/SOURCES.txt` & `apigeecli-0.9.0/apigeecli.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 apigee/api/deploy.py
 apigee/api/deployments.py
 apigee/api/developers.py
 apigee/api/keyvaluemaps.py
 apigee/api/maskconfigs.py
 apigee/api/permissions.py
 apigee/api/targetservers.py
+apigee/parsers/__init__.py
+apigee/parsers/parent_parser.py
 apigee/util/__init__.py
 apigee/util/authorization.py
 apigee/util/config.py
 apigee/util/mfa_with_pyotp.py
 apigee/util/prepend.py
 apigeecli.egg-info/PKG-INFO
 apigeecli.egg-info/SOURCES.txt
```

### Comparing `apigeecli-0.8.3/PKG-INFO` & `apigeecli-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: apigeecli
-Version: 0.8.3
+Version: 0.9.0
 Summary: Apigee Management API command-line interface with easy-to-use OAuth2 authentication
 Home-page: https://github.com/mdelotavo/apigee-cli
 Author: Matthew Delotavo
 Author-email: matthew.t.delotavo@gmail.com
 License: Apache license 2.0
-Download-URL: https://github.com/mdelotavo/apigee-cli/archive/v0.8.3.tar.gz
+Download-URL: https://github.com/mdelotavo/apigee-cli/archive/v0.9.0.tar.gz
 Description: ==========
         apigee-cli
         ==========
         
         This package provides a command-line interface for the Apigee Management API with easy-to-use OAuth2 authentication. ::
         
             usage: apigee [-h] [-V]
@@ -30,15 +30,15 @@
                                     keyvaluemaps
                 developers (devs)   developers
                 apps                developer apps
                 products (prods)    api products
                 ts (targetservers)  target servers
                 mask (maskconfigs)  data masks
                 perms (permissions)
-                                    set a permission for a role
+                                    manage permissions for a role
                 prepend (prefix)    prepend all matching strings with a prefix in all
                                     files in the specified directory (rudimentary stream
                                     editor). this is potentially VERY DANGEROUS. make sure
                                     you have version control such as Git to revert any
                                     changes in the target directory.
         
             optional arguments:
@@ -251,15 +251,15 @@
                                     the existing map. It can take several minutes before
                                     the new value is visible to runtime traffic.
                 list-keys (list-keys-in-an-environment-scoped-keyvaluemap)
                                     Note: This API is supported for Apigee Edge for the
                                     Public Cloud only. Lists keys in a KeyValueMap scoped
                                     to an environment. KVM names are case sensitive.
                 push (push-keyvaluemap)
-                                    Magically Push KeyValueMap to Apigee. This will create
+                                    Push KeyValueMap to Apigee. This will create
                                     KeyValueMap/entries if they do not exist, update
                                     existing KeyValueMap/entries, and delete entries on
                                     Apigee that are not present in the request body.
         
             optional arguments:
               -h, --help            show this help message and exit
         
@@ -283,17 +283,17 @@
                "value" : "value_two"
               }
              ]
             }'
         
         Then run::
         
-            $ apigee kvms create -e [env] -n Map_name -b "$body"
+            $ apigee kvms create -e [env] -b "$body"
         
-        To magically ``push`` a key value map in a file to Apigee Edge, run::
+        To ``push`` a key value map in a file to Apigee Edge, run::
         
             $ apigee kvms push -e dev -f test_kvm.json
         
         This will display a loading bar output like so::
         
             Updating existing entries in test-kvm                                                              |
             100% |#############################################################################################|
```

### Comparing `apigeecli-0.8.3/README.rst` & `apigeecli-0.9.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
                             keyvaluemaps
         developers (devs)   developers
         apps                developer apps
         products (prods)    api products
         ts (targetservers)  target servers
         mask (maskconfigs)  data masks
         perms (permissions)
-                            set a permission for a role
+                            manage permissions for a role
         prepend (prefix)    prepend all matching strings with a prefix in all
                             files in the specified directory (rudimentary stream
                             editor). this is potentially VERY DANGEROUS. make sure
                             you have version control such as Git to revert any
                             changes in the target directory.
 
     optional arguments:
@@ -242,15 +242,15 @@
                             the existing map. It can take several minutes before
                             the new value is visible to runtime traffic.
         list-keys (list-keys-in-an-environment-scoped-keyvaluemap)
                             Note: This API is supported for Apigee Edge for the
                             Public Cloud only. Lists keys in a KeyValueMap scoped
                             to an environment. KVM names are case sensitive.
         push (push-keyvaluemap)
-                            Magically Push KeyValueMap to Apigee. This will create
+                            Push KeyValueMap to Apigee. This will create
                             KeyValueMap/entries if they do not exist, update
                             existing KeyValueMap/entries, and delete entries on
                             Apigee that are not present in the request body.
 
     optional arguments:
       -h, --help            show this help message and exit
 
@@ -274,17 +274,17 @@
        "value" : "value_two"
       }
      ]
     }'
 
 Then run::
 
-    $ apigee kvms create -e [env] -n Map_name -b "$body"
+    $ apigee kvms create -e [env] -b "$body"
 
-To magically ``push`` a key value map in a file to Apigee Edge, run::
+To ``push`` a key value map in a file to Apigee Edge, run::
 
     $ apigee kvms push -e dev -f test_kvm.json
 
 This will display a loading bar output like so::
 
     Updating existing entries in test-kvm                                                              |
     100% |#############################################################################################|
```


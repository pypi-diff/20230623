# Comparing `tmp/onepassword local search-1.1.5.tar.gz` & `tmp/onepassword local search-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onepassword local search-1.1.5.tar", last modified: Sun Jan 29 18:36:48 2023, max compression
+gzip compressed data, was "onepassword local search-1.1.6.tar", last modified: Fri Jun 23 07:59:40 2023, max compression
```

## Comparing `onepassword local search-1.1.5.tar` & `onepassword local search-1.1.6.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 mickaelperrin   (501) staff       (20)        0 2023-01-29 18:36:48.611815 onepassword local search-1.1.5/
--rw-------   0 mickaelperrin   (501) staff       (20)    35148 2021-01-07 14:57:13.000000 onepassword local search-1.1.5/LICENSE
--rw-r--r--   0 mickaelperrin   (501) staff       (20)    11242 2023-01-29 18:36:48.611595 onepassword local search-1.1.5/PKG-INFO
--rw-------   0 mickaelperrin   (501) staff       (20)    10144 2022-05-06 11:17:55.000000 onepassword local search-1.1.5/README.md
-drwxr-xr-x   0 mickaelperrin   (501) staff       (20)        0 2023-01-29 18:36:48.607819 onepassword local search-1.1.5/onepassword_local_search/
--rw-------   0 mickaelperrin   (501) staff       (20)     4345 2022-05-06 13:21:02.000000 onepassword local search-1.1.5/onepassword_local_search/CliSimple.py
--rw-------   0 mickaelperrin   (501) staff       (20)    11277 2021-01-07 14:57:13.000000 onepassword local search-1.1.5/onepassword_local_search/CliSimple_test.py
--rw-------   0 mickaelperrin   (501) staff       (20)     5906 2022-05-18 11:40:13.000000 onepassword local search-1.1.5/onepassword_local_search/OnePassword.py
--rw-------   0 mickaelperrin   (501) staff       (20)       32 2021-01-07 14:57:13.000000 onepassword local search-1.1.5/onepassword_local_search/__init__.py
--rw-------   0 mickaelperrin   (501) staff       (20)      191 2021-01-07 14:57:13.000000 onepassword local search-1.1.5/onepassword_local_search/__main__.py
--rw-------   0 mickaelperrin   (501) staff       (20)       21 2023-01-29 18:35:21.000000 onepassword local search-1.1.5/onepassword_local_search/__version__.py
-drwxr-xr-x   0 mickaelperrin   (501) staff       (20)        0 2023-01-29 18:36:48.608861 onepassword local search-1.1.5/onepassword_local_search/exceptions/
--rw-------   0 mickaelperrin   (501) staff       (20)      262 2021-01-07 14:57:13.000000 onepassword local search-1.1.5/onepassword_local_search/exceptions/Hook.py
--rw-------   0 mickaelperrin   (501) staff       (20)      261 2021-01-07 14:57:13.000000 onepassword local search-1.1.5/onepassword_local_search/exceptions/ManagedException.py
--rw-------   0 mickaelperrin   (501) staff       (20)        0 2021-01-07 14:57:13.000000 onepassword local search-1.1.5/onepassword_local_search/exceptions/__init__.py
-drwxr-xr-x   0 mickaelperrin   (501) staff       (20)        0 2023-01-29 18:36:48.609400 onepassword local search-1.1.5/onepassword_local_search/lib/
--rw-------   0 mickaelperrin   (501) staff       (20)        0 2021-01-07 14:57:13.000000 onepassword local search-1.1.5/onepassword_local_search/lib/__init__.py
--rw-------   0 mickaelperrin   (501) staff       (20)     4146 2021-01-07 14:57:13.000000 onepassword local search-1.1.5/onepassword_local_search/lib/optestlib.py
--rw-------   0 mickaelperrin   (501) staff       (20)      906 2021-01-07 14:57:13.000000 onepassword local search-1.1.5/onepassword_local_search/lib/optestlib_test.py
--rw-------   0 mickaelperrin   (501) staff       (20)      878 2021-01-07 14:57:13.000000 onepassword local search-1.1.5/onepassword_local_search/lib/utils.py
--rw-------   0 mickaelperrin   (501) staff       (20)      468 2021-01-07 14:57:13.000000 onepassword local search-1.1.5/onepassword_local_search/lib/utils_test.py
-drwxr-xr-x   0 mickaelperrin   (501) staff       (20)        0 2023-01-29 18:36:48.609721 onepassword local search-1.1.5/onepassword_local_search/models/
--rw-------   0 mickaelperrin   (501) staff       (20)      502 2021-05-21 10:32:20.000000 onepassword local search-1.1.5/onepassword_local_search/models/Cipher.py
--rw-------   0 mickaelperrin   (501) staff       (20)     3477 2022-05-06 10:56:26.000000 onepassword local search-1.1.5/onepassword_local_search/models/Item.py
--rw-------   0 mickaelperrin   (501) staff       (20)        0 2021-01-07 14:57:13.000000 onepassword local search-1.1.5/onepassword_local_search/models/__init__.py
-drwxr-xr-x   0 mickaelperrin   (501) staff       (20)        0 2023-01-29 18:36:48.611402 onepassword local search-1.1.5/onepassword_local_search/services/
--rw-------   0 mickaelperrin   (501) staff       (20)     4142 2022-05-06 15:49:12.000000 onepassword local search-1.1.5/onepassword_local_search/services/AccountService.py
--rw-------   0 mickaelperrin   (501) staff       (20)     1672 2021-01-07 14:57:13.000000 onepassword local search-1.1.5/onepassword_local_search/services/AccountService_test.py
--rw-------   0 mickaelperrin   (501) staff       (20)     3434 2023-01-29 18:34:08.000000 onepassword local search-1.1.5/onepassword_local_search/services/ConfigFileService.py
--rw-------   0 mickaelperrin   (501) staff       (20)      880 2021-01-07 14:57:13.000000 onepassword local search-1.1.5/onepassword_local_search/services/ConfigFileService_test.py
--rw-------   0 mickaelperrin   (501) staff       (20)     7314 2022-05-06 10:56:26.000000 onepassword local search-1.1.5/onepassword_local_search/services/CryptoService.py
--rw-------   0 mickaelperrin   (501) staff       (20)     9425 2021-01-07 14:57:13.000000 onepassword local search-1.1.5/onepassword_local_search/services/CryptoService_test.py
--rw-------   0 mickaelperrin   (501) staff       (20)     2153 2022-05-06 10:56:26.000000 onepassword local search-1.1.5/onepassword_local_search/services/SecondaryCryptoService.py
--rw-------   0 mickaelperrin   (501) staff       (20)    13732 2021-01-07 14:57:13.000000 onepassword local search-1.1.5/onepassword_local_search/services/SecondaryCryptoService_test.py
--rw-------   0 mickaelperrin   (501) staff       (20)     7993 2022-05-06 10:56:26.000000 onepassword local search-1.1.5/onepassword_local_search/services/StorageService.py
--rw-------   0 mickaelperrin   (501) staff       (20)      844 2021-01-07 14:57:13.000000 onepassword local search-1.1.5/onepassword_local_search/services/StorageService_test.py
--rw-------   0 mickaelperrin   (501) staff       (20)        0 2021-01-07 14:57:13.000000 onepassword local search-1.1.5/onepassword_local_search/services/__init__.py
-drwxr-xr-x   0 mickaelperrin   (501) staff       (20)        0 2023-01-29 18:36:48.608487 onepassword local search-1.1.5/onepassword_local_search.egg-info/
--rw-------   0 mickaelperrin   (501) staff       (20)    11242 2023-01-29 18:36:48.000000 onepassword local search-1.1.5/onepassword_local_search.egg-info/PKG-INFO
--rw-------   0 mickaelperrin   (501) staff       (20)     1647 2023-01-29 18:36:48.000000 onepassword local search-1.1.5/onepassword_local_search.egg-info/SOURCES.txt
--rw-------   0 mickaelperrin   (501) staff       (20)        1 2023-01-29 18:36:48.000000 onepassword local search-1.1.5/onepassword_local_search.egg-info/dependency_links.txt
--rw-------   0 mickaelperrin   (501) staff       (20)       69 2023-01-29 18:36:48.000000 onepassword local search-1.1.5/onepassword_local_search.egg-info/entry_points.txt
--rw-------   0 mickaelperrin   (501) staff       (20)       50 2023-01-29 18:36:48.000000 onepassword local search-1.1.5/onepassword_local_search.egg-info/requires.txt
--rw-------   0 mickaelperrin   (501) staff       (20)       25 2023-01-29 18:36:48.000000 onepassword local search-1.1.5/onepassword_local_search.egg-info/top_level.txt
--rw-r--r--   0 mickaelperrin   (501) staff       (20)       38 2023-01-29 18:36:48.611855 onepassword local search-1.1.5/setup.cfg
--rw-------   0 mickaelperrin   (501) staff       (20)     4211 2021-01-07 14:57:13.000000 onepassword local search-1.1.5/setup.py
+drwxr-xr-x   0 mickaelperrin   (501) staff       (20)        0 2023-06-23 07:59:40.584227 onepassword local search-1.1.6/
+-rw-------   0 mickaelperrin   (501) staff       (20)    35148 2021-01-07 14:57:13.000000 onepassword local search-1.1.6/LICENSE
+-rw-r--r--   0 mickaelperrin   (501) staff       (20)    11242 2023-06-23 07:59:40.583924 onepassword local search-1.1.6/PKG-INFO
+-rw-------   0 mickaelperrin   (501) staff       (20)    10144 2022-05-06 11:17:55.000000 onepassword local search-1.1.6/README.md
+drwxr-xr-x   0 mickaelperrin   (501) staff       (20)        0 2023-06-23 07:59:40.580092 onepassword local search-1.1.6/onepassword_local_search/
+-rw-------   0 mickaelperrin   (501) staff       (20)     4486 2023-06-23 07:56:40.000000 onepassword local search-1.1.6/onepassword_local_search/CliSimple.py
+-rw-------   0 mickaelperrin   (501) staff       (20)    11277 2021-01-07 14:57:13.000000 onepassword local search-1.1.6/onepassword_local_search/CliSimple_test.py
+-rw-------   0 mickaelperrin   (501) staff       (20)     6003 2023-06-23 07:52:04.000000 onepassword local search-1.1.6/onepassword_local_search/OnePassword.py
+-rw-------   0 mickaelperrin   (501) staff       (20)       32 2021-01-07 14:57:13.000000 onepassword local search-1.1.6/onepassword_local_search/__init__.py
+-rw-------   0 mickaelperrin   (501) staff       (20)      191 2021-01-07 14:57:13.000000 onepassword local search-1.1.6/onepassword_local_search/__main__.py
+-rw-------   0 mickaelperrin   (501) staff       (20)       21 2023-06-23 07:58:47.000000 onepassword local search-1.1.6/onepassword_local_search/__version__.py
+drwxr-xr-x   0 mickaelperrin   (501) staff       (20)        0 2023-06-23 07:59:40.581766 onepassword local search-1.1.6/onepassword_local_search/exceptions/
+-rw-------   0 mickaelperrin   (501) staff       (20)      262 2021-01-07 14:57:13.000000 onepassword local search-1.1.6/onepassword_local_search/exceptions/Hook.py
+-rw-------   0 mickaelperrin   (501) staff       (20)      261 2021-01-07 14:57:13.000000 onepassword local search-1.1.6/onepassword_local_search/exceptions/ManagedException.py
+-rw-------   0 mickaelperrin   (501) staff       (20)        0 2021-01-07 14:57:13.000000 onepassword local search-1.1.6/onepassword_local_search/exceptions/__init__.py
+drwxr-xr-x   0 mickaelperrin   (501) staff       (20)        0 2023-06-23 07:59:40.582257 onepassword local search-1.1.6/onepassword_local_search/lib/
+-rw-------   0 mickaelperrin   (501) staff       (20)        0 2021-01-07 14:57:13.000000 onepassword local search-1.1.6/onepassword_local_search/lib/__init__.py
+-rw-------   0 mickaelperrin   (501) staff       (20)     4146 2021-01-07 14:57:13.000000 onepassword local search-1.1.6/onepassword_local_search/lib/optestlib.py
+-rw-------   0 mickaelperrin   (501) staff       (20)      906 2021-01-07 14:57:13.000000 onepassword local search-1.1.6/onepassword_local_search/lib/optestlib_test.py
+-rw-------   0 mickaelperrin   (501) staff       (20)      878 2021-01-07 14:57:13.000000 onepassword local search-1.1.6/onepassword_local_search/lib/utils.py
+-rw-------   0 mickaelperrin   (501) staff       (20)      468 2021-01-07 14:57:13.000000 onepassword local search-1.1.6/onepassword_local_search/lib/utils_test.py
+drwxr-xr-x   0 mickaelperrin   (501) staff       (20)        0 2023-06-23 07:59:40.582562 onepassword local search-1.1.6/onepassword_local_search/models/
+-rw-------   0 mickaelperrin   (501) staff       (20)      502 2021-05-21 10:32:20.000000 onepassword local search-1.1.6/onepassword_local_search/models/Cipher.py
+-rw-------   0 mickaelperrin   (501) staff       (20)     3477 2022-05-06 10:56:26.000000 onepassword local search-1.1.6/onepassword_local_search/models/Item.py
+-rw-------   0 mickaelperrin   (501) staff       (20)        0 2021-01-07 14:57:13.000000 onepassword local search-1.1.6/onepassword_local_search/models/__init__.py
+drwxr-xr-x   0 mickaelperrin   (501) staff       (20)        0 2023-06-23 07:59:40.583724 onepassword local search-1.1.6/onepassword_local_search/services/
+-rw-------   0 mickaelperrin   (501) staff       (20)     4142 2023-03-26 14:08:58.000000 onepassword local search-1.1.6/onepassword_local_search/services/AccountService.py
+-rw-------   0 mickaelperrin   (501) staff       (20)     1672 2021-01-07 14:57:13.000000 onepassword local search-1.1.6/onepassword_local_search/services/AccountService_test.py
+-rw-------   0 mickaelperrin   (501) staff       (20)     3434 2023-01-29 18:34:08.000000 onepassword local search-1.1.6/onepassword_local_search/services/ConfigFileService.py
+-rw-------   0 mickaelperrin   (501) staff       (20)      880 2021-01-07 14:57:13.000000 onepassword local search-1.1.6/onepassword_local_search/services/ConfigFileService_test.py
+-rw-------   0 mickaelperrin   (501) staff       (20)     7314 2022-05-06 10:56:26.000000 onepassword local search-1.1.6/onepassword_local_search/services/CryptoService.py
+-rw-------   0 mickaelperrin   (501) staff       (20)     9425 2021-01-07 14:57:13.000000 onepassword local search-1.1.6/onepassword_local_search/services/CryptoService_test.py
+-rw-------   0 mickaelperrin   (501) staff       (20)     2153 2023-03-26 14:07:31.000000 onepassword local search-1.1.6/onepassword_local_search/services/SecondaryCryptoService.py
+-rw-------   0 mickaelperrin   (501) staff       (20)    13732 2021-01-07 14:57:13.000000 onepassword local search-1.1.6/onepassword_local_search/services/SecondaryCryptoService_test.py
+-rw-------   0 mickaelperrin   (501) staff       (20)     7993 2022-05-06 10:56:26.000000 onepassword local search-1.1.6/onepassword_local_search/services/StorageService.py
+-rw-------   0 mickaelperrin   (501) staff       (20)      844 2021-01-07 14:57:13.000000 onepassword local search-1.1.6/onepassword_local_search/services/StorageService_test.py
+-rw-------   0 mickaelperrin   (501) staff       (20)        0 2021-01-07 14:57:13.000000 onepassword local search-1.1.6/onepassword_local_search/services/__init__.py
+drwxr-xr-x   0 mickaelperrin   (501) staff       (20)        0 2023-06-23 07:59:40.581242 onepassword local search-1.1.6/onepassword_local_search.egg-info/
+-rw-------   0 mickaelperrin   (501) staff       (20)    11242 2023-06-23 07:59:40.000000 onepassword local search-1.1.6/onepassword_local_search.egg-info/PKG-INFO
+-rw-------   0 mickaelperrin   (501) staff       (20)     1647 2023-06-23 07:59:40.000000 onepassword local search-1.1.6/onepassword_local_search.egg-info/SOURCES.txt
+-rw-------   0 mickaelperrin   (501) staff       (20)        1 2023-06-23 07:59:40.000000 onepassword local search-1.1.6/onepassword_local_search.egg-info/dependency_links.txt
+-rw-------   0 mickaelperrin   (501) staff       (20)       69 2023-06-23 07:59:40.000000 onepassword local search-1.1.6/onepassword_local_search.egg-info/entry_points.txt
+-rw-------   0 mickaelperrin   (501) staff       (20)       50 2023-06-23 07:59:40.000000 onepassword local search-1.1.6/onepassword_local_search.egg-info/requires.txt
+-rw-------   0 mickaelperrin   (501) staff       (20)       25 2023-06-23 07:59:40.000000 onepassword local search-1.1.6/onepassword_local_search.egg-info/top_level.txt
+-rw-r--r--   0 mickaelperrin   (501) staff       (20)       38 2023-06-23 07:59:40.584266 onepassword local search-1.1.6/setup.cfg
+-rw-------   0 mickaelperrin   (501) staff       (20)     4211 2021-01-07 14:57:13.000000 onepassword local search-1.1.6/setup.py
```

### Comparing `onepassword local search-1.1.5/LICENSE` & `onepassword local search-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `onepassword local search-1.1.5/PKG-INFO` & `onepassword local search-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onepassword local search
-Version: 1.1.5
+Version: 1.1.6
 Summary: Simple 1Password CLI to list and decrypt secrets by querying the local sqlite database
 Home-page: https://github.com/mickaelperrin/onepassword-local-search
 Author: Mickaël Perrin
 Author-email: dev@mickaelperrin.fr
 License: GPLv3
 Keywords: onepassword 1password cli password secrets
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `onepassword local search-1.1.5/README.md` & `onepassword local search-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `onepassword local search-1.1.5/onepassword_local_search/CliSimple.py` & `onepassword local search-1.1.6/onepassword_local_search/CliSimple.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,14 +35,15 @@
         action_is_authenticated = subparsers.add_parser('is-authenticated', help='check if authenticated locally')
 
         action_version = subparsers.add_parser('version')
 
         action_update_mapping = subparsers.add_parser('mapping', help='operations on uuid mapping')
         action_update_mapping.add_argument('subcommand', help='update or list', choices=['list', 'update'])
         action_update_mapping.add_argument('--use-lastpass-uuid', help='list using lastpass uuid', nargs='?', default=False, const=True)
+        action_update_mapping.add_argument('--verbose', help='more verbose output', nargs='?', default=False, const=True)
 
         self.args = parser.parse_args(args[1:])
 
         if self.args.disable_session_caching:
             from onepassword_local_search.services.CryptoService import CryptoService
             CryptoService.cleanup_sessions_cache()
 
@@ -76,15 +77,15 @@
             custom_uuid_mapping = None
         return self.onePassword.get(self.args.uuid, self.args.field, custom_uuid_mapping)
 
     def list(self):
         return self.onePassword.list(self.args.format, self.args.filter, self.args.filter_operator, result_encoding=self.args.output_encoding)
 
     def mapping(self):
-        return self.onePassword.mapping(self.args.subcommand, self.args.use_lastpass_uuid)
+        return self.onePassword.mapping(self.args.subcommand, self.args.use_lastpass_uuid, self.args.verbose)
 
     def version(self):
         return OnePassword.version()
 
     def is_authenticated(self):
         if not self.onePassword.is_authenticated():
             sys.exit(1)
```

### Comparing `onepassword local search-1.1.5/onepassword_local_search/CliSimple_test.py` & `onepassword local search-1.1.6/onepassword_local_search/CliSimple_test.py`

 * *Files identical despite different names*

### Comparing `onepassword local search-1.1.5/onepassword_local_search/OnePassword.py` & `onepassword local search-1.1.6/onepassword_local_search/OnePassword.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,24 +68,26 @@
 
     def list(self, result_format=None, result_fitler=None, filter_operator='AND', result_encoding=None):
         list_format = result_format if result_format else '{uuid} {title}'
         sf = SimpleFormatter(output_encoding=result_encoding)
         for item in self.get_items(result_fitler, filter_operator):
             print(sf.format(list_format, item).strip())
 
-    def mapping(self, subcommand, use_lastpass_uuid=False):
+    def mapping(self, subcommand, use_lastpass_uuid=False, verbose=False):
         self.storageService.checks_for_uuid_mapping()
         if subcommand == 'list':
             self.mapping_list(use_lastpass_uuid)
         else:
-            return getattr(self, 'mapping_' + subcommand)()
+            return getattr(self, 'mapping_' + subcommand)(verbose)
 
-    def mapping_update(self):
+    def mapping_update(self, verbose=False):
         self.storageService.truncate_uuid_mapping_table()
         for item in self.storageService.list(self.accountService.get_available_accounts_id()):
+            if verbose:
+                print(item['uuid'])
             encrypted_item = Item(item)
             decryptor = self.accountService.get_decryptor(encrypted_item.vaultId)
             decrypted_item = decryptor.decrypt_item(encrypted_item)
             custom_uuid = decrypted_item.get('UUID', strict=False)
             lastpass_uuid = decrypted_item.get('LASTPASS_ID', strict=False)
             if custom_uuid:
                 self.storageService.add_uuid_mapping(custom_uuid=custom_uuid, op_uuid=decrypted_item.uuid,
```

### Comparing `onepassword local search-1.1.5/onepassword_local_search/lib/optestlib.py` & `onepassword local search-1.1.6/onepassword_local_search/lib/optestlib.py`

 * *Files identical despite different names*

### Comparing `onepassword local search-1.1.5/onepassword_local_search/lib/optestlib_test.py` & `onepassword local search-1.1.6/onepassword_local_search/lib/optestlib_test.py`

 * *Files identical despite different names*

### Comparing `onepassword local search-1.1.5/onepassword_local_search/lib/utils.py` & `onepassword local search-1.1.6/onepassword_local_search/lib/utils.py`

 * *Files identical despite different names*

### Comparing `onepassword local search-1.1.5/onepassword_local_search/models/Item.py` & `onepassword local search-1.1.6/onepassword_local_search/models/Item.py`

 * *Files identical despite different names*

### Comparing `onepassword local search-1.1.5/onepassword_local_search/services/AccountService.py` & `onepassword local search-1.1.6/onepassword_local_search/services/AccountService.py`

 * *Files identical despite different names*

### Comparing `onepassword local search-1.1.5/onepassword_local_search/services/AccountService_test.py` & `onepassword local search-1.1.6/onepassword_local_search/services/AccountService_test.py`

 * *Files identical despite different names*

### Comparing `onepassword local search-1.1.5/onepassword_local_search/services/ConfigFileService.py` & `onepassword local search-1.1.6/onepassword_local_search/services/ConfigFileService.py`

 * *Files identical despite different names*

### Comparing `onepassword local search-1.1.5/onepassword_local_search/services/ConfigFileService_test.py` & `onepassword local search-1.1.6/onepassword_local_search/services/ConfigFileService_test.py`

 * *Files identical despite different names*

### Comparing `onepassword local search-1.1.5/onepassword_local_search/services/CryptoService.py` & `onepassword local search-1.1.6/onepassword_local_search/services/CryptoService.py`

 * *Files identical despite different names*

### Comparing `onepassword local search-1.1.5/onepassword_local_search/services/CryptoService_test.py` & `onepassword local search-1.1.6/onepassword_local_search/services/CryptoService_test.py`

 * *Files identical despite different names*

### Comparing `onepassword local search-1.1.5/onepassword_local_search/services/SecondaryCryptoService.py` & `onepassword local search-1.1.6/onepassword_local_search/services/SecondaryCryptoService.py`

 * *Files identical despite different names*

### Comparing `onepassword local search-1.1.5/onepassword_local_search/services/SecondaryCryptoService_test.py` & `onepassword local search-1.1.6/onepassword_local_search/services/SecondaryCryptoService_test.py`

 * *Files identical despite different names*

### Comparing `onepassword local search-1.1.5/onepassword_local_search/services/StorageService.py` & `onepassword local search-1.1.6/onepassword_local_search/services/StorageService.py`

 * *Files identical despite different names*

### Comparing `onepassword local search-1.1.5/onepassword_local_search/services/StorageService_test.py` & `onepassword local search-1.1.6/onepassword_local_search/services/StorageService_test.py`

 * *Files identical despite different names*

### Comparing `onepassword local search-1.1.5/onepassword_local_search.egg-info/PKG-INFO` & `onepassword local search-1.1.6/onepassword_local_search.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onepassword-local-search
-Version: 1.1.5
+Version: 1.1.6
 Summary: Simple 1Password CLI to list and decrypt secrets by querying the local sqlite database
 Home-page: https://github.com/mickaelperrin/onepassword-local-search
 Author: Mickaël Perrin
 Author-email: dev@mickaelperrin.fr
 License: GPLv3
 Keywords: onepassword 1password cli password secrets
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `onepassword local search-1.1.5/onepassword_local_search.egg-info/SOURCES.txt` & `onepassword local search-1.1.6/onepassword_local_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onepassword local search-1.1.5/setup.py` & `onepassword local search-1.1.6/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/libmozdata-0.2.3.tar.gz` & `tmp/libmozdata-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/libmozdata-0.2.3.tar", last modified: Wed May 24 22:18:32 2023, max compression
+gzip compressed data, was "dist/libmozdata-0.2.4.tar", last modified: Fri Jun 23 15:40:49 2023, max compression
```

## Comparing `libmozdata-0.2.3.tar` & `libmozdata-0.2.4.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:18:32.000000 libmozdata-0.2.3/
--rw-r--r--   0 root         (0) root         (0)      155 2023-05-24 22:18:31.000000 libmozdata-0.2.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      472 2023-05-24 22:18:32.000000 libmozdata-0.2.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1002 2023-05-24 22:18:31.000000 libmozdata-0.2.3/README.md
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-24 22:18:31.000000 libmozdata-0.2.3/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:18:32.000000 libmozdata-0.2.3/libmozdata/
--rw-r--r--   0 root         (0) root         (0)     7695 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/BZInfo.py
--rw-r--r--   0 root         (0) root         (0)     1828 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/FXRevision.py
--rw-r--r--   0 root         (0) root         (0)     4268 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/FileStats.py
--rw-r--r--   0 root         (0) root         (0)     5540 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/HGFileInfo.py
--rw-r--r--   0 root         (0) root         (0)      424 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38900 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/bugzilla.py
--rw-r--r--   0 root         (0) root         (0)     4042 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/buildhub.py
--rw-r--r--   0 root         (0) root         (0)     1800 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/config.py
--rw-r--r--   0 root         (0) root         (0)     7286 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/connection.py
--rw-r--r--   0 root         (0) root         (0)     2350 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/fx_trains.py
--rw-r--r--   0 root         (0) root         (0)     2106 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/handler.py
--rw-r--r--   0 root         (0) root         (0)    10234 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/hgmozilla.py
--rw-r--r--   0 root         (0) root         (0)     2764 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/lando.py
--rw-r--r--   0 root         (0) root         (0)    75057 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/modules.json
--rw-r--r--   0 root         (0) root         (0)     2781 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/modules.py
--rw-r--r--   0 root         (0) root         (0)    39379 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/patchanalysis.py
--rw-r--r--   0 root         (0) root         (0)    24114 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/phabricator.py
--rw-r--r--   0 root         (0) root         (0)     6327 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/redash.py
--rw-r--r--   0 root         (0) root         (0)     2216 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/release_owners.py
--rw-r--r--   0 root         (0) root         (0)     8039 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/socorro.py
--rw-r--r--   0 root         (0) root         (0)     8653 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/utils.py
--rw-r--r--   0 root         (0) root         (0)     1564 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/vcs_map.py
--rw-r--r--   0 root         (0) root         (0)     5014 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/versions.py
--rw-r--r--   0 root         (0) root         (0)     3581 2023-05-24 22:18:31.000000 libmozdata-0.2.3/libmozdata/wiki_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 22:18:32.000000 libmozdata-0.2.3/libmozdata.egg-info/
--rw-r--r--   0 root         (0) root         (0)      472 2023-05-24 22:18:32.000000 libmozdata-0.2.3/libmozdata.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      830 2023-05-24 22:18:32.000000 libmozdata-0.2.3/libmozdata.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 22:18:32.000000 libmozdata-0.2.3/libmozdata.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 22:18:32.000000 libmozdata-0.2.3/libmozdata.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      160 2023-05-24 22:18:32.000000 libmozdata-0.2.3/libmozdata.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-05-24 22:18:32.000000 libmozdata-0.2.3/libmozdata.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      160 2023-05-24 22:18:31.000000 libmozdata-0.2.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       79 2023-05-24 22:18:32.000000 libmozdata-0.2.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1214 2023-05-24 22:18:31.000000 libmozdata-0.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:40:49.000000 libmozdata-0.2.4/
+-rw-r--r--   0 root         (0) root         (0)      155 2023-06-23 15:40:49.000000 libmozdata-0.2.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      472 2023-06-23 15:40:49.000000 libmozdata-0.2.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-06-23 15:40:49.000000 libmozdata-0.2.4/README.md
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-23 15:40:49.000000 libmozdata-0.2.4/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:40:49.000000 libmozdata-0.2.4/libmozdata/
+-rw-r--r--   0 root         (0) root         (0)     7695 2023-06-23 15:40:49.000000 libmozdata-0.2.4/libmozdata/BZInfo.py
+-rw-r--r--   0 root         (0) root         (0)     1828 2023-06-23 15:40:49.000000 libmozdata-0.2.4/libmozdata/FXRevision.py
+-rw-r--r--   0 root         (0) root         (0)     4268 2023-06-23 15:40:49.000000 libmozdata-0.2.4/libmozdata/FileStats.py
+-rw-r--r--   0 root         (0) root         (0)     5540 2023-06-23 15:40:49.000000 libmozdata-0.2.4/libmozdata/HGFileInfo.py
+-rw-r--r--   0 root         (0) root         (0)      424 2023-06-23 15:40:49.000000 libmozdata-0.2.4/libmozdata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40064 2023-06-23 15:40:49.000000 libmozdata-0.2.4/libmozdata/bugzilla.py
+-rw-r--r--   0 root         (0) root         (0)     4042 2023-06-23 15:40:49.000000 libmozdata-0.2.4/libmozdata/buildhub.py
+-rw-r--r--   0 root         (0) root         (0)     2149 2023-06-23 15:40:49.000000 libmozdata-0.2.4/libmozdata/clouseau.py
+-rw-r--r--   0 root         (0) root         (0)     1800 2023-06-23 15:40:49.000000 libmozdata-0.2.4/libmozdata/config.py
+-rw-r--r--   0 root         (0) root         (0)     7341 2023-06-23 15:40:49.000000 libmozdata-0.2.4/libmozdata/connection.py
+-rw-r--r--   0 root         (0) root         (0)     2350 2023-06-23 15:40:49.000000 libmozdata-0.2.4/libmozdata/fx_trains.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2023-06-23 15:40:49.000000 libmozdata-0.2.4/libmozdata/handler.py
+-rw-r--r--   0 root         (0) root         (0)    10234 2023-06-23 15:40:49.000000 libmozdata-0.2.4/libmozdata/hgmozilla.py
+-rw-r--r--   0 root         (0) root         (0)     2764 2023-06-23 15:40:49.000000 libmozdata-0.2.4/libmozdata/lando.py
+-rw-r--r--   0 root         (0) root         (0)    75057 2023-06-23 15:40:49.000000 libmozdata-0.2.4/libmozdata/modules.json
+-rw-r--r--   0 root         (0) root         (0)     2781 2023-06-23 15:40:49.000000 libmozdata-0.2.4/libmozdata/modules.py
+-rw-r--r--   0 root         (0) root         (0)    39379 2023-06-23 15:40:49.000000 libmozdata-0.2.4/libmozdata/patchanalysis.py
+-rw-r--r--   0 root         (0) root         (0)    24114 2023-06-23 15:40:49.000000 libmozdata-0.2.4/libmozdata/phabricator.py
+-rw-r--r--   0 root         (0) root         (0)     6327 2023-06-23 15:40:49.000000 libmozdata-0.2.4/libmozdata/redash.py
+-rw-r--r--   0 root         (0) root         (0)     2216 2023-06-23 15:40:49.000000 libmozdata-0.2.4/libmozdata/release_owners.py
+-rw-r--r--   0 root         (0) root         (0)     9920 2023-06-23 15:40:49.000000 libmozdata-0.2.4/libmozdata/socorro.py
+-rw-r--r--   0 root         (0) root         (0)     8653 2023-06-23 15:40:49.000000 libmozdata-0.2.4/libmozdata/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1564 2023-06-23 15:40:49.000000 libmozdata-0.2.4/libmozdata/vcs_map.py
+-rw-r--r--   0 root         (0) root         (0)     5014 2023-06-23 15:40:49.000000 libmozdata-0.2.4/libmozdata/versions.py
+-rw-r--r--   0 root         (0) root         (0)     3581 2023-06-23 15:40:49.000000 libmozdata-0.2.4/libmozdata/wiki_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:40:49.000000 libmozdata-0.2.4/libmozdata.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      472 2023-06-23 15:40:49.000000 libmozdata-0.2.4/libmozdata.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      853 2023-06-23 15:40:49.000000 libmozdata-0.2.4/libmozdata.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 15:40:49.000000 libmozdata-0.2.4/libmozdata.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 15:40:49.000000 libmozdata-0.2.4/libmozdata.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      160 2023-06-23 15:40:49.000000 libmozdata-0.2.4/libmozdata.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-23 15:40:49.000000 libmozdata-0.2.4/libmozdata.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      160 2023-06-23 15:40:49.000000 libmozdata-0.2.4/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-06-23 15:40:49.000000 libmozdata-0.2.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1214 2023-06-23 15:40:49.000000 libmozdata-0.2.4/setup.py
```

### Comparing `libmozdata-0.2.3/README.md` & `libmozdata-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.3/libmozdata/BZInfo.py` & `libmozdata-0.2.4/libmozdata/BZInfo.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.3/libmozdata/FXRevision.py` & `libmozdata-0.2.4/libmozdata/FXRevision.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.3/libmozdata/FileStats.py` & `libmozdata-0.2.4/libmozdata/FileStats.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.3/libmozdata/HGFileInfo.py` & `libmozdata-0.2.4/libmozdata/HGFileInfo.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.3/libmozdata/bugzilla.py` & `libmozdata-0.2.4/libmozdata/bugzilla.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,23 +12,31 @@
 import libmozdata.versions
 
 from . import config, utils
 from .connection import Connection, Query
 from .handler import Handler
 
 
-class Bugzilla(Connection):
-    """Connection to bugzilla.mozilla.org"""
-
+class BugzillaBase(Connection):
     URL = config.get("Bugzilla", "URL", "https://bugzilla.mozilla.org")
     # URL = config.get('Allizgub', 'URL', 'https://bugzilla-dev.allizom.org')
-    API_URL = URL + "/rest/bug"
-    ATTACHMENT_API_URL = API_URL + "/attachment"
     TOKEN = config.get("Bugzilla", "token", "")
     # TOKEN = config.get('Allizgub', 'token', '')
+
+    def get_header(self):
+        header = super(BugzillaBase, self).get_header()
+        header["X-Bugzilla-API-Key"] = self.get_apikey()
+        return header
+
+
+class Bugzilla(BugzillaBase):
+    """Connection to bugzilla.mozilla.org"""
+
+    API_URL = BugzillaBase.URL + "/rest/bug"
+    ATTACHMENT_API_URL = API_URL + "/attachment"
     BUGZILLA_CHUNK_SIZE = 100
 
     def __init__(
         self,
         bugids=None,
         include_fields="_default",
         bughandler=None,
@@ -90,19 +98,14 @@
             self.bugs_results = []
             self.history_results = []
             self.comment_results = []
             self.attachment_results = []
             self.got_data = False
             self.no_private_bugids = None
 
-    def get_header(self):
-        header = super(Bugzilla, self).get_header()
-        header["X-Bugzilla-API-Key"] = self.get_apikey()
-        return header
-
     def put(self, data, attachment=False, retry_on_failure=False):
         """Put some data in bugs
 
         Args:
             data (dict): a dictionary
         """
         failures = []
@@ -812,20 +815,18 @@
                     verify=True,
                     timeout=self.TIMEOUT,
                     hooks={"response": cb},
                 )
             )
 
 
-class BugzillaUser(Connection):
+class BugzillaUser(BugzillaBase):
     """Connection to bugzilla.mozilla.org"""
 
-    URL = config.get("Bugzilla", "URL", "https://bugzilla.mozilla.org")
-    API_URL = URL + "/rest/user"
-    TOKEN = config.get("Bugzilla", "token", "")
+    API_URL = BugzillaBase.URL + "/rest/user"
 
     def __init__(
         self,
         user_names=None,
         search_strings=None,
         include_fields="_default",
         user_handler=None,
@@ -888,39 +889,32 @@
                         BugzillaUser.API_URL + "?" + search_string,
                         handler=self.__users_cb,
                     )
                 )
 
             super(BugzillaUser, self).__init__(BugzillaUser.URL, queries, **kwargs)
 
-    def get_header(self):
-        header = super(BugzillaUser, self).get_header()
-        header["X-Bugzilla-API-Key"] = self.get_apikey()
-        return header
-
     def __users_cb(self, res):
         if self.user_handler.isactive():
             for user in res["users"]:
                 self.user_handler.handle(user)
 
         if self.fault_user_handler.isactive():
             for user in res["faults"]:
                 self.fault_user_handler.handle(user)
 
 
-class BugzillaProduct(Connection):
+class BugzillaProduct(BugzillaBase):
     """
     Connection to bugzilla.mozilla.org
 
     API docs: https://bugzilla.readthedocs.io/en/latest/api/core/v1/product.html
     """
 
-    URL = config.get("Bugzilla", "URL", "https://bugzilla.mozilla.org")
-    API_URL = URL + "/rest/product"
-    TOKEN = config.get("Bugzilla", "token", "")
+    API_URL = BugzillaBase.URL + "/rest/product"
 
     def __init__(
         self,
         product_names=None,
         product_types=None,
         include_fields="_default",
         product_handler=None,
@@ -1003,35 +997,28 @@
 
         super(BugzillaProduct, self).__init__(
             BugzillaProduct.URL,
             Query(BugzillaProduct.API_URL, params, self.__products_cb),
             **kwargs,
         )
 
-    def get_header(self):
-        header = super(BugzillaProduct, self).get_header()
-        header["X-Bugzilla-API-Key"] = self.get_apikey()
-        return header
-
     def __products_cb(self, res):
         if not self.product_handler.isactive():
             return
 
         for product in res["products"]:
             self.product_handler.handle(product)
 
 
-class BugzillaShorten(Connection):
+class BugzillaShorten(BugzillaBase):
     """
     Connection to bugzilla.mozilla.org
     """
 
-    URL = config.get("Bugzilla", "URL", "https://bugzilla.mozilla.org")
-    API_URL = URL + "/rest/bitly/shorten"
-    TOKEN = config.get("Bugzilla", "token", "")
+    API_URL = BugzillaBase.URL + "/rest/bitly/shorten"
 
     def __init__(self, url, url_data=None, url_handler=None, **kwargs):
         """Constructor
 
         Args:
             url (List[str]): the url to shorten
             url_handler (Optional[function]): the handler to use with each retrieved url
@@ -1045,19 +1032,14 @@
 
         super(BugzillaShorten, self).__init__(
             BugzillaShorten.URL,
             Query(BugzillaShorten.API_URL, params, self.__urls_cb),
             **kwargs,
         )
 
-    def get_header(self):
-        header = super(BugzillaShorten, self).get_header()
-        header["X-Bugzilla-API-Key"] = self.get_apikey()
-        return header
-
     def __urls_cb(self, res):
         if not self.url_handler.isactive():
             return
 
         if not isinstance(res, dict):
             # This is a workaround to handle cases where Bugzilla returns 200
             # response with HTML content instead of 4xx error.
@@ -1065,22 +1047,20 @@
             if self.RAISE_ERROR:
                 raise HTTPError("The response is not a valid JSON")
             return
 
         self.url_handler.handle(res["url"])
 
 
-class BugzillaComponent(Connection):
+class BugzillaComponent(BugzillaBase):
     """
     Connection to bugzilla.mozilla.org
     """
 
-    URL = config.get("Bugzilla", "URL", "https://bugzilla.mozilla.org")
-    API_URL = URL + "/rest/component"
-    TOKEN = config.get("Bugzilla", "token", "")
+    API_URL = BugzillaBase.URL + "/rest/component"
 
     def __init__(
         self, product, component, component_data=None, component_handler=None, **kwargs
     ):
         """Constructor
 
         Args:
@@ -1101,19 +1081,14 @@
                 BugzillaComponent.API_URL,
                 params,
                 self.__components_cb,
             ),
             **kwargs,
         )
 
-    def get_header(self):
-        header = super(BugzillaComponent, self).get_header()
-        header["X-Bugzilla-API-Key"] = self.get_apikey()
-        return header
-
     def __components_cb(self, res):
         if not self.component_handler.isactive():
             return
 
         self.component_handler.handle(res)
 
     def put(self, data):
@@ -1131,7 +1106,90 @@
             params=query.params,
             json=data,
             headers=self.get_header(),
         )
         response.raise_for_status()
 
         return response.json()
+
+
+class BugFields(BugzillaBase):
+    """Fetching bug fields information from Bugzilla
+
+    Docs: https://bmo.readthedocs.io/en/latest/api/core/v1/field.html#fields
+    """
+
+    API_URL = BugzillaBase.URL + "/rest/field/bug"
+
+    def __init__(
+        self, field=None, handler=None, handlerdata=None, queries=None, **kwargs
+    ):
+        """Constructor
+
+        Args:
+            field (Optional[str]): the name of the field, if empty will fetch all fields
+            handler (Optional[function]): the handler to use with each retrieved field
+            handlerdata (Optional): the data to use with the field handler
+            queries (Optional[Query]): the queries to use
+        """
+        if not queries:
+            endpoint_url = f"{self.API_URL}/{field}" if field else self.API_URL
+            queries = Query(endpoint_url, None, handler, handlerdata)
+
+        super(BugFields, self).__init__(self.URL, queries, **kwargs)
+
+    @classmethod
+    def fetch_all_fields_info(cls):
+        """Get information about all fields
+
+        Returns:
+            list: the information about the fields
+        """
+
+        def handler(resp, data):
+            data.update(resp)
+
+        data = {}
+        cls(
+            handler=handler,
+            handlerdata=data,
+        ).wait()
+
+        return data["fields"]
+
+    @classmethod
+    def fetch_field_info(cls, field):
+        """Get information about a field
+
+        Args:
+            field (str): the name of the field
+
+        Returns:
+            dict: the information about the field
+        """
+
+        def handler(resp, data):
+            data.update(resp)
+
+        data = {}
+        cls(
+            field=field,
+            handler=handler,
+            handlerdata=data,
+        ).wait()
+
+        field_info = data["fields"][0]
+        assert field_info["name"] == field
+
+        return field_info
+
+    @classmethod
+    def fetch_field_values(cls, field):
+        """Get the legal values of a field
+
+        Args:
+            field (str): the name of the field
+
+        Returns:
+            List[str]: the legal values of the field
+        """
+        return [value["name"] for value in cls.fetch_field_info(field)["values"]]
```

### Comparing `libmozdata-0.2.3/libmozdata/buildhub.py` & `libmozdata-0.2.4/libmozdata/buildhub.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.3/libmozdata/config.py` & `libmozdata-0.2.4/libmozdata/config.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.3/libmozdata/connection.py` & `libmozdata-0.2.4/libmozdata/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
             "url: %s" % self.url + self.params_repr(params) for params in params_list
         )
 
 
 class Connection(object):
     """Represents a connection to a server"""
 
+    VERIFY_SSL = True
     TIMEOUT = 30
     MAX_RETRIES = 256
     MAX_WORKERS = multiprocessing.cpu_count()
     RAISE_ERROR = True
     CHUNK_SIZE = 32
     TOKEN = ""
     USER_AGENT = config.get("User-Agent", "name", "libmozdata")
@@ -186,39 +187,39 @@
                     if isinstance(query.params, dict):
                         self.results.append(
                             self.session.get(
                                 query.url,
                                 params=query.params,
                                 headers=header,
                                 auth=auth,
-                                verify=True,
+                                verify=self.VERIFY_SSL,
                                 timeout=self.TIMEOUT,
                                 hooks={"response": cb},
                             )
                         )
                     else:
                         for p in query.params:
                             self.results.append(
                                 self.session.get(
                                     query.url,
                                     params=p,
                                     headers=header,
                                     auth=auth,
-                                    verify=True,
+                                    verify=self.VERIFY_SSL,
                                     timeout=self.TIMEOUT,
                                     hooks={"response": cb},
                                 )
                             )
                 else:
                     self.results.append(
                         self.session.get(
                             query.url,
                             headers=header,
                             auth=auth,
-                            verify=True,
+                            verify=self.VERIFY_SSL,
                             timeout=self.TIMEOUT,
                             hooks={"response": cb},
                         )
                     )
 
     @staticmethod
     def chunks(data, chunk_size=CHUNK_SIZE):
```

### Comparing `libmozdata-0.2.3/libmozdata/fx_trains.py` & `libmozdata-0.2.4/libmozdata/fx_trains.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.3/libmozdata/handler.py` & `libmozdata-0.2.4/libmozdata/handler.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.3/libmozdata/hgmozilla.py` & `libmozdata-0.2.4/libmozdata/hgmozilla.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.3/libmozdata/lando.py` & `libmozdata-0.2.4/libmozdata/lando.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.3/libmozdata/modules.json` & `libmozdata-0.2.4/libmozdata/modules.json`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.3/libmozdata/modules.py` & `libmozdata-0.2.4/libmozdata/modules.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.3/libmozdata/patchanalysis.py` & `libmozdata-0.2.4/libmozdata/patchanalysis.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.3/libmozdata/phabricator.py` & `libmozdata-0.2.4/libmozdata/phabricator.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.3/libmozdata/redash.py` & `libmozdata-0.2.4/libmozdata/redash.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.3/libmozdata/release_owners.py` & `libmozdata-0.2.4/libmozdata/release_owners.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.3/libmozdata/socorro.py` & `libmozdata-0.2.4/libmozdata/socorro.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,18 +26,17 @@
     def get_header(self):
         header = super(Socorro, self).get_header()
         header["Auth-Token"] = self.get_apikey()
         return header
 
 
 class SuperSearch(Socorro):
-    """SuperSearch: https://crash-stats.mozilla.org/search/?product=&_dont_run=1"""
+    """SuperSearch: https://crash-stats.mozilla.org/api/#SuperSearch"""
 
     URL = Socorro.API_URL + "/SuperSearch/"
-    URL_UNREDACTED = Socorro.API_URL + "/SuperSearchUnredacted/"
     WEB_URL = Socorro.CRASH_STATS_URL + "/search/"
 
     def __init__(
         self, params=None, handler=None, handlerdata=None, queries=None, **kwargs
     ):
         """Constructor
 
@@ -46,43 +45,50 @@
             handler (Optional[function]): handler to use with the result of the query
             handlerdata (Optional): data used in second argument of the handler
             queries (Optional[List[Query]]): queries to execute
         """
         if queries is not None:
             super(SuperSearch, self).__init__(queries, **kwargs)
         else:
-            url = SuperSearch.URL
-            unredacted = False
-            if "_facets" in params:
-                facets = params["_facets"]
-                if "url" in facets or "email" in facets:
-                    url = SuperSearch.URL_UNREDACTED
-                    unredacted = True
-            if not unredacted and "_columns" in params:
-                columns = params["_columns"]
-                if "url" in columns or "email" in columns:
-                    url = SuperSearch.URL_UNREDACTED
-            if not unredacted:
-                for k, v in params.items():
-                    if (
-                        "url" in k
-                        or "email" in k
-                        or (
-                            (isinstance(v, list) or isinstance(v, six.string_types))
-                            and ("url" in v or "email" in v)
-                        )
-                    ):
-                        url = SuperSearch.URL_UNREDACTED
-                        unredacted = True
-                        break
-
+            if self.__has_deprecated_unredacted_params(params):
+                raise ValueError(
+                    "Requesting PII data using the `SuperSearch` class is not "
+                    "supported anymore. Please use `SuperSearchUnredacted` instead."
+                )
             super(SuperSearch, self).__init__(
-                Query(url, params, handler, handlerdata), **kwargs
+                Query(self.URL, params, handler, handlerdata), **kwargs
             )
 
+    def __has_deprecated_unredacted_params(self, params):
+        """Check if the params is requesting PII data that we used to
+        automatically support retrieving it by redirecting the request to the
+        unredacted endpoint (i.e., SuperSearchUnredacted).
+        """
+        unredacted = False
+        if "_facets" in params:
+            facets = params["_facets"]
+            if "url" in facets or "email" in facets:
+                unredacted = True
+        if not unredacted and "_columns" in params:
+            columns = params["_columns"]
+            if "url" in columns or "email" in columns:
+                unredacted = True
+        if not unredacted:
+            for k, v in params.items():
+                if (
+                    "url" in k
+                    or "email" in k
+                    or (
+                        (isinstance(v, list) or isinstance(v, six.string_types))
+                        and ("url" in v or "email" in v)
+                    )
+                ):
+                    unredacted = True
+        return unredacted
+
     @staticmethod
     def get_link(params):
         return utils.get_url(SuperSearch.WEB_URL) + utils.get_params_for_url(params)
 
     @staticmethod
     def get_search_date(start, end=None):
         """Get a search date list for [start, end[ (end can be in the future)
@@ -105,14 +111,20 @@
                 search_date = [">=" + _start, "<" + utils.get_date_str(_end)]
         else:
             search_date = [">=" + _start]
 
         return search_date
 
 
+class SuperSearchUnredacted(SuperSearch):
+    """SuperSearchUnredacted: https://crash-stats.mozilla.org/api/#SuperSearchUnredacted"""
+
+    URL = Socorro.API_URL + "/SuperSearchUnredacted/"
+
+
 class ProcessedCrash(Socorro):
     """ProcessedCrash: https://crash-stats.mozilla.org/api/#ProcessedCrash"""
 
     URL = Socorro.API_URL + "/ProcessedCrash/"
 
     def __init__(
         self, params=None, handler=None, handlerdata=None, queries=None, **kwargs
@@ -240,7 +252,54 @@
                 )
             Bugs(queries=queries).wait()
 
         for k, v in data.items():
             data[k] = list(v)
 
         return data
+
+
+class SignatureFirstDate(Socorro):
+    """SignatureFirstDate: https://crash-stats.mozilla.org/api/#SignatureFirstDate"""
+
+    URL = Socorro.API_URL + "/SignatureFirstDate/"
+
+    def __init__(
+        self, params=None, handler=None, handlerdata=None, queries=None, **kwargs
+    ):
+        """Constructor
+
+        Args:
+            params (Optional[dict]): the params for the query
+            handler (Optional[function]): handler to use with the result of the query
+            handlerdata (Optional): data used in second argument of the handler
+            queries (Optional[List[Query]]): queries to execute
+        """
+        if queries:
+            super(SignatureFirstDate, self).__init__(queries, **kwargs)
+        else:
+            super(SignatureFirstDate, self).__init__(
+                Query(SignatureFirstDate.URL, params, handler, handlerdata), **kwargs
+            )
+
+    @staticmethod
+    def get_signatures(signatures):
+        """Get the first date and build id for the specified signatures.
+
+        Args:
+            signatures (List[str]): signatures to check.
+
+        Returns:
+            dict: the first date for each signature.
+        """
+
+        def default_handler(json, data):
+            data.extend(json["hits"])
+
+        data = []
+        SignatureFirstDate(
+            params={"signatures": signatures},
+            handler=default_handler,
+            handlerdata=data,
+        ).wait()
+
+        return data
```

### Comparing `libmozdata-0.2.3/libmozdata/utils.py` & `libmozdata-0.2.4/libmozdata/utils.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.3/libmozdata/vcs_map.py` & `libmozdata-0.2.4/libmozdata/vcs_map.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.3/libmozdata/versions.py` & `libmozdata-0.2.4/libmozdata/versions.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.3/libmozdata/wiki_parser.py` & `libmozdata-0.2.4/libmozdata/wiki_parser.py`

 * *Files identical despite different names*

### Comparing `libmozdata-0.2.3/libmozdata.egg-info/SOURCES.txt` & `libmozdata-0.2.4/libmozdata.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 libmozdata/BZInfo.py
 libmozdata/FXRevision.py
 libmozdata/FileStats.py
 libmozdata/HGFileInfo.py
 libmozdata/__init__.py
 libmozdata/bugzilla.py
 libmozdata/buildhub.py
+libmozdata/clouseau.py
 libmozdata/config.py
 libmozdata/connection.py
 libmozdata/fx_trains.py
 libmozdata/handler.py
 libmozdata/hgmozilla.py
 libmozdata/lando.py
 libmozdata/modules.json
```

### Comparing `libmozdata-0.2.3/setup.py` & `libmozdata-0.2.4/setup.py`

 * *Files identical despite different names*


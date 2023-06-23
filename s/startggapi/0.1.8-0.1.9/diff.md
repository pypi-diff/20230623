# Comparing `tmp/startggapi-0.1.8.tar.gz` & `tmp/startggapi-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "startggapi-0.1.8.tar", last modified: Sun Aug 28 04:44:00 2022, max compression
+gzip compressed data, was "startggapi-0.1.9.tar", last modified: Sun Aug 28 06:09:19 2022, max compression
```

## Comparing `startggapi-0.1.8.tar` & `startggapi-0.1.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 04:44:00.164858 startggapi-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1095 2022-08-28 04:43:50.000000 startggapi-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      411 2022-08-28 04:44:00.164858 startggapi-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-08-28 04:43:50.000000 startggapi-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-28 04:44:00.164858 startggapi-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1048 2022-08-28 04:43:50.000000 startggapi-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 04:44:00.160858 startggapi-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 04:44:00.160858 startggapi-0.1.8/src/startggapi/
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-08-28 04:43:50.000000 startggapi-0.1.8/src/startggapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-08-28 04:43:50.000000 startggapi-0.1.8/src/startggapi/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 04:44:00.164858 startggapi-0.1.8/src/startggapi/_apis/
--rw-r--r--   0 runner    (1001) docker     (121)      554 2022-08-28 04:43:50.000000 startggapi-0.1.8/src/startggapi/_apis/BaseApi.py
--rw-r--r--   0 runner    (1001) docker     (121)     3523 2022-08-28 04:43:50.000000 startggapi-0.1.8/src/startggapi/_apis/EntrantApi.py
--rw-r--r--   0 runner    (1001) docker     (121)     3054 2022-08-28 04:43:50.000000 startggapi-0.1.8/src/startggapi/_apis/EventApi.py
--rw-r--r--   0 runner    (1001) docker     (121)     3360 2022-08-28 04:43:50.000000 startggapi-0.1.8/src/startggapi/_apis/QueryStrings.py
--rw-r--r--   0 runner    (1001) docker     (121)     3313 2022-08-28 04:43:50.000000 startggapi-0.1.8/src/startggapi/_apis/TournamentApi.py
--rw-r--r--   0 runner    (1001) docker     (121)      205 2022-08-28 04:43:50.000000 startggapi-0.1.8/src/startggapi/_apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      593 2022-08-28 04:43:50.000000 startggapi-0.1.8/src/startggapi/startggapi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 04:44:00.160858 startggapi-0.1.8/src/startggapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      411 2022-08-28 04:44:00.000000 startggapi-0.1.8/src/startggapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      509 2022-08-28 04:44:00.000000 startggapi-0.1.8/src/startggapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-28 04:44:00.000000 startggapi-0.1.8/src/startggapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-08-28 04:44:00.000000 startggapi-0.1.8/src/startggapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-08-28 04:44:00.000000 startggapi-0.1.8/src/startggapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 06:09:19.346647 startggapi-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1095 2022-08-28 06:09:09.000000 startggapi-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      411 2022-08-28 06:09:19.346647 startggapi-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      145 2022-08-28 06:09:09.000000 startggapi-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-28 06:09:19.346647 startggapi-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1048 2022-08-28 06:09:09.000000 startggapi-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 06:09:19.346647 startggapi-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 06:09:19.346647 startggapi-0.1.9/src/startggapi/
+-rw-r--r--   0 runner    (1001) docker     (121)      127 2022-08-28 06:09:09.000000 startggapi-0.1.9/src/startggapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2022-08-28 06:09:09.000000 startggapi-0.1.9/src/startggapi/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 06:09:19.346647 startggapi-0.1.9/src/startggapi/_apis/
+-rw-r--r--   0 runner    (1001) docker     (121)      554 2022-08-28 06:09:09.000000 startggapi-0.1.9/src/startggapi/_apis/BaseApi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3523 2022-08-28 06:09:09.000000 startggapi-0.1.9/src/startggapi/_apis/EntrantApi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3054 2022-08-28 06:09:09.000000 startggapi-0.1.9/src/startggapi/_apis/EventApi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3360 2022-08-28 06:09:09.000000 startggapi-0.1.9/src/startggapi/_apis/QueryStrings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3163 2022-08-28 06:09:09.000000 startggapi-0.1.9/src/startggapi/_apis/TournamentApi.py
+-rw-r--r--   0 runner    (1001) docker     (121)      205 2022-08-28 06:09:09.000000 startggapi-0.1.9/src/startggapi/_apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      593 2022-08-28 06:09:09.000000 startggapi-0.1.9/src/startggapi/startggapi.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 06:09:19.346647 startggapi-0.1.9/src/startggapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      411 2022-08-28 06:09:19.000000 startggapi-0.1.9/src/startggapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      509 2022-08-28 06:09:19.000000 startggapi-0.1.9/src/startggapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-28 06:09:19.000000 startggapi-0.1.9/src/startggapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       68 2022-08-28 06:09:19.000000 startggapi-0.1.9/src/startggapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2022-08-28 06:09:19.000000 startggapi-0.1.9/src/startggapi.egg-info/top_level.txt
```

### Comparing `startggapi-0.1.8/LICENSE` & `startggapi-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `startggapi-0.1.8/setup.py` & `startggapi-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `startggapi-0.1.8/src/startggapi/_apis/BaseApi.py` & `startggapi-0.1.9/src/startggapi/_apis/BaseApi.py`

 * *Files identical despite different names*

### Comparing `startggapi-0.1.8/src/startggapi/_apis/EntrantApi.py` & `startggapi-0.1.9/src/startggapi/_apis/EntrantApi.py`

 * *Files identical despite different names*

### Comparing `startggapi-0.1.8/src/startggapi/_apis/EventApi.py` & `startggapi-0.1.9/src/startggapi/_apis/EventApi.py`

 * *Files identical despite different names*

### Comparing `startggapi-0.1.8/src/startggapi/_apis/QueryStrings.py` & `startggapi-0.1.9/src/startggapi/_apis/QueryStrings.py`

 * *Files identical despite different names*

### Comparing `startggapi-0.1.8/src/startggapi/_apis/TournamentApi.py` & `startggapi-0.1.9/src/startggapi/_apis/TournamentApi.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,17 +71,14 @@
         data["query"] = lookup_query
 
         response = self._base.raw_request("https://api.start.gg/gql/alpha", data)
         return json.loads(response.content)
 
     def find_all_by_coords(self, coords, before_date=None, after_date=None, per_page=None, radius=None):
         default_page_size = 50
-        before_date = datetime.datetime.now() - datetime.timedelta(days=1)
-        after_date = datetime.datetime.now() - datetime.timedelta(days=7)
-
         all_tournaments = []
         if per_page:
             default_page_size = per_page
         response = self.find_by_coords(coords, before_date=before_date, after_date=after_date, page=1, per_page=default_page_size, radius=radius)
         all_tournaments += response["data"]["tournaments"]["nodes"]
         if "pageInfo" in response["data"]["tournaments"]:
             total_pages = response["data"]["tournaments"]["pageInfo"]["totalPages"]
```

### Comparing `startggapi-0.1.8/src/startggapi/startggapi.py` & `startggapi-0.1.9/src/startggapi/startggapi.py`

 * *Files identical despite different names*


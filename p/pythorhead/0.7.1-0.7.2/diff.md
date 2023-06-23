# Comparing `tmp/pythorhead-0.7.1.tar.gz` & `tmp/pythorhead-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythorhead-0.7.1.tar", last modified: Thu Jun 22 00:00:37 2023, max compression
+gzip compressed data, was "pythorhead-0.7.2.tar", last modified: Fri Jun 23 10:19:03 2023, max compression
```

## Comparing `pythorhead-0.7.1.tar` & `pythorhead-0.7.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:00:37.173448 pythorhead-0.7.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:00:37.169448 pythorhead-0.7.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:00:37.169448 pythorhead-0.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-22 00:00:21.000000 pythorhead-0.7.1/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-22 00:00:21.000000 pythorhead-0.7.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-06-22 00:00:27.000000 pythorhead-0.7.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-22 00:00:21.000000 pythorhead-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    41109 2023-06-22 00:00:37.173448 pythorhead-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-22 00:00:21.000000 pythorhead-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:00:37.169448 pythorhead-0.7.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-22 00:00:21.000000 pythorhead-0.7.1/examples/pm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-22 00:00:21.000000 pythorhead-0.7.1/examples/user.py
--rw-r--r--   0 runner    (1001) docker     (123)   121595 2023-06-22 00:00:21.000000 pythorhead-0.7.1/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-22 00:00:27.000000 pythorhead-0.7.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:00:37.173448 pythorhead-0.7.1/pythorhead/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-22 00:00:21.000000 pythorhead-0.7.1/pythorhead/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-22 00:00:21.000000 pythorhead-0.7.1/pythorhead/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-06-22 00:00:21.000000 pythorhead-0.7.1/pythorhead/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-22 00:00:21.000000 pythorhead-0.7.1/pythorhead/lemmy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-06-22 00:00:21.000000 pythorhead-0.7.1/pythorhead/post.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-22 00:00:21.000000 pythorhead-0.7.1/pythorhead/private_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-06-22 00:00:21.000000 pythorhead-0.7.1/pythorhead/requestor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-06-22 00:00:21.000000 pythorhead-0.7.1/pythorhead/site.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:00:37.173448 pythorhead-0.7.1/pythorhead/types/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-22 00:00:21.000000 pythorhead-0.7.1/pythorhead/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-22 00:00:21.000000 pythorhead-0.7.1/pythorhead/types/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-22 00:00:21.000000 pythorhead-0.7.1/pythorhead/types/listing.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-22 00:00:21.000000 pythorhead-0.7.1/pythorhead/types/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-22 00:00:21.000000 pythorhead-0.7.1/pythorhead/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:00:37.173448 pythorhead-0.7.1/pythorhead.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    41109 2023-06-22 00:00:37.000000 pythorhead-0.7.1/pythorhead.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-22 00:00:37.000000 pythorhead-0.7.1/pythorhead.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 00:00:37.000000 pythorhead-0.7.1/pythorhead.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-22 00:00:37.000000 pythorhead-0.7.1/pythorhead.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 00:00:21.000000 pythorhead-0.7.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 00:00:37.173448 pythorhead-0.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:03.254359 pythorhead-0.7.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:03.250359 pythorhead-0.7.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:03.250359 pythorhead-0.7.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-23 10:18:47.000000 pythorhead-0.7.2/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-23 10:18:47.000000 pythorhead-0.7.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-06-23 10:18:53.000000 pythorhead-0.7.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-23 10:18:47.000000 pythorhead-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    41109 2023-06-23 10:19:03.254359 pythorhead-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-23 10:18:47.000000 pythorhead-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:03.250359 pythorhead-0.7.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-23 10:18:47.000000 pythorhead-0.7.2/examples/pm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-23 10:18:47.000000 pythorhead-0.7.2/examples/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121595 2023-06-23 10:18:47.000000 pythorhead-0.7.2/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-23 10:18:53.000000 pythorhead-0.7.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:03.250359 pythorhead-0.7.2/pythorhead/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-23 10:18:47.000000 pythorhead-0.7.2/pythorhead/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-23 10:18:47.000000 pythorhead-0.7.2/pythorhead/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-06-23 10:18:47.000000 pythorhead-0.7.2/pythorhead/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-23 10:18:47.000000 pythorhead-0.7.2/pythorhead/lemmy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9197 2023-06-23 10:18:47.000000 pythorhead-0.7.2/pythorhead/post.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-23 10:18:47.000000 pythorhead-0.7.2/pythorhead/private_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-06-23 10:18:47.000000 pythorhead-0.7.2/pythorhead/requestor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-06-23 10:18:47.000000 pythorhead-0.7.2/pythorhead/site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:03.254359 pythorhead-0.7.2/pythorhead/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-23 10:18:47.000000 pythorhead-0.7.2/pythorhead/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-23 10:18:47.000000 pythorhead-0.7.2/pythorhead/types/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-23 10:18:47.000000 pythorhead-0.7.2/pythorhead/types/listing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-23 10:18:47.000000 pythorhead-0.7.2/pythorhead/types/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-23 10:18:47.000000 pythorhead-0.7.2/pythorhead/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:19:03.254359 pythorhead-0.7.2/pythorhead.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    41109 2023-06-23 10:19:03.000000 pythorhead-0.7.2/pythorhead.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-23 10:19:03.000000 pythorhead-0.7.2/pythorhead.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 10:19:03.000000 pythorhead-0.7.2/pythorhead.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-23 10:19:03.000000 pythorhead-0.7.2/pythorhead.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 10:18:47.000000 pythorhead-0.7.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 10:19:03.254359 pythorhead-0.7.2/setup.cfg
```

### Comparing `pythorhead-0.7.1/.github/workflows/pypi.yml` & `pythorhead-0.7.2/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `pythorhead-0.7.1/.gitignore` & `pythorhead-0.7.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pythorhead-0.7.1/CHANGELOG.md` & `pythorhead-0.7.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 # Changelog
 
+## [v0.7.2](https://github.com/db0/pythorhead/tree/v0.7.2) (2023-06-23)
+
+[Full Changelog](https://github.com/db0/pythorhead/compare/v0.7.1...v0.7.2)
+
+**Merged pull requests:**
+
+- added comment methods [\#20](https://github.com/db0/pythorhead/pull/20) ([retiolus](https://github.com/retiolus))
+- added post methods [\#19](https://github.com/db0/pythorhead/pull/19) ([retiolus](https://github.com/retiolus))
+
 ## [v0.7.1](https://github.com/db0/pythorhead/tree/v0.7.1) (2023-06-21)
 
 [Full Changelog](https://github.com/db0/pythorhead/compare/v0.7.0...v0.7.1)
 
 **Merged pull requests:**
 
 - feat: Allow multiple lemmy instances logged in to different sites [\#17](https://github.com/db0/pythorhead/pull/17) ([db0](https://github.com/db0))
```

### Comparing `pythorhead-0.7.1/LICENSE` & `pythorhead-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pythorhead-0.7.1/PKG-INFO` & `pythorhead-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythorhead
-Version: 0.7.1
+Version: 0.7.2
 Summary: A python library for interacting with Lemmy API
 Author-email: db0 <mail@dbzer0.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pythorhead-0.7.1/README.md` & `pythorhead-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `pythorhead-0.7.1/examples/pm.py` & `pythorhead-0.7.2/examples/pm.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.7.1/examples/user.py` & `pythorhead-0.7.2/examples/user.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.7.1/logo.png` & `pythorhead-0.7.2/logo.png`

 * *Files identical despite different names*

### Comparing `pythorhead-0.7.1/pyproject.toml` & `pythorhead-0.7.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "pythorhead"
 description = "A python library for interacting with Lemmy API"
 authors = [
     {name = "db0", email = "mail@dbzer0.com"},
 ]
-version = "v0.7.1"
+version = "v0.7.2"
 readme = "README.md"
 requires-python = ">=3.8,<3.11"
 license = { file="LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Affero General Public License v3",
     "Operating System :: OS Independent",
```

### Comparing `pythorhead-0.7.1/pythorhead/comment.py` & `pythorhead-0.7.2/pythorhead/comment.py`

 * *Files 6% similar despite different names*

```diff
@@ -248,8 +248,28 @@
             "/comment/report",
             json={
                 "comment_id": comment_id,
                 "reason": reason,
             },
         )
 
+    def mark_as_read(self, comment_reply_id: int, read: bool) -> Optional[dict]:
+        """
+
+        Mark a comment as read
+
+        Args:
+            comment_reply_id (int)
+            read (bool)
+
+        Returns:
+            Optional[dict]: comment data if successful
+        """
+
+        mark_as_read_comment = {
+            "comment_reply_id": comment_reply_id,
+            "read": read,
+        }
+        return self._requestor.request(Request.POST, "/comment/mark_as_read", json=mark_as_read_comment)
+
+
     __call__ = create
```

### Comparing `pythorhead-0.7.1/pythorhead/lemmy.py` & `pythorhead-0.7.2/pythorhead/lemmy.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.7.1/pythorhead/post.py` & `pythorhead-0.7.2/pythorhead/post.py`

 * *Files 9% similar despite different names*

```diff
@@ -270,8 +270,63 @@
         feature_post = {
             "post_id": post_id,
             "featured": feature,
             "feature_type": feature_type.value,
         }
         return self._requestor.request(Request.POST, "/post/feature", json=feature_post)
 
+    def lock(self, post_id: int, locked: bool) -> Optional[dict]:
+        """
+
+        A moderator can lock a post ( IE disable new comments )
+
+        Args:
+            post_id (int)
+            locked (bool)
+
+        Returns:
+            Optional[dict]: post data if successful
+        """
+
+        lock_post = {
+            "post_id": post_id,
+            "locked": locked,
+        }
+        return self._requestor.request(Request.POST, "/post/lock", json=lock_post)
+
+    def mark_as_read(self, post_id: int, read: bool) -> Optional[dict]:
+        """
+
+        Mark a post as read
+
+        Args:
+            post_id (int)
+            read (bool)
+
+        Returns:
+            Optional[dict]: post data if successful
+        """
+
+        mark_as_read_post = {
+            "post_id": post_id,
+            "read": read,
+        }
+        return self._requestor.request(Request.POST, "/post/mark_as_read", json=mark_as_read_post)
+
+    def site_metadata(self, url: str) -> Optional[dict]:
+        """
+
+        Fetch metadata for any given site.
+
+        Args:
+            url (str)
+
+        Returns:
+            Optional[dict]: post data if successful
+        """
+
+        site_metadata_post = {
+            "url": url,
+        }
+        return self._requestor.request(Request.GET, "/post/site_metadata", params=site_metadata_post)
+
     __call__ = create
```

### Comparing `pythorhead-0.7.1/pythorhead/private_message.py` & `pythorhead-0.7.2/pythorhead/private_message.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.7.1/pythorhead/requestor.py` & `pythorhead-0.7.2/pythorhead/requestor.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.7.1/pythorhead/site.py` & `pythorhead-0.7.2/pythorhead/site.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.7.1/pythorhead/user.py` & `pythorhead-0.7.2/pythorhead/user.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.7.1/pythorhead.egg-info/PKG-INFO` & `pythorhead-0.7.2/pythorhead.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythorhead
-Version: 0.7.1
+Version: 0.7.2
 Summary: A python library for interacting with Lemmy API
 Author-email: db0 <mail@dbzer0.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pythorhead-0.7.1/pythorhead.egg-info/SOURCES.txt` & `pythorhead-0.7.2/pythorhead.egg-info/SOURCES.txt`

 * *Files identical despite different names*


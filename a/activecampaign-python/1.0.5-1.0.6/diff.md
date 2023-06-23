# Comparing `tmp/activecampaign-python-1.0.5.tar.gz` & `tmp/activecampaign_python-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "activecampaign-python-1.0.5.tar", last modified: Wed Nov 23 16:39:02 2022, max compression
+gzip compressed data, was "activecampaign_python-1.0.6.tar", max compression
```

## Comparing `activecampaign-python-1.0.5.tar` & `activecampaign_python-1.0.6.tar`

### file list

```diff
@@ -1,31 +1,20 @@
-drwxr-xr-x   0 ingmferrer  (1000) ingmferrer  (1000)        0 2022-11-23 16:39:02.471392 activecampaign-python-1.0.5/
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)     1065 2022-07-06 14:57:32.000000 activecampaign-python-1.0.5/LICENSE
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)       18 2022-07-06 14:57:32.000000 activecampaign-python-1.0.5/MANIFEST.in
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)    11982 2022-11-23 16:39:02.471392 activecampaign-python-1.0.5/PKG-INFO
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)    11627 2022-07-06 14:57:32.000000 activecampaign-python-1.0.5/README.md
-drwxr-xr-x   0 ingmferrer  (1000) ingmferrer  (1000)        0 2022-11-23 16:39:02.461392 activecampaign-python-1.0.5/activecampaign/
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)        0 2022-07-06 14:57:32.000000 activecampaign-python-1.0.5/activecampaign/__init__.py
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)      245 2022-07-06 14:57:32.000000 activecampaign-python-1.0.5/activecampaign/automations.py
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)     2118 2022-11-23 16:37:32.000000 activecampaign-python-1.0.5/activecampaign/client.py
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)     5856 2022-07-13 14:20:12.000000 activecampaign-python-1.0.5/activecampaign/contacts.py
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)      255 2022-11-23 16:37:32.000000 activecampaign-python-1.0.5/activecampaign/dealActivities.py
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)     4374 2022-11-23 16:37:32.000000 activecampaign-python-1.0.5/activecampaign/deals.py
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)     3782 2022-11-23 16:37:32.000000 activecampaign-python-1.0.5/activecampaign/deepdataintegrations.py
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)      258 2022-11-23 16:37:32.000000 activecampaign-python-1.0.5/activecampaign/emailActivities.py
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)       86 2022-07-06 14:57:32.000000 activecampaign-python-1.0.5/activecampaign/exception.py
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)     1485 2022-07-06 14:57:32.000000 activecampaign-python-1.0.5/activecampaign/lists.py
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)      268 2022-07-06 14:57:32.000000 activecampaign-python-1.0.5/activecampaign/messages.py
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)     1165 2022-07-06 14:57:32.000000 activecampaign-python-1.0.5/activecampaign/notes.py
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)     1099 2022-07-06 14:57:32.000000 activecampaign-python-1.0.5/activecampaign/tags.py
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)     1157 2022-07-06 14:57:32.000000 activecampaign-python-1.0.5/activecampaign/tasks.py
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)     2148 2022-07-06 14:57:32.000000 activecampaign-python-1.0.5/activecampaign/users.py
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)     1380 2022-07-06 14:57:32.000000 activecampaign-python-1.0.5/activecampaign/webhooks.py
-drwxr-xr-x   0 ingmferrer  (1000) ingmferrer  (1000)        0 2022-11-23 16:39:02.471392 activecampaign-python-1.0.5/activecampaign_python.egg-info/
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)    11982 2022-11-23 16:39:02.000000 activecampaign-python-1.0.5/activecampaign_python.egg-info/PKG-INFO
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)      746 2022-11-23 16:39:02.000000 activecampaign-python-1.0.5/activecampaign_python.egg-info/SOURCES.txt
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)        1 2022-11-23 16:39:02.000000 activecampaign-python-1.0.5/activecampaign_python.egg-info/dependency_links.txt
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)        1 2022-07-13 15:26:43.000000 activecampaign-python-1.0.5/activecampaign_python.egg-info/not-zip-safe
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)        9 2022-11-23 16:39:02.000000 activecampaign-python-1.0.5/activecampaign_python.egg-info/requires.txt
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)       15 2022-11-23 16:39:02.000000 activecampaign-python-1.0.5/activecampaign_python.egg-info/top_level.txt
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)       38 2022-11-23 16:39:02.471392 activecampaign-python-1.0.5/setup.cfg
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)      631 2022-11-23 16:38:45.000000 activecampaign-python-1.0.5/setup.py
+-rw-r--r--   0        0        0     1065 2023-03-27 20:59:00.982544 activecampaign_python-1.0.6/LICENSE
+-rw-r--r--   0        0        0    11611 2023-03-27 20:59:00.982784 activecampaign_python-1.0.6/README.md
+-rw-r--r--   0        0        0        0 2023-03-27 20:59:00.982882 activecampaign_python-1.0.6/activecampaign/__init__.py
+-rw-r--r--   0        0        0      245 2023-03-27 20:59:00.983020 activecampaign_python-1.0.6/activecampaign/automations.py
+-rw-r--r--   0        0        0     2118 2023-03-27 20:59:00.983114 activecampaign_python-1.0.6/activecampaign/client.py
+-rw-r--r--   0        0        0     5856 2023-03-27 20:59:00.983212 activecampaign_python-1.0.6/activecampaign/contacts.py
+-rw-r--r--   0        0        0      255 2023-03-27 20:59:00.983313 activecampaign_python-1.0.6/activecampaign/dealActivities.py
+-rw-r--r--   0        0        0     4374 2023-03-27 20:59:00.983429 activecampaign_python-1.0.6/activecampaign/deals.py
+-rw-r--r--   0        0        0     3782 2023-03-27 20:59:00.983524 activecampaign_python-1.0.6/activecampaign/deepdataintegrations.py
+-rw-r--r--   0        0        0      258 2023-03-27 20:59:00.983601 activecampaign_python-1.0.6/activecampaign/emailActivities.py
+-rw-r--r--   0        0        0       86 2023-03-27 20:59:00.983691 activecampaign_python-1.0.6/activecampaign/exception.py
+-rw-r--r--   0        0        0     1485 2023-03-27 20:59:00.983787 activecampaign_python-1.0.6/activecampaign/lists.py
+-rw-r--r--   0        0        0      268 2023-03-27 20:59:00.983875 activecampaign_python-1.0.6/activecampaign/messages.py
+-rw-r--r--   0        0        0     1165 2023-03-27 20:59:00.983965 activecampaign_python-1.0.6/activecampaign/notes.py
+-rw-r--r--   0        0        0     1099 2023-03-27 20:59:00.984046 activecampaign_python-1.0.6/activecampaign/tags.py
+-rw-r--r--   0        0        0     1157 2023-03-27 20:59:00.984140 activecampaign_python-1.0.6/activecampaign/tasks.py
+-rw-r--r--   0        0        0     2148 2023-03-27 20:59:00.984242 activecampaign_python-1.0.6/activecampaign/users.py
+-rw-r--r--   0        0        0     1380 2023-03-27 20:59:00.984331 activecampaign_python-1.0.6/activecampaign/webhooks.py
+-rw-r--r--   0        0        0      415 2023-03-27 20:59:50.362250 activecampaign_python-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0    12272 1970-01-01 00:00:00.000000 activecampaign_python-1.0.6/PKG-INFO
```

### Comparing `activecampaign-python-1.0.5/LICENSE` & `activecampaign_python-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `activecampaign-python-1.0.5/PKG-INFO` & `activecampaign_python-1.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: activecampaign-python
-Version: 1.0.5
-Summary: ActiveCampaign API written in python
-Home-page: https://github.com/GearPlug/activecampaign-python
-Author: Miguel Ferrer
-Author-email: ingferrermiguel@gmail.com
-License: MIT
-Keywords: activecampaign
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # activecampaign-python
 ActiveCampaign API wrapper written in python.
 
 This library supports the latest API version 3. If you are looking for API version 1 which is also supported by ActiveCampaign then check below.
 
 ## Installing (API v3)
 
@@ -594,37 +581,37 @@
     }
 }
 response = client.tags.create_a_tag(data)
 ```
 
 #### Retrieve a tag
 ```
-response = client.webhooks.retrieve_a_tag("tag_id")
+response = client.tags.retrieve_a_tag("tag_id")
 ```
 
 #### Update a tag
 ```
 data = {
     "tag":{
         "tag": "My Tag",
         "tagType": "contact",
         "description": "Description"
     }
 }
-response = client.webhooks.update_a_tag("tag_id", data)
+response = client.tags.update_a_tag("tag_id", data)
 ```
 
 #### Delete a tag
 ```
-response = client.webhooks.delete_a_tag("tag_id")
+response = client.tags.delete_a_tag("tag_id")
 ```
 
 #### List all tags
 ```
-response = client.webhooks.list_all_tags(search='Tag Name')
+response = client.tags.list_all_tags(search='Tag Name')
 ```
 
 ## About API v1
 
 You can clone and checkout our tag v0.1.1.
 
 ```
@@ -632,9 +619,7 @@
 $ git checkout tags/v0.1.1 -b <branch_name>
 ```
 
 Also you can install this version in pip
 ```
 $ pip install activecampaign-python=0.1.1
 ```
-
-
```

### Comparing `activecampaign-python-1.0.5/README.md` & `activecampaign_python-1.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: activecampaign-python
+Version: 1.0.6
+Summary: API wrapper for ActiveCampaign written in Python
+License: MIT
+Author: Miguel Ferrer
+Author-email: ingferrermiguel@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: requests (>=2.26.0,<3.0.0)
+Description-Content-Type: text/markdown
+
 # activecampaign-python
 ActiveCampaign API wrapper written in python.
 
 This library supports the latest API version 3. If you are looking for API version 1 which is also supported by ActiveCampaign then check below.
 
 ## Installing (API v3)
 
@@ -581,37 +599,37 @@
     }
 }
 response = client.tags.create_a_tag(data)
 ```
 
 #### Retrieve a tag
 ```
-response = client.webhooks.retrieve_a_tag("tag_id")
+response = client.tags.retrieve_a_tag("tag_id")
 ```
 
 #### Update a tag
 ```
 data = {
     "tag":{
         "tag": "My Tag",
         "tagType": "contact",
         "description": "Description"
     }
 }
-response = client.webhooks.update_a_tag("tag_id", data)
+response = client.tags.update_a_tag("tag_id", data)
 ```
 
 #### Delete a tag
 ```
-response = client.webhooks.delete_a_tag("tag_id")
+response = client.tags.delete_a_tag("tag_id")
 ```
 
 #### List all tags
 ```
-response = client.webhooks.list_all_tags(search='Tag Name')
+response = client.tags.list_all_tags(search='Tag Name')
 ```
 
 ## About API v1
 
 You can clone and checkout our tag v0.1.1.
 
 ```
@@ -619,7 +637,8 @@
 $ git checkout tags/v0.1.1 -b <branch_name>
 ```
 
 Also you can install this version in pip
 ```
 $ pip install activecampaign-python=0.1.1
 ```
+
```

### Comparing `activecampaign-python-1.0.5/activecampaign/client.py` & `activecampaign_python-1.0.6/activecampaign/client.py`

 * *Files identical despite different names*

### Comparing `activecampaign-python-1.0.5/activecampaign/contacts.py` & `activecampaign_python-1.0.6/activecampaign/contacts.py`

 * *Files identical despite different names*

### Comparing `activecampaign-python-1.0.5/activecampaign/deals.py` & `activecampaign_python-1.0.6/activecampaign/deals.py`

 * *Files identical despite different names*

### Comparing `activecampaign-python-1.0.5/activecampaign/deepdataintegrations.py` & `activecampaign_python-1.0.6/activecampaign/deepdataintegrations.py`

 * *Files identical despite different names*

### Comparing `activecampaign-python-1.0.5/activecampaign/lists.py` & `activecampaign_python-1.0.6/activecampaign/lists.py`

 * *Files identical despite different names*

### Comparing `activecampaign-python-1.0.5/activecampaign/notes.py` & `activecampaign_python-1.0.6/activecampaign/notes.py`

 * *Files identical despite different names*

### Comparing `activecampaign-python-1.0.5/activecampaign/tags.py` & `activecampaign_python-1.0.6/activecampaign/tags.py`

 * *Files identical despite different names*

### Comparing `activecampaign-python-1.0.5/activecampaign/tasks.py` & `activecampaign_python-1.0.6/activecampaign/tasks.py`

 * *Files identical despite different names*

### Comparing `activecampaign-python-1.0.5/activecampaign/users.py` & `activecampaign_python-1.0.6/activecampaign/users.py`

 * *Files identical despite different names*

### Comparing `activecampaign-python-1.0.5/activecampaign/webhooks.py` & `activecampaign_python-1.0.6/activecampaign/webhooks.py`

 * *Files identical despite different names*


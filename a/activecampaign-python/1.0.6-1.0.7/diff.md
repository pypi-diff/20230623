# Comparing `tmp/activecampaign_python-1.0.6.tar.gz` & `tmp/activecampaign_python-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "activecampaign_python-1.0.6.tar", max compression
+gzip compressed data, was "activecampaign_python-1.0.7.tar", max compression
```

## Comparing `activecampaign_python-1.0.6.tar` & `activecampaign_python-1.0.7.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1065 2023-03-27 20:59:00.982544 activecampaign_python-1.0.6/LICENSE
--rw-r--r--   0        0        0    11611 2023-03-27 20:59:00.982784 activecampaign_python-1.0.6/README.md
--rw-r--r--   0        0        0        0 2023-03-27 20:59:00.982882 activecampaign_python-1.0.6/activecampaign/__init__.py
--rw-r--r--   0        0        0      245 2023-03-27 20:59:00.983020 activecampaign_python-1.0.6/activecampaign/automations.py
--rw-r--r--   0        0        0     2118 2023-03-27 20:59:00.983114 activecampaign_python-1.0.6/activecampaign/client.py
--rw-r--r--   0        0        0     5856 2023-03-27 20:59:00.983212 activecampaign_python-1.0.6/activecampaign/contacts.py
--rw-r--r--   0        0        0      255 2023-03-27 20:59:00.983313 activecampaign_python-1.0.6/activecampaign/dealActivities.py
--rw-r--r--   0        0        0     4374 2023-03-27 20:59:00.983429 activecampaign_python-1.0.6/activecampaign/deals.py
--rw-r--r--   0        0        0     3782 2023-03-27 20:59:00.983524 activecampaign_python-1.0.6/activecampaign/deepdataintegrations.py
--rw-r--r--   0        0        0      258 2023-03-27 20:59:00.983601 activecampaign_python-1.0.6/activecampaign/emailActivities.py
--rw-r--r--   0        0        0       86 2023-03-27 20:59:00.983691 activecampaign_python-1.0.6/activecampaign/exception.py
--rw-r--r--   0        0        0     1485 2023-03-27 20:59:00.983787 activecampaign_python-1.0.6/activecampaign/lists.py
--rw-r--r--   0        0        0      268 2023-03-27 20:59:00.983875 activecampaign_python-1.0.6/activecampaign/messages.py
--rw-r--r--   0        0        0     1165 2023-03-27 20:59:00.983965 activecampaign_python-1.0.6/activecampaign/notes.py
--rw-r--r--   0        0        0     1099 2023-03-27 20:59:00.984046 activecampaign_python-1.0.6/activecampaign/tags.py
--rw-r--r--   0        0        0     1157 2023-03-27 20:59:00.984140 activecampaign_python-1.0.6/activecampaign/tasks.py
--rw-r--r--   0        0        0     2148 2023-03-27 20:59:00.984242 activecampaign_python-1.0.6/activecampaign/users.py
--rw-r--r--   0        0        0     1380 2023-03-27 20:59:00.984331 activecampaign_python-1.0.6/activecampaign/webhooks.py
--rw-r--r--   0        0        0      415 2023-03-27 20:59:50.362250 activecampaign_python-1.0.6/pyproject.toml
--rw-r--r--   0        0        0    12272 1970-01-01 00:00:00.000000 activecampaign_python-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-03-27 20:59:00.982544 activecampaign_python-1.0.7/LICENSE
+-rw-r--r--   0        0        0    15391 2023-06-23 13:30:45.288998 activecampaign_python-1.0.7/README.md
+-rw-r--r--   0        0        0        0 2023-03-27 20:59:00.982882 activecampaign_python-1.0.7/activecampaign/__init__.py
+-rw-r--r--   0        0        0      245 2023-03-27 20:59:00.983020 activecampaign_python-1.0.7/activecampaign/automations.py
+-rw-r--r--   0        0        0     2208 2023-06-23 13:30:45.289185 activecampaign_python-1.0.7/activecampaign/client.py
+-rw-r--r--   0        0        0     5856 2023-03-27 20:59:00.983212 activecampaign_python-1.0.7/activecampaign/contacts.py
+-rw-r--r--   0        0        0     6205 2023-06-23 13:30:45.289308 activecampaign_python-1.0.7/activecampaign/customobjects.py
+-rw-r--r--   0        0        0      255 2023-03-27 20:59:00.983313 activecampaign_python-1.0.7/activecampaign/dealActivities.py
+-rw-r--r--   0        0        0     4374 2023-03-27 20:59:00.983429 activecampaign_python-1.0.7/activecampaign/deals.py
+-rw-r--r--   0        0        0     3782 2023-03-27 20:59:00.983524 activecampaign_python-1.0.7/activecampaign/deepdataintegrations.py
+-rw-r--r--   0        0        0      258 2023-03-27 20:59:00.983601 activecampaign_python-1.0.7/activecampaign/emailActivities.py
+-rw-r--r--   0        0        0       86 2023-03-27 20:59:00.983691 activecampaign_python-1.0.7/activecampaign/exception.py
+-rw-r--r--   0        0        0     1485 2023-03-27 20:59:00.983787 activecampaign_python-1.0.7/activecampaign/lists.py
+-rw-r--r--   0        0        0      268 2023-03-27 20:59:00.983875 activecampaign_python-1.0.7/activecampaign/messages.py
+-rw-r--r--   0        0        0     1165 2023-03-27 20:59:00.983965 activecampaign_python-1.0.7/activecampaign/notes.py
+-rw-r--r--   0        0        0     1099 2023-03-27 20:59:00.984046 activecampaign_python-1.0.7/activecampaign/tags.py
+-rw-r--r--   0        0        0     1157 2023-03-27 20:59:00.984140 activecampaign_python-1.0.7/activecampaign/tasks.py
+-rw-r--r--   0        0        0     2148 2023-03-27 20:59:00.984242 activecampaign_python-1.0.7/activecampaign/users.py
+-rw-r--r--   0        0        0     1380 2023-03-27 20:59:00.984331 activecampaign_python-1.0.7/activecampaign/webhooks.py
+-rw-r--r--   0        0        0      415 2023-06-23 13:30:45.290732 activecampaign_python-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0    16052 1970-01-01 00:00:00.000000 activecampaign_python-1.0.7/PKG-INFO
```

### Comparing `activecampaign_python-1.0.6/LICENSE` & `activecampaign_python-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `activecampaign_python-1.0.6/README.md` & `activecampaign_python-1.0.7/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -606,14 +606,180 @@
 ```
 
 #### List all tags
 ```
 response = client.tags.list_all_tags(search='Tag Name')
 ```
 
+### Custom Objects
+#### Create a schema
+```
+data = {
+  "schema": {
+    "slug": "object-name",
+    "labels": {
+      "singular": "ObjectName",
+      "plural": "ObjectNames"
+    },
+    "description": "Some Description",
+    "fields": [
+      {
+        "id": "some-field-id",
+        "labels": {
+          "singular": "ID",
+          "plural": "IDs"
+        },
+        "type": "text",
+        "required": True,
+      },
+    ],
+    "relationships": [
+      {
+        "id": "primary-contact",
+        "labels": {
+          "singular": "Primary Contact",
+          "plural": "Primary Contacts"
+        },
+        "description": "Primary contact to this object",
+        "namespace": "contacts",
+        "hasMany": False
+      }
+    ]
+  }
+}
+response = client.customobjects.create_a_schema(data=data)
+```
+
+#### Retrieve a schema
+```
+response = client.customobjects.retrieve_a_schema(schema_id="some-id", show_all_fields=False)
+```
+
+#### Update a schema
+```
+data = {
+  "schema": {
+    "slug": "object-name",
+    "labels": {
+      "singular": "ObjectName",
+      "plural": "ObjectNames"
+    },
+    "description": "Some Description",
+    "fields": [
+      {
+        "id": "some-field-id",
+        "labels": {
+          "singular": "ID",
+          "plural": "IDs"
+        },
+        "type": "text",
+        "required": True,
+      },
+      {
+        "id": "some-other-field-id",
+        "labels": {
+          "singular": "OtherID",
+          "plural": "OtherIDs"
+        },
+        "type": "text",
+        "required": True,
+      },
+    ],
+    "relationships": [
+      {
+        "id": "primary-contact",
+        "labels": {
+          "singular": "Primary Contact",
+          "plural": "Primary Contacts"
+        },
+        "description": "Primary contact to this object",
+        "namespace": "contacts",
+        "hasMany": False
+      }
+    ]
+  }
+}
+response = client.customobjects.update_a_schema(schema_id="some-schema-id", data=data, show_all_fields=False)
+```
+
+#### Delete a schema
+```
+response = client.customobjects.delete_a_schema(schema_id="some-id")
+```
+WARNING: This deletes all associated records
+
+#### List all schemas
+```
+response = client.customobjects.list_all_schemas(schema_relationship="contact", limit=20, offset=0, ordering=None, show_all_fields=False)
+```
+
+#### Delete field in schema
+```
+response = client.customobjects.delete_a_field(schema_id="some-id", field_id="some-field-id", show_all_fields=False)
+```
+
+#### Create a public schema
+```
+data = {
+
+}
+response = client.customobjects.create_a_public_schema(data=data)
+```
+
+#### Create a child schema
+```
+response = client.customobjects.create_a_child_schema(parent_id="some-parent-schema-id")
+```
+
+#### Upsert custom object record
+```
+data = {
+  "record": {
+    "fields": [
+      {
+        "id": "some-field-id",
+        "value": "asdf-1234"
+      },
+      {
+        "id": "some-other-field-id",
+        "value": "asdf-5678"
+      },
+    ]
+  }
+}
+response = client.customobjects.create_or_update_record(schema_id="some-id", data=data)
+```
+
+#### Retrieve a record
+```
+response = client.customobjects.retrieve_a_record(schema_id="some-id", record_id="some-record-id")
+```
+
+#### Retrieve a record by external id
+```
+response = client.customobjects.retrieve_a_record_by_external_id(schema_id="some-id", external_id="some-record-id")
+```
+
+#### Delete a record
+```
+response = client.customobjects.delete_a_record(schema_id="some-id", record_id="some-record-id")
+```
+
+#### Delete a record by external id
+```
+response = client.customobjects.delete_a_record_by_external_id(schema_id="some-id", external_id="some-record-id")
+```
+
+#### List all records
+```
+response = client.customobjects.list_all_records(
+        schema_id="some-id", contact_id="some-contact-id", deal_id=None, account_id=None,
+        limit=20, offset=0)
+```
+
 ## About API v1
 
 You can clone and checkout our tag v0.1.1.
 
 ```
 $ git clone https://github.com/GearPlug/activecampaign-python.git
 $ git checkout tags/v0.1.1 -b <branch_name>
```

### Comparing `activecampaign_python-1.0.6/activecampaign/client.py` & `activecampaign_python-1.0.7/activecampaign/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from .tasks import Tasks
 from .users import Users
 from .webhooks import Webhooks
 from .messages import Messages
 from .tags import Tags
 from .emailActivities import EmailActivities
 from .dealActivities import DealActivities
+from .customobjects import CustomObjects
 
 
 class Client(object):
     BASE_URL = '{}/api/3'
 
     def __init__(self, url, api_key):
         self.BASE_URL = self.BASE_URL.format(url)
@@ -31,14 +32,15 @@
         self.users = Users(self)
         self.webhooks = Webhooks(self)
         self.messages = Messages(self)
         self.deepdataintegrations = DeepDataIntegrations(self)
         self.tags = Tags(self)
         self.emailActivities = EmailActivities(self)
         self.dealActivities = DealActivities(self)
+        self.customobjects = CustomObjects(self)
 
     def _get(self, endpoint, **kwargs):
         return self._request('GET', endpoint, **kwargs)
 
     def _post(self, endpoint, **kwargs):
         return self._request('POST', endpoint, **kwargs)
```

### Comparing `activecampaign_python-1.0.6/activecampaign/contacts.py` & `activecampaign_python-1.0.7/activecampaign/contacts.py`

 * *Files identical despite different names*

### Comparing `activecampaign_python-1.0.6/activecampaign/deals.py` & `activecampaign_python-1.0.7/activecampaign/deals.py`

 * *Files identical despite different names*

### Comparing `activecampaign_python-1.0.6/activecampaign/deepdataintegrations.py` & `activecampaign_python-1.0.7/activecampaign/deepdataintegrations.py`

 * *Files identical despite different names*

### Comparing `activecampaign_python-1.0.6/activecampaign/lists.py` & `activecampaign_python-1.0.7/activecampaign/lists.py`

 * *Files identical despite different names*

### Comparing `activecampaign_python-1.0.6/activecampaign/notes.py` & `activecampaign_python-1.0.7/activecampaign/notes.py`

 * *Files identical despite different names*

### Comparing `activecampaign_python-1.0.6/activecampaign/tags.py` & `activecampaign_python-1.0.7/activecampaign/tags.py`

 * *Files identical despite different names*

### Comparing `activecampaign_python-1.0.6/activecampaign/tasks.py` & `activecampaign_python-1.0.7/activecampaign/tasks.py`

 * *Files identical despite different names*

### Comparing `activecampaign_python-1.0.6/activecampaign/users.py` & `activecampaign_python-1.0.7/activecampaign/users.py`

 * *Files identical despite different names*

### Comparing `activecampaign_python-1.0.6/activecampaign/webhooks.py` & `activecampaign_python-1.0.7/activecampaign/webhooks.py`

 * *Files identical despite different names*

### Comparing `activecampaign_python-1.0.6/PKG-INFO` & `activecampaign_python-1.0.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: activecampaign-python
-Version: 1.0.6
+Version: 1.0.7
 Summary: API wrapper for ActiveCampaign written in Python
 License: MIT
 Author: Miguel Ferrer
 Author-email: ingferrermiguel@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -624,14 +624,180 @@
 ```
 
 #### List all tags
 ```
 response = client.tags.list_all_tags(search='Tag Name')
 ```
 
+### Custom Objects
+#### Create a schema
+```
+data = {
+  "schema": {
+    "slug": "object-name",
+    "labels": {
+      "singular": "ObjectName",
+      "plural": "ObjectNames"
+    },
+    "description": "Some Description",
+    "fields": [
+      {
+        "id": "some-field-id",
+        "labels": {
+          "singular": "ID",
+          "plural": "IDs"
+        },
+        "type": "text",
+        "required": True,
+      },
+    ],
+    "relationships": [
+      {
+        "id": "primary-contact",
+        "labels": {
+          "singular": "Primary Contact",
+          "plural": "Primary Contacts"
+        },
+        "description": "Primary contact to this object",
+        "namespace": "contacts",
+        "hasMany": False
+      }
+    ]
+  }
+}
+response = client.customobjects.create_a_schema(data=data)
+```
+
+#### Retrieve a schema
+```
+response = client.customobjects.retrieve_a_schema(schema_id="some-id", show_all_fields=False)
+```
+
+#### Update a schema
+```
+data = {
+  "schema": {
+    "slug": "object-name",
+    "labels": {
+      "singular": "ObjectName",
+      "plural": "ObjectNames"
+    },
+    "description": "Some Description",
+    "fields": [
+      {
+        "id": "some-field-id",
+        "labels": {
+          "singular": "ID",
+          "plural": "IDs"
+        },
+        "type": "text",
+        "required": True,
+      },
+      {
+        "id": "some-other-field-id",
+        "labels": {
+          "singular": "OtherID",
+          "plural": "OtherIDs"
+        },
+        "type": "text",
+        "required": True,
+      },
+    ],
+    "relationships": [
+      {
+        "id": "primary-contact",
+        "labels": {
+          "singular": "Primary Contact",
+          "plural": "Primary Contacts"
+        },
+        "description": "Primary contact to this object",
+        "namespace": "contacts",
+        "hasMany": False
+      }
+    ]
+  }
+}
+response = client.customobjects.update_a_schema(schema_id="some-schema-id", data=data, show_all_fields=False)
+```
+
+#### Delete a schema
+```
+response = client.customobjects.delete_a_schema(schema_id="some-id")
+```
+WARNING: This deletes all associated records
+
+#### List all schemas
+```
+response = client.customobjects.list_all_schemas(schema_relationship="contact", limit=20, offset=0, ordering=None, show_all_fields=False)
+```
+
+#### Delete field in schema
+```
+response = client.customobjects.delete_a_field(schema_id="some-id", field_id="some-field-id", show_all_fields=False)
+```
+
+#### Create a public schema
+```
+data = {
+
+}
+response = client.customobjects.create_a_public_schema(data=data)
+```
+
+#### Create a child schema
+```
+response = client.customobjects.create_a_child_schema(parent_id="some-parent-schema-id")
+```
+
+#### Upsert custom object record
+```
+data = {
+  "record": {
+    "fields": [
+      {
+        "id": "some-field-id",
+        "value": "asdf-1234"
+      },
+      {
+        "id": "some-other-field-id",
+        "value": "asdf-5678"
+      },
+    ]
+  }
+}
+response = client.customobjects.create_or_update_record(schema_id="some-id", data=data)
+```
+
+#### Retrieve a record
+```
+response = client.customobjects.retrieve_a_record(schema_id="some-id", record_id="some-record-id")
+```
+
+#### Retrieve a record by external id
+```
+response = client.customobjects.retrieve_a_record_by_external_id(schema_id="some-id", external_id="some-record-id")
+```
+
+#### Delete a record
+```
+response = client.customobjects.delete_a_record(schema_id="some-id", record_id="some-record-id")
+```
+
+#### Delete a record by external id
+```
+response = client.customobjects.delete_a_record_by_external_id(schema_id="some-id", external_id="some-record-id")
+```
+
+#### List all records
+```
+response = client.customobjects.list_all_records(
+        schema_id="some-id", contact_id="some-contact-id", deal_id=None, account_id=None,
+        limit=20, offset=0)
+```
+
 ## About API v1
 
 You can clone and checkout our tag v0.1.1.
 
 ```
 $ git clone https://github.com/GearPlug/activecampaign-python.git
 $ git checkout tags/v0.1.1 -b <branch_name>
```


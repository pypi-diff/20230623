# Comparing `tmp/python_keycloak-3.0.0.tar.gz` & `tmp/python_keycloak-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_keycloak-3.0.0.tar", max compression
+gzip compressed data, was "python_keycloak-3.1.0.tar", max compression
```

## Comparing `python_keycloak-3.0.0.tar` & `python_keycloak-3.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     6341 2023-05-28 13:27:36.721203 python_keycloak-3.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     3192 2023-05-28 13:27:36.721203 python_keycloak-3.0.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1111 2023-05-28 13:27:36.721203 python_keycloak-3.0.0/LICENSE
--rw-r--r--   0        0        0    14613 2023-05-28 13:27:36.721203 python_keycloak-3.0.0/README.md
--rw-r--r--   0        0        0     2342 2023-05-28 13:27:56.941684 python_keycloak-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     2375 2023-05-28 13:27:36.721203 python_keycloak-3.0.0/src/keycloak/__init__.py
--rw-r--r--   0        0        0     1268 2023-05-28 13:27:36.721203 python_keycloak-3.0.0/src/keycloak/_version.py
--rw-r--r--   0        0        0     3823 2023-05-28 13:27:36.721203 python_keycloak-3.0.0/src/keycloak/authorization/__init__.py
--rw-r--r--   0        0        0     4421 2023-05-28 13:27:36.721203 python_keycloak-3.0.0/src/keycloak/authorization/permission.py
--rw-r--r--   0        0        0     5252 2023-05-28 13:27:36.721203 python_keycloak-3.0.0/src/keycloak/authorization/policy.py
--rw-r--r--   0        0        0     2306 2023-05-28 13:27:36.721203 python_keycloak-3.0.0/src/keycloak/authorization/role.py
--rw-r--r--   0        0        0     8909 2023-05-28 13:27:36.721203 python_keycloak-3.0.0/src/keycloak/connection.py
--rw-r--r--   0        0        0     5464 2023-05-28 13:27:36.725204 python_keycloak-3.0.0/src/keycloak/exceptions.py
--rw-r--r--   0        0        0   161511 2023-05-28 13:27:36.725204 python_keycloak-3.0.0/src/keycloak/keycloak_admin.py
--rw-r--r--   0        0        0    25390 2023-05-28 13:27:36.725204 python_keycloak-3.0.0/src/keycloak/keycloak_openid.py
--rw-r--r--   0        0        0    15376 2023-05-28 13:27:36.725204 python_keycloak-3.0.0/src/keycloak/keycloak_uma.py
--rw-r--r--   0        0        0    11781 2023-05-28 13:27:36.725204 python_keycloak-3.0.0/src/keycloak/openid_connection.py
--rw-r--r--   0        0        0     8767 2023-05-28 13:27:36.725204 python_keycloak-3.0.0/src/keycloak/uma_permissions.py
--rw-r--r--   0        0        0    11800 2023-05-28 13:27:36.725204 python_keycloak-3.0.0/src/keycloak/urls_patterns.py
--rw-r--r--   0        0        0    16384 1970-01-01 00:00:00.000000 python_keycloak-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     6459 2023-06-23 05:23:09.561340 python_keycloak-3.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     3192 2023-06-23 05:23:09.561340 python_keycloak-3.1.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1111 2023-06-23 05:23:09.561340 python_keycloak-3.1.0/LICENSE
+-rw-r--r--   0        0        0    14613 2023-06-23 05:23:09.561340 python_keycloak-3.1.0/README.md
+-rw-r--r--   0        0        0     2342 2023-06-23 05:23:28.349686 python_keycloak-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2375 2023-06-23 05:23:09.565341 python_keycloak-3.1.0/src/keycloak/__init__.py
+-rw-r--r--   0        0        0     1268 2023-06-23 05:23:09.565341 python_keycloak-3.1.0/src/keycloak/_version.py
+-rw-r--r--   0        0        0     3823 2023-06-23 05:23:09.565341 python_keycloak-3.1.0/src/keycloak/authorization/__init__.py
+-rw-r--r--   0        0        0     4421 2023-06-23 05:23:09.565341 python_keycloak-3.1.0/src/keycloak/authorization/permission.py
+-rw-r--r--   0        0        0     5252 2023-06-23 05:23:09.565341 python_keycloak-3.1.0/src/keycloak/authorization/policy.py
+-rw-r--r--   0        0        0     2306 2023-06-23 05:23:09.565341 python_keycloak-3.1.0/src/keycloak/authorization/role.py
+-rw-r--r--   0        0        0     8909 2023-06-23 05:23:09.565341 python_keycloak-3.1.0/src/keycloak/connection.py
+-rw-r--r--   0        0        0     5464 2023-06-23 05:23:09.565341 python_keycloak-3.1.0/src/keycloak/exceptions.py
+-rw-r--r--   0        0        0   161673 2023-06-23 05:23:09.565341 python_keycloak-3.1.0/src/keycloak/keycloak_admin.py
+-rw-r--r--   0        0        0    25390 2023-06-23 05:23:09.565341 python_keycloak-3.1.0/src/keycloak/keycloak_openid.py
+-rw-r--r--   0        0        0    15376 2023-06-23 05:23:09.565341 python_keycloak-3.1.0/src/keycloak/keycloak_uma.py
+-rw-r--r--   0        0        0    11781 2023-06-23 05:23:09.565341 python_keycloak-3.1.0/src/keycloak/openid_connection.py
+-rw-r--r--   0        0        0     8767 2023-06-23 05:23:09.565341 python_keycloak-3.1.0/src/keycloak/uma_permissions.py
+-rw-r--r--   0        0        0    11800 2023-06-23 05:23:09.565341 python_keycloak-3.1.0/src/keycloak/urls_patterns.py
+-rw-r--r--   0        0        0    16384 1970-01-01 00:00:00.000000 python_keycloak-3.1.0/PKG-INFO
```

### Comparing `python_keycloak-3.0.0/CHANGELOG.md` & `python_keycloak-3.1.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+## v3.0.0 (2023-05-28)
+
+### BREAKING CHANGE
+
+- Changes the exchange token API
+
+### Refactor
+
+- Exchange token method
+
 ## v2.16.6 (2023-05-28)
 
 ### Fix
 
 - relax the version constraints
 
 ## v2.16.5 (2023-05-28)
```

### Comparing `python_keycloak-3.0.0/CONTRIBUTING.md` & `python_keycloak-3.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.0.0/LICENSE` & `python_keycloak-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.0.0/README.md` & `python_keycloak-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.0.0/pyproject.toml` & `python_keycloak-3.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-keycloak"
-version = "v3.0.0"
+version = "v3.1.0"
 description = "python-keycloak is a Python package providing access to the Keycloak API."
 license = "MIT"
 readme = "README.md"
 keywords = [ "keycloak", "openid", "oidc" ]
 authors = [
     "Marcos Pereira <marcospereira.mpj@gmail.com>",
     "Richard Nemeth <ryshoooo@gmail.com>"
```

### Comparing `python_keycloak-3.0.0/src/keycloak/__init__.py` & `python_keycloak-3.1.0/src/keycloak/__init__.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.0.0/src/keycloak/_version.py` & `python_keycloak-3.1.0/src/keycloak/_version.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.0.0/src/keycloak/authorization/__init__.py` & `python_keycloak-3.1.0/src/keycloak/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.0.0/src/keycloak/authorization/permission.py` & `python_keycloak-3.1.0/src/keycloak/authorization/permission.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.0.0/src/keycloak/authorization/policy.py` & `python_keycloak-3.1.0/src/keycloak/authorization/policy.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.0.0/src/keycloak/authorization/role.py` & `python_keycloak-3.1.0/src/keycloak/authorization/role.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.0.0/src/keycloak/connection.py` & `python_keycloak-3.1.0/src/keycloak/connection.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.0.0/src/keycloak/exceptions.py` & `python_keycloak-3.1.0/src/keycloak/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.0.0/src/keycloak/keycloak_admin.py` & `python_keycloak-3.1.0/src/keycloak/keycloak_admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -863,32 +863,42 @@
         :type user_id: str
         :return: UserRepresentation
         """
         params_path = {"realm-name": self.connection.realm_name, "id": user_id}
         data_raw = self.connection.raw_get(urls_patterns.URL_ADMIN_USER.format(**params_path))
         return raise_error_from_response(data_raw, KeycloakGetError)
 
-    def get_user_groups(self, user_id, brief_representation=True):
+    def get_user_groups(self, user_id, query=None, brief_representation=True):
         """Get user groups.
 
         Returns a list of groups of which the user is a member
 
         :param user_id: User id
         :type user_id: str
+        :param query: Additional query options
+        :type query: dict
         :param brief_representation: whether to omit attributes in the response
         :type brief_representation: bool
         :return: user groups list
         :rtype: list
         """
+        query = query or {}
+
         params = {"briefRepresentation": brief_representation}
+
+        query.update(params)
+
         params_path = {"realm-name": self.connection.realm_name, "id": user_id}
-        data_raw = self.connection.raw_get(
-            urls_patterns.URL_ADMIN_USER_GROUPS.format(**params_path), **params
-        )
-        return raise_error_from_response(data_raw, KeycloakGetError)
+
+        url = urls_patterns.URL_ADMIN_USER_GROUPS.format(**params_path)
+
+        if "first" in query or "max" in query:
+            return self.__fetch_paginated(url, query)
+
+        return self.__fetch_all(url, query)
 
     def update_user(self, user_id, payload):
         """Update the user.
 
         :param user_id: User id
         :type user_id: str
         :param payload: UserRepresentation
```

### Comparing `python_keycloak-3.0.0/src/keycloak/keycloak_openid.py` & `python_keycloak-3.1.0/src/keycloak/keycloak_openid.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.0.0/src/keycloak/keycloak_uma.py` & `python_keycloak-3.1.0/src/keycloak/keycloak_uma.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.0.0/src/keycloak/openid_connection.py` & `python_keycloak-3.1.0/src/keycloak/openid_connection.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.0.0/src/keycloak/uma_permissions.py` & `python_keycloak-3.1.0/src/keycloak/uma_permissions.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.0.0/src/keycloak/urls_patterns.py` & `python_keycloak-3.1.0/src/keycloak/urls_patterns.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.0.0/PKG-INFO` & `python_keycloak-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-keycloak
-Version: 3.0.0
+Version: 3.1.0
 Summary: python-keycloak is a Python package providing access to the Keycloak API.
 License: MIT
 Keywords: keycloak,openid,oidc
 Author: Marcos Pereira
 Author-email: marcospereira.mpj@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
```


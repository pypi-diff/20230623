# Comparing `tmp/python_keycloak-3.1.1.tar.gz` & `tmp/python_keycloak-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_keycloak-3.1.1.tar", max compression
+gzip compressed data, was "python_keycloak-3.2.0.tar", max compression
```

## Comparing `python_keycloak-3.1.1.tar` & `python_keycloak-3.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     6561 2023-06-23 05:55:12.239542 python_keycloak-3.1.1/CHANGELOG.md
--rw-r--r--   0        0        0     3192 2023-06-23 05:55:12.239542 python_keycloak-3.1.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1111 2023-06-23 05:55:12.239542 python_keycloak-3.1.1/LICENSE
--rw-r--r--   0        0        0    14613 2023-06-23 05:55:12.239542 python_keycloak-3.1.1/README.md
--rw-r--r--   0        0        0     2342 2023-06-23 05:55:32.940044 python_keycloak-3.1.1/pyproject.toml
--rw-r--r--   0        0        0     2375 2023-06-23 05:55:12.243542 python_keycloak-3.1.1/src/keycloak/__init__.py
--rw-r--r--   0        0        0     1268 2023-06-23 05:55:12.243542 python_keycloak-3.1.1/src/keycloak/_version.py
--rw-r--r--   0        0        0     3823 2023-06-23 05:55:12.243542 python_keycloak-3.1.1/src/keycloak/authorization/__init__.py
--rw-r--r--   0        0        0     4421 2023-06-23 05:55:12.243542 python_keycloak-3.1.1/src/keycloak/authorization/permission.py
--rw-r--r--   0        0        0     5252 2023-06-23 05:55:12.243542 python_keycloak-3.1.1/src/keycloak/authorization/policy.py
--rw-r--r--   0        0        0     2306 2023-06-23 05:55:12.243542 python_keycloak-3.1.1/src/keycloak/authorization/role.py
--rw-r--r--   0        0        0     8909 2023-06-23 05:55:12.243542 python_keycloak-3.1.1/src/keycloak/connection.py
--rw-r--r--   0        0        0     5464 2023-06-23 05:55:12.243542 python_keycloak-3.1.1/src/keycloak/exceptions.py
--rw-r--r--   0        0        0   161673 2023-06-23 05:55:12.243542 python_keycloak-3.1.1/src/keycloak/keycloak_admin.py
--rw-r--r--   0        0        0    25390 2023-06-23 05:55:12.243542 python_keycloak-3.1.1/src/keycloak/keycloak_openid.py
--rw-r--r--   0        0        0    15376 2023-06-23 05:55:12.243542 python_keycloak-3.1.1/src/keycloak/keycloak_uma.py
--rw-r--r--   0        0        0    11781 2023-06-23 05:55:12.243542 python_keycloak-3.1.1/src/keycloak/openid_connection.py
--rw-r--r--   0        0        0     8767 2023-06-23 05:55:12.243542 python_keycloak-3.1.1/src/keycloak/uma_permissions.py
--rw-r--r--   0        0        0    11799 2023-06-23 05:55:12.243542 python_keycloak-3.1.1/src/keycloak/urls_patterns.py
--rw-r--r--   0        0        0    16384 1970-01-01 00:00:00.000000 python_keycloak-3.1.1/PKG-INFO
+-rw-r--r--   0        0        0     6644 2023-06-23 21:41:28.262439 python_keycloak-3.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     3192 2023-06-23 21:41:28.262439 python_keycloak-3.2.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1111 2023-06-23 21:41:28.262439 python_keycloak-3.2.0/LICENSE
+-rw-r--r--   0        0        0    14613 2023-06-23 21:41:28.262439 python_keycloak-3.2.0/README.md
+-rw-r--r--   0        0        0     2342 2023-06-23 21:41:48.862524 python_keycloak-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2375 2023-06-23 21:41:28.262439 python_keycloak-3.2.0/src/keycloak/__init__.py
+-rw-r--r--   0        0        0     1268 2023-06-23 21:41:28.262439 python_keycloak-3.2.0/src/keycloak/_version.py
+-rw-r--r--   0        0        0     3823 2023-06-23 21:41:28.262439 python_keycloak-3.2.0/src/keycloak/authorization/__init__.py
+-rw-r--r--   0        0        0     4421 2023-06-23 21:41:28.262439 python_keycloak-3.2.0/src/keycloak/authorization/permission.py
+-rw-r--r--   0        0        0     5252 2023-06-23 21:41:28.262439 python_keycloak-3.2.0/src/keycloak/authorization/policy.py
+-rw-r--r--   0        0        0     2306 2023-06-23 21:41:28.262439 python_keycloak-3.2.0/src/keycloak/authorization/role.py
+-rw-r--r--   0        0        0     8909 2023-06-23 21:41:28.262439 python_keycloak-3.2.0/src/keycloak/connection.py
+-rw-r--r--   0        0        0     5464 2023-06-23 21:41:28.262439 python_keycloak-3.2.0/src/keycloak/exceptions.py
+-rw-r--r--   0        0        0   164471 2023-06-23 21:41:28.266439 python_keycloak-3.2.0/src/keycloak/keycloak_admin.py
+-rw-r--r--   0        0        0    25390 2023-06-23 21:41:28.266439 python_keycloak-3.2.0/src/keycloak/keycloak_openid.py
+-rw-r--r--   0        0        0    15376 2023-06-23 21:41:28.266439 python_keycloak-3.2.0/src/keycloak/keycloak_uma.py
+-rw-r--r--   0        0        0    11781 2023-06-23 21:41:28.266439 python_keycloak-3.2.0/src/keycloak/openid_connection.py
+-rw-r--r--   0        0        0     8767 2023-06-23 21:41:28.266439 python_keycloak-3.2.0/src/keycloak/uma_permissions.py
+-rw-r--r--   0        0        0    11898 2023-06-23 21:41:28.266439 python_keycloak-3.2.0/src/keycloak/urls_patterns.py
+-rw-r--r--   0        0        0    16384 1970-01-01 00:00:00.000000 python_keycloak-3.2.0/PKG-INFO
```

### Comparing `python_keycloak-3.1.1/CHANGELOG.md` & `python_keycloak-3.2.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## v3.1.1 (2023-06-23)
+
+### Fix
+
+- remove duplicate slash in URL_ADMIN_IDP (#459)
+
 ## v3.1.0 (2023-06-23)
 
 ### Feat
 
 - Add query to get users group method and permit pagination (#444)
 
 ## v3.0.0 (2023-05-28)
```

### Comparing `python_keycloak-3.1.1/CONTRIBUTING.md` & `python_keycloak-3.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.1.1/LICENSE` & `python_keycloak-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.1.1/README.md` & `python_keycloak-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.1.1/pyproject.toml` & `python_keycloak-3.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-keycloak"
-version = "v3.1.1"
+version = "v3.2.0"
 description = "python-keycloak is a Python package providing access to the Keycloak API."
 license = "MIT"
 readme = "README.md"
 keywords = [ "keycloak", "openid", "oidc" ]
 authors = [
     "Marcos Pereira <marcospereira.mpj@gmail.com>",
     "Richard Nemeth <ryshoooo@gmail.com>"
```

### Comparing `python_keycloak-3.1.1/src/keycloak/__init__.py` & `python_keycloak-3.2.0/src/keycloak/__init__.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.1.1/src/keycloak/_version.py` & `python_keycloak-3.2.0/src/keycloak/_version.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.1.1/src/keycloak/authorization/__init__.py` & `python_keycloak-3.2.0/src/keycloak/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.1.1/src/keycloak/authorization/permission.py` & `python_keycloak-3.2.0/src/keycloak/authorization/permission.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.1.1/src/keycloak/authorization/policy.py` & `python_keycloak-3.2.0/src/keycloak/authorization/policy.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.1.1/src/keycloak/authorization/role.py` & `python_keycloak-3.2.0/src/keycloak/authorization/role.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.1.1/src/keycloak/connection.py` & `python_keycloak-3.2.0/src/keycloak/connection.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.1.1/src/keycloak/exceptions.py` & `python_keycloak-3.2.0/src/keycloak/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.1.1/src/keycloak/keycloak_admin.py` & `python_keycloak-3.2.0/src/keycloak/keycloak_admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1628,14 +1628,51 @@
             urls_patterns.URL_ADMIN_CLIENT_AUTHZ_ROLE_BASED_POLICY.format(**params_path),
             data=json.dumps(payload),
         )
         return raise_error_from_response(
             data_raw, KeycloakPostError, expected_codes=[201], skip_exists=skip_exists
         )
 
+    def create_client_authz_policy(self, client_id, payload, skip_exists=False):
+        """Create an authz policy of client.
+
+        Payload example::
+
+            payload={
+                "name": "Policy-time-based",
+                "type": "time",
+                "logic": "POSITIVE",
+                "decisionStrategy": "UNANIMOUS",
+                "config": {
+                    "hourEnd": "18",
+                    "hour": "9"
+                }
+            }
+
+        :param client_id: id in ClientRepresentation
+            https://www.keycloak.org/docs-api/18.0/rest-api/index.html#_clientrepresentation
+        :type client_id: str
+        :param payload: No Document
+        :type payload: dict
+        :param skip_exists: Skip creation in case the object exists
+        :type skip_exists: bool
+        :return: Keycloak server response
+        :rtype: bytes
+
+        """
+        params_path = {"realm-name": self.connection.realm_name, "id": client_id}
+
+        data_raw = self.connection.raw_post(
+            urls_patterns.URL_ADMIN_CLIENT_AUTHZ_POLICIES.format(**params_path),
+            data=json.dumps(payload),
+        )
+        return raise_error_from_response(
+            data_raw, KeycloakPostError, expected_codes=[201], skip_exists=skip_exists
+        )
+
     def create_client_authz_resource_based_permission(self, client_id, payload, skip_exists=False):
         """Create resource-based permission of client.
 
         Payload example::
 
             payload={
                 "type": "resource",
@@ -1667,14 +1704,56 @@
             urls_patterns.URL_ADMIN_CLIENT_AUTHZ_RESOURCE_BASED_PERMISSION.format(**params_path),
             data=json.dumps(payload),
         )
         return raise_error_from_response(
             data_raw, KeycloakPostError, expected_codes=[201], skip_exists=skip_exists
         )
 
+    def create_client_authz_scope_based_permission(self, client_id, payload, skip_exists=False):
+        """Create scope-based permission of client.
+
+        Payload example::
+
+            payload={
+                "type": "resource",
+                "logic": "POSITIVE",
+                "decisionStrategy": "UNANIMOUS",
+                "name": "Permission-Name",
+                "resources": [
+                    resource_id
+                ],
+                "policies": [
+                    policy_id
+                ],
+                "scopes": [
+                    scope_id
+                ]
+
+        :param client_id: id in ClientRepresentation
+            https://www.keycloak.org/docs-api/18.0/rest-api/index.html#_clientrepresentation
+        :type client_id: str
+        :param payload: PolicyRepresentation
+            https://www.keycloak.org/docs-api/18.0/rest-api/index.html#_policyrepresentation
+        :type payload: dict
+        :param skip_exists: Skip creation in case the object already exists
+        :type skip_exists: bool
+        :return: Keycloak server response
+        :rtype: bytes
+
+        """
+        params_path = {"realm-name": self.realm_name, "id": client_id}
+
+        data_raw = self.raw_post(
+            urls_patterns.URL_ADMIN_CLIENT_AUTHZ_SCOPE_BASED_PERMISSION.format(**params_path),
+            data=json.dumps(payload),
+        )
+        return raise_error_from_response(
+            data_raw, KeycloakPostError, expected_codes=[201], skip_exists=skip_exists
+        )
+
     def get_client_authz_scopes(self, client_id):
         """Get scopes from client.
 
         :param client_id: id in ClientRepresentation
             https://www.keycloak.org/docs-api/18.0/rest-api/index.html#_clientrepresentation
         :type client_id: str
         :return: Keycloak server response
```

### Comparing `python_keycloak-3.1.1/src/keycloak/keycloak_openid.py` & `python_keycloak-3.2.0/src/keycloak/keycloak_openid.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.1.1/src/keycloak/keycloak_uma.py` & `python_keycloak-3.2.0/src/keycloak/keycloak_uma.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.1.1/src/keycloak/openid_connection.py` & `python_keycloak-3.2.0/src/keycloak/openid_connection.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.1.1/src/keycloak/uma_permissions.py` & `python_keycloak-3.2.0/src/keycloak/uma_permissions.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.1.1/src/keycloak/urls_patterns.py` & `python_keycloak-3.2.0/src/keycloak/urls_patterns.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,14 +117,15 @@
 URL_ADMIN_CLIENT_AUTHZ_SCOPES = URL_ADMIN_CLIENT_AUTHZ + "/scope?max=-1"
 URL_ADMIN_CLIENT_AUTHZ_PERMISSIONS = URL_ADMIN_CLIENT_AUTHZ + "/permission?max=-1"
 URL_ADMIN_CLIENT_AUTHZ_POLICIES = URL_ADMIN_CLIENT_AUTHZ + "/policy?max=-1&permission=false"
 URL_ADMIN_CLIENT_AUTHZ_ROLE_BASED_POLICY = URL_ADMIN_CLIENT_AUTHZ + "/policy/role?max=-1"
 URL_ADMIN_CLIENT_AUTHZ_RESOURCE_BASED_PERMISSION = (
     URL_ADMIN_CLIENT_AUTHZ + "/permission/resource?max=-1"
 )
+URL_ADMIN_CLIENT_AUTHZ_SCOPE_BASED_PERMISSION = URL_ADMIN_CLIENT_AUTHZ + "/permission/scope?max=-1"
 URL_ADMIN_CLIENT_AUTHZ_POLICY = URL_ADMIN_CLIENT_AUTHZ + "/policy/{policy-id}"
 URL_ADMIN_CLIENT_AUTHZ_POLICY_SCOPES = URL_ADMIN_CLIENT_AUTHZ_POLICY + "/scopes"
 URL_ADMIN_CLIENT_AUTHZ_POLICY_RESOURCES = URL_ADMIN_CLIENT_AUTHZ_POLICY + "/resources"
 URL_ADMIN_CLIENT_AUTHZ_SCOPE_PERMISSION = URL_ADMIN_CLIENT_AUTHZ + "/permission/scope/{scope-id}"
 URL_ADMIN_CLIENT_AUTHZ_CLIENT_POLICY = URL_ADMIN_CLIENT_AUTHZ + "/policy/client"
 
 URL_ADMIN_CLIENT_SERVICE_ACCOUNT_USER = URL_ADMIN_CLIENT + "/service-account-user"
@@ -208,10 +209,9 @@
     "admin/realms/{realm-name}/attack-detection/brute-force/users/{id}"
 )
 
 URL_ADMIN_CLEAR_KEYS_CACHE = URL_ADMIN_REALM + "/clear-keys-cache"
 URL_ADMIN_CLEAR_REALM_CACHE = URL_ADMIN_REALM + "/clear-realm-cache"
 URL_ADMIN_CLEAR_USER_CACHE = URL_ADMIN_REALM + "/clear-user-cache"
 
-
 # UMA URLS
 URL_UMA_WELL_KNOWN = URL_WELL_KNOWN_BASE + "/uma2-configuration"
```

### Comparing `python_keycloak-3.1.1/PKG-INFO` & `python_keycloak-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-keycloak
-Version: 3.1.1
+Version: 3.2.0
 Summary: python-keycloak is a Python package providing access to the Keycloak API.
 License: MIT
 Keywords: keycloak,openid,oidc
 Author: Marcos Pereira
 Author-email: marcospereira.mpj@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
```


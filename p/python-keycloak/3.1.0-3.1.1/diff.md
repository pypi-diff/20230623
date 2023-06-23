# Comparing `tmp/python_keycloak-3.1.0.tar.gz` & `tmp/python_keycloak-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_keycloak-3.1.0.tar", max compression
+gzip compressed data, was "python_keycloak-3.1.1.tar", max compression
```

## Comparing `python_keycloak-3.1.0.tar` & `python_keycloak-3.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     6459 2023-06-23 05:23:09.561340 python_keycloak-3.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     3192 2023-06-23 05:23:09.561340 python_keycloak-3.1.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1111 2023-06-23 05:23:09.561340 python_keycloak-3.1.0/LICENSE
--rw-r--r--   0        0        0    14613 2023-06-23 05:23:09.561340 python_keycloak-3.1.0/README.md
--rw-r--r--   0        0        0     2342 2023-06-23 05:23:28.349686 python_keycloak-3.1.0/pyproject.toml
--rw-r--r--   0        0        0     2375 2023-06-23 05:23:09.565341 python_keycloak-3.1.0/src/keycloak/__init__.py
--rw-r--r--   0        0        0     1268 2023-06-23 05:23:09.565341 python_keycloak-3.1.0/src/keycloak/_version.py
--rw-r--r--   0        0        0     3823 2023-06-23 05:23:09.565341 python_keycloak-3.1.0/src/keycloak/authorization/__init__.py
--rw-r--r--   0        0        0     4421 2023-06-23 05:23:09.565341 python_keycloak-3.1.0/src/keycloak/authorization/permission.py
--rw-r--r--   0        0        0     5252 2023-06-23 05:23:09.565341 python_keycloak-3.1.0/src/keycloak/authorization/policy.py
--rw-r--r--   0        0        0     2306 2023-06-23 05:23:09.565341 python_keycloak-3.1.0/src/keycloak/authorization/role.py
--rw-r--r--   0        0        0     8909 2023-06-23 05:23:09.565341 python_keycloak-3.1.0/src/keycloak/connection.py
--rw-r--r--   0        0        0     5464 2023-06-23 05:23:09.565341 python_keycloak-3.1.0/src/keycloak/exceptions.py
--rw-r--r--   0        0        0   161673 2023-06-23 05:23:09.565341 python_keycloak-3.1.0/src/keycloak/keycloak_admin.py
--rw-r--r--   0        0        0    25390 2023-06-23 05:23:09.565341 python_keycloak-3.1.0/src/keycloak/keycloak_openid.py
--rw-r--r--   0        0        0    15376 2023-06-23 05:23:09.565341 python_keycloak-3.1.0/src/keycloak/keycloak_uma.py
--rw-r--r--   0        0        0    11781 2023-06-23 05:23:09.565341 python_keycloak-3.1.0/src/keycloak/openid_connection.py
--rw-r--r--   0        0        0     8767 2023-06-23 05:23:09.565341 python_keycloak-3.1.0/src/keycloak/uma_permissions.py
--rw-r--r--   0        0        0    11800 2023-06-23 05:23:09.565341 python_keycloak-3.1.0/src/keycloak/urls_patterns.py
--rw-r--r--   0        0        0    16384 1970-01-01 00:00:00.000000 python_keycloak-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     6561 2023-06-23 05:55:12.239542 python_keycloak-3.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     3192 2023-06-23 05:55:12.239542 python_keycloak-3.1.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1111 2023-06-23 05:55:12.239542 python_keycloak-3.1.1/LICENSE
+-rw-r--r--   0        0        0    14613 2023-06-23 05:55:12.239542 python_keycloak-3.1.1/README.md
+-rw-r--r--   0        0        0     2342 2023-06-23 05:55:32.940044 python_keycloak-3.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2375 2023-06-23 05:55:12.243542 python_keycloak-3.1.1/src/keycloak/__init__.py
+-rw-r--r--   0        0        0     1268 2023-06-23 05:55:12.243542 python_keycloak-3.1.1/src/keycloak/_version.py
+-rw-r--r--   0        0        0     3823 2023-06-23 05:55:12.243542 python_keycloak-3.1.1/src/keycloak/authorization/__init__.py
+-rw-r--r--   0        0        0     4421 2023-06-23 05:55:12.243542 python_keycloak-3.1.1/src/keycloak/authorization/permission.py
+-rw-r--r--   0        0        0     5252 2023-06-23 05:55:12.243542 python_keycloak-3.1.1/src/keycloak/authorization/policy.py
+-rw-r--r--   0        0        0     2306 2023-06-23 05:55:12.243542 python_keycloak-3.1.1/src/keycloak/authorization/role.py
+-rw-r--r--   0        0        0     8909 2023-06-23 05:55:12.243542 python_keycloak-3.1.1/src/keycloak/connection.py
+-rw-r--r--   0        0        0     5464 2023-06-23 05:55:12.243542 python_keycloak-3.1.1/src/keycloak/exceptions.py
+-rw-r--r--   0        0        0   161673 2023-06-23 05:55:12.243542 python_keycloak-3.1.1/src/keycloak/keycloak_admin.py
+-rw-r--r--   0        0        0    25390 2023-06-23 05:55:12.243542 python_keycloak-3.1.1/src/keycloak/keycloak_openid.py
+-rw-r--r--   0        0        0    15376 2023-06-23 05:55:12.243542 python_keycloak-3.1.1/src/keycloak/keycloak_uma.py
+-rw-r--r--   0        0        0    11781 2023-06-23 05:55:12.243542 python_keycloak-3.1.1/src/keycloak/openid_connection.py
+-rw-r--r--   0        0        0     8767 2023-06-23 05:55:12.243542 python_keycloak-3.1.1/src/keycloak/uma_permissions.py
+-rw-r--r--   0        0        0    11799 2023-06-23 05:55:12.243542 python_keycloak-3.1.1/src/keycloak/urls_patterns.py
+-rw-r--r--   0        0        0    16384 1970-01-01 00:00:00.000000 python_keycloak-3.1.1/PKG-INFO
```

### Comparing `python_keycloak-3.1.0/CHANGELOG.md` & `python_keycloak-3.1.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## v3.1.0 (2023-06-23)
+
+### Feat
+
+- Add query to get users group method and permit pagination (#444)
+
 ## v3.0.0 (2023-05-28)
 
 ### BREAKING CHANGE
 
 - Changes the exchange token API
 
 ### Refactor
```

### Comparing `python_keycloak-3.1.0/CONTRIBUTING.md` & `python_keycloak-3.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.1.0/LICENSE` & `python_keycloak-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.1.0/README.md` & `python_keycloak-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.1.0/pyproject.toml` & `python_keycloak-3.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-keycloak"
-version = "v3.1.0"
+version = "v3.1.1"
 description = "python-keycloak is a Python package providing access to the Keycloak API."
 license = "MIT"
 readme = "README.md"
 keywords = [ "keycloak", "openid", "oidc" ]
 authors = [
     "Marcos Pereira <marcospereira.mpj@gmail.com>",
     "Richard Nemeth <ryshoooo@gmail.com>"
```

### Comparing `python_keycloak-3.1.0/src/keycloak/__init__.py` & `python_keycloak-3.1.1/src/keycloak/__init__.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.1.0/src/keycloak/_version.py` & `python_keycloak-3.1.1/src/keycloak/_version.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.1.0/src/keycloak/authorization/__init__.py` & `python_keycloak-3.1.1/src/keycloak/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.1.0/src/keycloak/authorization/permission.py` & `python_keycloak-3.1.1/src/keycloak/authorization/permission.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.1.0/src/keycloak/authorization/policy.py` & `python_keycloak-3.1.1/src/keycloak/authorization/policy.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.1.0/src/keycloak/authorization/role.py` & `python_keycloak-3.1.1/src/keycloak/authorization/role.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.1.0/src/keycloak/connection.py` & `python_keycloak-3.1.1/src/keycloak/connection.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.1.0/src/keycloak/exceptions.py` & `python_keycloak-3.1.1/src/keycloak/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.1.0/src/keycloak/keycloak_admin.py` & `python_keycloak-3.1.1/src/keycloak/keycloak_admin.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.1.0/src/keycloak/keycloak_openid.py` & `python_keycloak-3.1.1/src/keycloak/keycloak_openid.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.1.0/src/keycloak/keycloak_uma.py` & `python_keycloak-3.1.1/src/keycloak/keycloak_uma.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.1.0/src/keycloak/openid_connection.py` & `python_keycloak-3.1.1/src/keycloak/openid_connection.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.1.0/src/keycloak/uma_permissions.py` & `python_keycloak-3.1.1/src/keycloak/uma_permissions.py`

 * *Files identical despite different names*

### Comparing `python_keycloak-3.1.0/src/keycloak/urls_patterns.py` & `python_keycloak-3.1.1/src/keycloak/urls_patterns.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
 URL_ADMIN_REALM_ROLES = "admin/realms/{realm-name}/roles"
 URL_ADMIN_REALM_ROLES_MEMBERS = URL_ADMIN_REALM_ROLES + "/{role-name}/users"
 URL_ADMIN_REALMS = "admin/realms"
 URL_ADMIN_REALM = "admin/realms/{realm-name}"
 URL_ADMIN_IDPS = "admin/realms/{realm-name}/identity-provider/instances"
 URL_ADMIN_IDP_MAPPERS = "admin/realms/{realm-name}/identity-provider/instances/{idp-alias}/mappers"
 URL_ADMIN_IDP_MAPPER_UPDATE = URL_ADMIN_IDP_MAPPERS + "/{mapper-id}"
-URL_ADMIN_IDP = "admin/realms//{realm-name}/identity-provider/instances/{alias}"
+URL_ADMIN_IDP = "admin/realms/{realm-name}/identity-provider/instances/{alias}"
 URL_ADMIN_REALM_ROLES_ROLE_BY_NAME = "admin/realms/{realm-name}/roles/{role-name}"
 URL_ADMIN_REALM_ROLES_COMPOSITE_REALM_ROLE = (
     "admin/realms/{realm-name}/roles/{role-name}/composites"
 )
 URL_ADMIN_REALM_EXPORT = (
     "admin/realms/{realm-name}/partial-export?exportClients={export-clients}&"
     + "exportGroupsAndRoles={export-groups-and-roles}"
```

### Comparing `python_keycloak-3.1.0/PKG-INFO` & `python_keycloak-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-keycloak
-Version: 3.1.0
+Version: 3.1.1
 Summary: python-keycloak is a Python package providing access to the Keycloak API.
 License: MIT
 Keywords: keycloak,openid,oidc
 Author: Marcos Pereira
 Author-email: marcospereira.mpj@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
```


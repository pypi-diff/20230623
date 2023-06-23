# Comparing `tmp/qotto_auth_client-2.2.1.tar.gz` & `tmp/qotto_auth_client-2.2.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qotto_auth_client-2.2.1.tar", max compression
+gzip compressed data, was "qotto_auth_client-2.2.2a0.tar", max compression
```

## Comparing `qotto_auth_client-2.2.1.tar` & `qotto_auth_client-2.2.2a0.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     1062 2022-08-03 08:46:30.145586 qotto_auth_client-2.2.1/LICENSE
--rw-r--r--   0        0        0     1364 2022-11-22 08:13:56.153627 qotto_auth_client-2.2.1/README.md
--rw-r--r--   0        0        0     1164 2023-03-28 10:47:23.435810 qotto_auth_client-2.2.1/pyproject.toml
--rw-r--r--   0        0        0      782 2023-01-20 08:10:36.504176 qotto_auth_client-2.2.1/qottoauth/__init__.py
--rw-r--r--   0        0        0      342 2022-11-23 14:46:03.536748 qotto_auth_client-2.2.1/qottoauth/api/__init__.py
--rw-r--r--   0        0        0     1516 2023-01-20 08:10:36.504176 qotto_auth_client-2.2.1/qottoauth/api/base.py
--rw-r--r--   0        0        0     4088 2023-01-20 08:10:36.504176 qotto_auth_client-2.2.1/qottoauth/api/cached.py
--rw-r--r--   0        0        0     5211 2023-02-22 20:08:40.637617 qotto_auth_client-2.2.1/qottoauth/api/gql.py
--rw-r--r--   0        0        0    37307 2023-03-28 10:47:11.239832 qotto_auth_client-2.2.1/qottoauth/api/test.py
--rw-r--r--   0        0        0     9525 2023-03-28 10:47:11.239832 qotto_auth_client-2.2.1/qottoauth/models.py
--rw-r--r--   0        0        0       27 2022-01-10 15:06:15.651000 qotto_auth_client-2.2.1/qottoauth/py.typed
--rw-r--r--   0        0        0    35838 2023-03-28 10:47:11.239832 qotto_auth_client-2.2.1/qottoauth/service.py
--rw-r--r--   0        0        0     2124 1970-01-01 00:00:00.000000 qotto_auth_client-2.2.1/setup.py
--rw-r--r--   0        0        0     2052 1970-01-01 00:00:00.000000 qotto_auth_client-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2022-08-03 08:46:30.145586 qotto_auth_client-2.2.2a0/LICENSE
+-rw-r--r--   0        0        0     1364 2022-11-22 08:13:56.153627 qotto_auth_client-2.2.2a0/README.md
+-rw-r--r--   0        0        0     1166 2023-06-23 07:52:14.585403 qotto_auth_client-2.2.2a0/pyproject.toml
+-rw-r--r--   0        0        0      782 2023-01-20 08:10:36.504176 qotto_auth_client-2.2.2a0/qottoauth/__init__.py
+-rw-r--r--   0        0        0      342 2022-11-23 14:46:03.536748 qotto_auth_client-2.2.2a0/qottoauth/api/__init__.py
+-rw-r--r--   0        0        0     1516 2023-01-20 08:10:36.504176 qotto_auth_client-2.2.2a0/qottoauth/api/base.py
+-rw-r--r--   0        0        0     4088 2023-01-20 08:10:36.504176 qotto_auth_client-2.2.2a0/qottoauth/api/cached.py
+-rw-r--r--   0        0        0     5211 2023-02-22 20:08:40.637617 qotto_auth_client-2.2.2a0/qottoauth/api/gql.py
+-rw-r--r--   0        0        0    37650 2023-06-23 07:50:30.514172 qotto_auth_client-2.2.2a0/qottoauth/api/test.py
+-rw-r--r--   0        0        0     9525 2023-03-28 10:47:11.239832 qotto_auth_client-2.2.2a0/qottoauth/models.py
+-rw-r--r--   0        0        0       27 2022-01-10 15:06:15.651000 qotto_auth_client-2.2.2a0/qottoauth/py.typed
+-rw-r--r--   0        0        0    36482 2023-06-22 21:06:47.346705 qotto_auth_client-2.2.2a0/qottoauth/service.py
+-rw-r--r--   0        0        0     2054 1970-01-01 00:00:00.000000 qotto_auth_client-2.2.2a0/PKG-INFO
```

### Comparing `qotto_auth_client-2.2.1/LICENSE` & `qotto_auth_client-2.2.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `qotto_auth_client-2.2.1/README.md` & `qotto_auth_client-2.2.2a0/README.md`

 * *Files identical despite different names*

### Comparing `qotto_auth_client-2.2.1/pyproject.toml` & `qotto_auth_client-2.2.2a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qotto-auth-client"
-version = "2.2.1"
+version = "2.2.2a0"
 description = "Qotto/QottoAuthClient"
 authors = ["Qotto Dev Team <dev@qotto.net>"]
 readme = "README.md"
 #homepage
 #repository = "https://gitlab.com/qotto/oss/eventy"
 #documentation = "https://qotto.gitlab.io/oss/eventy"
 #keywords
```

### Comparing `qotto_auth_client-2.2.1/qottoauth/__init__.py` & `qotto_auth_client-2.2.2a0/qottoauth/__init__.py`

 * *Files identical despite different names*

### Comparing `qotto_auth_client-2.2.1/qottoauth/api/base.py` & `qotto_auth_client-2.2.2a0/qottoauth/api/base.py`

 * *Files identical despite different names*

### Comparing `qotto_auth_client-2.2.1/qottoauth/api/cached.py` & `qotto_auth_client-2.2.2a0/qottoauth/api/cached.py`

 * *Files identical despite different names*

### Comparing `qotto_auth_client-2.2.1/qottoauth/api/gql.py` & `qotto_auth_client-2.2.2a0/qottoauth/api/gql.py`

 * *Files identical despite different names*

### Comparing `qotto_auth_client-2.2.1/qottoauth/api/test.py` & `qotto_auth_client-2.2.2a0/qottoauth/api/test.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,14 +236,23 @@
                 updated_permission: Permission = permission.update(name=name, description=description)
                 self._permissions[permission.id] = updated_permission
                 return dict(permission=updated_permission.to_dict())
         new_permission = Permission(uuid, application, code, name, description)
         self._permissions[new_permission.id] = new_permission
         return dict(permission=new_permission.to_dict())
 
+    def registerPermissions(
+            self,
+            applicationId: str, permissions: list[dict[str, Any]], **kwargs,
+    ) -> dict:
+        result = []
+        for permission_info in permissions:
+            result.append(self.registerPermission(applicationId, **permission_info)['permission'])
+        return dict(permissions=result)
+
     def deletePermission(self, permissionId: str) -> dict:
         if permissionId in self._permissions:
             del self._permissions[permissionId]
             for authorization_id, permission_id_set in self._authorization_permissions.items():
                 permission_id_set.discard(permissionId)
             return dict(deleted=True)
         return dict(deleted=False)
```

### Comparing `qotto_auth_client-2.2.1/qottoauth/models.py` & `qotto_auth_client-2.2.2a0/qottoauth/models.py`

 * *Files identical despite different names*

### Comparing `qotto_auth_client-2.2.1/qottoauth/service.py` & `qotto_auth_client-2.2.2a0/qottoauth/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import logging
-from datetime import datetime, date
-from typing import Union, Any, Optional
+from datetime import date, datetime
+from typing import Any, Optional, Union
 
 import jwt
 
-from qottoauth import Namespace, Matching
+from qottoauth import Matching, Namespace
 from qottoauth.api import QottoAuthApi
-from qottoauth.models import (
-    Application, Permission, Organization, User, Identity, Authorization, Role, Actor, CookiePair, Member, Account,
-    UserRequest, TokenInfo,
-)
+from qottoauth.models import (Account, Actor, Application, Authorization,
+                              CookiePair, Identity, Member, Organization,
+                              Permission, Role, TokenInfo, User, UserRequest)
 
 __all__ = [
     'QottoAuthService',
 ]
 
 logger = logging.getLogger(__name__)
 
@@ -125,14 +124,27 @@
         payload = self.api.mutation(
             name='registerPermission',
             input_value=dict(applicationId=application_id, uuid=uuid, code=code, name=name, description=description),
             body='permission { ' + Permission.body() + ' }',
         )
         return Permission.from_dict(payload['permission'])
 
+    def register_permissions(
+            self,
+            application: Union[Application, str],
+            permissions: list[dict[str, Any]],
+    ) -> list[Permission]:
+        application_id = application.id if isinstance(application, Application) else application
+        payload = self.api.mutation(
+            name='registerPermissions',
+            input_value=dict(applicationId=application_id, permissions=permissions),
+            body='permissions { ' + Permission.body() + ' }',
+        )
+        return [Permission.from_dict(permission) for permission in payload['permissions']]
+
     def delete_permission(self, permission: Union[Permission, str]) -> bool:
         permission_id = permission.id if isinstance(permission, Permission) else permission
         payload = self.api.mutation(
             name='deletePermission',
             input_value=dict(permissionId=permission_id),
             body='deleted',
         )
```

### Comparing `qotto_auth_client-2.2.1/PKG-INFO` & `qotto_auth_client-2.2.2a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qotto-auth-client
-Version: 2.2.1
+Version: 2.2.2a0
 Summary: Qotto/QottoAuthClient
 Author: Qotto Dev Team
 Author-email: dev@qotto.net
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```


# Comparing `tmp/strawberry_azure_auth-1.3.0.tar.gz` & `tmp/strawberry_azure_auth-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strawberry_azure_auth-1.3.0.tar", max compression
+gzip compressed data, was "strawberry_azure_auth-2.0.0.tar", max compression
```

## Comparing `strawberry_azure_auth-1.3.0.tar` & `strawberry_azure_auth-2.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1065 2023-06-01 16:54:52.285143 strawberry_azure_auth-1.3.0/LICENSE
--rw-r--r--   0        0        0     3418 2023-06-01 16:54:52.285143 strawberry_azure_auth-1.3.0/README.md
--rw-r--r--   0        0        0      955 2023-06-01 16:54:52.285143 strawberry_azure_auth-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      167 2023-06-01 16:54:52.285143 strawberry_azure_auth-1.3.0/strawberry_azure_auth/__init__.py
--rw-r--r--   0        0        0      154 2023-06-01 16:54:52.285143 strawberry_azure_auth-1.3.0/strawberry_azure_auth/channels/__init__.py
--rw-r--r--   0        0        0     1318 2023-06-01 16:54:52.285143 strawberry_azure_auth-1.3.0/strawberry_azure_auth/channels/context.py
--rw-r--r--   0        0        0     3566 2023-06-01 16:54:52.285143 strawberry_azure_auth-1.3.0/strawberry_azure_auth/channels/handlers.py
--rw-r--r--   0        0        0     8597 2023-06-01 16:54:52.285143 strawberry_azure_auth-1.3.0/strawberry_azure_auth/channels/schema.py
--rw-r--r--   0        0        0        0 2023-06-01 16:54:52.285143 strawberry_azure_auth-1.3.0/strawberry_azure_auth/django/__init__.py
--rw-r--r--   0        0        0      920 2023-06-01 16:54:52.285143 strawberry_azure_auth-1.3.0/strawberry_azure_auth/django/context.py
--rw-r--r--   0        0        0    10706 2023-06-01 16:54:52.285143 strawberry_azure_auth-1.3.0/strawberry_azure_auth/extension.py
--rw-r--r--   0        0        0     5569 2023-06-01 16:54:52.285143 strawberry_azure_auth-1.3.0/strawberry_azure_auth/openid.py
--rw-r--r--   0        0        0     1164 2023-06-01 16:54:52.285143 strawberry_azure_auth-1.3.0/strawberry_azure_auth/permissions.py
--rw-r--r--   0        0        0      519 2023-06-01 16:54:52.285143 strawberry_azure_auth-1.3.0/strawberry_azure_auth/types.py
--rw-r--r--   0        0        0     1585 2023-06-01 16:54:52.285143 strawberry_azure_auth-1.3.0/strawberry_azure_auth/utils.py
--rw-r--r--   0        0        0     4174 1970-01-01 00:00:00.000000 strawberry_azure_auth-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-23 15:27:15.962402 strawberry_azure_auth-2.0.0/LICENSE
+-rw-r--r--   0        0        0     3466 2023-06-23 15:27:15.962402 strawberry_azure_auth-2.0.0/README.md
+-rw-r--r--   0        0        0      957 2023-06-23 15:27:15.962402 strawberry_azure_auth-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      167 2023-06-23 15:27:15.962402 strawberry_azure_auth-2.0.0/strawberry_azure_auth/__init__.py
+-rw-r--r--   0        0        0      154 2023-06-23 15:27:15.962402 strawberry_azure_auth-2.0.0/strawberry_azure_auth/channels/__init__.py
+-rw-r--r--   0        0        0     2020 2023-06-23 15:27:15.962402 strawberry_azure_auth-2.0.0/strawberry_azure_auth/channels/context.py
+-rw-r--r--   0        0        0     2059 2023-06-23 15:27:15.962402 strawberry_azure_auth-2.0.0/strawberry_azure_auth/channels/handlers.py
+-rw-r--r--   0        0        0     8623 2023-06-23 15:27:15.962402 strawberry_azure_auth-2.0.0/strawberry_azure_auth/channels/schema.py
+-rw-r--r--   0        0        0        0 2023-06-23 15:27:15.962402 strawberry_azure_auth-2.0.0/strawberry_azure_auth/django/__init__.py
+-rw-r--r--   0        0        0      905 2023-06-23 15:27:15.962402 strawberry_azure_auth-2.0.0/strawberry_azure_auth/django/context.py
+-rw-r--r--   0        0        0     9431 2023-06-23 15:27:15.962402 strawberry_azure_auth-2.0.0/strawberry_azure_auth/extension.py
+-rw-r--r--   0        0        0     5569 2023-06-23 15:27:15.962402 strawberry_azure_auth-2.0.0/strawberry_azure_auth/openid.py
+-rw-r--r--   0        0        0     1159 2023-06-23 15:27:15.962402 strawberry_azure_auth-2.0.0/strawberry_azure_auth/permissions.py
+-rw-r--r--   0        0        0      579 2023-06-23 15:27:15.962402 strawberry_azure_auth-2.0.0/strawberry_azure_auth/types.py
+-rw-r--r--   0        0        0     1585 2023-06-23 15:27:15.962402 strawberry_azure_auth-2.0.0/strawberry_azure_auth/utils.py
+-rw-r--r--   0        0        0     4205 1970-01-01 00:00:00.000000 strawberry_azure_auth-2.0.0/PKG-INFO
```

### Comparing `strawberry_azure_auth-1.3.0/LICENSE` & `strawberry_azure_auth-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `strawberry_azure_auth-1.3.0/README.md` & `strawberry_azure_auth-2.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -29,43 +29,43 @@
 from strawberry_azure_auth import AzureAuthExtension  # <--
 
 schema = strawberry.Schema(
     query=...,
     extensions=[
         AzureAuthExtension(  # <--
             client_id=...,
-            tenant_id=...,
-            scopes=...
+            tenant_id=...
         )
     ]
 )
 ```
 
 ### Channels
 
 Currently, strawberry schema extensions don't apply to graphql subscriptions
 (see [issue #2097](https://github.com/strawberry-graphql/strawberry/issues/2097)).
 
 To make the authentication extension work with channels,
 this package comes with custom http/ websocket "graphql consumer" classes
 and a custom `Schema` class that provides extension support for subscriptions:
 
+> :warning: The `Schema` class will be removed in the future when Strawberry adds extension support for subscriptions!
+
 ```python
 # example/schema.py
 from strawberry_azure_auth import AzureAuthExtension  # <--
 from strawberry_azure_auth.channels import Schema  # <--
 
 schema = Schema(  # <--
     query=...,
     subscription=...,
     extensions=[
         AzureAuthExtension(  # <--
             client_id=...,
-            tenant_id=...,
-            scopes=...
+            tenant_id=...
         )
     ]
 )
 ```
 
 ```python
 # example/asgi.py
@@ -125,13 +125,12 @@
 
 schema = strawberry.Schema(
     query=...,
     extensions=[
         AzureAuthExtension(
             client_id=...,
             tenant_id=...,
-            scopes=...,
             roles=["Example.Read"]  # <--
         )
     ]
 )
 ```
```

### Comparing `strawberry_azure_auth-1.3.0/pyproject.toml` & `strawberry_azure_auth-2.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "strawberry-azure-auth"
-version = "1.3.0"
+version = "2.0.0"
 description = "Azure AD authentication for Strawberry GraphQL"
 authors = ["skarre-r <skarre-r@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/skarre-r/strawberry-azure-auth"
 packages = [{include = "strawberry_azure_auth"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 httpx = "^0.24.1"
 pyjwt = { version = "^2.7.0", extras = ["crypto"] }
-strawberry-graphql = { version = "~0.179.0", extras = ["channels"] }
-strawberry-graphql-django = "^0.9.4"
+strawberry-graphql = { version = ">=0.187.4", extras = ["channels"] }
+strawberry-graphql-django = ">=0.9.5"
 
 [tool.poetry.group.dev.dependencies]
-ruff = "^0.0.270"
-mypy = "^1.3.0"
+ruff = "^0.0.275"
+mypy = "^1.4.0"
 black = "^23.3.0"
 pre-commit = "^3.3.1"
 ipython = "^8.13.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `strawberry_azure_auth-1.3.0/strawberry_azure_auth/channels/context.py` & `strawberry_azure_auth-2.0.0/strawberry_azure_auth/channels/context.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,59 @@
 from __future__ import annotations
 
-__all__ = ["ChannelsContext", "ChannelsExecutionContext"]
+__all__ = ["ChannelsWebsocketContext", "ChannelsHTTPContext", "ChannelsExecutionContext"]
 
 import dataclasses
-from strawberry.channels.context import StrawberryChannelsContext
+from typing import Any, TYPE_CHECKING
 from strawberry.types.execution import ExecutionContext
 
+if TYPE_CHECKING:
+    from strawberry.channels.handlers.base import ChannelsConsumer
+    from strawberry.channels.handlers.http_handler import ChannelsRequest
+    from strawberry.http.temporal_response import TemporalResponse
+
+
+@dataclasses.dataclass
+class ChannelsHTTPContext:
+    request: ChannelsRequest
+    response: TemporalResponse
+
+    upn: str | None = None
+    roles: list[str] = dataclasses.field(default_factory=list)
+    authorized: bool = False
+
+    @property
+    def access_token(self) -> str | None:
+        for header in ["authorization", "Authorization"]:
+            authorization_header: str | None = self.request.headers.get(header)
+            if authorization_header and authorization_header.lower().startswith("bearer "):
+                _, access_token = authorization_header.split(" ")
+                return access_token
+        return None
+
 
 @dataclasses.dataclass
-class ChannelsContext(StrawberryChannelsContext):
+class ChannelsWebsocketContext:
+    request: ChannelsConsumer
+    connection_params: dict[str, Any] | None = None
+
     upn: str | None = None
     roles: list[str] = dataclasses.field(default_factory=list)
     authorized: bool = False
 
-    _handle_authentication: bool = True
-    _handle_authorization: bool = True
+    @property
+    def ws(self) -> ChannelsConsumer:
+        return self.request
 
     @property
     def access_token(self) -> str | None:
-        # check connection params
-        authorization_param: str | None = (
-            self.connection_params.get("Authorization") if self.connection_params else None
-        )
-        if authorization_param and authorization_param.lower().startswith("bearer "):
-            _, access_token = authorization_param.split(" ")
-            return access_token
-        # check headers
-        authorization_header: str | None = self.request.headers.get("Authorization")
-        if authorization_header and authorization_header.lower().startswith("bearer "):
-            _, access_token = authorization_header.split(" ")
-            return access_token
+        if self.connection_params:
+            for param in ["authorization", "Authorization"]:
+                authorization_param: str | None = self.connection_params.get(param)
+                if authorization_param and authorization_param.lower().startswith("bearer "):
+                    _, access_token = authorization_param.split(" ")
+                    return access_token
         return None
 
 
 class ChannelsExecutionContext(ExecutionContext):
-    context: ChannelsContext
+    context: ChannelsHTTPContext | ChannelsWebsocketContext
```

### Comparing `strawberry_azure_auth-1.3.0/strawberry_azure_auth/channels/schema.py` & `strawberry_azure_auth-2.0.0/strawberry_azure_auth/channels/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
     """
 
     def __init__(
         self,
         query: type,
         mutation: type | None = None,
         subscription: type | None = None,
-        directives: Iterable[StrawberryDirective] = (),
+        directives: Iterable[StrawberryDirective] = (),  # type: ignore[type-arg]
         types: Iterable[type | StrawberryType] = (),
         extensions: Iterable[type[SchemaExtension] | SchemaExtension] = (),
         execution_context_class: type[ExecutionContext] | None = None,
         config: StrawberryConfig | None = None,
         scalar_overrides: dict[object, type | ScalarWrapper | ScalarDefinition] | None = None,
         schema_directives: Iterable[object] = (),
         debug: bool = False,
```

### Comparing `strawberry_azure_auth-1.3.0/strawberry_azure_auth/django/context.py` & `strawberry_azure_auth-2.0.0/strawberry_azure_auth/django/context.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,21 +10,19 @@
 
 @dataclasses.dataclass
 class DjangoContext(StrawberryDjangoContext):
     upn: str | None = None
     roles: list[str] = dataclasses.field(default_factory=list)
     authorized: bool = False
 
-    _handle_authentication: bool = True
-    _handle_authorization: bool = True
-
     @property
     def access_token(self) -> str | None:
-        authorization_header: str | None = self.request.headers.get("Authorization")
-        if authorization_header and authorization_header.lower().startswith("bearer "):
-            _, access_token = authorization_header.split(" ")
-            return access_token
+        for header in ["authorization", "Authorization"]:
+            authorization_header: str | None = self.request.headers.get(header)
+            if authorization_header and authorization_header.lower().startswith("bearer "):
+                _, access_token = authorization_header.split(" ")
+                return access_token
         return None
 
 
 class DjangoExecutionContext(ExecutionContext):
     context: DjangoContext
```

### Comparing `strawberry_azure_auth-1.3.0/strawberry_azure_auth/extension.py` & `strawberry_azure_auth-2.0.0/strawberry_azure_auth/extension.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 __all__ = ["AzureAuthExtension"]
 
-
 import jwt
+import asyncio
 import logging
 import contextlib
 from uuid import UUID
 from typing import Any
 from graphql import GraphQLError, ExecutionResult
 from strawberry.extensions.base_extension import SchemaExtension
 from strawberry.utils.await_maybe import AsyncIteratorOrIterator
@@ -30,85 +30,70 @@
         >>> from strawberry_azure_auth import AzureAuthExtension
         ...
         >>> schema = Schema(
         ...     query=...,
         ...     extensions=[
         ...         AzureAuthExtension(
         ...             client_id=...,
-        ...             tenant_id=...,
-        ...             scopes=...
+        ...             tenant_id=...
         ...         )
         ...     ]
     """
 
     execution_context: ExecutionContext
 
-    # TODO: rename the 'allow_unauthenticated' and 'allow_unauthorized' params
     def __init__(
         self,
         *,
         client_id: str,
         tenant_id: str,
-        scopes: str | list[str],
+        scopes: str | list[str] | None = None,
         roles: list[str] | None = None,
         enable_caching: bool = False,
         allow_introspection: bool = True,
-        allow_unauthenticated: bool = False,
         allow_unauthorized: bool = False,
         execution_context: ExecutionContext | None = None,
     ) -> None:
         """
         :param client_id: Your Azure application's client ID.
         :param tenant_id: Your Azure tenant ID.
-        :param scopes: Scope(s) defined by your Azure application.
+        :param scopes: Optional scope(s) defined by your Azure application.
             The provided scopes are used to validate the 'scp' claim
             which means that all access tokens must include at least one of them.
         :param roles: Optional role(s) defined by your Azure application.
-            If any are provided, they will be used to validate the 'roles' claim
+            The provided roles are used to validate the 'roles' claim
             which means that all access tokens must include at least one of them.
-            Does nothing if the `allow_unauthorized_operations` param is set to `True`.
         :param enable_caching: Whether to cache the OpenID configuration using Django's built-in cache framework or not.
             Useful during development to avoid re-fetching the OpenID document every time the application restarts.
             Off by default.
-        :param allow_introspection: Whether to allow introspection queries or not.
+        :param allow_introspection: Whether to allow unauthenticated introspection queries or not.
             Enabled by default.
-        :param allow_unauthenticated: Whether to allow unauthenticated requests or not.
-            By default, all unauthenticated requests will be stopped before they're executed.
-            Settings this to `True` will let those requests through, leaving it up to the permission classes to
-            allow or block operations.
-            Useful if you have *any* operations that should not require authentication.
-            WARNING: Using this in conjunction with the 'allow_unauthorized' flag
-            will disable the authentication completely!
         :param allow_unauthorized: Whether to allow unauthorized requests or not.
-            By default, all unauthorized requests will be stopped by the extension (when using the 'roles' flag)
-            or by any permission classes that inherit from
-            the :class:`RoleBasedPermission<strawberry_azure_auth.permissions.RoleBasedPermission>` class.
-            WARNING: Settings this to `True` will disable the permission handling, and
-            using it in conjunction with the 'allow_unauthenticated' flag will disable the authentication completely!
+            By default, the extension stops all unauthorized requests before they're executed.
+            Set this to `True` to turn of this behavior.
+            Useful if you have *any* operations that should not require authentication.
         """
         super().__init__(execution_context=execution_context)  # type: ignore[arg-type]
         self._client_id: str = client_id
         self._tenant_id: str = tenant_id
-        self._scopes: list[str] = scopes.split(" ") if isinstance(scopes, str) else scopes
+        self._scopes: list[str] = scopes.split(" ") if isinstance(scopes, str) else scopes if scopes else []
         self._roles: list[str] | None = roles
         self._allow_introspection: bool = allow_introspection
-        self._allow_unauthenticated: bool = allow_unauthenticated
         self._allow_unauthorized: bool = allow_unauthorized
         self._openid: OpenIDConfig = OpenIDConfig(
             client_id=client_id, tenant_id=tenant_id, enable_caching=enable_caching
         )
+        with contextlib.suppress(Exception):
+            asyncio.run_coroutine_threadsafe(coro=self._openid.load_config(), loop=asyncio.get_event_loop())
 
     async def on_operation(self) -> AsyncIteratorOrIterator[None]:
         """
         Hook that runs at the start/ end of every request/ operation:
         Authenticate incoming requests by validating the provided access tokens.
         """
-        self.execution_context.context._handle_authentication = not self._allow_unauthenticated
-        self.execution_context.context._handle_authorization = not self._allow_unauthorized
-
         if not self.execution_context.context.authorized and (
             access_token := self.execution_context.context.access_token
         ):
             header: dict[str, str] = jwt.get_unverified_header(jwt=access_token)
             if kid := header.get("kid"):
                 await self._openid.load_config()
                 if (issuer := self._openid.issuer) and (signing_key := self._openid.signing_keys.get(kid)):
@@ -121,36 +106,26 @@
                         self.execution_context.context.roles = claims.get("roles", [])
         yield
 
     async def on_execute(self) -> AsyncIteratorOrIterator[None]:
         """
         Hook that runs before / after the 'GraphQL execution step':
         Stop the execution of unauthorized requests by manually setting the execution result.
-        This behaviour can be controlled using the 'roles', 'allow_introspection', 'allow_unauthenticated',
-        and 'allow_unauthorized' parameters.
+        This behavior can be controlled with the 'allow_introspection' and 'allow_unauthorized' parameters.
         """
         if not bool(
             self._allow_introspection
             and is_introspection_query(graphql_document=self.execution_context.graphql_document)
         ):
-            if not self._allow_unauthenticated and not self.execution_context.context.authorized:
+            if not self._allow_unauthorized and not self.execution_context.context.authorized:
                 self.execution_context.result = ExecutionResult(
                     data=None, errors=[GraphQLError(message="Unauthorized")]
                 )
-                if hasattr(self.execution_context.context, "response"):  # django http
+                if hasattr(self.execution_context.context, "response"):
                     self.execution_context.context.response.status_code = 401
-            elif (
-                not self._allow_unauthorized
-                and self.execution_context.context.authorized
-                and self._roles
-                and not any(role in self._roles for role in self.execution_context.context.roles)
-            ):
-                self.execution_context.result = ExecutionResult(data=None, errors=[GraphQLError(message="Forbidden")])
-                if hasattr(self.execution_context.context, "response"):  # django http
-                    self.execution_context.context.response.status_code = 403
         yield
 
     # region - Internal methods
     def _validate_token(self, token: str, signing_key: RSAPublicKey, issuer: str) -> dict[str, Any]:
         """
         Attempt to decode and validate the supplied access token:
         If the token is valid, its claims are returned.
@@ -187,21 +162,14 @@
         Overview: https://learn.microsoft.com/en-us/azure/active-directory/develop/access-tokens#payload-claims
         """
         # sub: Subject (whom the token refers to), a unique string per user per application (ID).
         sub: str | None = claims.get("sub")
         if not sub or not isinstance(sub, str):
             raise jwt.InvalidTokenError("Invalid 'sub' claim")
 
-        # scp: Scopes exposed by the application for which the client application has requested (and received) consent.
-        scp: str | None = claims.get("scp")
-        if not scp or not isinstance(scp, str):
-            raise jwt.InvalidTokenError("Invalid 'scp' claim")
-        if self._scopes and scp not in self._scopes:
-            raise jwt.InvalidTokenError("invalid 'scp' claim")
-
         # tid: The tenant ID (GUID) that the user is signing in to.
         tid: str | None = claims.get("tid")
         if not tid or not isinstance(tid, str) or tid != self._tenant_id:
             raise jwt.InvalidTokenError("Invalid 'tid' claim")
 
         # uti: Token identifier claim (jti in JWT spec), a unique, per-token identifier.
         uti: str | None = claims.get("uti")
@@ -218,8 +186,24 @@
             raise jwt.InvalidTokenError("Invalid 'oid' claim")
 
         # azp: Authorized party, the application ID (GUID) of the client using the token.
         azp: str | None = claims.get("azp")
         if not azp or not isinstance(azp, str) or azp != self._client_id:
             raise jwt.InvalidTokenError("Invalid 'azp' claim")
 
+        # scp: Scopes exposed by the application for which the client application has requested (and received) consent.
+        if self._scopes:
+            scp: str | None = claims.get("scp")
+            if not scp or not isinstance(scp, str):
+                raise jwt.InvalidTokenError("Invalid 'scp' claim")
+            if scp not in self._scopes:
+                raise jwt.InvalidTokenError("invalid 'scp' claim")
+
+        # roles: Permissions exposed by the application that the requesting user has been given.
+        if self._roles:
+            roles: list[str] | None = claims.get("roles")
+            if not roles:
+                raise jwt.InvalidTokenError("Invalid 'roles' claim")
+            if not any(role in roles for role in self._roles):
+                raise jwt.InvalidTokenError("Invalid 'roles' claim")
+
     # endregion
```

### Comparing `strawberry_azure_auth-1.3.0/strawberry_azure_auth/openid.py` & `strawberry_azure_auth-2.0.0/strawberry_azure_auth/openid.py`

 * *Files identical despite different names*

### Comparing `strawberry_azure_auth-1.3.0/strawberry_azure_auth/permissions.py` & `strawberry_azure_auth-2.0.0/strawberry_azure_auth/permissions.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,18 +20,20 @@
         ...     roles = ["App.Read"]
     """
 
     message: str
     roles: list[str]
 
     async def has_permission(self, source: Any, info: Info, **kwargs: Any) -> bool:
-        if info.context._handle_authentication and not info.context.authorized:
-            self.message = "Unauthorized"
+        if not info.context.authorized:
+            if not self.message:
+                self.message = "Unauthorized"
             if hasattr(info.context, "response"):
                 info.context.response.status_code = 401
             return False
-        if info.context._handle_authorization and not any(role in info.context.roles for role in self.roles):
-            self.message = "Forbidden"
+        if not any(role in info.context.roles for role in self.roles):
+            if not self.message:
+                self.message = "Forbidden"
             if hasattr(info.context, "response"):
                 info.context.response.status_code = 403
             return False
         return True
```

### Comparing `strawberry_azure_auth-1.3.0/strawberry_azure_auth/types.py` & `strawberry_azure_auth-2.0.0/strawberry_azure_auth/types.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 __all__ = ["Context", "ExecutionContext", "Info"]
 
 from typing import TypeAlias, Union, Any
 from strawberry.types.info import Info as StrawberryInfo
 
-from .channels.context import ChannelsContext, ChannelsExecutionContext
+from .channels.context import ChannelsHTTPContext, ChannelsWebsocketContext, ChannelsExecutionContext
 from .django.context import DjangoContext, DjangoExecutionContext
 
 
-Context: TypeAlias = Union[ChannelsContext, DjangoContext]
+Context: TypeAlias = Union[ChannelsHTTPContext, ChannelsWebsocketContext, DjangoContext]
 ExecutionContext: TypeAlias = Union[ChannelsExecutionContext, DjangoExecutionContext]
 
 Info: TypeAlias = StrawberryInfo[Context, Any]
```

### Comparing `strawberry_azure_auth-1.3.0/strawberry_azure_auth/utils.py` & `strawberry_azure_auth-2.0.0/strawberry_azure_auth/utils.py`

 * *Files identical despite different names*

### Comparing `strawberry_azure_auth-1.3.0/PKG-INFO` & `strawberry_azure_auth-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: strawberry-azure-auth
-Version: 1.3.0
+Version: 2.0.0
 Summary: Azure AD authentication for Strawberry GraphQL
 Home-page: https://github.com/skarre-r/strawberry-azure-auth
 License: MIT
 Author: skarre-r
 Author-email: skarre-r@protonmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: pyjwt[crypto] (>=2.7.0,<3.0.0)
-Requires-Dist: strawberry-graphql-django (>=0.9.4,<0.10.0)
-Requires-Dist: strawberry-graphql[channels] (>=0.179.0,<0.180.0)
+Requires-Dist: strawberry-graphql-django (>=0.9.5)
+Requires-Dist: strawberry-graphql[channels] (>=0.187.4)
 Project-URL: Repository, https://github.com/skarre-r/strawberry-azure-auth
 Description-Content-Type: text/markdown
 
 # strawberry-azure-auth
 
 Azure AD authentication for [Strawberry GraphQL](https://github.com/strawberry-graphql/strawberry),
 inspired by [fastapi-azure-auth](https://github.com/Intility/fastapi-azure-auth).
@@ -48,43 +48,43 @@
 from strawberry_azure_auth import AzureAuthExtension  # <--
 
 schema = strawberry.Schema(
     query=...,
     extensions=[
         AzureAuthExtension(  # <--
             client_id=...,
-            tenant_id=...,
-            scopes=...
+            tenant_id=...
         )
     ]
 )
 ```
 
 ### Channels
 
 Currently, strawberry schema extensions don't apply to graphql subscriptions
 (see [issue #2097](https://github.com/strawberry-graphql/strawberry/issues/2097)).
 
 To make the authentication extension work with channels,
 this package comes with custom http/ websocket "graphql consumer" classes
 and a custom `Schema` class that provides extension support for subscriptions:
 
+> :warning: The `Schema` class will be removed in the future when Strawberry adds extension support for subscriptions!
+
 ```python
 # example/schema.py
 from strawberry_azure_auth import AzureAuthExtension  # <--
 from strawberry_azure_auth.channels import Schema  # <--
 
 schema = Schema(  # <--
     query=...,
     subscription=...,
     extensions=[
         AzureAuthExtension(  # <--
             client_id=...,
-            tenant_id=...,
-            scopes=...
+            tenant_id=...
         )
     ]
 )
 ```
 
 ```python
 # example/asgi.py
@@ -144,14 +144,13 @@
 
 schema = strawberry.Schema(
     query=...,
     extensions=[
         AzureAuthExtension(
             client_id=...,
             tenant_id=...,
-            scopes=...,
             roles=["Example.Read"]  # <--
         )
     ]
 )
 ```
```


# Comparing `tmp/strawberry_django_plus-3.0.1.tar.gz` & `tmp/strawberry_django_plus-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strawberry_django_plus-3.0.1.tar", max compression
+gzip compressed data, was "strawberry_django_plus-3.0.2.tar", max compression
```

## Comparing `strawberry_django_plus-3.0.1.tar` & `strawberry_django_plus-3.0.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1094 2023-06-17 17:55:21.212398 strawberry_django_plus-3.0.1/LICENSE
--rw-r--r--   0        0        0     3354 2023-06-17 17:55:21.212398 strawberry_django_plus-3.0.1/README.md
--rw-r--r--   0        0        0     4208 2023-06-17 17:55:21.216398 strawberry_django_plus-3.0.1/pyproject.toml
--rw-r--r--   0        0        0     3001 2023-06-17 17:55:21.216398 strawberry_django_plus-3.0.1/strawberry_django_plus/__init__.py
--rw-r--r--   0        0        0     5649 2023-06-17 17:55:21.216398 strawberry_django_plus-3.0.1/strawberry_django_plus/descriptors.py
--rw-r--r--   0        0        0     5752 2023-06-17 17:55:21.216398 strawberry_django_plus-3.0.1/strawberry_django_plus/directives.py
--rw-r--r--   0        0        0    29442 2023-06-17 17:55:21.216398 strawberry_django_plus-3.0.1/strawberry_django_plus/field.py
--rw-r--r--   0        0        0     3033 2023-06-17 17:55:21.216398 strawberry_django_plus-3.0.1/strawberry_django_plus/filters.py
--rw-r--r--   0        0        0     1556 2023-06-17 17:55:21.216398 strawberry_django_plus-3.0.1/strawberry_django_plus/gql/__init__.py
--rw-r--r--   0        0        0     1515 2023-06-17 17:55:21.216398 strawberry_django_plus-3.0.1/strawberry_django_plus/gql/django.py
--rw-r--r--   0        0        0        0 2023-06-17 17:55:21.216398 strawberry_django_plus-3.0.1/strawberry_django_plus/integrations/__init__.py
--rw-r--r--   0        0        0     1939 2023-06-17 17:55:21.216398 strawberry_django_plus-3.0.1/strawberry_django_plus/integrations/guardian.py
--rw-r--r--   0        0        0        0 2023-06-17 17:55:21.216398 strawberry_django_plus-3.0.1/strawberry_django_plus/management/commands/__init__.py
--rw-r--r--   0        0        0     1168 2023-06-17 17:55:21.216398 strawberry_django_plus-3.0.1/strawberry_django_plus/management/commands/export_schema.py
--rw-r--r--   0        0        0        0 2023-06-17 17:55:21.216398 strawberry_django_plus-3.0.1/strawberry_django_plus/middlewares/__init__.py
--rw-r--r--   0        0        0      896 2023-06-17 17:55:21.216398 strawberry_django_plus-3.0.1/strawberry_django_plus/middlewares/user_warmup.py
--rw-r--r--   0        0        0        0 2023-06-17 17:55:21.216398 strawberry_django_plus-3.0.1/strawberry_django_plus/mutations/__init__.py
--rw-r--r--   0        0        0    24104 2023-06-17 17:55:21.216398 strawberry_django_plus-3.0.1/strawberry_django_plus/mutations/fields.py
--rw-r--r--   0        0        0    14791 2023-06-17 17:55:21.216398 strawberry_django_plus-3.0.1/strawberry_django_plus/mutations/resolvers.py
--rw-r--r--   0        0        0    26439 2023-06-17 17:55:21.220398 strawberry_django_plus-3.0.1/strawberry_django_plus/optimizer.py
--rw-r--r--   0        0        0     1340 2023-06-17 17:55:21.220398 strawberry_django_plus-3.0.1/strawberry_django_plus/ordering.py
--rw-r--r--   0        0        0    28085 2023-06-17 17:55:21.220398 strawberry_django_plus-3.0.1/strawberry_django_plus/permissions.py
--rw-r--r--   0        0        0        0 2023-06-17 17:55:21.220398 strawberry_django_plus-3.0.1/strawberry_django_plus/py.typed
--rw-r--r--   0        0        0     2532 2023-06-17 17:55:21.220398 strawberry_django_plus-3.0.1/strawberry_django_plus/relay.py
--rw-r--r--   0        0        0     1027 2023-06-17 17:55:21.220398 strawberry_django_plus-3.0.1/strawberry_django_plus/settings.py
--rw-r--r--   0        0        0        0 2023-06-17 17:55:21.220398 strawberry_django_plus-3.0.1/strawberry_django_plus/test/__init__.py
--rw-r--r--   0        0        0     2408 2023-06-17 17:55:21.220398 strawberry_django_plus-3.0.1/strawberry_django_plus/test/client.py
--rw-r--r--   0        0        0    16382 2023-06-17 17:55:21.220398 strawberry_django_plus-3.0.1/strawberry_django_plus/type.py
--rw-r--r--   0        0        0     9889 2023-06-17 17:55:21.220398 strawberry_django_plus-3.0.1/strawberry_django_plus/types.py
--rw-r--r--   0        0        0        0 2023-06-17 17:55:21.220398 strawberry_django_plus-3.0.1/strawberry_django_plus/utils/__init__.py
--rw-r--r--   0        0        0     6916 2023-06-17 17:55:21.220398 strawberry_django_plus-3.0.1/strawberry_django_plus/utils/aio.py
--rw-r--r--   0        0        0    13223 2023-06-17 17:55:21.220398 strawberry_django_plus-3.0.1/strawberry_django_plus/utils/inspect.py
--rw-r--r--   0        0        0     1077 2023-06-17 17:55:21.220398 strawberry_django_plus-3.0.1/strawberry_django_plus/utils/pyutils.py
--rw-r--r--   0        0        0     5865 2023-06-17 17:55:21.220398 strawberry_django_plus-3.0.1/strawberry_django_plus/utils/query.py
--rw-r--r--   0        0        0    16244 2023-06-17 17:55:21.220398 strawberry_django_plus-3.0.1/strawberry_django_plus/utils/resolvers.py
--rw-r--r--   0        0        0      938 2023-06-17 17:55:21.220398 strawberry_django_plus-3.0.1/strawberry_django_plus/utils/typing.py
--rw-r--r--   0        0        0     4875 1970-01-01 00:00:00.000000 strawberry_django_plus-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1094 2023-06-23 19:13:11.079420 strawberry_django_plus-3.0.2/LICENSE
+-rw-r--r--   0        0        0     3354 2023-06-23 19:13:11.079420 strawberry_django_plus-3.0.2/README.md
+-rw-r--r--   0        0        0     4208 2023-06-23 19:13:11.079420 strawberry_django_plus-3.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3088 2023-06-23 19:13:11.079420 strawberry_django_plus-3.0.2/strawberry_django_plus/__init__.py
+-rw-r--r--   0        0        0     5649 2023-06-23 19:13:11.079420 strawberry_django_plus-3.0.2/strawberry_django_plus/descriptors.py
+-rw-r--r--   0        0        0     5800 2023-06-23 19:13:11.079420 strawberry_django_plus-3.0.2/strawberry_django_plus/directives.py
+-rw-r--r--   0        0        0    30229 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/field.py
+-rw-r--r--   0        0        0     3033 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/filters.py
+-rw-r--r--   0        0        0     1556 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/gql/__init__.py
+-rw-r--r--   0        0        0     1515 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/gql/django.py
+-rw-r--r--   0        0        0        0 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/integrations/__init__.py
+-rw-r--r--   0        0        0     1939 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/integrations/guardian.py
+-rw-r--r--   0        0        0        0 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/management/commands/__init__.py
+-rw-r--r--   0        0        0     1168 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/management/commands/export_schema.py
+-rw-r--r--   0        0        0        0 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/middlewares/__init__.py
+-rw-r--r--   0        0        0      896 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/middlewares/user_warmup.py
+-rw-r--r--   0        0        0        0 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/mutations/__init__.py
+-rw-r--r--   0        0        0    24115 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/mutations/fields.py
+-rw-r--r--   0        0        0    14791 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/mutations/resolvers.py
+-rw-r--r--   0        0        0    26666 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/optimizer.py
+-rw-r--r--   0        0        0     1340 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/ordering.py
+-rw-r--r--   0        0        0    28069 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/permissions.py
+-rw-r--r--   0        0        0        0 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/py.typed
+-rw-r--r--   0        0        0     2532 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/relay.py
+-rw-r--r--   0        0        0     1027 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/settings.py
+-rw-r--r--   0        0        0        0 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/test/__init__.py
+-rw-r--r--   0        0        0     2408 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/test/client.py
+-rw-r--r--   0        0        0    17885 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/type.py
+-rw-r--r--   0        0        0     9889 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/types.py
+-rw-r--r--   0        0        0        0 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/utils/__init__.py
+-rw-r--r--   0        0        0     6916 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/utils/aio.py
+-rw-r--r--   0        0        0    13343 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/utils/inspect.py
+-rw-r--r--   0        0        0     1077 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/utils/pyutils.py
+-rw-r--r--   0        0        0     5865 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/utils/query.py
+-rw-r--r--   0        0        0    16244 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/utils/resolvers.py
+-rw-r--r--   0        0        0      938 2023-06-23 19:13:11.083420 strawberry_django_plus-3.0.2/strawberry_django_plus/utils/typing.py
+-rw-r--r--   0        0        0     4875 1970-01-01 00:00:00.000000 strawberry_django_plus-3.0.2/PKG-INFO
```

### Comparing `strawberry_django_plus-3.0.1/LICENSE` & `strawberry_django_plus-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.1/README.md` & `strawberry_django_plus-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.1/pyproject.toml` & `strawberry_django_plus-3.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strawberry-django-plus"
-version = "3.0.1"
+version = "3.0.2"
 description = "Enhanced Strawberry GraphQL integration with Django"
 authors = ["Thiago Bellini Ribeiro <thiago@bellini.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/blb-ventures/strawberry-django-plus"
 repository = "https://github.com/blb-ventures/strawberry-django-plus"
 documentation = "https://strawberry-django-plus.readthedocs.io"
@@ -29,15 +29,15 @@
 ]
 packages = [{ include = "strawberry_django_plus" }]
 include = ["strawberry_django_plus/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 django = ">= 3.2"
-strawberry-graphql = ">=0.184.0"
+strawberry-graphql = ">=0.187.5"
 strawberry-graphql-django = ">= 0.9.4"
 typing-extensions = ">= 4.2.0"
 django-choices-field = { version = ">=2.0", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 codecov = "^2.1.12"
```

### Comparing `strawberry_django_plus-3.0.1/strawberry_django_plus/__init__.py` & `strawberry_django_plus-3.0.2/strawberry_django_plus/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import inspect
 import re
 
 from strawberry import object_type
 from strawberry.enum import EnumDefinition
 from strawberry.field import StrawberryField
 from strawberry.schema.name_converter import NameConverter
+from strawberry.type import get_object_definition
 from strawberry.types.fields.resolver import StrawberryResolver
 
 _cls_docs = {}
 _original_process_type = object_type._process_type
 _original_process_type = object_type._process_type
 _original_wrap_dataclass = object_type._wrap_dataclass
 _original_field_init = StrawberryField.__init__
 _original_field_call = StrawberryField.__call__
 _original_enum_init = EnumDefinition.__init__
 _original_from_generic = NameConverter.from_generic
 
-__version__ = "3.0.1"  # x-release-please-version
+__version__ = "3.0.2"  # x-release-please-version
 
 
 def _get_doc(obj):
     if not obj.__doc__:
         return None
     return inspect.cleandoc(obj.__doc__)
 
@@ -28,17 +29,18 @@
 def _process_type(cls, *args, **kwargs):
     from strawberry_django_plus.directives import SchemaDirectiveWithResolver
 
     if kwargs.get("description") is None:
         kwargs["description"] = _cls_docs.get(cls)
     ret = _original_process_type(cls, *args, **kwargs)
 
-    for d in ret._type_definition.directives:
+    type_def = get_object_definition(ret, strict=True)
+    for d in type_def.directives or []:
         if isinstance(d, SchemaDirectiveWithResolver):
-            d.register(ret._type_definition)
+            d.register(type_def)
 
     return ret
 
 
 def _wrap_dataclass(cls):
     _cls_docs[cls] = _get_doc(cls)
     return _original_wrap_dataclass(cls)
```

### Comparing `strawberry_django_plus-3.0.1/strawberry_django_plus/descriptors.py` & `strawberry_django_plus-3.0.2/strawberry_django_plus/descriptors.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.1/strawberry_django_plus/directives.py` & `strawberry_django_plus-3.0.2/strawberry_django_plus/directives.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,25 +25,25 @@
     GraphQLUnionType,
     GraphQLWrappingType,
 )
 from strawberry.extensions import SchemaExtension
 from strawberry.field import StrawberryField
 from strawberry.private import Private
 from strawberry.schema.schema import Schema
-from strawberry.types.types import TypeDefinition
+from strawberry.types.types import StrawberryObjectDefinition
 from strawberry.utils.await_maybe import AwaitableOrValue
 from typing_extensions import TypeAlias
 
 try:
     # Try to use the smaller/faster cache decorator if available
     _cache = functools.cache  # type: ignore
 except AttributeError:
     _cache = functools.lru_cache
 
-Origin: TypeAlias = Union[TypeDefinition, StrawberryField]
+Origin: TypeAlias = Union[StrawberryObjectDefinition, StrawberryField]
 
 _origin_cache: DefaultDict[Origin, List["SchemaDirectiveWithResolver"]] = defaultdict(list)
 
 
 @dataclasses.dataclass
 @functools.total_ordering
 class SchemaDirectiveWithResolver:
@@ -83,15 +83,15 @@
     ) -> AwaitableOrValue[Any]:
         raise NotImplementedError
 
 
 @dataclasses.dataclass
 class SchemaDirectiveHelperReturnType:
     ret_type: Union[GraphQLObjectType, GraphQLInterfaceType, GraphQLScalarType, GraphQLEnumType]
-    type_def: Optional[TypeDefinition] = dataclasses.field(default=None)
+    type_def: Optional[StrawberryObjectDefinition] = dataclasses.field(default=None)
 
 
 @dataclasses.dataclass
 class SchemaDirectiveHelper:
     directives: List[SchemaDirectiveWithResolver]
     ret_possibilities: List[SchemaDirectiveHelperReturnType]
     optional: bool
@@ -132,15 +132,15 @@
 
         schema = cast(
             Schema,
             info.schema._strawberry_schema,  # type: ignore
         )
 
         type_def = schema.get_type_by_name(type_name)
-        if isinstance(type_def, TypeDefinition):
+        if isinstance(type_def, StrawberryObjectDefinition):
             field = next(
                 (
                     f
                     for f in type_def.fields
                     if field_name == schema.config.name_converter.get_graphql_name(f)
                 ),
                 None,
```

### Comparing `strawberry_django_plus-3.0.1/strawberry_django_plus/field.py` & `strawberry_django_plus-3.0.2/strawberry_django_plus/field.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import dataclasses
 import inspect
 from functools import cached_property
 from typing import (
+    TYPE_CHECKING,
     Any,
     Awaitable,
     Callable,
     Dict,
     Iterable,
     List,
     Literal,
@@ -34,18 +35,17 @@
 from strawberry.arguments import StrawberryArgument
 from strawberry.auto import StrawberryAuto
 from strawberry.extensions.field_extension import FieldExtension, SyncExtensionResolver
 from strawberry.field import _RESOLVER_TYPE, UNRESOLVED, StrawberryField
 from strawberry.lazy_type import LazyType
 from strawberry.permission import BasePermission
 from strawberry.relay.types import NodeIterableType
-from strawberry.type import StrawberryContainer, StrawberryType
+from strawberry.type import StrawberryContainer, StrawberryType, get_object_definition
 from strawberry.types.fields.resolver import StrawberryResolver
 from strawberry.types.info import Info
-from strawberry.types.types import TypeDefinition
 from strawberry.union import StrawberryUnion
 from strawberry_django.arguments import argument
 from strawberry_django.fields.field import (
     StrawberryDjangoField as _StrawberryDjangoField,
 )
 from strawberry_django.fields.types import get_model_field, is_optional
 from strawberry_django.utils import unwrap_type
@@ -55,14 +55,17 @@
 
 from . import optimizer
 from .descriptors import ModelProperty
 from .permissions import filter_with_perms
 from .utils import resolvers
 from .utils.typing import TypeOrSequence
 
+if TYPE_CHECKING:
+    from strawberry_django_plus.type import StrawberryDjangoType
+
 __all__ = [
     "StrawberryDjangoField",
     "StrawberryDjangoConnectionExtension",
     "field",
     "node",
     "connection",
 ]
@@ -122,15 +125,34 @@
 
     @property
     def type(self) -> Union[StrawberryType, type, Literal[UNRESOLVED]]:  # type: ignore # noqa: A003
         resolved = super().type
         if resolved is UNRESOLVED:
             return resolved
 
-        if isinstance(resolved, StrawberryAuto) and self.origin_django_type:
+        resolved_type = resolved
+        while isinstance(resolved_type, StrawberryContainer):
+            resolved_type = resolved_type.of_type
+        resolved_django_type: Optional["StrawberryDjangoType"] = getattr(
+            resolved_type,
+            "_django_type",
+            None,
+        )
+
+        if self.origin_django_type and (
+            # FIXME: Why does this come as Any sometimes when using future annotations?
+            resolved is Any
+            or isinstance(resolved, StrawberryAuto)
+            # If the resolved type is an input but the origin is not, or vice versa,
+            # resolve this again
+            or (
+                resolved_django_type
+                and resolved_django_type.is_input != self.origin_django_type.is_input
+            )
+        ):
             model_field = get_model_field(
                 self.origin_django_type.model,
                 self.django_name or self.name,
             )
             resolved_type = resolve_model_field_type(model_field, self.origin_django_type)
             if is_optional(
                 model_field,
@@ -168,17 +190,20 @@
 
         return filters if filters is not UNSET else None
 
     @cached_property
     def type_origin(self) -> Optional[Type]:
         origin = self.type
 
-        tdef = cast(Optional[TypeDefinition], getattr(origin, "_type_definition", None))
-        if tdef and tdef.concrete_of and issubclass(tdef.concrete_of.origin, relay.Connection):
-            origin = tdef.type_var_map[relay.NodeType]  # type: ignore
+        if (
+            (tdef := get_object_definition(origin))
+            and tdef.concrete_of
+            and issubclass(tdef.concrete_of.origin, relay.Connection)
+        ):
+            origin = tdef.type_var_map[cast(TypeVar, relay.NodeType)]
             if isinstance(origin, LazyType):
                 origin = origin.resolve_type()
 
         while isinstance(origin, StrawberryContainer):
             origin = origin.of_type
 
         if isinstance(origin, StrawberryUnion):
```

### Comparing `strawberry_django_plus-3.0.1/strawberry_django_plus/filters.py` & `strawberry_django_plus-3.0.2/strawberry_django_plus/filters.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.1/strawberry_django_plus/gql/__init__.py` & `strawberry_django_plus-3.0.2/strawberry_django_plus/gql/__init__.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.1/strawberry_django_plus/gql/django.py` & `strawberry_django_plus-3.0.2/strawberry_django_plus/gql/django.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.1/strawberry_django_plus/integrations/guardian.py` & `strawberry_django_plus-3.0.2/strawberry_django_plus/integrations/guardian.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.1/strawberry_django_plus/management/commands/export_schema.py` & `strawberry_django_plus-3.0.2/strawberry_django_plus/management/commands/export_schema.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.1/strawberry_django_plus/middlewares/user_warmup.py` & `strawberry_django_plus-3.0.2/strawberry_django_plus/middlewares/user_warmup.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.1/strawberry_django_plus/mutations/fields.py` & `strawberry_django_plus-3.0.2/strawberry_django_plus/mutations/fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 )
 from strawberry import UNSET, relay
 from strawberry.annotation import StrawberryAnnotation
 from strawberry.arguments import StrawberryArgument
 from strawberry.extensions.field_extension import FieldExtension
 from strawberry.field_extensions import InputMutationExtension
 from strawberry.permission import BasePermission
-from strawberry.type import StrawberryType
+from strawberry.type import StrawberryType, get_object_definition
 from strawberry.types.fields.resolver import StrawberryResolver
 from strawberry.types.info import Info
 from strawberry.utils.await_maybe import AwaitableOrValue
 from strawberry.utils.str_converters import to_camel_case
 
 from strawberry_django_plus.field import StrawberryDjangoField
 from strawberry_django_plus.optimizer import DjangoOptimizerExtension
@@ -171,15 +171,15 @@
         super().__init__(*args, **kwargs)
         self.input_type = input_type
         self.full_clean = full_clean
 
     @property
     def arguments(self) -> List[StrawberryArgument]:
         namespace = sys.modules[self.input_type.__module__].__dict__
-        type_def = getattr(self.input_type, "_type_definition", None)
+        type_def = get_object_definition(self.input_type)
         return [
             StrawberryArgument(
                 python_name="input",
                 graphql_name=None,
                 type_annotation=StrawberryAnnotation(self.input_type, namespace=namespace),
                 description=type_def and type_def.description,
             ),
```

### Comparing `strawberry_django_plus-3.0.1/strawberry_django_plus/mutations/resolvers.py` & `strawberry_django_plus-3.0.2/strawberry_django_plus/mutations/resolvers.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.1/strawberry_django_plus/optimizer.py` & `strawberry_django_plus-3.0.2/strawberry_django_plus/optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,19 +30,20 @@
 from django.db.models.manager import BaseManager
 from django.db.models.query import QuerySet
 from graphql.language.ast import OperationType
 from graphql.type.definition import GraphQLResolveInfo, get_named_type
 from strawberry import relay
 from strawberry.extensions import SchemaExtension
 from strawberry.lazy_type import LazyType
+from strawberry.object_type import StrawberryObjectDefinition
 from strawberry.schema.schema import Schema
+from strawberry.type import get_object_definition
 from strawberry.types.execution import ExecutionContext
 from strawberry.types.info import Info
 from strawberry.types.nodes import InlineFragment, Selection, convert_selections
-from strawberry.types.types import TypeDefinition
 from strawberry.utils.await_maybe import AwaitableOrValue
 from strawberry.utils.typing import eval_type
 from strawberry_django.fields.types import resolve_model_field_name
 from typing_extensions import TypeAlias, assert_never, assert_type
 
 from .descriptors import ModelProperty
 from .utils import resolvers
@@ -63,15 +64,21 @@
     "optimize",
 ]
 
 _T = TypeVar("_T")
 _M = TypeVar("_M", bound=models.Model)
 
 _sentinel = object()
-_interfaces: "defaultdict[Schema, Dict[TypeDefinition, List[TypeDefinition]]]" = defaultdict(dict)
+_interfaces: """
+defaultdict[
+    Schema,
+    Dict[StrawberryObjectDefinition, List[StrawberryObjectDefinition]],
+]""" = defaultdict(
+    dict,
+)
 
 
 PrefetchCallable: TypeAlias = Callable[[GraphQLResolveInfo], Prefetch]
 PrefetchType: TypeAlias = Union[str, Prefetch, PrefetchCallable]
 
 
 def _get_prefetch_queryset(
@@ -96,15 +103,15 @@
         remote_type = remote_type_defs[0]
     return remote_type.get_queryset(remote_model.objects.all(), info)
 
 
 def _get_model_hints(
     model: Type[models.Model],
     schema: Schema,
-    type_def: TypeDefinition,
+    type_def: StrawberryObjectDefinition,
     selection: Selection,
     *,
     info: GraphQLResolveInfo,
     config: Optional["OptimizerConfig"] = None,
     prefix: str = "",
     model_cache: Optional[Dict[Type[models.Model], List[Tuple[int, "OptimizerStore"]]]] = None,
     level: int = 0,
@@ -122,22 +129,25 @@
         if level > 0:
             return None
 
         n_type = type_def.type_var_map[cast(TypeVar, relay.NodeType)]
         if isinstance(n_type, LazyType):
             n_type = n_type.resolve_type()
 
-        n_type_def = cast(TypeDefinition, n_type._type_definition)  # type: ignore
+        n_type_def = get_object_definition(n_type, strict=True)
 
         for edges in get_selections(selection, typename=typename).values():
             if edges.name != "edges":
                 continue
 
-            e_type = relay.Edge._type_definition.resolve_generic(relay.Edge[n_type])  # type: ignore
-            e_typename = schema.config.name_converter.from_object(e_type._type_definition)
+            e_type_def = get_object_definition(relay.Edge, strict=True)
+            e_type = e_type_def.resolve_generic(relay.Edge[cast(Type[relay.Node], n_type)])
+            e_typename = schema.config.name_converter.from_object(
+                get_object_definition(e_type, strict=True),
+            )
             for node in get_selections(edges, typename=e_typename).values():
                 if node.name != "node":
                     continue
 
                 new_store = _get_model_hints(
                     model=model,
                     schema=schema,
@@ -373,15 +383,15 @@
         if type_def.is_interface:
             type_defs = _interfaces[schema].get(type_def)
             if type_defs is None:
                 type_defs = []
 
                 for t in schema.schema_converter.type_map.values():
                     tdef = t.definition
-                    if not isinstance(tdef, TypeDefinition):
+                    if not isinstance(tdef, StrawberryObjectDefinition):
                         continue
 
                     if issubclass(tdef.origin, type_def.origin):
                         dj_type = get_django_type(tdef.origin)
                         if dj_type and issubclass(qs.model, dj_type.model):
                             type_defs.append(tdef)
```

### Comparing `strawberry_django_plus-3.0.1/strawberry_django_plus/ordering.py` & `strawberry_django_plus-3.0.2/strawberry_django_plus/ordering.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.1/strawberry_django_plus/permissions.py` & `strawberry_django_plus-3.0.2/strawberry_django_plus/permissions.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,15 +272,15 @@
             )
 
         return self.resolve_for_user(
             helper,
             resolver,
             root,
             info,
-            cast(UserType, user),
+            user,
             **kwargs,
         )
 
     def resolve_for_user(
         self,
         helper: SchemaDirectiveHelper,
         resolver: Callable,
```

### Comparing `strawberry_django_plus-3.0.1/strawberry_django_plus/relay.py` & `strawberry_django_plus-3.0.2/strawberry_django_plus/relay.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.1/strawberry_django_plus/settings.py` & `strawberry_django_plus-3.0.2/strawberry_django_plus/settings.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.1/strawberry_django_plus/test/client.py` & `strawberry_django_plus-3.0.2/strawberry_django_plus/test/client.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.1/strawberry_django_plus/type.py` & `strawberry_django_plus-3.0.2/strawberry_django_plus/type.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import copy
 import dataclasses
 import inspect
 import sys
 import types
 from functools import cached_property
 from typing import (
     Callable,
@@ -23,15 +24,15 @@
 from strawberry import UNSET, relay
 from strawberry.annotation import StrawberryAnnotation
 from strawberry.exceptions import (
     MissingFieldAnnotationError,
 )
 from strawberry.field import StrawberryField
 from strawberry.private import is_private
-from strawberry.types.types import TypeDefinition
+from strawberry.type import get_object_definition
 from strawberry.unset import UnsetType
 from strawberry_django.fields.field import field as _field
 from strawberry_django.fields.types import get_model_field, resolve_model_field_name
 from strawberry_django.type import StrawberryDjangoType as _StraberryDjangoType
 from strawberry_django.utils import get_annotations
 from typing_extensions import dataclass_transform
 
@@ -84,53 +85,78 @@
     select_related: Optional[TypeOrSequence[str]] = None,
     prefetch_related: Optional[TypeOrSequence[PrefetchType]] = None,
     disable_optimization: bool = False,
     partial: bool = False,
     is_filter: Union[Literal["lookups"], bool] = False,
     **kwargs,
 ) -> _O:
+    is_input = kwargs.get("is_input", False)
     django_type = StrawberryDjangoType(
         origin=cls,
         model=model,
         field_cls=field_cls,
         is_partial=partial,
-        is_input=kwargs.get("is_input", False),
+        is_input=is_input,
         is_filter=is_filter,
         filters=filters,
         order=order,
         pagination=pagination,
         disable_optimization=disable_optimization,
         store=OptimizerStore.with_hints(
             only=only,
             select_related=select_related,
             prefetch_related=prefetch_related,
         ),
     )
 
-    if django_type.is_input:
+    auto_fields: set[str] = set()
+    for field_name, field_annotation in get_annotations(cls).items():
+        annotation = field_annotation.annotation
+        if is_private(annotation):
+            continue
+
+        if is_auto(annotation):
+            auto_fields.add(field_name)
+
         # FIXME: For input types it is imported to set the default value to UNSET
         # Is there a better way of doing this?
-        seen_fields = set()
-        for attr_name, attr in cls.__dict__.items():
-            seen_fields.add(attr_name)
-            if isinstance(attr, dataclasses.Field) and attr.default is dataclasses.MISSING:
-                attr.default = UNSET
-                if isinstance(attr, StrawberryField):
-                    attr.default_value = UNSET
-
-        for field_name, field_annotation in get_annotations(cls).items():
-            if field_name in seen_fields:
-                continue
+        if is_input:
+            # First check if the field is defined in the class. If it is,
+            # then we just need to set its default value to UNSET in case
+            # it is MISSING
+            if field_name in cls.__dict__:
+                field = cls.__dict__[field_name]
+                if isinstance(field, dataclasses.Field) and field.default is dataclasses.MISSING:
+                    field.default = UNSET
+                    if isinstance(field, StrawberryField):
+                        field.default_value = UNSET
 
-            annotation = field_annotation.annotation
-            if is_private(annotation):
                 continue
 
             if not hasattr(cls, field_name):
-                setattr(cls, field_name, UNSET)
+                base_field = getattr(cls, "__dataclass_fields__", {}).get(field_name)
+                if base_field is not None and isinstance(base_field, StrawberryField):
+                    new_field = copy.copy(base_field)
+                    for attr in [
+                        "_arguments",
+                        "permission_classes",
+                        "directives",
+                        "extensions",
+                    ]:
+                        old_attr = getattr(base_field, attr)
+                        if old_attr is not None:
+                            setattr(new_field, attr, old_attr[:])
+                else:
+                    new_field = _field(default=UNSET)
+
+                new_field.type_annotation = field_annotation
+                new_field.default = UNSET
+                if isinstance(base_field, StrawberryField):
+                    new_field.default_value = UNSET
+                setattr(cls, field_name, new_field)
 
     # Make sure model is also considered a "virtual subclass" of cls
     if "is_type_of" not in cls.__dict__:
         cls.is_type_of = lambda obj, info: isinstance(obj, (cls, model))  # type: ignore
 
     # Default querying methods for relay
     if issubclass(cls, relay.Node):
@@ -171,21 +197,34 @@
             meth = getattr(cls, attr)
             if isinstance(meth, types.MethodType) and meth.__self__ is not cls:
                 setattr(cls, attr, types.MethodType(cast(classmethod, meth).__func__, cls))
 
     strawberry.type(cls, **kwargs)
 
     # update annotations and fields
-    type_def = cast(TypeDefinition, cls._type_definition)  # type: ignore
+    type_def = get_object_definition(cls, strict=True)
     new_fields: List[StrawberryField] = []
-    for f in type_def._fields:
-        django_name: Optional[str] = getattr(f, "django_name", None) or f.name
+    for f in type_def.fields:
+        django_name: Optional[str] = getattr(f, "django_name", None) or f.python_name or f.name
         description: Optional[str] = getattr(f, "description", None)
-        type_annotation: Optional[StrawberryAnnotation] = getattr(f, "type_annotation", None)
-        f_is_auto = type_annotation is not None and is_auto(type_annotation.annotation)
+        type_annotation: Optional[StrawberryAnnotation] = getattr(
+            f,
+            "type_annotation",
+            None,
+        )
+
+        if f.name in auto_fields:
+            f_is_auto = True
+            # Force the field to be auto again for it to be re-evaluated
+            if type_annotation:
+                type_annotation.annotation = strawberry.auto
+        else:
+            f_is_auto = type_annotation is not None and is_auto(
+                type_annotation.annotation,
+            )
 
         try:
             if django_name is None:
                 raise FieldDoesNotExist  # noqa: TRY301
             model_attr = get_model_field(django_type.model, django_name)
         except FieldDoesNotExist as e:
             model_attr = getattr(django_type.model, django_name, None)
@@ -267,23 +306,24 @@
                 only=store and store.only,
                 select_related=store and store.select_related,
                 prefetch_related=store and store.prefetch_related,
                 disable_optimization=getattr(f, "disable_optimization", False),
                 extensions=getattr(f, "extensions", ()),
             )
 
+        f.django_name = django_name
         f.is_relation = is_relation
-        if f.origin_django_type is None:
-            f.origin_django_type = django_type  # type: ignore
+        f.origin_django_type = django_type  # type: ignore
 
         new_fields.append(f)
         if f.base_resolver and f.python_name:
             setattr(cls, f.python_name, f)
 
-    cls._type_definition._fields = new_fields  # type: ignore
+    type_def = get_object_definition(cls, strict=True)
+    type_def._fields = new_fields
     cls._django_type = django_type  # type: ignore
 
     return cls
 
 
 @dataclasses.dataclass
 class StrawberryDjangoType(_StraberryDjangoType[_O, _M]):
```

### Comparing `strawberry_django_plus-3.0.1/strawberry_django_plus/types.py` & `strawberry_django_plus-3.0.2/strawberry_django_plus/types.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.1/strawberry_django_plus/utils/aio.py` & `strawberry_django_plus-3.0.2/strawberry_django_plus/utils/aio.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.1/strawberry_django_plus/utils/inspect.py` & `strawberry_django_plus-3.0.2/strawberry_django_plus/utils/inspect.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,22 +22,27 @@
 from django.db.models.expressions import Expression
 from django.db.models.fields import Field
 from django.db.models.fields.reverse_related import ForeignObjectRel
 from django.db.models.query import Prefetch, QuerySet
 from django.db.models.sql.query import Query
 from django.db.models.sql.where import WhereNode
 from strawberry.lazy_type import LazyType
-from strawberry.type import StrawberryContainer, StrawberryType, StrawberryTypeVar
+from strawberry.type import (
+    StrawberryContainer,
+    StrawberryType,
+    StrawberryTypeVar,
+    get_object_definition,
+)
 from strawberry.types.nodes import (
     FragmentSpread,
     InlineFragment,
     SelectedField,
     Selection,
 )
-from strawberry.types.types import TypeDefinition
+from strawberry.types.types import StrawberryObjectDefinition
 from strawberry.union import StrawberryUnion
 from strawberry.utils.str_converters import to_camel_case
 from strawberry_django.fields.types import resolve_model_field_name
 from typing_extensions import assert_never
 
 from .pyutils import dicttree_insersection_differs, dicttree_merge
 from .typing import DictTree
@@ -117,31 +122,31 @@
     if ensure_type and not isinstance(django_type, StrawberryDjangoType):
         raise TypeError(f"{type_} does not contain a StrawberryDjangoType")
 
     return django_type
 
 
 def get_possible_types(
-    gql_type: Union[TypeDefinition, StrawberryType, type],
-    type_def: Optional[TypeDefinition] = None,
+    gql_type: Union[StrawberryObjectDefinition, StrawberryType, type],
+    type_def: Optional[StrawberryObjectDefinition] = None,
 ) -> Generator[type, None, None]:
     """Resolve all possible types for gql_type.
 
     Args:
         gql_type:
             The type to retrieve possibilities from.
         type_def:
             Optional type definition to use to resolve type vars. This is
             mostly used internally, no need to pass this.
 
     Yields:
         All possibilities for the type
 
     """
-    if isinstance(gql_type, TypeDefinition):
+    if isinstance(gql_type, StrawberryObjectDefinition):
         yield from get_possible_types(gql_type.origin, type_def=gql_type)
     elif isinstance(gql_type, LazyType):
         yield from get_possible_types(gql_type.resolve_type())
     elif isinstance(gql_type, StrawberryTypeVar) and type_def is not None:
         # Try to resolve TypeVar
         for f in type_def.fields:
             f_type = f.type
@@ -163,35 +168,35 @@
     elif isinstance(gql_type, type):
         yield gql_type
     else:
         assert_never(gql_type)
 
 
 def get_possible_type_definitions(
-    gql_type: Union[TypeDefinition, StrawberryType, type],
-) -> Generator[TypeDefinition, None, None]:
+    gql_type: Union[StrawberryObjectDefinition, StrawberryType, type],
+) -> Generator[StrawberryObjectDefinition, None, None]:
     """Resolve all possible type definitions for gql_type.
 
     Args:
         gql_type:
             The type to retrieve possibilities from.
 
     Yields:
         All possibilities for the type
 
     """
-    if isinstance(gql_type, TypeDefinition):
+    if isinstance(gql_type, StrawberryObjectDefinition):
         yield gql_type
         return
 
     for t in get_possible_types(gql_type):
-        if isinstance(t, TypeDefinition):
+        if isinstance(t, StrawberryObjectDefinition):
             yield t
-        elif hasattr(t, "_type_definition"):
-            yield t._type_definition  # type: ignore
+        elif type_def := get_object_definition(t):
+            yield type_def
 
 
 def get_selections(
     selection: Selection,
     *,
     typename: Optional[str] = None,
 ) -> Dict[str, SelectedField]:
```

### Comparing `strawberry_django_plus-3.0.1/strawberry_django_plus/utils/pyutils.py` & `strawberry_django_plus-3.0.2/strawberry_django_plus/utils/pyutils.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.1/strawberry_django_plus/utils/query.py` & `strawberry_django_plus-3.0.2/strawberry_django_plus/utils/query.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.1/strawberry_django_plus/utils/resolvers.py` & `strawberry_django_plus-3.0.2/strawberry_django_plus/utils/resolvers.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.1/strawberry_django_plus/utils/typing.py` & `strawberry_django_plus-3.0.2/strawberry_django_plus/utils/typing.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-3.0.1/PKG-INFO` & `strawberry_django_plus-3.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strawberry-django-plus
-Version: 3.0.1
+Version: 3.0.2
 Summary: Enhanced Strawberry GraphQL integration with Django
 Home-page: https://github.com/blb-ventures/strawberry-django-plus
 License: MIT
 Keywords: strawberry,django,graphql,relay,optimizer
 Author: Thiago Bellini Ribeiro
 Author-email: thiago@bellini.dev
 Requires-Python: >=3.8,<4.0
@@ -23,15 +23,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: enum
 Requires-Dist: django (>=3.2)
 Requires-Dist: django-choices-field (>=2.0) ; extra == "enum"
-Requires-Dist: strawberry-graphql (>=0.184.0)
+Requires-Dist: strawberry-graphql (>=0.187.5)
 Requires-Dist: strawberry-graphql-django (>=0.9.4)
 Requires-Dist: typing-extensions (>=4.2.0)
 Project-URL: Documentation, https://strawberry-django-plus.readthedocs.io
 Project-URL: Repository, https://github.com/blb-ventures/strawberry-django-plus
 Description-Content-Type: text/markdown
 
 # strawberry-django-plus
```


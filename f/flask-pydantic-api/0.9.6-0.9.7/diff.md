# Comparing `tmp/flask_pydantic_api-0.9.6-py3-none-any.whl.zip` & `tmp/flask_pydantic_api-0.9.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 12899 bytes, number of entries: 12
+Zip file size: 12909 bytes, number of entries: 12
 -rw-r--r--  2.0 unx       98 b- defN 23-Apr-06 01:39 flask_pydantic_api/__init__.py
--rw-r--r--  2.0 unx     7285 b- defN 23-Jun-22 05:00 flask_pydantic_api/api_wrapper.py
+-rw-r--r--  2.0 unx     7700 b- defN 23-Jun-23 00:54 flask_pydantic_api/api_wrapper.py
 -rw-r--r--  2.0 unx      819 b- defN 23-Mar-18 20:39 flask_pydantic_api/apidocs_views.py
 -rw-r--r--  2.0 unx     7733 b- defN 23-Jun-22 06:26 flask_pydantic_api/openapi.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-19 03:04 flask_pydantic_api/py.typed
 -rw-r--r--  2.0 unx     2342 b- defN 23-May-30 22:54 flask_pydantic_api/utils.py
 -rw-r--r--  2.0 unx      447 b- defN 23-Mar-18 20:21 flask_pydantic_api/templates/rapidoc.html
--rw-r--r--  2.0 unx     1073 b- defN 23-Jun-22 06:30 flask_pydantic_api-0.9.6.dist-info/LICENSE
--rw-r--r--  2.0 unx    12093 b- defN 23-Jun-22 06:30 flask_pydantic_api-0.9.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-22 06:30 flask_pydantic_api-0.9.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 23-Jun-22 06:30 flask_pydantic_api-0.9.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1056 b- defN 23-Jun-22 06:30 flask_pydantic_api-0.9.6.dist-info/RECORD
-12 files, 33057 bytes uncompressed, 11093 bytes compressed:  66.4%
+-rw-r--r--  2.0 unx     1073 b- defN 23-Jun-23 01:02 flask_pydantic_api-0.9.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx    12062 b- defN 23-Jun-23 01:02 flask_pydantic_api-0.9.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-23 01:02 flask_pydantic_api-0.9.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 23-Jun-23 01:02 flask_pydantic_api-0.9.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1056 b- defN 23-Jun-23 01:02 flask_pydantic_api-0.9.7.dist-info/RECORD
+12 files, 33441 bytes uncompressed, 11103 bytes compressed:  66.8%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: flask_pydantic_api/utils.py
 Comment: 
 
 Filename: flask_pydantic_api/templates/rapidoc.html
 Comment: 
 
-Filename: flask_pydantic_api-0.9.6.dist-info/LICENSE
+Filename: flask_pydantic_api-0.9.7.dist-info/LICENSE
 Comment: 
 
-Filename: flask_pydantic_api-0.9.6.dist-info/METADATA
+Filename: flask_pydantic_api-0.9.7.dist-info/METADATA
 Comment: 
 
-Filename: flask_pydantic_api-0.9.6.dist-info/WHEEL
+Filename: flask_pydantic_api-0.9.7.dist-info/WHEEL
 Comment: 
 
-Filename: flask_pydantic_api-0.9.6.dist-info/top_level.txt
+Filename: flask_pydantic_api-0.9.7.dist-info/top_level.txt
 Comment: 
 
-Filename: flask_pydantic_api-0.9.6.dist-info/RECORD
+Filename: flask_pydantic_api-0.9.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## flask_pydantic_api/api_wrapper.py

```diff
@@ -1,13 +1,12 @@
 import asyncio
 from functools import wraps
 from itertools import chain
 from typing import Any, Callable, Dict, List, Optional, Tuple, Type, Union
 
-from asgiref.sync import async_to_sync
 from flask import abort, current_app, jsonify, make_response, request
 from pydantic import BaseModel, ValidationError
 from pydantic.tools import parse_obj_as
 
 from .utils import get_annotated_models, model_has_uploaded_file_type
 
 augment_schema_with_fieldsets: Optional[Callable] = None
@@ -101,89 +100,96 @@
     def wrap(view_func: Callable) -> Callable:
         request_model_param_name, request_model, response_models = get_annotated_models(
             view_func
         )
 
         @wraps(view_func)
         def wrapped_endpoint(*args: Any, **kwargs: Any) -> Callable:
-            body, kwargs = (
-                get_request_args(
-                    for_model=request_model,
-                    view_kwargs=kwargs,
-                    merge_path_parameters=merge_path_parameters,
-                )
-                or None
-            )
-            fieldsets: List[str] = []
-
-            # Pydantic validation and casting of inputs
+            event_loop = asyncio.new_event_loop()
             try:
-                # fieldsets for pydantic_enhanced_serializer
-                if (
-                    body
-                    and render_fieldset_model
-                    and request_fields_name
-                    and request_fields_name in body
-                ):
-                    fieldsets = body.pop(request_fields_name, [])
-                    try:
-                        parse_obj_as(Union[str, List[str]], fieldsets)  # type: ignore
-                    except ValidationError as e:
-                        for error in e.errors():
-                            if error["loc"][0] == "__root__":
-                                error["loc"] = tuple(
-                                    [request_fields_name, *error["loc"][1:]]
-                                )
-                        raise
-
-                # api input model
-                if request_model and request_model_param_name:
-                    kwargs[request_model_param_name] = request_model(**body or {})
-
-            except ValidationError as e:
-                if current_app.config.get("FLASK_PYDANTIC_API_RENDER_ERRORS", False):
-                    response = jsonify({"errors": e.errors()})
-                    response.status_code = current_app.config.get(
-                        "FLASK_PYDANTIC_API_ERROR_STATUS_CODE", 400
+                body, kwargs = (
+                    get_request_args(
+                        for_model=request_model,
+                        view_kwargs=kwargs,
+                        merge_path_parameters=merge_path_parameters,
                     )
-                    return response
+                    or None
+                )
+                fieldsets: List[str] = []
 
-                raise
+                # Pydantic validation and casting of inputs
+                try:
+                    # fieldsets for pydantic_enhanced_serializer
+                    if (
+                        body
+                        and render_fieldset_model
+                        and request_fields_name
+                        and request_fields_name in body
+                    ):
+                        fieldsets = body.pop(request_fields_name, [])
+                        try:
+                            parse_obj_as(Union[str, List[str]], fieldsets)  # type: ignore
+                        except ValidationError as e:
+                            for error in e.errors():
+                                if error["loc"][0] == "__root__":
+                                    error["loc"] = tuple(
+                                        [request_fields_name, *error["loc"][1:]]
+                                    )
+                            raise
+
+                    # api input model
+                    if request_model and request_model_param_name:
+                        kwargs[request_model_param_name] = request_model(**body or {})
+
+                except ValidationError as e:
+                    if current_app.config.get(
+                        "FLASK_PYDANTIC_API_RENDER_ERRORS", False
+                    ):
+                        response = jsonify({"errors": e.errors()})
+                        response.status_code = current_app.config.get(
+                            "FLASK_PYDANTIC_API_ERROR_STATUS_CODE", 400
+                        )
+                        return response
 
-            try:
-                if asyncio.iscoroutinefunction(view_func):
-                    result = async_to_sync(view_func)(*args, **kwargs)
-                else:
-                    result = view_func(*args, **kwargs)
-
-                if response_models and isinstance(result, dict):
-                    result = response_models[0](**result)
-
-                if isinstance(result, BaseModel):
-                    if render_fieldset_model:
-                        loop = asyncio.get_event_loop()
-                        result_data = loop.run_until_complete(
-                            render_fieldset_model(
-                                model=result,
-                                fieldsets=fieldsets,
-                                maximum_expansion_depth=maximum_expansion_depth,
-                                raise_error_on_expansion_not_found=False,
-                            )
+                    raise
+
+                try:
+                    if asyncio.iscoroutinefunction(view_func):
+                        result: Any = event_loop.run_until_complete(
+                            view_func(*args, **kwargs)
                         )
                     else:
-                        result_data = result.dict()
+                        result = view_func(*args, **kwargs)
 
-                    result = make_response(result_data, success_status_code)
+                    if response_models and isinstance(result, dict):
+                        result = response_models[0](**result)
 
-            except ValidationError as e:
-                raise Exception(
-                    "pydantic model error on api response serialization; "
-                    f"endpoint: {request.endpoint}; "
-                    f"error: {str(e)}"
-                )
+                    if isinstance(result, BaseModel):
+                        if render_fieldset_model:
+                            result_data = event_loop.run_until_complete(
+                                render_fieldset_model(
+                                    model=result,
+                                    fieldsets=fieldsets,
+                                    maximum_expansion_depth=maximum_expansion_depth,
+                                    raise_error_on_expansion_not_found=False,
+                                )
+                            )
+                        else:
+                            result_data = result.dict()
+
+                        result = make_response(result_data, success_status_code)
+
+                except ValidationError as e:
+                    raise Exception(
+                        "pydantic model error on api response serialization; "
+                        f"endpoint: {request.endpoint}; "
+                        f"error: {str(e)}"
+                    )
+            finally:
+                event_loop.close()
 
             return result
 
         augment_pydantic_enhanced_serializer_model_schemas(
             request_model, *(response_models or [])
         )
```

## Comparing `flask_pydantic_api-0.9.6.dist-info/LICENSE` & `flask_pydantic_api-0.9.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `flask_pydantic_api-0.9.6.dist-info/METADATA` & `flask_pydantic_api-0.9.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-pydantic-api
-Version: 0.9.6
+Version: 0.9.7
 Summary: Pydantic based API support for Flask
 Home-page: https://github.com/adamsussman/flask-pydantic-api
 Author: Adam Sussman
 Author-email: adam.sussman@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pydantic
@@ -13,15 +13,14 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Internet
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: asgiref (>=3.6)
 Requires-Dist: flask (>=2.2)
 Requires-Dist: pydantic (>=1.8)
 Requires-Dist: openapi-schema-pydantic (>=1.2)
 Provides-Extra: dev
 Requires-Dist: mypy ; extra == 'dev'
 Requires-Dist: black ; extra == 'dev'
 Requires-Dist: ipdb ; extra == 'dev'
```

## Comparing `flask_pydantic_api-0.9.6.dist-info/RECORD` & `flask_pydantic_api-0.9.7.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 flask_pydantic_api/__init__.py,sha256=KICwgGx_FRhKuNBAcoy1GHBo9C4Jn0QUEwChlmdGS18,98
-flask_pydantic_api/api_wrapper.py,sha256=Iy61agmROlazyFcrUo4WacVGM1zativTF8GdoMwACq4,7285
+flask_pydantic_api/api_wrapper.py,sha256=JKUeOYT-Y30NR1KCoF6YVScc6KEf-EsdKw0CGqDqCos,7700
 flask_pydantic_api/apidocs_views.py,sha256=sSsr1zVE35UtVPHH0on6HRoZO1vYO1xXRMETq4Fcp1U,819
 flask_pydantic_api/openapi.py,sha256=7kTBYCDQ10F-wwggoiZQtTKEs3vEXudXkZOeDMxamO8,7733
 flask_pydantic_api/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 flask_pydantic_api/utils.py,sha256=mQ-33XUZ_VOHjSgxv2hCyAIIeOCZnCeemRsyDW6D-ng,2342
 flask_pydantic_api/templates/rapidoc.html,sha256=VLYAdPmRJ7dVQmpLmykMUA8KsVEF77tP-Xo2mbBHbBw,447
-flask_pydantic_api-0.9.6.dist-info/LICENSE,sha256=INaSDKc7Y-fYndT1E_X93xe_8Ez3nkemMNtk3TaFH9c,1073
-flask_pydantic_api-0.9.6.dist-info/METADATA,sha256=jHoW-THbI8uWqNooikzE-Ph9fsURfBiACFinHOd_wxM,12093
-flask_pydantic_api-0.9.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-flask_pydantic_api-0.9.6.dist-info/top_level.txt,sha256=lFmuWAb1KRWKxzT1wPHWpS8eUwnDY1WPWAzqkUDVlU4,19
-flask_pydantic_api-0.9.6.dist-info/RECORD,,
+flask_pydantic_api-0.9.7.dist-info/LICENSE,sha256=INaSDKc7Y-fYndT1E_X93xe_8Ez3nkemMNtk3TaFH9c,1073
+flask_pydantic_api-0.9.7.dist-info/METADATA,sha256=sJCPIUS1MRQFexA19hrUswPs-k9UNUMSB3aTMYwyPCo,12062
+flask_pydantic_api-0.9.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+flask_pydantic_api-0.9.7.dist-info/top_level.txt,sha256=lFmuWAb1KRWKxzT1wPHWpS8eUwnDY1WPWAzqkUDVlU4,19
+flask_pydantic_api-0.9.7.dist-info/RECORD,,
```


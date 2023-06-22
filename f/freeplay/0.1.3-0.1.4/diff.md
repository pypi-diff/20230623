# Comparing `tmp/freeplay-0.1.3.tar.gz` & `tmp/freeplay-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeplay-0.1.3.tar", max compression
+gzip compressed data, was "freeplay-0.1.4.tar", max compression
```

## Comparing `freeplay-0.1.3.tar` & `freeplay-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2023-05-18 13:19:32.515553 freeplay-0.1.3/README.md
--rw-r--r--   0        0        0       62 2023-05-18 23:25:20.631072 freeplay-0.1.3/freeplay/__init__.py
--rw-r--r--   0        0        0     1834 2023-06-09 01:58:55.719111 freeplay-0.1.3/freeplay/api_support.py
--rw-r--r--   0        0        0      188 2023-06-15 16:32:13.004072 freeplay-0.1.3/freeplay/errors.py
--rw-r--r--   0        0        0     3107 2023-05-26 16:05:17.190253 freeplay-0.1.3/freeplay/freeplay.py
--rw-r--r--   0        0        0    16543 2023-06-16 16:10:27.584703 freeplay-0.1.3/freeplay/freeplay_encapsulated.py
--rw-r--r--   0        0        0      391 2023-06-20 19:15:43.760617 freeplay-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 freeplay-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-15 03:23:13.376261 freeplay-0.1.4/README.md
+-rw-r--r--   0        0        0       62 2023-05-30 19:38:09.617870 freeplay-0.1.4/freeplay/__init__.py
+-rw-r--r--   0        0        0     1834 2023-06-08 17:54:13.585930 freeplay-0.1.4/freeplay/api_support.py
+-rw-r--r--   0        0        0      188 2023-06-15 15:26:56.089064 freeplay-0.1.4/freeplay/errors.py
+-rw-r--r--   0        0        0     3107 2023-06-21 16:31:59.846196 freeplay-0.1.4/freeplay/freeplay.py
+-rw-r--r--   0        0        0    19252 2023-06-22 20:50:42.558516 freeplay-0.1.4/freeplay/freeplay_encapsulated.py
+-rw-r--r--   0        0        0      391 2023-06-22 20:46:25.284996 freeplay-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 freeplay-0.1.4/PKG-INFO
```

### Comparing `freeplay-0.1.3/freeplay/api_support.py` & `freeplay-0.1.4/freeplay/api_support.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.1.3/freeplay/freeplay.py` & `freeplay-0.1.4/freeplay/freeplay.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.1.3/freeplay/freeplay_encapsulated.py` & `freeplay-0.1.4/freeplay/freeplay_encapsulated.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 
 from . import api_support
 from .errors import TemplateNotFoundError, APIKeyMissingError, AuthorizationError, FreeplayError
 
 JsonDom = dict[str, Any]
 
 logger = logging.getLogger(__name__)
+default_tag = 'latest'
+
 
 @dataclass
 class CompletionResponse:
     content: str
     is_complete: bool
 
 
@@ -239,39 +241,43 @@
             **kwargs: str
     ) -> None:
         self.api_base = api_base
         self.freeplay_api_key = freeplay_api_key
         self.flavor = flavor
         self.extra_init_args = kwargs
 
-    def create_session(self, project_id: str) -> JsonDom:
+    def create_session(self, project_id: str, tag: str, test_run_id: Optional[str] = None) -> JsonDom:
+        request_body = {'test_run_id': test_run_id} if test_run_id is not None else None
         response = api_support.post_raw(api_key=self.freeplay_api_key,
-                                        url=f'{self.api_base}/projects/{project_id}/sessions/tag/latest')
+                                        url=f'{self.api_base}/projects/{project_id}/sessions/tag/{tag}',
+                                        payload=request_body)
 
         if response.status_code == 201:
             return cast(dict[str, Any], json.loads(response.content))
         elif response.status_code == 401:
             raise AuthorizationError()
         else:
             raise FreeplayError(f'Unknown response while creating a session. Response code: {response.status_code}')
 
-    def get_prompts(self, project_id: str) -> PromptTemplates:
+    def get_prompts(self, project_id: str, tag: str) -> PromptTemplates:
         prompts = api_support.get(
             target_type=PromptTemplates,
             api_key=self.freeplay_api_key,
-            url=f'{self.api_base}/projects/{project_id}/templates/all/latest'
+            url=f'{self.api_base}/projects/{project_id}/templates/all/{tag}'
         )
         return prompts
 
     def prepare_and_make_call(
             self,
             session_id: str,
             prompts: PromptTemplates,
             template_name: str,
-            variables: dict[str, str]
+            variables: dict[str, str],
+            tag: str,
+            test_run_id: Optional[str] = None
     ) -> Optional[CompletionResponse]:
         # format prompt
         templates = [t for t in prompts.templates if t.name == template_name]
         if len(templates) == 0:
             raise TemplateNotFoundError(f'Could not find template with name "{template_name}"')
         target_template = templates[0]
         formatted_prompt = self.flavor.format(target_template, variables)
@@ -292,24 +298,29 @@
             return_content,
             is_complete,
             end,
             formatted_prompt,
             session_id,
             start,
             target_template,
-            variables)
+            variables,
+            tag,
+            test_run_id
+        )
 
         return completion_response
 
     def prepare_and_make_call_stream(
             self,
             session_id: str,
             prompts: PromptTemplates,
             template_name: str,
-            variables: dict[str, str]
+            variables: dict[str, str],
+            tag: str,
+            test_run_id: Optional[str] = None
     ) -> Generator[CompletionChunk, None, None]:
         # format prompt
         templates = [t for t in prompts.templates if t.name == template_name]
         if len(templates) == 0:
             raise TemplateNotFoundError(f'Could not find template with name "{template_name}"')
         target_template = templates[0]
         formatted_prompt = self.flavor.format(target_template, variables)
@@ -329,128 +340,184 @@
         self.__record_call(''.join(text_chunks),
                            last_is_complete,
                            end,
                            formatted_prompt,
                            session_id,
                            start,
                            target_template,
-                           variables)
+                           variables,
+                           tag,
+                           test_run_id)
 
     def __record_call(
             self,
             completion_content: str,
             completion_is_complete: bool,
             end: int,
             formatted_prompt: str,
             session_id: str,
             start: int,
             target_template: PromptTemplateWithMetadata,
-            variables: dict[str, str]
+            variables: dict[str, str],
+            tag: str,
+            test_run_id: Optional[str]
     ) -> None:
 
         record_payload = {
             "session_id": session_id,
             "project_version_id": target_template.project_version_id,
             "prompt_template_id": target_template.prompt_template_id,
             "start_time": start,
             "end_time": end,
-            "tag": "",
+            "tag": tag,
             "inputs": variables,
             "prompt_content": formatted_prompt,
             "return_content": completion_content,
             "format_type": self.flavor.record_format_type,
             "is_complete": completion_is_complete
         }
 
+        if test_run_id is not None:
+            record_payload['test_run_id'] = test_run_id
+
         try:
-            _recorded_response = api_support.post_raw(
+            recorded_response = api_support.post_raw(
                 api_key=self.freeplay_api_key,
                 url=f'{self.api_base}/v1/record',
                 payload=record_payload
             )
-        except Exception:
-            logger.warning(f'There was an error recording to FreePlay. Session will not be logged.')
+            recorded_response.raise_for_status()
+        except Exception as e:
+            status_code = -1
+            if hasattr(e, 'response') and hasattr(e.response, 'status_code'):
+                status_code = e.response.status_code
+            logger.warning(f'There was an error recording to Freeplay. Call will not be logged. '
+                           f'Status: {status_code}. {e.__class__}')
 
 
 class Session:
     def __init__(
             self,
             call_support: CallSupport,
             session_id: str,
-            prompts: PromptTemplates
+            prompts: PromptTemplates,
+            tag: str = default_tag,
+            test_run_id: Optional[str] = None
     ) -> None:
+        self.tag = tag
         self.call_support = call_support
         self.session_id = session_id
         self.prompts = prompts
+        self.test_run_id = test_run_id
 
     def get_completion(
             self,
             template_name: str,
             variables: dict[str, str]
     ) -> Optional[CompletionResponse]:
         return self.call_support.prepare_and_make_call(self.session_id,
                                                        self.prompts,
                                                        template_name,
-                                                       variables)
+                                                       variables,
+                                                       self.tag,
+                                                       self.test_run_id)
 
     def get_completion_stream(
             self,
             template_name: str,
             variables: dict[str, str]
     ) -> Generator[CompletionChunk, None, None]:
         return self.call_support.prepare_and_make_call_stream(self.session_id,
                                                               self.prompts,
                                                               template_name,
-                                                              variables)
+                                                              variables,
+                                                              self.tag,
+                                                              self.test_run_id)
+
+
+@dataclass()
+class FreeplayTestRun:
+    def __init__(
+            self,
+            call_support: CallSupport,
+            test_run_id: str,
+            inputs: list[dict[str, str]]
+    ):
+        self.call_support = call_support
+        self.test_run_id = test_run_id
+        self.inputs = inputs
+
+    def get_inputs(self) -> list[dict[str, str]]:
+        return self.inputs
+
+    def create_session(self, project_id: str, tag: str = default_tag) -> Session:
+        project_session = self.call_support.create_session(project_id, tag, self.test_run_id)
+        prompts = self.call_support.get_prompts(project_id, tag)
+        return Session(self.call_support, project_session['session_id'], prompts, tag, self.test_run_id)
 
 
 # This SDK prototype does not support full functionality of either OpenAI's API or Freeplay's
 # The simplifications are:
 #  - Always assumes there is a single choice returned, does not support multiple
-#  - Always uses the 'latest' tag for project versions. Doesn't support configurable tags
-#  - Does not support recording a tag from a call
 #  - Does not support an "escape hatch" to allow use of features we don't explicitly expose
 class Freeplay:
     def __init__(
             self,
             flavor: Flavor,
             freeplay_api_key: str,
             api_base: str,
             **kwargs: str
     ) -> None:
         if not freeplay_api_key or not freeplay_api_key.strip():
             raise APIKeyMissingError("Freeplay API key not set. It must be set to the Freeplay API.")
 
         self.call_support = CallSupport(flavor, freeplay_api_key, api_base, **kwargs)
+        self.freeplay_api_key = freeplay_api_key
+        self.api_base = api_base
 
-    def create_session(self, project_id: str) -> Session:
-        project_session = self.call_support.create_session(project_id)
-        prompts = self.call_support.get_prompts(project_id)
-        return Session(self.call_support, project_session['session_id'], prompts)
+    def create_session(self, project_id: str, tag: str = default_tag) -> Session:
+        project_session = self.call_support.create_session(project_id, tag)
+        prompts = self.call_support.get_prompts(project_id, tag)
+        return Session(self.call_support, project_session['session_id'], prompts, tag)
 
     def get_completion(
             self,
             project_id: str,
             template_name: str,
-            variables: dict[str, str]
+            variables: dict[str, str],
+            tag: str = default_tag
     ) -> Optional[CompletionResponse]:
-        project_session = self.call_support.create_session(project_id)
-        prompts = self.call_support.get_prompts(project_id)
+        project_session = self.call_support.create_session(project_id, tag)
+        prompts = self.call_support.get_prompts(project_id, tag)
 
         return self.call_support.prepare_and_make_call(project_session['session_id'],
                                                        prompts,
                                                        template_name,
-                                                       variables)
+                                                       variables,
+                                                       tag)
 
     def get_completion_stream(
             self,
             project_id: str,
             template_name: str,
-            variables: dict[str, str]
+            variables: dict[str, str],
+            tag: str = default_tag
     ) -> Generator[CompletionChunk, None, None]:
-        project_session = self.call_support.create_session(project_id)
-        prompts = self.call_support.get_prompts(project_id)
+        project_session = self.call_support.create_session(project_id, tag)
+        prompts = self.call_support.get_prompts(project_id, tag)
 
         return self.call_support.prepare_and_make_call_stream(project_session['session_id'],
                                                               prompts,
                                                               template_name,
-                                                              variables)
+                                                              variables,
+                                                              tag)
+
+    def create_test_run(self, project_id: str, playlist: str) -> FreeplayTestRun:
+        response = api_support.post_raw(
+            api_key=self.freeplay_api_key,
+            url=f'{self.api_base}/projects/{project_id}/test-runs',
+            payload={'playlist_name': playlist},
+        )
+
+        json_dom = response.json()
+
+        return FreeplayTestRun(self.call_support, json_dom['test_run_id'], json_dom['inputs'])
```

### Comparing `freeplay-0.1.3/PKG-INFO` & `freeplay-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeplay
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 License: MIT
 Author: FreePlay Engineering
 Author-email: engineering@freeplay.ai
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


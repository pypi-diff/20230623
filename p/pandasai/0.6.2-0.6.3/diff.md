# Comparing `tmp/pandasai-0.6.2.tar.gz` & `tmp/pandasai-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasai-0.6.2.tar", max compression
+gzip compressed data, was "pandasai-0.6.3.tar", max compression
```

## Comparing `pandasai-0.6.2.tar` & `pandasai-0.6.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1055 2023-06-19 23:45:08.536893 pandasai-0.6.2/LICENSE
--rw-r--r--   0        0        0     7705 2023-06-19 23:45:08.536893 pandasai-0.6.2/README.md
--rw-r--r--   0        0        0    23288 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/__init__.py
--rw-r--r--   0        0        0     1440 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/constants.py
--rw-r--r--   0        0        0     1509 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     3814 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/helpers/_optional.py
--rw-r--r--   0        0        0     5434 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1742 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/helpers/cache.py
--rw-r--r--   0        0        0      566 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     1493 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     3252 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0     4369 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/helpers/shortcuts.py
--rw-r--r--   0        0        0        0 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     4354 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    10885 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/llm/base.py
--rw-r--r--   0        0        0      542 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1213 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/llm/falcon.py
--rw-r--r--   0        0        0     1828 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0      577 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/llm/langchain.py
--rw-r--r--   0        0        0     1482 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     2932 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/llm/openai.py
--rw-r--r--   0        0        0     1220 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0        0 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/middlewares/__init__.py
--rw-r--r--   0        0        0      663 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/middlewares/base.py
--rw-r--r--   0        0        0      558 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/middlewares/charts.py
--rw-r--r--   0        0        0      653 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/middlewares/streamlit.py
--rw-r--r--   0        0        0        0 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0      647 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1697 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1262 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1514 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      460 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1343 2023-06-19 23:45:08.544894 pandasai-0.6.2/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     1712 2023-06-19 23:45:08.544894 pandasai-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     8807 1970-01-01 00:00:00.000000 pandasai-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-06-23 13:57:34.498989 pandasai-0.6.3/LICENSE
+-rw-r--r--   0        0        0     7705 2023-06-23 13:57:34.498989 pandasai-0.6.3/README.md
+-rw-r--r--   0        0        0    24332 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/__init__.py
+-rw-r--r--   0        0        0     1440 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/constants.py
+-rw-r--r--   0        0        0     1509 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     3814 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/helpers/_optional.py
+-rw-r--r--   0        0        0     5434 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1742 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0      566 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     1493 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     3252 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0     4369 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/helpers/shortcuts.py
+-rw-r--r--   0        0        0        0 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     4119 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    10885 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/llm/base.py
+-rw-r--r--   0        0        0      542 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1213 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/llm/falcon.py
+-rw-r--r--   0        0        0     1828 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0      577 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/llm/langchain.py
+-rw-r--r--   0        0        0     1482 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     2932 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/llm/openai.py
+-rw-r--r--   0        0        0     1220 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0        0 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/middlewares/__init__.py
+-rw-r--r--   0        0        0      663 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/middlewares/base.py
+-rw-r--r--   0        0        0      558 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/middlewares/charts.py
+-rw-r--r--   0        0        0      653 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/middlewares/streamlit.py
+-rw-r--r--   0        0        0        0 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0      647 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1697 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1262 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1514 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      460 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1343 2023-06-23 13:57:34.506990 pandasai-0.6.3/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     1712 2023-06-23 13:57:34.510990 pandasai-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     8807 1970-01-01 00:00:00.000000 pandasai-0.6.3/PKG-INFO
```

### Comparing `pandasai-0.6.2/LICENSE` & `pandasai-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.2/README.md` & `pandasai-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.2/pandasai/__init__.py` & `pandasai-0.6.3/pandasai/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 import io
 import logging
 import re
 import sys
 import uuid
 import time
 from contextlib import redirect_stdout
-from typing import List, Optional, Union
+from typing import List, Optional, Union, Dict, Type
 
 import astor
 import pandas as pd
 from .constants import (
     WHITELISTED_BUILTINS,
     WHITELISTED_LIBRARIES,
 )
@@ -56,14 +56,15 @@
 from .helpers.notebook import Notebook
 from .helpers.save_chart import add_save_chart
 from .helpers.shortcuts import Shortcuts
 from .llm.base import LLM
 from .llm.langchain import LangchainLLM
 from .middlewares.base import Middleware
 from .middlewares.charts import ChartsMiddleware
+from .prompts.base import Prompt
 from .prompts.correct_error_prompt import CorrectErrorPrompt
 from .prompts.correct_multiples_prompt import CorrectMultipleDataframesErrorPrompt
 from .prompts.generate_python_code import GeneratePythonCodePrompt
 from .prompts.generate_response import GenerateResponsePrompt
 from .prompts.multiple_dataframes import MultipleDataframesPrompt
 
 
@@ -147,14 +148,15 @@
         verbose=False,
         enforce_privacy=False,
         save_charts=False,
         enable_cache=True,
         middlewares=None,
         custom_whitelisted_dependencies=None,
         enable_logging=True,
+        non_default_prompts: Optional[Dict[str, Type[Prompt]]] = None,
     ):
         """
 
         __init__ method of the Class PandasAI
 
         Args:
             llm (object): LLMs option to be used for API access. Default is None
@@ -168,14 +170,16 @@
             Default to False
             enable_cache (bool): Enable the cache to store the results.
             Default to True
             middlewares (list): List of middlewares to be used. Default to None
             custom_whitelisted_dependencies (list): List of custom dependencies to
             be used. Default to None
             enable_logging (bool): Enable the logging. Default to True
+            non_default_prompts (dict): Mapping from keys to replacement prompt classes.
+            Used to override specific types of prompts. Defaults to None.
         """
 
         # configure the logging
         # noinspection PyArgumentList
         # https://stackoverflow.com/questions/61226587/pycharm-does-not-recognize-logging-basicconfig-handlers-argument
         if enable_logging:
             handlers = [logging.FileHandler("pandasai.log")]
@@ -199,14 +203,18 @@
         self._load_llm(llm)
         self._is_conversational_answer = conversational
         self._verbose = verbose
         self._enforce_privacy = enforce_privacy
         self._save_charts = save_charts
         self._process_id = str(uuid.uuid4())
 
+        self._non_default_prompts = (
+            {} if non_default_prompts is None else non_default_prompts
+        )
+
         self.notebook = Notebook()
         self._in_notebook = self.notebook.in_notebook()
 
         self._enable_cache = enable_cache
         if self._enable_cache:
             self._cache = Cache()
 
@@ -249,16 +257,18 @@
         """
 
         if self._enforce_privacy:
             # we don't want to send potentially sensitive data to the LLM server
             # if the user has set enforce_privacy to True
             return answer
 
-        instruction = GenerateResponsePrompt(question=question, answer=answer)
-        return self._llm.call(instruction, "")
+        generate_response_instruction = self._non_default_prompts.get(
+            "generate_response", GenerateResponsePrompt
+        )(question=question, answer=answer)
+        return self._llm.call(generate_response_instruction, "")
 
     def run(
         self,
         data_frame: Union[pd.DataFrame, List[pd.DataFrame]],
         prompt: str,
         is_conversational_answer: bool = None,
         show_code: bool = False,
@@ -303,36 +313,42 @@
                     heads = [
                         anonymize_dataframe_head(dataframe)
                         if anonymize_df
                         else dataframe.head(rows_to_display)
                         for dataframe in data_frame
                     ]
 
+                    multiple_dataframes_instruction = self._non_default_prompts.get(
+                        "multiple_dataframes", MultipleDataframesPrompt
+                    )
                     code = self._llm.generate_code(
-                        MultipleDataframesPrompt(dataframes=heads),
+                        multiple_dataframes_instruction(dataframes=heads),
                         prompt,
                     )
 
                     self._original_instructions = {
                         "question": prompt,
                         "df_head": heads,
                     }
 
                 else:
                     df_head = data_frame.head(rows_to_display)
                     if anonymize_df:
                         df_head = anonymize_dataframe_head(df_head)
 
+                    generate_code_instruction = self._non_default_prompts.get(
+                        "generate_python_code", GeneratePythonCodePrompt
+                    )(
+                        prompt=prompt,
+                        df_head=df_head,
+                        num_rows=data_frame.shape[0],
+                        num_columns=data_frame.shape[1],
+                    )
                     code = self._llm.generate_code(
-                        GeneratePythonCodePrompt(
-                            prompt=prompt,
-                            df_head=df_head,
-                            num_rows=data_frame.shape[0],
-                            num_columns=data_frame.shape[1],
-                        ),
+                        generate_code_instruction,
                         prompt,
                     )
 
                     self._original_instructions = {
                         "question": prompt,
                         "df_head": df_head,
                         "num_rows": data_frame.shape[0],
@@ -545,22 +561,28 @@
             multiple (bool): A boolean to indicate if the code is for multiple
             dataframes
 
         Returns (str): A python code
         """
 
         if multiple:
-            error_correcting_instruction = CorrectMultipleDataframesErrorPrompt(
+            error_correcting_instruction = self._non_default_prompts.get(
+                "correct_multiple_dataframes_error",
+                CorrectMultipleDataframesErrorPrompt,
+            )(
                 code=code,
                 error_returned=e,
                 question=self._original_instructions["question"],
                 df_head=self._original_instructions["df_head"],
             )
+
         else:
-            error_correcting_instruction = CorrectErrorPrompt(
+            error_correcting_instruction = self._non_default_prompts.get(
+                "correct_error", CorrectErrorPrompt
+            )(
                 code=code,
                 error_returned=e,
                 question=self._original_instructions["question"],
                 df_head=self._original_instructions["df_head"],
                 num_rows=self._original_instructions["num_rows"],
                 num_columns=self._original_instructions["num_columns"],
             )
```

### Comparing `pandasai-0.6.2/pandasai/constants.py` & `pandasai-0.6.3/pandasai/constants.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.2/pandasai/exceptions.py` & `pandasai-0.6.3/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.2/pandasai/helpers/_optional.py` & `pandasai-0.6.3/pandasai/helpers/_optional.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.2/pandasai/helpers/anonymizer.py` & `pandasai-0.6.3/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.2/pandasai/helpers/cache.py` & `pandasai-0.6.3/pandasai/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.2/pandasai/helpers/from_excel.py` & `pandasai-0.6.3/pandasai/helpers/from_excel.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.2/pandasai/helpers/notebook.py` & `pandasai-0.6.3/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.2/pandasai/helpers/save_chart.py` & `pandasai-0.6.3/pandasai/helpers/save_chart.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.2/pandasai/helpers/shortcuts.py` & `pandasai-0.6.3/pandasai/helpers/shortcuts.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.2/pandasai/llm/azure_openai.py` & `pandasai-0.6.3/pandasai/llm/azure_openai.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,16 +12,14 @@
 """
 
 import os
 from typing import Any, Dict, Optional
 
 import openai
 from dotenv import load_dotenv
-from openai import InvalidRequestError
-from openai.error import APIConnectionError
 
 from ..exceptions import APIKeyNotFoundError, UnsupportedOpenAIModelError
 from .base import BaseOpenAI
 
 load_dotenv()
 
 
@@ -32,71 +30,66 @@
 
     api_base: str
     api_type: str = "azure"
     api_version: str
     engine: str
 
     def __init__(
-        self,
-        api_token: Optional[str] = None,
-        api_base: Optional[str] = None,
-        api_version: Optional[str] = None,
-        deployment_name: str = None,
-        **kwargs,
+            self,
+            api_token: Optional[str] = None,
+            api_base: Optional[str] = None,
+            api_version: Optional[str] = None,
+            deployment_name: str = None,
+            is_chat_model: Optional[bool] = False,
+            **kwargs,
     ):
         """
         __init__ method of AzureOpenAI Class
 
         Args:
             api_token (str): Azure OpenAI API token.
             api_base (str): Base url of the Azure endpoint.
                 It should look like the following:
                 <https://YOUR_RESOURCE_NAME.openai.azure.com/>
-            api_version (str): Version of the Azure OpenAI API. Be aware the API
-            version may change.
-            deployment_name: Custom name of the deployed model
+            api_version (str): Version of the Azure OpenAI API.
+                Be aware the API version may change.
+            deployment_name (str): Custom name of the deployed model
+            is_chat_model (bool): Whether ``deployment_name`` corresponds to a Chat
+                or a Completion model
             **kwargs: Inference Parameters
         """
 
-        self.api_token = api_token or os.getenv("AZURE_OPENAI_KEY") or None
-        self.api_base = api_base or os.getenv("AZURE_OPENAI_ENDPOINT") or None
-        self.api_version = api_version or "2023-03-15-preview"
+        self.api_token = api_token or os.getenv("OPENAI_API_KEY") or None
+        self.api_base = api_base or os.getenv("OPENAI_API_BASE") or None
+        self.api_version = api_version or os.getenv("OPENAI_API_VERSION")
         if self.api_token is None:
-            raise APIKeyNotFoundError("Azure OpenAI key is required")
+            raise APIKeyNotFoundError(
+                "Azure OpenAI key is required. Please add an environment variable "
+                "`OPENAI_API_KEY` or pass `api_token` as a named parameter"
+            )
         if self.api_base is None:
-            raise APIKeyNotFoundError("Azure OpenAI base endpoint is required")
-
+            raise APIKeyNotFoundError(
+                "Azure OpenAI base is required. Please add an environment variable "
+                "`OPENAI_API_BASE` or pass `api_base` as a named parameter"
+            )
+        if self.api_version is None:
+            raise APIKeyNotFoundError(
+                "Azure OpenAI version is required. Please add an environment variable "
+                "`OPENAI_API_VERSION` or pass `api_version` as a named parameter"
+            )
         openai.api_key = self.api_token
         openai.api_base = self.api_base
         openai.api_version = self.api_version
         openai.api_type = self.api_type
 
         if deployment_name is None:
             raise UnsupportedOpenAIModelError("Model deployment name is required.")
-        try:
-            model_name = openai.Deployment.retrieve(deployment_name).model
-            model_capabilities = openai.Model.retrieve(model_name).capabilities
-            if (
-                not model_capabilities.completion
-                and not model_capabilities.chat_completion
-            ):
-                raise UnsupportedOpenAIModelError(
-                    "Model deployment name does not correspond to a "
-                    "chat nor a completion model."
-                )
-            self.is_chat_model = model_capabilities.chat_completion
-            self.engine = deployment_name
-        except InvalidRequestError as ex:
-            raise UnsupportedOpenAIModelError(
-                "Model deployment name does not correspond to a valid model entity."
-            ) from ex
-        except APIConnectionError as ex:
-            raise UnsupportedOpenAIModelError(
-                f"Invalid Azure OpenAI Base Endpoint {api_base}"
-            ) from ex
+
+        self.is_chat_model = is_chat_model
+        self.engine = deployment_name
 
         self._set_params(**kwargs)
 
     @property
     def _default_params(self) -> Dict[str, Any]:
         """Get the default parameters for calling OpenAI API
```

### Comparing `pandasai-0.6.2/pandasai/llm/base.py` & `pandasai-0.6.3/pandasai/llm/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.2/pandasai/llm/fake.py` & `pandasai-0.6.3/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.2/pandasai/llm/falcon.py` & `pandasai-0.6.3/pandasai/llm/falcon.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.2/pandasai/llm/google_palm.py` & `pandasai-0.6.3/pandasai/llm/google_palm.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.2/pandasai/llm/langchain.py` & `pandasai-0.6.3/pandasai/llm/langchain.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.2/pandasai/llm/open_assistant.py` & `pandasai-0.6.3/pandasai/llm/open_assistant.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.2/pandasai/llm/openai.py` & `pandasai-0.6.3/pandasai/llm/openai.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.2/pandasai/llm/starcoder.py` & `pandasai-0.6.3/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.2/pandasai/middlewares/base.py` & `pandasai-0.6.3/pandasai/middlewares/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.2/pandasai/middlewares/charts.py` & `pandasai-0.6.3/pandasai/middlewares/charts.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.2/pandasai/middlewares/streamlit.py` & `pandasai-0.6.3/pandasai/middlewares/streamlit.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.2/pandasai/prompts/base.py` & `pandasai-0.6.3/pandasai/prompts/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.2/pandasai/prompts/correct_error_prompt.py` & `pandasai-0.6.3/pandasai/prompts/correct_error_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.2/pandasai/prompts/correct_multiples_prompt.py` & `pandasai-0.6.3/pandasai/prompts/correct_multiples_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.2/pandasai/prompts/generate_python_code.py` & `pandasai-0.6.3/pandasai/prompts/generate_python_code.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.2/pandasai/prompts/multiple_dataframes.py` & `pandasai-0.6.3/pandasai/prompts/multiple_dataframes.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.6.2/pyproject.toml` & `pandasai-0.6.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pandasai"
-version = "0.6.2"
+version = "0.6.3"
 description = "Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational."
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 [tool.poetry.dependencies]
```

### Comparing `pandasai-0.6.2/PKG-INFO` & `pandasai-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasai
-Version: 0.6.2
+Version: 0.6.3
 Summary: Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational.
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```


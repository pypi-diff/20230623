# Comparing `tmp/prompton-0.0.5.tar.gz` & `tmp/prompton-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompton-0.0.5.tar", max compression
+gzip compressed data, was "prompton-0.0.7.tar", max compression
```

## Comparing `prompton-0.0.5.tar` & `prompton-0.0.7.tar`

### file list

```diff
@@ -1,67 +1,72 @@
--rw-r--r--   0        0        0      100 2023-06-12 11:15:10.410454 prompton-0.0.5/README.md
--rw-r--r--   0        0        0     2450 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/__init__.py
--rw-r--r--   0        0        0     2307 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/client.py
--rw-r--r--   0        0        0      348 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/core/__init__.py
--rw-r--r--   0        0        0      426 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      367 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/errors/__init__.py
--rw-r--r--   0        0        0      248 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/errors/bad_request_error.py
--rw-r--r--   0        0        0      246 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/errors/not_found_error.py
--rw-r--r--   0        0        0      250 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/errors/unauthorized_error.py
--rw-r--r--   0        0        0      257 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0      268 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/resources/authentication/__init__.py
--rw-r--r--   0        0        0     6099 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/resources/authentication/client.py
--rw-r--r--   0        0        0       65 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/resources/inferences/__init__.py
--rw-r--r--   0        0        0     9839 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/resources/inferences/client.py
--rw-r--r--   0        0        0       65 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/resources/orgs/__init__.py
--rw-r--r--   0        0        0    14702 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/resources/orgs/client.py
--rw-r--r--   0        0        0       65 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/resources/prompt_versions/__init__.py
--rw-r--r--   0        0        0    16684 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/resources/prompt_versions/client.py
--rw-r--r--   0        0        0       65 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/resources/prompts/__init__.py
--rw-r--r--   0        0        0    15828 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/resources/prompts/client.py
--rw-r--r--   0        0        0       65 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/resources/server_status/__init__.py
--rw-r--r--   0        0        0     2307 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/resources/server_status/client.py
--rw-r--r--   0        0        0       65 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/resources/users/__init__.py
--rw-r--r--   0        0        0    13165 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/resources/users/client.py
--rw-r--r--   0        0        0     3121 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/__init__.py
--rw-r--r--   0        0        0      900 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/api_status_response.py
--rw-r--r--   0        0        0      936 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/body_get_access_token_extended_token_post.py
--rw-r--r--   0        0        0     1274 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/chat_gpt_chat_completition_config.py
--rw-r--r--   0        0        0      152 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/chat_gpt_chat_completition_config_stop.py
--rw-r--r--   0        0        0     1458 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/chat_gpt_chat_completition_request.py
--rw-r--r--   0        0        0      153 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/chat_gpt_chat_completition_request_stop.py
--rw-r--r--   0        0        0     1012 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/chat_gpt_chat_completition_response.py
--rw-r--r--   0        0        0      856 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/chat_gpt_completition_choice.py
--rw-r--r--   0        0        0      843 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/chat_gpt_message.py
--rw-r--r--   0        0        0      666 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/chat_gpt_role.py
--rw-r--r--   0        0        0      809 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/chat_gpt_token_usage.py
--rw-r--r--   0        0        0      773 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/db_status.py
--rw-r--r--   0        0        0      843 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/http_validation_error.py
--rw-r--r--   0        0        0     2205 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/inference_create_by_prompt_id.py
--rw-r--r--   0        0        0     1805 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/inference_create_by_prompt_version_id.py
--rw-r--r--   0        0        0      813 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/inference_error.py
--rw-r--r--   0        0        0      926 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/inference_post_response.py
--rw-r--r--   0        0        0      293 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/inference_post_response_response.py
--rw-r--r--   0        0        0     2510 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/inference_read.py
--rw-r--r--   0        0        0      285 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/inference_read_response.py
--rw-r--r--   0        0        0      965 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/inference_request_data.py
--rw-r--r--   0        0        0     1229 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/inference_response_data.py
--rw-r--r--   0        0        0     1082 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/inference_response_error.py
--rw-r--r--   0        0        0     1049 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/inference_response_status.py
--rw-r--r--   0        0        0      330 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/new_inference_request.py
--rw-r--r--   0        0        0     1136 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/org_read.py
--rw-r--r--   0        0        0     1275 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/prompt_read.py
--rw-r--r--   0        0        0      507 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/prompt_status.py
--rw-r--r--   0        0        0      152 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/prompt_version_providers.py
--rw-r--r--   0        0        0     1810 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/prompt_version_read.py
--rw-r--r--   0        0        0      837 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/prompt_version_status.py
--rw-r--r--   0        0        0      767 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/token.py
--rw-r--r--   0        0        0     1327 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/user_read.py
--rw-r--r--   0        0        0      686 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/user_roles.py
--rw-r--r--   0        0        0      869 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/validation_error.py
--rw-r--r--   0        0        0      128 2023-06-18 17:10:00.000000 prompton-0.0.5/prompton/types/validation_error_loc_item.py
--rw-r--r--   0        0        0      450 2023-06-18 18:13:00.945912 prompton-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      721 1970-01-01 00:00:00.000000 prompton-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      100 2023-06-12 11:15:10.410454 prompton-0.0.7/README.md
+-rw-r--r--   0        0        0     2604 2023-06-23 10:41:42.511265 prompton-0.0.7/prompton/__init__.py
+-rw-r--r--   0        0        0     2572 2023-06-23 10:41:42.511532 prompton-0.0.7/prompton/client.py
+-rw-r--r--   0        0        0      348 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      426 2023-06-23 10:41:42.511776 prompton-0.0.7/prompton/errors/__init__.py
+-rw-r--r--   0        0        0      248 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/errors/bad_request_error.py
+-rw-r--r--   0        0        0      246 2023-06-23 10:41:42.511945 prompton-0.0.7/prompton/errors/conflict_error.py
+-rw-r--r--   0        0        0      246 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/errors/not_found_error.py
+-rw-r--r--   0        0        0      250 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      257 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0      292 2023-06-23 10:41:42.512166 prompton-0.0.7/prompton/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/resources/authentication/__init__.py
+-rw-r--r--   0        0        0     6099 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/resources/authentication/client.py
+-rw-r--r--   0        0        0       65 2023-06-23 10:41:42.512434 prompton-0.0.7/prompton/resources/feedbacks/__init__.py
+-rw-r--r--   0        0        0    11981 2023-06-23 10:41:42.512614 prompton-0.0.7/prompton/resources/feedbacks/client.py
+-rw-r--r--   0        0        0       65 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/resources/inferences/__init__.py
+-rw-r--r--   0        0        0     9839 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/resources/inferences/client.py
+-rw-r--r--   0        0        0       65 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/resources/orgs/__init__.py
+-rw-r--r--   0        0        0    14815 2023-06-23 10:41:42.512891 prompton-0.0.7/prompton/resources/orgs/client.py
+-rw-r--r--   0        0        0       65 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/resources/prompt_versions/__init__.py
+-rw-r--r--   0        0        0    16783 2023-06-23 10:41:42.513249 prompton-0.0.7/prompton/resources/prompt_versions/client.py
+-rw-r--r--   0        0        0       65 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/resources/prompts/__init__.py
+-rw-r--r--   0        0        0    15927 2023-06-23 10:41:42.513504 prompton-0.0.7/prompton/resources/prompts/client.py
+-rw-r--r--   0        0        0       65 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/resources/server_status/__init__.py
+-rw-r--r--   0        0        0     2307 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/resources/server_status/client.py
+-rw-r--r--   0        0        0       65 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/resources/users/__init__.py
+-rw-r--r--   0        0        0    13599 2023-06-23 10:41:42.513707 prompton-0.0.7/prompton/resources/users/client.py
+-rw-r--r--   0        0        0     3263 2023-06-23 10:41:42.513866 prompton-0.0.7/prompton/types/__init__.py
+-rw-r--r--   0        0        0      900 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/types/api_status_response.py
+-rw-r--r--   0        0        0      936 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/types/body_get_access_token_extended_token_post.py
+-rw-r--r--   0        0        0     1274 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/types/chat_gpt_chat_completition_config.py
+-rw-r--r--   0        0        0      152 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/types/chat_gpt_chat_completition_config_stop.py
+-rw-r--r--   0        0        0     1458 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/types/chat_gpt_chat_completition_request.py
+-rw-r--r--   0        0        0      153 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/types/chat_gpt_chat_completition_request_stop.py
+-rw-r--r--   0        0        0     1012 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/types/chat_gpt_chat_completition_response.py
+-rw-r--r--   0        0        0      856 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/types/chat_gpt_completition_choice.py
+-rw-r--r--   0        0        0      843 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/types/chat_gpt_message.py
+-rw-r--r--   0        0        0      666 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/types/chat_gpt_role.py
+-rw-r--r--   0        0        0      809 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/types/chat_gpt_token_usage.py
+-rw-r--r--   0        0        0      773 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/types/db_status.py
+-rw-r--r--   0        0        0      909 2023-06-23 10:41:42.513996 prompton-0.0.7/prompton/types/default_post_response.py
+-rw-r--r--   0        0        0     2068 2023-06-23 10:41:42.514129 prompton-0.0.7/prompton/types/feedback_read.py
+-rw-r--r--   0        0        0      843 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/types/http_validation_error.py
+-rw-r--r--   0        0        0     2205 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/types/inference_create_by_prompt_id.py
+-rw-r--r--   0        0        0     1805 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/types/inference_create_by_prompt_version_id.py
+-rw-r--r--   0        0        0      813 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/types/inference_error.py
+-rw-r--r--   0        0        0      926 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/types/inference_post_response.py
+-rw-r--r--   0        0        0      293 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/types/inference_post_response_response.py
+-rw-r--r--   0        0        0     2510 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/types/inference_read.py
+-rw-r--r--   0        0        0      285 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/types/inference_read_response.py
+-rw-r--r--   0        0        0      965 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/types/inference_request_data.py
+-rw-r--r--   0        0        0     1229 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/types/inference_response_data.py
+-rw-r--r--   0        0        0     1082 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/types/inference_response_error.py
+-rw-r--r--   0        0        0     1049 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/types/inference_response_status.py
+-rw-r--r--   0        0        0      330 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/types/new_inference_request.py
+-rw-r--r--   0        0        0     1136 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/types/org_read.py
+-rw-r--r--   0        0        0     1275 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/types/prompt_read.py
+-rw-r--r--   0        0        0      507 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/types/prompt_status.py
+-rw-r--r--   0        0        0      152 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/types/prompt_version_providers.py
+-rw-r--r--   0        0        0     1810 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/types/prompt_version_read.py
+-rw-r--r--   0        0        0      837 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/types/prompt_version_status.py
+-rw-r--r--   0        0        0      767 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/types/token.py
+-rw-r--r--   0        0        0     1327 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/types/user_read.py
+-rw-r--r--   0        0        0      686 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/types/user_roles.py
+-rw-r--r--   0        0        0      869 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/types/validation_error.py
+-rw-r--r--   0        0        0      128 2023-06-23 09:36:30.000000 prompton-0.0.7/prompton/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0      450 2023-06-23 10:51:46.761674 prompton-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      721 1970-01-01 00:00:00.000000 prompton-0.0.7/PKG-INFO
```

### Comparing `prompton-0.0.5/prompton/__init__.py` & `prompton-0.0.7/prompton/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
-from .errors import BadRequestError, NotFoundError, UnauthorizedError, UnprocessableEntityError
-from .resources import authentication, inferences, orgs, prompt_versions, prompts, server_status, users
+from .errors import BadRequestError, ConflictError, NotFoundError, UnauthorizedError, UnprocessableEntityError
+from .resources import authentication, feedbacks, inferences, orgs, prompt_versions, prompts, server_status, users
 from .types import (
     ApiStatusResponse,
     BodyGetAccessTokenExtendedTokenPost,
     ChatGptChatCompletitionConfig,
     ChatGptChatCompletitionConfigStop,
     ChatGptChatCompletitionRequest,
     ChatGptChatCompletitionRequestStop,
     ChatGptChatCompletitionResponse,
     ChatGptCompletitionChoice,
     ChatGptMessage,
     ChatGptRole,
     ChatGptTokenUsage,
     DbStatus,
+    DefaultPostResponse,
+    FeedbackRead,
     HttpValidationError,
     InferenceCreateByPromptId,
     InferenceCreateByPromptVersionId,
     InferenceError,
     InferencePostResponse,
     InferencePostResponseResponse,
     InferenceRead,
@@ -50,15 +52,18 @@
     "ChatGptChatCompletitionRequest",
     "ChatGptChatCompletitionRequestStop",
     "ChatGptChatCompletitionResponse",
     "ChatGptCompletitionChoice",
     "ChatGptMessage",
     "ChatGptRole",
     "ChatGptTokenUsage",
+    "ConflictError",
     "DbStatus",
+    "DefaultPostResponse",
+    "FeedbackRead",
     "HttpValidationError",
     "InferenceCreateByPromptId",
     "InferenceCreateByPromptVersionId",
     "InferenceError",
     "InferencePostResponse",
     "InferencePostResponseResponse",
     "InferenceRead",
@@ -79,14 +84,15 @@
     "UnauthorizedError",
     "UnprocessableEntityError",
     "UserRead",
     "UserRoles",
     "ValidationError",
     "ValidationErrorLocItem",
     "authentication",
+    "feedbacks",
     "inferences",
     "orgs",
     "prompt_versions",
     "prompts",
     "server_status",
     "users",
 ]
```

### Comparing `prompton-0.0.5/prompton/client.py` & `prompton-0.0.7/prompton/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import typing
 
 from .resources.authentication.client import AsyncAuthenticationClient, AuthenticationClient
+from .resources.feedbacks.client import AsyncFeedbacksClient, FeedbacksClient
 from .resources.inferences.client import AsyncInferencesClient, InferencesClient
 from .resources.orgs.client import AsyncOrgsClient, OrgsClient
 from .resources.prompt_versions.client import AsyncPromptVersionsClient, PromptVersionsClient
 from .resources.prompts.client import AsyncPromptsClient, PromptsClient
 from .resources.server_status.client import AsyncServerStatusClient, ServerStatusClient
 from .resources.users.client import AsyncUsersClient, UsersClient
 
@@ -18,20 +19,22 @@
         self.server_status = ServerStatusClient(environment=self._environment, token=self._token)
         self.authentication = AuthenticationClient(environment=self._environment, token=self._token)
         self.prompts = PromptsClient(environment=self._environment, token=self._token)
         self.prompt_versions = PromptVersionsClient(environment=self._environment, token=self._token)
         self.inferences = InferencesClient(environment=self._environment, token=self._token)
         self.orgs = OrgsClient(environment=self._environment, token=self._token)
         self.users = UsersClient(environment=self._environment, token=self._token)
+        self.feedbacks = FeedbacksClient(environment=self._environment, token=self._token)
 
 
 class AsyncPromptonApi:
     def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
         self._token = token
         self.server_status = AsyncServerStatusClient(environment=self._environment, token=self._token)
         self.authentication = AsyncAuthenticationClient(environment=self._environment, token=self._token)
         self.prompts = AsyncPromptsClient(environment=self._environment, token=self._token)
         self.prompt_versions = AsyncPromptVersionsClient(environment=self._environment, token=self._token)
         self.inferences = AsyncInferencesClient(environment=self._environment, token=self._token)
         self.orgs = AsyncOrgsClient(environment=self._environment, token=self._token)
         self.users = AsyncUsersClient(environment=self._environment, token=self._token)
+        self.feedbacks = AsyncFeedbacksClient(environment=self._environment, token=self._token)
```

### Comparing `prompton-0.0.5/prompton/core/datetime_utils.py` & `prompton-0.0.7/prompton/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.5/prompton/core/jsonable_encoder.py` & `prompton-0.0.7/prompton/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.5/prompton/resources/authentication/client.py` & `prompton-0.0.7/prompton/resources/authentication/client.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.5/prompton/resources/inferences/client.py` & `prompton-0.0.7/prompton/resources/inferences/client.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.5/prompton/resources/orgs/client.py` & `prompton-0.0.7/prompton/resources/orgs/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...errors.bad_request_error import BadRequestError
 from ...errors.not_found_error import NotFoundError
 from ...errors.unauthorized_error import UnauthorizedError
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
+from ...types.default_post_response import DefaultPostResponse
 from ...types.org_read import OrgRead
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class OrgsClient:
@@ -38,29 +39,29 @@
             return pydantic.parse_obj_as(typing.List[OrgRead], _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def add_org(self, *, name: str, access_keys: typing.Optional[typing.Dict[str, str]] = OMIT) -> typing.Any:
+    def add_org(self, *, name: str, access_keys: typing.Optional[typing.Dict[str, str]] = OMIT) -> DefaultPostResponse:
         _request: typing.Dict[str, typing.Any] = {"name": name}
         if access_keys is not OMIT:
             _request["access_keys"] = access_keys
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment}/", "orgs"),
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(DefaultPostResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -172,30 +173,32 @@
             return pydantic.parse_obj_as(typing.List[OrgRead], _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def add_org(self, *, name: str, access_keys: typing.Optional[typing.Dict[str, str]] = OMIT) -> typing.Any:
+    async def add_org(
+        self, *, name: str, access_keys: typing.Optional[typing.Dict[str, str]] = OMIT
+    ) -> DefaultPostResponse:
         _request: typing.Dict[str, typing.Any] = {"name": name}
         if access_keys is not OMIT:
             _request["access_keys"] = access_keys
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment}/", "orgs"),
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(DefaultPostResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
```

### Comparing `prompton-0.0.5/prompton/resources/prompt_versions/client.py` & `prompton-0.0.7/prompton/resources/prompt_versions/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...errors.bad_request_error import BadRequestError
 from ...errors.not_found_error import NotFoundError
 from ...errors.unauthorized_error import UnauthorizedError
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
 from ...types.chat_gpt_chat_completition_config import ChatGptChatCompletitionConfig
 from ...types.chat_gpt_message import ChatGptMessage
+from ...types.default_post_response import DefaultPostResponse
 from ...types.prompt_version_providers import PromptVersionProviders
 from ...types.prompt_version_read import PromptVersionRead
 from ...types.prompt_version_status import PromptVersionStatus
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
@@ -61,15 +62,15 @@
         status: typing.Optional[PromptVersionStatus] = OMIT,
         provider: typing.Optional[PromptVersionProviders] = OMIT,
         name: str,
         description: typing.Optional[str] = OMIT,
         prompt_id: str,
         template: typing.Optional[typing.List[ChatGptMessage]] = OMIT,
         model_config: typing.Optional[ChatGptChatCompletitionConfig] = OMIT,
-    ) -> typing.Any:
+    ) -> DefaultPostResponse:
         _request: typing.Dict[str, typing.Any] = {"name": name, "prompt_id": prompt_id}
         if status is not OMIT:
             _request["status"] = status
         if provider is not OMIT:
             _request["provider"] = provider
         if description is not OMIT:
             _request["description"] = description
@@ -83,15 +84,15 @@
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(DefaultPostResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -218,15 +219,15 @@
         status: typing.Optional[PromptVersionStatus] = OMIT,
         provider: typing.Optional[PromptVersionProviders] = OMIT,
         name: str,
         description: typing.Optional[str] = OMIT,
         prompt_id: str,
         template: typing.Optional[typing.List[ChatGptMessage]] = OMIT,
         model_config: typing.Optional[ChatGptChatCompletitionConfig] = OMIT,
-    ) -> typing.Any:
+    ) -> DefaultPostResponse:
         _request: typing.Dict[str, typing.Any] = {"name": name, "prompt_id": prompt_id}
         if status is not OMIT:
             _request["status"] = status
         if provider is not OMIT:
             _request["provider"] = provider
         if description is not OMIT:
             _request["description"] = description
@@ -241,15 +242,15 @@
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(DefaultPostResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
```

### Comparing `prompton-0.0.5/prompton/resources/prompts/client.py` & `prompton-0.0.7/prompton/resources/prompts/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...errors.bad_request_error import BadRequestError
 from ...errors.not_found_error import NotFoundError
 from ...errors.unauthorized_error import UnauthorizedError
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
+from ...types.default_post_response import DefaultPostResponse
 from ...types.prompt_read import PromptRead
 from ...types.prompt_status import PromptStatus
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
@@ -49,15 +50,15 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def add_prompt(
         self, *, status: typing.Optional[PromptStatus] = OMIT, name: str, description: typing.Optional[str] = OMIT
-    ) -> typing.Any:
+    ) -> DefaultPostResponse:
         _request: typing.Dict[str, typing.Any] = {"name": name}
         if status is not OMIT:
             _request["status"] = status
         if description is not OMIT:
             _request["description"] = description
         _response = httpx.request(
             "POST",
@@ -65,15 +66,15 @@
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(DefaultPostResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
@@ -198,15 +199,15 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def add_prompt(
         self, *, status: typing.Optional[PromptStatus] = OMIT, name: str, description: typing.Optional[str] = OMIT
-    ) -> typing.Any:
+    ) -> DefaultPostResponse:
         _request: typing.Dict[str, typing.Any] = {"name": name}
         if status is not OMIT:
             _request["status"] = status
         if description is not OMIT:
             _request["description"] = description
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
@@ -215,15 +216,15 @@
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(DefaultPostResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
```

### Comparing `prompton-0.0.5/prompton/resources/server_status/client.py` & `prompton-0.0.7/prompton/resources/server_status/client.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.5/prompton/resources/users/client.py` & `prompton-0.0.7/prompton/resources/users/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,19 @@
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...errors.bad_request_error import BadRequestError
+from ...errors.conflict_error import ConflictError
 from ...errors.not_found_error import NotFoundError
 from ...errors.unauthorized_error import UnauthorizedError
 from ...errors.unprocessable_entity_error import UnprocessableEntityError
+from ...types.default_post_response import DefaultPostResponse
 from ...types.user_read import UserRead
 from ...types.user_roles import UserRoles
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
@@ -56,15 +58,15 @@
         *,
         full_name: typing.Optional[str] = OMIT,
         disabled: typing.Optional[bool] = OMIT,
         role: typing.Optional[UserRoles] = OMIT,
         org_id: str,
         email: str,
         plain_password: str,
-    ) -> typing.Any:
+    ) -> DefaultPostResponse:
         _request: typing.Dict[str, typing.Any] = {"org_id": org_id, "email": email, "plain_password": plain_password}
         if full_name is not OMIT:
             _request["full_name"] = full_name
         if disabled is not OMIT:
             _request["disabled"] = disabled
         if role is not OMIT:
             _request["role"] = role
@@ -74,19 +76,21 @@
             json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(DefaultPostResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+        if _response.status_code == 409:
+            raise ConflictError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
@@ -178,15 +182,15 @@
         *,
         full_name: typing.Optional[str] = OMIT,
         disabled: typing.Optional[bool] = OMIT,
         role: typing.Optional[UserRoles] = OMIT,
         org_id: str,
         email: str,
         plain_password: str,
-    ) -> typing.Any:
+    ) -> DefaultPostResponse:
         _request: typing.Dict[str, typing.Any] = {"org_id": org_id, "email": email, "plain_password": plain_password}
         if full_name is not OMIT:
             _request["full_name"] = full_name
         if disabled is not OMIT:
             _request["disabled"] = disabled
         if role is not OMIT:
             _request["role"] = role
@@ -197,19 +201,21 @@
                 json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(DefaultPostResponse, _response.json())  # type: ignore
         if _response.status_code == 400:
             raise BadRequestError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 401:
             raise UnauthorizedError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
+        if _response.status_code == 409:
+            raise ConflictError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(typing.Any, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `prompton-0.0.5/prompton/types/__init__.py` & `prompton-0.0.7/prompton/types/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from .chat_gpt_chat_completition_request_stop import ChatGptChatCompletitionRequestStop
 from .chat_gpt_chat_completition_response import ChatGptChatCompletitionResponse
 from .chat_gpt_completition_choice import ChatGptCompletitionChoice
 from .chat_gpt_message import ChatGptMessage
 from .chat_gpt_role import ChatGptRole
 from .chat_gpt_token_usage import ChatGptTokenUsage
 from .db_status import DbStatus
+from .default_post_response import DefaultPostResponse
+from .feedback_read import FeedbackRead
 from .http_validation_error import HttpValidationError
 from .inference_create_by_prompt_id import InferenceCreateByPromptId
 from .inference_create_by_prompt_version_id import InferenceCreateByPromptVersionId
 from .inference_error import InferenceError
 from .inference_post_response import InferencePostResponse
 from .inference_post_response_response import InferencePostResponseResponse
 from .inference_read import InferenceRead
@@ -46,14 +48,16 @@
     "ChatGptChatCompletitionRequestStop",
     "ChatGptChatCompletitionResponse",
     "ChatGptCompletitionChoice",
     "ChatGptMessage",
     "ChatGptRole",
     "ChatGptTokenUsage",
     "DbStatus",
+    "DefaultPostResponse",
+    "FeedbackRead",
     "HttpValidationError",
     "InferenceCreateByPromptId",
     "InferenceCreateByPromptVersionId",
     "InferenceError",
     "InferencePostResponse",
     "InferencePostResponseResponse",
     "InferenceRead",
```

### Comparing `prompton-0.0.5/prompton/types/api_status_response.py` & `prompton-0.0.7/prompton/types/api_status_response.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.5/prompton/types/body_get_access_token_extended_token_post.py` & `prompton-0.0.7/prompton/types/body_get_access_token_extended_token_post.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.5/prompton/types/chat_gpt_chat_completition_config.py` & `prompton-0.0.7/prompton/types/chat_gpt_chat_completition_config.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.5/prompton/types/chat_gpt_chat_completition_request.py` & `prompton-0.0.7/prompton/types/chat_gpt_chat_completition_request.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.5/prompton/types/chat_gpt_chat_completition_response.py` & `prompton-0.0.7/prompton/types/chat_gpt_chat_completition_response.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.5/prompton/types/chat_gpt_completition_choice.py` & `prompton-0.0.7/prompton/types/chat_gpt_completition_choice.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.5/prompton/types/chat_gpt_message.py` & `prompton-0.0.7/prompton/types/chat_gpt_message.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.5/prompton/types/chat_gpt_role.py` & `prompton-0.0.7/prompton/types/chat_gpt_role.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.5/prompton/types/chat_gpt_token_usage.py` & `prompton-0.0.7/prompton/types/chat_gpt_token_usage.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.5/prompton/types/db_status.py` & `prompton-0.0.7/prompton/types/db_status.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.5/prompton/types/http_validation_error.py` & `prompton-0.0.7/prompton/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.5/prompton/types/inference_create_by_prompt_id.py` & `prompton-0.0.7/prompton/types/inference_create_by_prompt_id.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.5/prompton/types/inference_create_by_prompt_version_id.py` & `prompton-0.0.7/prompton/types/inference_create_by_prompt_version_id.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.5/prompton/types/inference_error.py` & `prompton-0.0.7/prompton/types/inference_error.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.5/prompton/types/inference_post_response.py` & `prompton-0.0.7/prompton/types/inference_post_response.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.5/prompton/types/inference_read.py` & `prompton-0.0.7/prompton/types/inference_read.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.5/prompton/types/inference_request_data.py` & `prompton-0.0.7/prompton/types/inference_request_data.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.5/prompton/types/inference_response_data.py` & `prompton-0.0.7/prompton/types/inference_response_data.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.5/prompton/types/inference_response_error.py` & `prompton-0.0.7/prompton/types/inference_response_error.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.5/prompton/types/inference_response_status.py` & `prompton-0.0.7/prompton/types/inference_response_status.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.5/prompton/types/org_read.py` & `prompton-0.0.7/prompton/types/org_read.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.5/prompton/types/prompt_read.py` & `prompton-0.0.7/prompton/types/prompt_read.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.5/prompton/types/prompt_version_read.py` & `prompton-0.0.7/prompton/types/prompt_version_read.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.5/prompton/types/prompt_version_status.py` & `prompton-0.0.7/prompton/types/prompt_version_status.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.5/prompton/types/token.py` & `prompton-0.0.7/prompton/types/token.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.5/prompton/types/user_read.py` & `prompton-0.0.7/prompton/types/user_read.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.5/prompton/types/user_roles.py` & `prompton-0.0.7/prompton/types/user_roles.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.5/prompton/types/validation_error.py` & `prompton-0.0.7/prompton/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `prompton-0.0.5/PKG-INFO` & `prompton-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompton
-Version: 0.0.5
+Version: 0.0.7
 Summary: Chat prompt template evaluation and inference monitoring
 Author: PromptOn
 Author-email: hello@prompton.ai
 Requires-Python: >=3.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```


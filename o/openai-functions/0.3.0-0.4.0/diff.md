# Comparing `tmp/openai_functions-0.3.0.tar.gz` & `tmp/openai_functions-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_functions-0.3.0.tar", max compression
+gzip compressed data, was "openai_functions-0.4.0.tar", max compression
```

## Comparing `openai_functions-0.3.0.tar` & `openai_functions-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     2629 2023-06-23 20:50:25.777069 openai_functions-0.3.0/README.md
--rw-r--r--   0        0        0      308 2023-06-23 20:51:06.616455 openai_functions-0.3.0/openai_functions/__init__.py
--rw-r--r--   0        0        0     5596 2023-06-23 19:06:11.339113 openai_functions-0.3.0/openai_functions/function_wrapper.py
--rw-r--r--   0        0        0      160 2023-06-23 09:03:37.241129 openai_functions-0.3.0/openai_functions/json_type.py
--rw-r--r--   0        0        0     3372 2023-06-23 20:40:56.693784 openai_functions-0.3.0/openai_functions/openai_types.py
--rw-r--r--   0        0        0      156 2023-06-23 09:03:50.609263 openai_functions-0.3.0/openai_functions/parsers/__init__.py
--rw-r--r--   0        0        0     1668 2023-06-23 18:20:13.721023 openai_functions-0.3.0/openai_functions/parsers/abc.py
--rw-r--r--   0        0        0      977 2023-06-23 18:20:30.777150 openai_functions-0.3.0/openai_functions/parsers/atomic_type_parser.py
--rw-r--r--   0        0        0      201 2023-06-23 07:38:18.327910 openai_functions-0.3.0/openai_functions/parsers/bool_parser.py
--rw-r--r--   0        0        0     1641 2023-06-23 18:20:59.916367 openai_functions-0.3.0/openai_functions/parsers/dataclass_parser.py
--rw-r--r--   0        0        0      760 2023-06-23 13:05:10.173401 openai_functions-0.3.0/openai_functions/parsers/default.py
--rw-r--r--   0        0        0     1194 2023-06-23 18:21:17.923529 openai_functions-0.3.0/openai_functions/parsers/dict_parser.py
--rw-r--r--   0        0        0     1067 2023-06-23 18:21:23.392642 openai_functions-0.3.0/openai_functions/parsers/enum_parser.py
--rw-r--r--   0        0        0      205 2023-06-23 07:38:08.368818 openai_functions-0.3.0/openai_functions/parsers/float_parser.py
--rw-r--r--   0        0        0      640 2023-06-23 13:22:33.435179 openai_functions-0.3.0/openai_functions/parsers/int_parser.py
--rw-r--r--   0        0        0      993 2023-06-23 18:21:35.574892 openai_functions-0.3.0/openai_functions/parsers/list_parser.py
--rw-r--r--   0        0        0      691 2023-06-23 18:21:54.432274 openai_functions-0.3.0/openai_functions/parsers/none_parser.py
--rw-r--r--   0        0        0      204 2023-06-23 07:39:45.512719 openai_functions-0.3.0/openai_functions/parsers/str_parser.py
--rw-r--r--   0        0        0     1273 2023-06-23 18:22:28.365942 openai_functions-0.3.0/openai_functions/parsers/union_parser.py
--rw-r--r--   0        0        0        0 2023-06-23 18:45:36.035799 openai_functions-0.3.0/openai_functions/py.typed
--rw-r--r--   0        0        0    11932 2023-06-23 20:45:27.576270 openai_functions-0.3.0/openai_functions/runner.py
--rw-r--r--   0        0        0      557 2023-06-23 20:48:30.033977 openai_functions-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3231 1970-01-01 00:00:00.000000 openai_functions-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2689 2023-06-23 21:23:30.745575 openai_functions-0.4.0/README.md
+-rw-r--r--   0        0        0      385 2023-06-23 21:21:35.696216 openai_functions-0.4.0/openai_functions/__init__.py
+-rw-r--r--   0        0        0    12507 2023-06-23 21:20:40.873554 openai_functions-0.4.0/openai_functions/conversation.py
+-rw-r--r--   0        0        0     6245 2023-06-23 20:59:37.510332 openai_functions-0.4.0/openai_functions/function_wrapper.py
+-rw-r--r--   0        0        0      160 2023-06-23 09:03:37.241129 openai_functions-0.4.0/openai_functions/json_type.py
+-rw-r--r--   0        0        0     4042 2023-06-23 21:18:19.040787 openai_functions-0.4.0/openai_functions/openai_types.py
+-rw-r--r--   0        0        0      156 2023-06-23 09:03:50.609263 openai_functions-0.4.0/openai_functions/parsers/__init__.py
+-rw-r--r--   0        0        0     1668 2023-06-23 18:20:13.721023 openai_functions-0.4.0/openai_functions/parsers/abc.py
+-rw-r--r--   0        0        0      977 2023-06-23 18:20:30.777150 openai_functions-0.4.0/openai_functions/parsers/atomic_type_parser.py
+-rw-r--r--   0        0        0      201 2023-06-23 07:38:18.327910 openai_functions-0.4.0/openai_functions/parsers/bool_parser.py
+-rw-r--r--   0        0        0     1641 2023-06-23 18:20:59.916367 openai_functions-0.4.0/openai_functions/parsers/dataclass_parser.py
+-rw-r--r--   0        0        0      760 2023-06-23 13:05:10.173401 openai_functions-0.4.0/openai_functions/parsers/default.py
+-rw-r--r--   0        0        0     1194 2023-06-23 18:21:17.923529 openai_functions-0.4.0/openai_functions/parsers/dict_parser.py
+-rw-r--r--   0        0        0     1067 2023-06-23 18:21:23.392642 openai_functions-0.4.0/openai_functions/parsers/enum_parser.py
+-rw-r--r--   0        0        0      205 2023-06-23 07:38:08.368818 openai_functions-0.4.0/openai_functions/parsers/float_parser.py
+-rw-r--r--   0        0        0      640 2023-06-23 13:22:33.435179 openai_functions-0.4.0/openai_functions/parsers/int_parser.py
+-rw-r--r--   0        0        0      993 2023-06-23 18:21:35.574892 openai_functions-0.4.0/openai_functions/parsers/list_parser.py
+-rw-r--r--   0        0        0      691 2023-06-23 18:21:54.432274 openai_functions-0.4.0/openai_functions/parsers/none_parser.py
+-rw-r--r--   0        0        0      204 2023-06-23 07:39:45.512719 openai_functions-0.4.0/openai_functions/parsers/str_parser.py
+-rw-r--r--   0        0        0     1273 2023-06-23 18:22:28.365942 openai_functions-0.4.0/openai_functions/parsers/union_parser.py
+-rw-r--r--   0        0        0        0 2023-06-23 18:45:36.035799 openai_functions-0.4.0/openai_functions/py.typed
+-rw-r--r--   0        0        0      557 2023-06-23 21:28:18.697839 openai_functions-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3291 1970-01-01 00:00:00.000000 openai_functions-0.4.0/PKG-INFO
```

### Comparing `openai_functions-0.3.0/README.md` & `openai_functions-0.4.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -15,31 +15,31 @@
 ## Usage
 
 1. Import the necessary modules:
 
 ```python
 import enum
 import openai
-from openai_functions import Runner
+from openai_functions import Conversation
 ```
 
-2. Create a `Runner` instance:
+2. Create a `Conversation` instance:
 
 ```python
-runner = Runner()
+conversation = Conversation()
 ```
 
-3. Define your functions using the `@runner.add_function` decorator:
+3. Define your functions using the `@conversation.add_function` decorator:
 
 ```python
 class Unit(enum.Enum):
     FAHRENHEIT = "fahrenheit"
     CELSIUS = "celsius"
 
-@runner.add_function()
+@conversation.add_function()
 def get_current_weather(location: str, unit: Unit = Unit.FAHRENHEIT) -> dict:
     """
     Get the current weather in a given location.
 
     Args:
         location (str): The city and state, e.g., San Francisco, CA
         unit (Unit): The unit to use, e.g. fahrenheit or celsius
@@ -52,29 +52,29 @@
         "temperature": "72",
         "unit": unit.value,
         "forecast": ["sunny", "windy"],
     }
     return weather_info
 ```
 
-4. Add user messages using the `runner.add_message` method:
+4. Add user messages using the `conversation.add_message` method:
 
 ```python
-runner.add_message(
+conversation.add_message(
     {
         "role": "user",
         "content": "What's the weather in San Francisco?",
     }
 )
 ```
 
-5. Call the `runner.run_until_response()` method to trigger the conversation and retrieve the response:
+5. Call the `conversation.run_until_response()` method to trigger the conversation and retrieve the response:
 
 ```python
-print(runner.run_until_response())
+print(conversation.run_until_response())
 ```
 
 ## How it Works
 
 `openai-functions` takes care of the following tasks:
 
 - Parsing the function signatures and docstrings.
```

### Comparing `openai_functions-0.3.0/openai_functions/function_wrapper.py` & `openai_functions-0.4.0/openai_functions/function_wrapper.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,85 @@
 """Wrap a function for jsonschema io."""
 from __future__ import annotations
+from dataclasses import dataclass
 import inspect
 from typing import Any, Callable, OrderedDict, TYPE_CHECKING, Type
 
 from docstring_parser import Docstring, parse
 
 from .parsers import ArgSchemaParser, defargparsers
 
 if TYPE_CHECKING:
     from .json_type import JsonType
 
 
+@dataclass
+class WrapperConfig:
+    """Configuration for a FunctionWrapper"""
+
+    parsers: list[Type[ArgSchemaParser]] | None = None
+    save_return: bool = True
+    serialize: bool = True
+    interpret_as_response: bool = False
+
+
 class FunctionWrapper:
     """Wraps a function for jsonschema io"""
 
     def __init__(
         self,
         func: Callable[..., JsonType],
-        parsers: list[Type[ArgSchemaParser]] | None = None,
-        save_return: bool = True,
-        serialize: bool = True,
-        interpret_as_response: bool = False,
+        config: WrapperConfig | None = None,
     ) -> None:
         """Initialize a FunctionWrapper
 
         Args:
             func (Callable[..., JsonType]): The function to wrap
-            parsers (list[Type[ArgSchemaParser]], optional): The parsers to use.
-            save_return (bool): Whether to send the return value of this
-                function to the AI. Defaults to True.
-            serialize (bool): Whether to serialize the return value of this
-                function. Defaults to True. Otherwise, the return value must be a
-                string.
-            interpret_as_response (bool): Whether to interpret the return
-                value of this function as a response of the agent. Defaults to False.
+            config (WrapperConfig | None, optional): The configuration for the wrapper.
         """
         self.func = func
-        self.parsers = parsers or defargparsers
-        self.save_return = save_return
-        self.serialize = serialize
-        self.interpret_as_response = interpret_as_response
+        self.config = config or WrapperConfig()
+
+    @property
+    def parsers(self) -> list[Type[ArgSchemaParser]]:
+        """Get the parsers for this function
+
+        Returns:
+            list[Type[ArgSchemaParser]]: The parsers
+        """
+        return self.config.parsers or defargparsers
+
+    @property
+    def save_return(self) -> bool:
+        """Get whether to send the return value of this function to the AI
+
+        Returns:
+            bool: Whether to send the return value to the AI
+        """
+        return self.config.save_return
+
+    @property
+    def serialize(self) -> bool:
+        """Get whether to serialize the return value of this function
+
+        The function should return strictly a string if this is false.
+
+        Returns:
+            bool: Whether to serialize the return value
+        """
+        return self.config.serialize
+
+    @property
+    def interpret_as_response(self) -> bool:
+        """Get whether to interpret the return value as an assistant response
+
+        Returns:
+            bool: Whether to interpret the return value as a response
+        """
+        return self.config.interpret_as_response
 
     @property
     def argument_parsers(self) -> OrderedDict[str, ArgSchemaParser]:
         """Get the argument parsers for this function
 
         Returns:
             OrderedDict[str, ArgSchemaParser]: The argument parsers
```

### Comparing `openai_functions-0.3.0/openai_functions/openai_types.py` & `openai_functions-0.4.0/openai_functions/openai_types.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """A module for type definitions for OpenAI API responses"""
 from __future__ import annotations
 from typing import Literal, NotRequired, TypedDict, overload
+from typing_extensions import TypeGuard
 
 
 class FunctionCall(TypedDict):
     """A type for OpenAI function calls"""
 
     name: str
     arguments: str
@@ -14,14 +15,21 @@
     """A type for OpenAI messages that are not function calls"""
 
     role: Literal["system", "user", "assistant"]
     content: str | None
     function_call: NotRequired[FunctionCall]
 
 
+class FinalResponseMessageType(TypedDict):
+    """A type for OpenAI messages that are final responses"""
+
+    role: Literal["assistant"]
+    content: str
+
+
 class FunctionMessageType(TypedDict):
     """A type for OpenAI messages"""
 
     role: Literal["function"]
     name: str
     content: str | None
 
@@ -121,7 +129,26 @@
             and self.content == other.content
             and self.role == other.role
             and self.function_call == other.function_call
         )
 
     def __hash__(self) -> int:
         return hash((self.content, self.role))
+
+
+class FinalResponseMessage(Message):
+    """A container for OpenAI final response messages"""
+
+    message: FinalResponseMessageType  # type: ignore
+
+    @property
+    def content(self) -> str:
+        """Get the content of the message
+
+        Returns:
+            str: The content of the message
+        """
+        return self.message["content"]
+
+
+def is_final_response_message(message: Message) -> TypeGuard[FinalResponseMessage]:
+    return message.is_final_response
```

### Comparing `openai_functions-0.3.0/openai_functions/parsers/abc.py` & `openai_functions-0.4.0/openai_functions/parsers/abc.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.3.0/openai_functions/parsers/atomic_type_parser.py` & `openai_functions-0.4.0/openai_functions/parsers/atomic_type_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.3.0/openai_functions/parsers/dataclass_parser.py` & `openai_functions-0.4.0/openai_functions/parsers/dataclass_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.3.0/openai_functions/parsers/default.py` & `openai_functions-0.4.0/openai_functions/parsers/default.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.3.0/openai_functions/parsers/dict_parser.py` & `openai_functions-0.4.0/openai_functions/parsers/dict_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.3.0/openai_functions/parsers/enum_parser.py` & `openai_functions-0.4.0/openai_functions/parsers/enum_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.3.0/openai_functions/parsers/int_parser.py` & `openai_functions-0.4.0/openai_functions/parsers/int_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.3.0/openai_functions/parsers/list_parser.py` & `openai_functions-0.4.0/openai_functions/parsers/list_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.3.0/openai_functions/parsers/none_parser.py` & `openai_functions-0.4.0/openai_functions/parsers/none_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.3.0/openai_functions/parsers/union_parser.py` & `openai_functions-0.4.0/openai_functions/parsers/union_parser.py`

 * *Files identical despite different names*

### Comparing `openai_functions-0.3.0/openai_functions/runner.py` & `openai_functions-0.4.0/openai_functions/conversation.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,21 @@
 from __future__ import annotations
 from functools import partial
 import json
 from typing import Callable, Protocol, TYPE_CHECKING, overload, runtime_checkable
 
 import openai
 
-from .function_wrapper import FunctionWrapper
-from .openai_types import FunctionMessageType, Message
+from .function_wrapper import FunctionWrapper, WrapperConfig
+from .openai_types import (
+    FinalResponseMessage,
+    FunctionMessageType,
+    Message,
+    is_final_response_message,
+)
 
 if TYPE_CHECKING:
     from .json_type import JsonType
     from .openai_types import FunctionCall, MessageType, NonFunctionMessageType
 
 
 @runtime_checkable
@@ -38,15 +43,15 @@
         """Get whether to continue running after this function"""
 
     @property
     def interpret_as_response(self) -> bool:  # type: ignore
         """Get whether to interpret the return value of this function as a response"""
 
 
-class Runner:
+class Conversation:
     """A class for running OpenAI functions"""
 
     def __init__(
         self,
         functions: list[OpenAIFunction] | None = None,
         model: str = "gpt-3.5-turbo-0613",
     ) -> None:
@@ -84,19 +89,19 @@
         """Add a message
 
         Args:
             message (Message): The message
         """
         self.messages.append(message)
 
-    def add_message(self, message: Message | MessageType) -> None:
+    def add_message(self, message: Message | MessageType | str) -> None:
         """Add a message
 
         Args:
-            message (Message | MessageType): The message
+            message (Message | MessageType | str): The message
         """
         if isinstance(message, Message):
             self._add_message(message)
         else:
             self._add_message(Message(message))
 
     def add_messages(self, messages: list[Message | MessageType]) -> None:
@@ -108,15 +113,15 @@
         for message in messages:
             self.add_message(message)
 
     def pop_message(self, index: int = -1) -> Message:
         """Pop a message
 
         Args:
-            index (int, optional): The index. Defaults to -1.
+            index (int): The index. Defaults to -1.
 
         Returns:
             Message: The message
         """
         return self.messages.pop(index)
 
     def clear_messages(self) -> None:
@@ -157,15 +162,19 @@
     def get_function_result(
         self, function: OpenAIFunction, arguments: dict[str, JsonType]
     ) -> str | None:
         """Get the result of a function
 
         Args:
             function (OpenAIFunction): The function
-            arguments (JsonType): The arguments
+            arguments (dict[str, JsonType]): The arguments
+
+        Raises:
+            TypeError: If the function returns a non-string value
+                while serialize is False
 
         Returns:
             str | None: The result
         """
         result = function(arguments)
 
         if function.save_return:
@@ -191,16 +200,16 @@
 
     def add_function_result(
         self, function_name: str, function_result: str | None
     ) -> bool:
         """Add a function result
 
         Args:
-            function_name (str | None): The function name
-            function_result (str): The function result
+            function_name (str): The function name
+            function_result (str | None): The function result
 
         Returns:
             bool: Whether the function result was added
         """
         if function_result is None:
             return False
         response: FunctionMessageType = {
@@ -282,23 +291,23 @@
         if self.run_function_if_needed():
             return self.messages[-1]
 
         message = self._generate_message()
         self.add_message(message)
         return Message(message)
 
-    def run_until_response(self) -> Message:
+    def run_until_response(self) -> FinalResponseMessage:
         """Run until a response is generated
 
         Returns:
             Message: The response
         """
         while True:
             message = self.generate_message()
-            if message.is_final_response:
+            if is_final_response_message(message):
                 return message
 
     def _add_function(self, function: OpenAIFunction) -> None:
         """Add a function
 
         Args:
             function (OpenAIFunction): The function
@@ -359,15 +368,16 @@
         """
         if isinstance(function, OpenAIFunction):
             self._add_function(function)
             return function
         if callable(function):
             self._add_function(
                 FunctionWrapper(
-                    function, None, save_return, serialize, interpret_as_response
+                    function,
+                    WrapperConfig(None, save_return, serialize, interpret_as_response),
                 )
             )
             return function
 
         return partial(
             self.add_function,
             save_return=save_return,
@@ -394,7 +404,19 @@
         if isinstance(function, str):
             self._remove_function(function)
             return
         if isinstance(function, OpenAIFunction):
             self._remove_function(function.name)
             return
         self._remove_function(function.__name__)
+
+    def ask(self, question: str) -> str:
+        """Ask the AI a question
+
+        Args:
+            question (str): The question
+
+        Returns:
+            str: The answer to the question
+        """
+        self.add_message(question)
+        return self.run_until_response().content
```

### Comparing `openai_functions-0.3.0/pyproject.toml` & `openai_functions-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openai-functions"
-version = "0.3.0"
+version = "0.4.0"
 description = ""
 authors = ["rizerphe <44440399+rizerphe@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "openai_functions"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `openai_functions-0.3.0/PKG-INFO` & `openai_functions-0.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-functions
-Version: 0.3.0
+Version: 0.4.0
 Summary: 
 Author: rizerphe
 Author-email: 44440399+rizerphe@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -32,31 +32,31 @@
 ## Usage
 
 1. Import the necessary modules:
 
 ```python
 import enum
 import openai
-from openai_functions import Runner
+from openai_functions import Conversation
 ```
 
-2. Create a `Runner` instance:
+2. Create a `Conversation` instance:
 
 ```python
-runner = Runner()
+conversation = Conversation()
 ```
 
-3. Define your functions using the `@runner.add_function` decorator:
+3. Define your functions using the `@conversation.add_function` decorator:
 
 ```python
 class Unit(enum.Enum):
     FAHRENHEIT = "fahrenheit"
     CELSIUS = "celsius"
 
-@runner.add_function()
+@conversation.add_function()
 def get_current_weather(location: str, unit: Unit = Unit.FAHRENHEIT) -> dict:
     """
     Get the current weather in a given location.
 
     Args:
         location (str): The city and state, e.g., San Francisco, CA
         unit (Unit): The unit to use, e.g. fahrenheit or celsius
@@ -69,29 +69,29 @@
         "temperature": "72",
         "unit": unit.value,
         "forecast": ["sunny", "windy"],
     }
     return weather_info
 ```
 
-4. Add user messages using the `runner.add_message` method:
+4. Add user messages using the `conversation.add_message` method:
 
 ```python
-runner.add_message(
+conversation.add_message(
     {
         "role": "user",
         "content": "What's the weather in San Francisco?",
     }
 )
 ```
 
-5. Call the `runner.run_until_response()` method to trigger the conversation and retrieve the response:
+5. Call the `conversation.run_until_response()` method to trigger the conversation and retrieve the response:
 
 ```python
-print(runner.run_until_response())
+print(conversation.run_until_response())
 ```
 
 ## How it Works
 
 `openai-functions` takes care of the following tasks:
 
 - Parsing the function signatures and docstrings.
```


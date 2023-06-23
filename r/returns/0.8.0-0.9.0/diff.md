# Comparing `tmp/returns-0.8.0.tar.gz` & `tmp/returns-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "returns-0.8.0.tar", last modified: Mon Jun 17 11:29:27 2019, max compression
+gzip compressed data, was "returns-0.9.0.tar", last modified: Mon Jul  1 14:25:44 2019, max compression
```

## Comparing `returns-0.8.0.tar` & `returns-0.9.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1289 2019-02-18 10:58:23.944528 returns-0.8.0/LICENSE
--rw-r--r--   0        0        0     8599 2019-06-16 19:25:42.435747 returns-0.8.0/README.md
--rw-r--r--   0        0        0     1231 2019-06-17 11:14:01.641893 returns-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      863 2019-06-16 11:32:30.914881 returns-0.8.0/returns/__init__.py
--rw-r--r--   0        0        0       24 2019-06-15 09:08:35.201472 returns-0.8.0/returns/contrib/__init__.py
--rw-r--r--   0        0        0       24 2019-06-15 09:08:35.203073 returns-0.8.0/returns/contrib/mypy/__init__.py
--rw-r--r--   0        0        0     2495 2019-06-17 10:12:49.940000 returns-0.8.0/returns/contrib/mypy/decorator_plugin.py
--rw-r--r--   0        0        0      734 2019-06-17 10:13:15.692467 returns-0.8.0/returns/converters.py
--rw-r--r--   0        0        0     1323 2019-06-17 08:37:33.306625 returns-0.8.0/returns/functions.py
--rw-r--r--   0        0        0     2662 2019-06-17 10:52:30.815663 returns-0.8.0/returns/io.py
--rw-r--r--   0        0        0     7819 2019-06-17 11:18:00.054026 returns-0.8.0/returns/maybe.py
--rw-r--r--   0        0        0     1989 2019-06-17 10:13:15.710115 returns-0.8.0/returns/pipeline.py
--rw-r--r--   0        0        0       24 2019-02-02 10:57:55.845849 returns-0.8.0/returns/primitives/__init__.py
--rw-r--r--   0        0        0     4862 2019-06-17 10:13:15.719758 returns-0.8.0/returns/primitives/container.py
--rw-r--r--   0        0        0      772 2019-06-17 11:19:14.102260 returns-0.8.0/returns/primitives/exceptions.py
--rw-r--r--   0        0        0        0 2019-02-02 17:57:39.341987 returns-0.8.0/returns/py.typed
--rw-r--r--   0        0        0     7950 2019-06-17 11:18:19.890383 returns-0.8.0/returns/result.py
--rw-r--r--   0        0        0      724 2019-06-17 08:49:26.153486 returns-0.8.0/returns/unsafe.py
--rw-r--r--   0        0        0     9570 1970-01-01 00:00:00.000000 returns-0.8.0/setup.py
--rw-r--r--   0        0        0      885 1970-01-01 00:00:00.000000 returns-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1289 2019-02-18 10:58:23.944528 returns-0.9.0/LICENSE
+-rw-r--r--   0        0        0     8921 2019-06-21 07:31:59.292285 returns-0.9.0/README.md
+-rw-r--r--   0        0        0     1231 2019-07-01 12:04:55.071410 returns-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      992 2019-06-19 13:32:40.008661 returns-0.9.0/returns/__init__.py
+-rw-r--r--   0        0        0       24 2019-06-15 09:08:35.201472 returns-0.9.0/returns/contrib/__init__.py
+-rw-r--r--   0        0        0       24 2019-06-15 09:08:35.203073 returns-0.9.0/returns/contrib/mypy/__init__.py
+-rw-r--r--   0        0        0     2495 2019-06-30 11:22:26.934565 returns-0.9.0/returns/contrib/mypy/decorator_plugin.py
+-rw-r--r--   0        0        0     1284 2019-06-30 11:47:14.170549 returns-0.9.0/returns/converters.py
+-rw-r--r--   0        0        0     1323 2019-06-17 08:37:33.306625 returns-0.9.0/returns/functions.py
+-rw-r--r--   0        0        0     2653 2019-06-19 13:32:40.008965 returns-0.9.0/returns/io.py
+-rw-r--r--   0        0        0     8047 2019-06-30 10:10:30.608667 returns-0.9.0/returns/maybe.py
+-rw-r--r--   0        0        0     1989 2019-06-17 10:13:15.710115 returns-0.9.0/returns/pipeline.py
+-rw-r--r--   0        0        0       24 2019-02-02 10:57:55.845849 returns-0.9.0/returns/primitives/__init__.py
+-rw-r--r--   0        0        0     5157 2019-06-30 10:12:15.724455 returns-0.9.0/returns/primitives/container.py
+-rw-r--r--   0        0        0      705 2019-06-19 13:32:40.009671 returns-0.9.0/returns/primitives/exceptions.py
+-rw-r--r--   0        0        0        0 2019-02-02 17:57:39.341987 returns-0.9.0/returns/py.typed
+-rw-r--r--   0        0        0     8707 2019-06-30 11:25:26.619705 returns-0.9.0/returns/result.py
+-rw-r--r--   0        0        0      724 2019-06-17 08:49:26.153486 returns-0.9.0/returns/unsafe.py
+-rw-r--r--   0        0        0     9899 1970-01-01 00:00:00.000000 returns-0.9.0/setup.py
+-rw-r--r--   0        0        0      885 1970-01-01 00:00:00.000000 returns-0.9.0/PKG-INFO
```

### Comparing `returns-0.8.0/LICENSE` & `returns-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `returns-0.8.0/README.md` & `returns-0.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -20,18 +20,20 @@
 
 ## Installation
 
 ```bash
 pip install returns
 ```
 
-You might also need to [configure](https://returns.readthedocs.io/en/latest/pages/container.html#type-safety)
-`mypy` correctly and install our plugin:
+You might also want to [configure](https://returns.readthedocs.io/en/latest/pages/container.html#type-safety)
+`mypy` correctly and install our plugin
+to fix [this existing issue](https://github.com/python/mypy/issues/3157):
 
 ```ini
+# In setup.cfg or mypy.ini:
 [mypy]
 plugins =
   returns.contrib.mypy.decorator_plugin
 ```
 
 Make sure you know how to get started, [check out our docs](https://returns.readthedocs.io/en/latest/)!
 
@@ -215,43 +217,47 @@
 Whenever we access `FetchUserProfile` we now know
 that it does `IO` and might fail.
 So, we act accordingly!
 
 
 ## Maybe container
 
-Have you ever since code with a lot of `if some is not None` conditions?
-It really bloats your source code and makes it unreadable.
+`None` is called the [worst mistake in the history of Computer Science](https://www.infoq.com/presentations/Null-References-The-Billion-Dollar-Mistake-Tony-Hoare/).
 
-But, having `None` in your source code is even worth.
-Actually, `None` is called the [worth mistake in the history of Computer Science](https://www.infoq.com/presentations/Null-References-The-Billion-Dollar-Mistake-Tony-Hoare/).
-
-So, what to do? Use `Maybe` container!
-It consists of `Some(...)` and `Nothing` types,
-representing existing state and `None` state respectively.
+So, what can we do?
+You can use `Optional` and write a lot of `if some is not None` conditions.
+But, having them here and there makes your code unreadable.
+
+Or you can use
+[Maybe](https://returns.readthedocs.io/en/latest/pages/maybe.html) container!
+It consists of `Some` and `Nothing` types,
+representing existing state and empty (instead of `None`) state respectively.
 
 ```python
 from typing import Optional
-from returns.maybe import Maybe
+from returns.maybe import Maybe, maybe
 
+@maybe
 def bad_function() -> Optional[int]:
     ...
 
-maybe_result: Maybe[float] = Maybe.new(
-    bad_function(),
-).map(
+maybe_result: Maybe[float] = bad_function().map(
     lambda number: number / 2,
 )
-# => Maybe will return Some(float) only if there's a non-None value
+# => Maybe will return Some[float] only if there's a non-None value
 #    Otherwise, will return Nothing
 ```
 
+It follows the same composition rules as the `Result` type.
+You can be sure that `.map()` method won't be called for `Nothing`.
 Forget about `None`-related errors forever!
 
 
 ## More!
 
 Want more? [Go to the docs!](https://returns.readthedocs.io)
 Or read these articles:
 
 - [Python exceptions considered an anti-pattern](https://sobolevn.me/2019/02/python-exceptions-considered-an-antipattern)
 - [Enforcing Single Responsibility Principle in Python](https://sobolevn.me/2019/03/enforcing-srp)
+
+Do you have an article to submit? Feel free to open a pull request!
```

### Comparing `returns-0.8.0/pyproject.toml` & `returns-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "returns"
-version = "0.8.0"
+version = "0.9.0"
 description = "Make your functions return something meaningful, typed, and safe!"
 license = "MIT"
 
 authors = [
   "sobolevn <mail@sobolevn.me>"
 ]
 
@@ -33,15 +33,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.6"
 typing-extensions = "^3.7"
 
 [tool.poetry.dev-dependencies]
 mypy = "^0.701"
-wemake-python-styleguide = "^0.8.1"
+wemake-python-styleguide = "^0.9.0"
 flake8-pytest = "^1.3"
 
 safety = "^1.8"
 
 pytest = "^4.6"
 pytest-cov = "^2.7"
 pytest-randomly = "^3.0"
@@ -50,12 +50,12 @@
 
 sphinx = "^2.1"
 sphinx-autodoc-typehints = "^1.6"
 sphinxcontrib-mermaid = "^0.3.1"
 sphinx-typlog-theme = "^0.7.1"
 doc8 = "^0.8.0"
 m2r = "^0.2.1"
-tomlkit = "^0.5.3"
+tomlkit = "^0.5.4"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `returns-0.8.0/returns/__init__.py` & `returns-0.9.0/returns/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
   import returns
   result: returns.Result[int, str]
 
 See: https://github.com/dry-python/returns/issues/73
 """
 
+from returns.converters import maybe_to_result, result_to_maybe
 from returns.functions import compose, raise_exception
 from returns.io import IO, impure
 from returns.maybe import Maybe, Nothing, Some, maybe
 from returns.pipeline import is_successful, pipeline
 from returns.primitives.exceptions import UnwrapFailedError
 from returns.result import Failure, Result, Success, safe
 
@@ -41,8 +42,12 @@
     'Result',
     'Success',
     'UnwrapFailedError',
 
     # pipeline:
     'is_successful',
     'pipeline',
+
+    # Converters:
+    'result_to_maybe',
+    'maybe_to_result',
 )
```

### Comparing `returns-0.8.0/returns/contrib/mypy/decorator_plugin.py` & `returns-0.9.0/returns/contrib/mypy/decorator_plugin.py`

 * *Files identical despite different names*

### Comparing `returns-0.8.0/returns/functions.py` & `returns-0.9.0/returns/functions.py`

 * *Files identical despite different names*

### Comparing `returns-0.8.0/returns/io.py` & `returns-0.9.0/returns/io.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # -*- coding: utf-8 -*-
 
 from functools import wraps
 from inspect import iscoroutinefunction
-from typing import Callable, Coroutine, TypeVar, overload
+from typing import Callable, Coroutine, Generic, TypeVar, overload
 
 from typing_extensions import final
 
-from returns.primitives.container import Container, GenericContainerOneSlot
+from returns.primitives.container import BaseContainer
 
 _ValueType = TypeVar('_ValueType')
 _NewValueType = TypeVar('_NewValueType')
 
 # Helpers:
 _FirstType = TypeVar('_FirstType')
 _SecondType = TypeVar('_SecondType')
 
 
 @final
-class IO(GenericContainerOneSlot[_ValueType]):
+class IO(Generic[_ValueType], BaseContainer):
     """
     Explicit marker for impure function results.
 
     We call it "marker" since once it is marked, it cannot be unmarked.
 
     ``IO`` is also a container.
     But, it is different in a way
@@ -29,15 +29,15 @@
     There's no way to directly get its internal value.
     """
 
     _inner_value: _ValueType
 
     def __init__(self, inner_value: _ValueType) -> None:
         """Required for typing."""
-        Container.__init__(self, inner_value)  # type: ignore # noqa: Z462
+        BaseContainer.__init__(self, inner_value)  # type: ignore # noqa: Z462
 
     def map(  # noqa: A003
         self,
         function: Callable[[_ValueType], _NewValueType],
     ) -> 'IO[_NewValueType]':
         """
         Applies function to the inner value.
```

### Comparing `returns-0.8.0/returns/maybe.py` & `returns-0.9.0/returns/maybe.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,81 +1,97 @@
 # -*- coding: utf-8 -*-
 
 from abc import ABCMeta, abstractmethod
 from functools import wraps
 from inspect import iscoroutinefunction
-from typing import Any, Callable, Coroutine, Optional, TypeVar, Union, overload
+from typing import (
+    Any,
+    Callable,
+    Coroutine,
+    Generic,
+    Optional,
+    TypeVar,
+    Union,
+    overload,
+)
 
 from typing_extensions import final
 
-from returns.primitives.container import (
-    Container,
-    FixableContainer,
-    GenericContainerOneSlot,
-    ValueUnwrapContainer,
-)
+from returns.primitives.container import BaseContainer
 from returns.primitives.exceptions import UnwrapFailedError
 
 # Aliases:
 _ValueType = TypeVar('_ValueType')
 _NewValueType = TypeVar('_NewValueType')
 _ErrorType = TypeVar('_ErrorType')
 
 
 class Maybe(
-    GenericContainerOneSlot[_ValueType],
-    FixableContainer,
-    ValueUnwrapContainer,
+    Generic[_ValueType],
+    BaseContainer,
     metaclass=ABCMeta,
 ):
     """
     Represents a result of a series of commutation that can return ``None``.
 
     An alternative to using exceptions or constant ``is None`` checks.
     ``Maybe`` is an abstract type and should not be instantiated directly.
     Instead use ``Some`` and ``Nothing``.
     """
 
+    _inner_value: Optional[_ValueType]
+
     @classmethod
     def new(cls, inner_value: Optional[_ValueType]) -> 'Maybe[_ValueType]':
         """Creates new instance of Maybe container based on a value."""
         if inner_value is None:
             return _Nothing(inner_value)
         return _Some(inner_value)
 
     @abstractmethod  # noqa: A003
     def map(
         self,
         function: Callable[[_ValueType], Optional[_NewValueType]],
     ) -> 'Maybe[_NewValueType]':  # pragma: no cover
-        """Abstract method to compose container with pure function."""
+        """Abstract method to compose container with a pure function."""
         raise NotImplementedError()
 
     @abstractmethod
     def bind(
         self,
         function: Callable[[_ValueType], 'Maybe[_NewValueType]'],
     ) -> 'Maybe[_NewValueType]':  # pragma: no cover
         """Abstract method to compose container with other container."""
         raise NotImplementedError()
 
     @abstractmethod
     def fix(
         self,
-        function: Callable[[], Optional[_NewValueType]],
+        function: Union[
+            # We use this union to make a good balance
+            # between correct and useful typing:
+            Callable[[None], Optional[_NewValueType]],  # correct
+            Callable[[], Optional[_NewValueType]],  # useful
+        ],
     ) -> 'Maybe[_NewValueType]':  # pragma: no cover
-        """Abstract method to compose container with pure function."""
+        """Abstract method to compose container with a pure function."""
         raise NotImplementedError()
 
     @abstractmethod
     def rescue(
         self,
-        function: Callable[[], 'Maybe[_NewValueType]'],
+        function: Union[
+            # We use this union to make a good balance
+            # between correct and useful typing:
+            Callable[[None], 'Maybe[_NewValueType]'],  # correct
+            Callable[[], 'Maybe[_NewValueType]'],  # useful
+        ],
     ) -> 'Maybe[_NewValueType]':  # pragma: no cover
         """Abstract method to compose container with other container."""
+        # TODO: allow Callable[[None], 'Maybe[_NewValueType]']
         raise NotImplementedError()
 
     @abstractmethod
     def value_or(
         self,
         default_value: _NewValueType,
     ) -> Union[_ValueType, _NewValueType]:  # pragma: no cover
@@ -83,33 +99,28 @@
         raise NotImplementedError()
 
     @abstractmethod
     def unwrap(self) -> _ValueType:  # pragma: no cover
         """Get value or raise exception."""
         raise NotImplementedError()
 
-    @abstractmethod
-    def failure(self) -> None:  # pragma: no cover
-        """Get failed value or raise exception."""
-        raise NotImplementedError()
-
 
 @final  # noqa: Z214
 class _Nothing(Maybe[Any]):
     """Represents an empty state."""
 
     _inner_value: None
 
     def __init__(self, inner_value: None = None) -> None:  # noqa: Z459
         """
         Wraps the given value in the Container.
 
         'value' can only be ``None``.
         """
-        Container.__init__(self, inner_value)  # type: ignore # noqa: Z462
+        BaseContainer.__init__(self, inner_value)  # type: ignore # noqa: Z462
 
     def __str__(self):
         """Custom str definition without state inside."""
         return '<Nothing>'
 
     def map(self, function):  # noqa: A003
         """Returns the 'Nothing' instance that was used to call the method."""
@@ -124,51 +135,53 @@
         Applies function to the inner value.
 
         Applies 'function' to the contents of the 'Some' instance
         and returns a new 'Some' object containing the result.
         'function' should not accept any arguments
         and return a non-container result.
         """
-        return Maybe.new(function())
+        try:
+            return Maybe.new(function())
+        except TypeError:
+            return Maybe.new(function(self._inner_value))
 
     def rescue(self, function):
         """
         Applies 'function' to the result of a previous calculation.
 
         'function' should not accept any arguments
         and return Maybe a 'Nothing' or 'Some' type object.
         """
-        return function()
+        try:
+            return function()
+        except TypeError:
+            return function(self._inner_value)
 
     def value_or(self, default_value):
         """Returns the value if we deal with 'Some' or default if 'Nothing'."""
         return default_value
 
     def unwrap(self):
         """Raises an exception, since it does not have a value inside."""
         raise UnwrapFailedError(self)
 
-    def failure(self):
-        """Unwraps inner error value from failed container."""
-        return self._inner_value
-
 
 @final
 class _Some(Maybe[_ValueType]):
     """
     Represents a calculation which has succeeded and contains the value.
 
     Quite similar to ``Success`` type.
     """
 
     _inner_value: _ValueType
 
     def __init__(self, inner_value: _ValueType) -> None:
         """Required for typing."""
-        Container.__init__(self, inner_value)  # type: ignore # noqa: Z462
+        BaseContainer.__init__(self, inner_value)  # type: ignore # noqa: Z462
 
     def map(self, function):  # noqa: A003
         """
         Applies function to the inner value.
 
         Applies 'function' to the contents of the 'Some' instance
         and returns a new 'Maybe' object containing the result.
@@ -198,18 +211,14 @@
         """Returns the value if we deal with 'Some' or default if 'Nothing'."""
         return self._inner_value
 
     def unwrap(self):
         """Returns the unwrapped value from the inside of this container."""
         return self._inner_value
 
-    def failure(self):
-        """Raises an exception, since it does not have an error inside."""
-        raise UnwrapFailedError(self)
-
 
 def Some(inner_value: Optional[_ValueType]) -> Maybe[_ValueType]:  # noqa: N802
     """Public unit function of protected `_Some` type."""
     return Maybe.new(inner_value)
 
 
 #: Public unit value of protected `_Nothing` type.
```

### Comparing `returns-0.8.0/returns/pipeline.py` & `returns-0.9.0/returns/pipeline.py`

 * *Files identical despite different names*

### Comparing `returns-0.8.0/returns/primitives/exceptions.py` & `returns-0.9.0/returns/primitives/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 # -*- coding: utf-8 -*-
 
-from typing import TYPE_CHECKING, TypeVar
+from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:  # pragma: no cover
-    from returns.primitives.container import Container  # noqa: F401, Z435
-
-_ContainerType = TypeVar('_ContainerType', bound='Container')
+    from returns.primitives.container import BaseContainer  # noqa: F401, Z435
 
 
 class UnwrapFailedError(Exception):
     """Raised when a container can not be unwrapped into a meaningful value."""
 
-    def __init__(self, container: _ContainerType) -> None:
+    def __init__(self, container: 'BaseContainer') -> None:
         """
         Saves halted container in the inner state.
 
         So, this container can later be unpacked from this exception
         and used as a regular value.
         """
         super().__init__()
```

### Comparing `returns-0.8.0/returns/result.py` & `returns-0.9.0/returns/result.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,29 @@
 # -*- coding: utf-8 -*-
 
 from abc import ABCMeta, abstractmethod
 from functools import wraps
 from inspect import iscoroutinefunction
-from typing import Any, Callable, Coroutine, TypeVar, Union, overload
+from typing import Any, Callable, Coroutine, Generic, TypeVar, Union, overload
 
 from typing_extensions import final
 
-from returns.primitives.container import (
-    Container,
-    FixableContainer,
-    GenericContainerTwoSlots,
-    ValueUnwrapContainer,
-)
+from returns.primitives.container import BaseContainer
 from returns.primitives.exceptions import UnwrapFailedError
 
 # Regular type vars, work correctly:
 _ValueType = TypeVar('_ValueType')
 _NewValueType = TypeVar('_NewValueType')
 _ErrorType = TypeVar('_ErrorType')
 _NewErrorType = TypeVar('_NewErrorType')
 
 
 class Result(
-    GenericContainerTwoSlots[_ValueType, _ErrorType],
-    FixableContainer,
-    ValueUnwrapContainer,
+    Generic[_ValueType, _ErrorType],
+    BaseContainer,
     metaclass=ABCMeta,
 ):
     """Base class for _Failure and _Success."""
 
     _inner_value: Union[_ValueType, _ErrorType]
 
     @abstractmethod  # noqa: A003
@@ -55,14 +49,22 @@
         self,
         function: Callable[[_ErrorType], _NewValueType],
     ) -> 'Result[_NewValueType, _ErrorType]':  # pragma: no cover
         """Abstract method to compose container with pure function."""
         raise NotImplementedError()
 
     @abstractmethod
+    def map_failure(
+        self,
+        function: Callable[[_ErrorType], _NewErrorType],
+    ) -> 'Result[_ValueType, _NewErrorType]':  # pragma: no cover
+        """Abstract method to compose container with pure function."""
+        raise NotImplementedError()
+
+    @abstractmethod
     def rescue(
         self,
         function: Callable[
             [_ErrorType], 'Result[_NewValueType, _NewErrorType]',
         ],
     ) -> 'Result[_NewValueType, _NewErrorType]':  # pragma: no cover
         """Abstract method to compose container with other container."""
@@ -83,33 +85,44 @@
 
     @abstractmethod
     def failure(self) -> _ErrorType:  # pragma: no cover
         """Get failed value or raise exception."""
         raise NotImplementedError()
 
 
-@final
+@final  # noqa: Z214
 class _Failure(Result[Any, _ErrorType]):
     """
     Represents a calculation which has failed.
 
     It should contain an error code or message.
     Should not be used directly.
     """
 
     _inner_value: _ErrorType
 
     def __init__(self, inner_value: _ErrorType) -> None:
         """Required for typing."""
-        Container.__init__(self, inner_value)  # type: ignore # noqa: Z462
+        BaseContainer.__init__(self, inner_value)  # type: ignore # noqa: Z462
 
     def map(self, function):  # noqa: A003
         """Returns the '_Failure' instance that was used to call the method."""
         return self
 
+    def map_failure(self, function):
+        """
+        Applies function to the error value.
+
+        Applies 'function' to the contents of the '_Failure' instance
+        and returns a new '_Failure' object containing the result.
+        'function' should accept a single "normal" (non-container) argument
+        and return a non-container result.
+        """
+        return _Failure(function(self._inner_value))
+
     def bind(self, function):
         """Returns the '_Failure' instance that was used to call the method."""
         return self
 
     def fix(self, function):
         """
         Applies function to the inner value.
@@ -142,40 +155,44 @@
         raise UnwrapFailedError(self)
 
     def failure(self):
         """Unwraps inner error value from failed container."""
         return self._inner_value
 
 
-@final
+@final  # noqa: Z214
 class _Success(Result[_ValueType, Any]):
     """
     Represents a calculation which has succeeded and contains the result.
 
     Contains the computation value.
     Should not be used directly.
     """
 
     _inner_value: _ValueType
 
     def __init__(self, inner_value: _ValueType) -> None:
         """Required for typing."""
-        Container.__init__(self, inner_value)  # type: ignore # noqa: Z462
+        BaseContainer.__init__(self, inner_value)  # type: ignore # noqa: Z462
 
     def map(self, function):  # noqa: A003
         """
         Applies function to the inner value.
 
         Applies 'function' to the contents of the '_Success' instance
         and returns a new '_Success' object containing the result.
         'function' should accept a single "normal" (non-container) argument
         and return a non-container result.
         """
         return _Success(function(self._inner_value))
 
+    def map_failure(self, function):
+        """Returns the '_Success' instance that was used to call the method."""
+        return self
+
     def bind(self, function):
         """
         Applies 'function' to the result of a previous calculation.
 
         'function' should accept a single "normal" (non-container) argument
         and return Result a '_Failure' or '_Success' type object.
         """
```

### Comparing `returns-0.8.0/returns/unsafe.py` & `returns-0.9.0/returns/unsafe.py`

 * *Files identical despite different names*

### Comparing `returns-0.8.0/setup.py` & `returns-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['typing-extensions>=3.7,<4.0']
 
 setup_kwargs = {
     'name': 'returns',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'Make your functions return something meaningful, typed, and safe!',
-    'long_description': '[![Returns logo](https://raw.githubusercontent.com/dry-python/brand/master/logo/returns.png)](https://github.com/dry-python/returns)\n\n-----\n\n[![Build Status](https://travis-ci.org/dry-python/returns.svg?branch=master)](https://travis-ci.org/dry-python/returns) [![Coverage Status](https://coveralls.io/repos/github/dry-python/returns/badge.svg?branch=master)](https://coveralls.io/github/dry-python/returns?branch=master) [![Documentation Status](https://readthedocs.org/projects/returns/badge/?version=latest)](https://returns.readthedocs.io/en/latest/?badge=latest) [![Python Version](https://img.shields.io/pypi/pyversions/returns.svg)](https://pypi.org/project/returns/) [![wemake-python-styleguide](https://img.shields.io/badge/style-wemake-000000.svg)](https://github.com/wemake-services/wemake-python-styleguide)\n\n-----\n\nMake your functions return something meaningful, typed, and safe!\n\n\n## Features\n\n- Provides a bunch of primitives to write declarative business logic\n- Enforces better architecture\n- Fully typed with annotations and checked with `mypy`, [PEP561 compatible](https://www.python.org/dev/peps/pep-0561/)\n- Pythonic and pleasant to write and to read (!)\n- Support functions and coroutines, framework agnostic\n\n\n## Installation\n\n```bash\npip install returns\n```\n\nYou might also need to [configure](https://returns.readthedocs.io/en/latest/pages/container.html#type-safety)\n`mypy` correctly and install our plugin:\n\n```ini\n[mypy]\nplugins =\n  returns.contrib.mypy.decorator_plugin\n```\n\nMake sure you know how to get started, [check out our docs](https://returns.readthedocs.io/en/latest/)!\n\n\n## Contents\n\n- [Result container](#result-container) that let\'s you to get rid of exceptions\n- [IO marker](#io-marker) that marks all impure operations and structures them\n- [Maybe container](#maybe-container) that allows you to write `None`-free code\n\n\n## Result container\n\nPlease, make sure that you are also aware of\n[Railway Oriented Programming](https://fsharpforfunandprofit.com/rop/).\n\n### Straight-forward approach\n\nConsider this code that you can find in **any** `python` project.\n\n```python\nimport requests\n\ndef fetch_user_profile(user_id: int) -> \'UserProfile\':\n    """Fetches UserProfile dict from foreign API."""\n    response = requests.get(\'/api/users/{0}\'.format(user_id))\n    response.raise_for_status()\n    return response.json()\n```\n\nSeems legit, does not it?\nIt also seems like a pretty straight forward code to test.\nAll you need is to mock `requests.get` to return the structure you need.\n\nBut, there are hidden problems in this tiny code sample\nthat are almost impossible to spot at the first glance.\n\n### Hidden problems\n\nLet\'s have a look at the exact same code,\nbut with the all hidden problems explained.\n\n```python\nimport requests\n\ndef fetch_user_profile(user_id: int) -> \'UserProfile\':\n    """Fetches UserProfile dict from foreign API."""\n    response = requests.get(\'/api/users/{0}\'.format(user_id))\n\n    # What if we try to find user that does not exist?\n    # Or network will go down? Or the server will return 500?\n    # In this case the next line will fail with an exception.\n    # We need to handle all possible errors in this function\n    # and do not return corrupt data to consumers.\n    response.raise_for_status()\n\n    # What if we have received invalid JSON?\n    # Next line will raise an exception!\n    return response.json()\n```\n\nNow, all (probably all?) problems are clear.\nHow can we be sure that this function will be safe\nto use inside our complex business logic?\n\nWe really can not be sure!\nWe will have to create **lots** of `try` and `except` cases\njust to catch the expected exceptions.\n\nOur code will become complex and unreadable with all this mess!\n\n### Pipeline example\n\n```python\nimport requests\nfrom returns.result import Result, pipeline, safe\n\nclass FetchUserProfile(object):\n    """Single responsibility callable object that fetches user profile."""\n\n    @pipeline\n    def __call__(self, user_id: int) -> Result[\'UserProfile\', Exception]:\n        """Fetches UserProfile dict from foreign API."""\n        response = self._make_request(user_id).unwrap()\n        return self._parse_json(response)\n\n    @safe\n    def _make_request(self, user_id: int) -> requests.Response:\n        response = requests.get(\'/api/users/{0}\'.format(user_id))\n        response.raise_for_status()\n        return response\n\n    @safe\n    def _parse_json(self, response: requests.Response) -> \'UserProfile\':\n        return response.json()\n```\n\nNow we have a clean and a safe way to express our business need.\nWe start from making a request, that might fail at any moment.\n\nNow, instead of returning a regular value\nit returns a wrapped value inside a special container\nthanks to the\n[@safe](https://returns.readthedocs.io/en/latest/pages/functions.html#returns.functions.safe)\ndecorator.\n\nIt will return [Success[Response] or Failure[Exception]](https://returns.readthedocs.io/en/latest/pages/result.html).\nAnd will never throw this exception at us.\n\nWhen we will need raw value, we can use `.unwrap()` method to get it.\nIf the result is `Failure[Exception]`\nwe will actually raise an exception at this point.\nBut it is safe to use `.unwrap()` inside\n[@pipeline](https://returns.readthedocs.io/en/latest/pages/functions.html#returns.functions.pipeline)\nfunctions.\nBecause it will catch this exception\nand wrap it inside a new `Failure[Exception]`!\n\nAnd we can clearly see all result patterns\nthat might happen in this particular case:\n- `Success[UserProfile]`\n- `Failure[HttpException]`\n- `Failure[JsonDecodeException]`\n\nAnd we can work with each of them precisely.\nIt is a good practice to create `Enum` classes or `Union` types\nwith a list of all the possible errors.\n\n\n## IO marker\n\nBut is that all we can improve?\nLet\'s look at `FetchUserProfile` from another angle.\nAll its methods look like regular ones:\nit is impossible to tell whether they are pure or impure from the first sight.\n\nIt leads to a very important consequence:\n*we start to mix pure and impure code together*.\nWe should not do that!\n\nWhen these two concepts are mixed\nwe suffer really bad when testing or reusing it.\nAlmost everything should be pure by default.\nAnd we should explicitly mark impure parts of the program.\n\n### Explicit IO\n\nLet\'s refactor it to make our\n[IO](https://returns.readthedocs.io/en/latest/pages/io.html) explicit!\n\n```python\nimport requests\nfrom returns.io import IO, impure\nfrom returns.result import Result, pipeline, safe\n\nclass FetchUserProfile(object):\n    """Single responsibility callable object that fetches user profile."""\n\n    @pipeline\n    def __call__(self, user_id: int) -> IO[Result[\'UserProfile\', Exception]]:\n        """Fetches UserProfile dict from foreign API."""\n        return self._make_request(user_id).map(\n            lambda response: self._parse_json(response.unwrap())\n        )\n\n    @impure\n    @safe\n    def _make_request(self, user_id: int) -> requests.Response:\n        response = requests.get(\'/api/users/{0}\'.format(user_id))\n        response.raise_for_status()\n        return response\n\n    @safe\n    def _parse_json(self,response: requests.Response) -> \'UserProfile\':\n        return response.json()\n```\n\nNow we have explicit markers where the `IO` did happen\nand these markers cannot be removed.\n\nWhenever we access `FetchUserProfile` we now know\nthat it does `IO` and might fail.\nSo, we act accordingly!\n\n\n## Maybe container\n\nHave you ever since code with a lot of `if some is not None` conditions?\nIt really bloats your source code and makes it unreadable.\n\nBut, having `None` in your source code is even worth.\nActually, `None` is called the [worth mistake in the history of Computer Science](https://www.infoq.com/presentations/Null-References-The-Billion-Dollar-Mistake-Tony-Hoare/).\n\nSo, what to do? Use `Maybe` container!\nIt consists of `Some(...)` and `Nothing` types,\nrepresenting existing state and `None` state respectively.\n\n```python\nfrom typing import Optional\nfrom returns.maybe import Maybe\n\ndef bad_function() -> Optional[int]:\n    ...\n\nmaybe_result: Maybe[float] = Maybe.new(\n    bad_function(),\n).map(\n    lambda number: number / 2,\n)\n# => Maybe will return Some(float) only if there\'s a non-None value\n#    Otherwise, will return Nothing\n```\n\nForget about `None`-related errors forever!\n\n\n## More!\n\nWant more? [Go to the docs!](https://returns.readthedocs.io)\nOr read these articles:\n\n- [Python exceptions considered an anti-pattern](https://sobolevn.me/2019/02/python-exceptions-considered-an-antipattern)\n- [Enforcing Single Responsibility Principle in Python](https://sobolevn.me/2019/03/enforcing-srp)\n',
+    'long_description': '[![Returns logo](https://raw.githubusercontent.com/dry-python/brand/master/logo/returns.png)](https://github.com/dry-python/returns)\n\n-----\n\n[![Build Status](https://travis-ci.org/dry-python/returns.svg?branch=master)](https://travis-ci.org/dry-python/returns) [![Coverage Status](https://coveralls.io/repos/github/dry-python/returns/badge.svg?branch=master)](https://coveralls.io/github/dry-python/returns?branch=master) [![Documentation Status](https://readthedocs.org/projects/returns/badge/?version=latest)](https://returns.readthedocs.io/en/latest/?badge=latest) [![Python Version](https://img.shields.io/pypi/pyversions/returns.svg)](https://pypi.org/project/returns/) [![wemake-python-styleguide](https://img.shields.io/badge/style-wemake-000000.svg)](https://github.com/wemake-services/wemake-python-styleguide)\n\n-----\n\nMake your functions return something meaningful, typed, and safe!\n\n\n## Features\n\n- Provides a bunch of primitives to write declarative business logic\n- Enforces better architecture\n- Fully typed with annotations and checked with `mypy`, [PEP561 compatible](https://www.python.org/dev/peps/pep-0561/)\n- Pythonic and pleasant to write and to read (!)\n- Support functions and coroutines, framework agnostic\n\n\n## Installation\n\n```bash\npip install returns\n```\n\nYou might also want to [configure](https://returns.readthedocs.io/en/latest/pages/container.html#type-safety)\n`mypy` correctly and install our plugin\nto fix [this existing issue](https://github.com/python/mypy/issues/3157):\n\n```ini\n# In setup.cfg or mypy.ini:\n[mypy]\nplugins =\n  returns.contrib.mypy.decorator_plugin\n```\n\nMake sure you know how to get started, [check out our docs](https://returns.readthedocs.io/en/latest/)!\n\n\n## Contents\n\n- [Result container](#result-container) that let\'s you to get rid of exceptions\n- [IO marker](#io-marker) that marks all impure operations and structures them\n- [Maybe container](#maybe-container) that allows you to write `None`-free code\n\n\n## Result container\n\nPlease, make sure that you are also aware of\n[Railway Oriented Programming](https://fsharpforfunandprofit.com/rop/).\n\n### Straight-forward approach\n\nConsider this code that you can find in **any** `python` project.\n\n```python\nimport requests\n\ndef fetch_user_profile(user_id: int) -> \'UserProfile\':\n    """Fetches UserProfile dict from foreign API."""\n    response = requests.get(\'/api/users/{0}\'.format(user_id))\n    response.raise_for_status()\n    return response.json()\n```\n\nSeems legit, does not it?\nIt also seems like a pretty straight forward code to test.\nAll you need is to mock `requests.get` to return the structure you need.\n\nBut, there are hidden problems in this tiny code sample\nthat are almost impossible to spot at the first glance.\n\n### Hidden problems\n\nLet\'s have a look at the exact same code,\nbut with the all hidden problems explained.\n\n```python\nimport requests\n\ndef fetch_user_profile(user_id: int) -> \'UserProfile\':\n    """Fetches UserProfile dict from foreign API."""\n    response = requests.get(\'/api/users/{0}\'.format(user_id))\n\n    # What if we try to find user that does not exist?\n    # Or network will go down? Or the server will return 500?\n    # In this case the next line will fail with an exception.\n    # We need to handle all possible errors in this function\n    # and do not return corrupt data to consumers.\n    response.raise_for_status()\n\n    # What if we have received invalid JSON?\n    # Next line will raise an exception!\n    return response.json()\n```\n\nNow, all (probably all?) problems are clear.\nHow can we be sure that this function will be safe\nto use inside our complex business logic?\n\nWe really can not be sure!\nWe will have to create **lots** of `try` and `except` cases\njust to catch the expected exceptions.\n\nOur code will become complex and unreadable with all this mess!\n\n### Pipeline example\n\n```python\nimport requests\nfrom returns.result import Result, pipeline, safe\n\nclass FetchUserProfile(object):\n    """Single responsibility callable object that fetches user profile."""\n\n    @pipeline\n    def __call__(self, user_id: int) -> Result[\'UserProfile\', Exception]:\n        """Fetches UserProfile dict from foreign API."""\n        response = self._make_request(user_id).unwrap()\n        return self._parse_json(response)\n\n    @safe\n    def _make_request(self, user_id: int) -> requests.Response:\n        response = requests.get(\'/api/users/{0}\'.format(user_id))\n        response.raise_for_status()\n        return response\n\n    @safe\n    def _parse_json(self, response: requests.Response) -> \'UserProfile\':\n        return response.json()\n```\n\nNow we have a clean and a safe way to express our business need.\nWe start from making a request, that might fail at any moment.\n\nNow, instead of returning a regular value\nit returns a wrapped value inside a special container\nthanks to the\n[@safe](https://returns.readthedocs.io/en/latest/pages/functions.html#returns.functions.safe)\ndecorator.\n\nIt will return [Success[Response] or Failure[Exception]](https://returns.readthedocs.io/en/latest/pages/result.html).\nAnd will never throw this exception at us.\n\nWhen we will need raw value, we can use `.unwrap()` method to get it.\nIf the result is `Failure[Exception]`\nwe will actually raise an exception at this point.\nBut it is safe to use `.unwrap()` inside\n[@pipeline](https://returns.readthedocs.io/en/latest/pages/functions.html#returns.functions.pipeline)\nfunctions.\nBecause it will catch this exception\nand wrap it inside a new `Failure[Exception]`!\n\nAnd we can clearly see all result patterns\nthat might happen in this particular case:\n- `Success[UserProfile]`\n- `Failure[HttpException]`\n- `Failure[JsonDecodeException]`\n\nAnd we can work with each of them precisely.\nIt is a good practice to create `Enum` classes or `Union` types\nwith a list of all the possible errors.\n\n\n## IO marker\n\nBut is that all we can improve?\nLet\'s look at `FetchUserProfile` from another angle.\nAll its methods look like regular ones:\nit is impossible to tell whether they are pure or impure from the first sight.\n\nIt leads to a very important consequence:\n*we start to mix pure and impure code together*.\nWe should not do that!\n\nWhen these two concepts are mixed\nwe suffer really bad when testing or reusing it.\nAlmost everything should be pure by default.\nAnd we should explicitly mark impure parts of the program.\n\n### Explicit IO\n\nLet\'s refactor it to make our\n[IO](https://returns.readthedocs.io/en/latest/pages/io.html) explicit!\n\n```python\nimport requests\nfrom returns.io import IO, impure\nfrom returns.result import Result, pipeline, safe\n\nclass FetchUserProfile(object):\n    """Single responsibility callable object that fetches user profile."""\n\n    @pipeline\n    def __call__(self, user_id: int) -> IO[Result[\'UserProfile\', Exception]]:\n        """Fetches UserProfile dict from foreign API."""\n        return self._make_request(user_id).map(\n            lambda response: self._parse_json(response.unwrap())\n        )\n\n    @impure\n    @safe\n    def _make_request(self, user_id: int) -> requests.Response:\n        response = requests.get(\'/api/users/{0}\'.format(user_id))\n        response.raise_for_status()\n        return response\n\n    @safe\n    def _parse_json(self,response: requests.Response) -> \'UserProfile\':\n        return response.json()\n```\n\nNow we have explicit markers where the `IO` did happen\nand these markers cannot be removed.\n\nWhenever we access `FetchUserProfile` we now know\nthat it does `IO` and might fail.\nSo, we act accordingly!\n\n\n## Maybe container\n\n`None` is called the [worst mistake in the history of Computer Science](https://www.infoq.com/presentations/Null-References-The-Billion-Dollar-Mistake-Tony-Hoare/).\n\nSo, what can we do?\nYou can use `Optional` and write a lot of `if some is not None` conditions.\nBut, having them here and there makes your code unreadable.\n\nOr you can use\n[Maybe](https://returns.readthedocs.io/en/latest/pages/maybe.html) container!\nIt consists of `Some` and `Nothing` types,\nrepresenting existing state and empty (instead of `None`) state respectively.\n\n```python\nfrom typing import Optional\nfrom returns.maybe import Maybe, maybe\n\n@maybe\ndef bad_function() -> Optional[int]:\n    ...\n\nmaybe_result: Maybe[float] = bad_function().map(\n    lambda number: number / 2,\n)\n# => Maybe will return Some[float] only if there\'s a non-None value\n#    Otherwise, will return Nothing\n```\n\nIt follows the same composition rules as the `Result` type.\nYou can be sure that `.map()` method won\'t be called for `Nothing`.\nForget about `None`-related errors forever!\n\n\n## More!\n\nWant more? [Go to the docs!](https://returns.readthedocs.io)\nOr read these articles:\n\n- [Python exceptions considered an anti-pattern](https://sobolevn.me/2019/02/python-exceptions-considered-an-antipattern)\n- [Enforcing Single Responsibility Principle in Python](https://sobolevn.me/2019/03/enforcing-srp)\n\nDo you have an article to submit? Feel free to open a pull request!\n',
     'author': 'sobolevn',
     'author_email': 'mail@sobolevn.me',
     'url': 'https://returns.readthedocs.io',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.6,<4.0',
```

### Comparing `returns-0.8.0/PKG-INFO` & `returns-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returns
-Version: 0.8.0
+Version: 0.9.0
 Summary: Make your functions return something meaningful, typed, and safe!
 Home-page: https://returns.readthedocs.io
 Author: sobolevn
 Author-email: mail@sobolevn.me
 Keywords: functional programming,fp,monads,monad,type-safety,mypy,railway-oriented-programming
 Requires-Python: >=3.6,<4.0
 Classifier: Development Status :: 4 - Beta
```


# Comparing `tmp/asyncz-0.2.0.tar.gz` & `tmp/asyncz-0.3.0.tar.gz`

## Comparing `asyncz-0.2.0.tar` & `asyncz-0.3.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/__init__.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/_mapping.py
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/datastructures.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/enums.py
--rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/py.typed
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/state.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/typing.py
--rw-r--r--   0        0        0    11206 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/contrib/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/contrib/esmerald/__init__.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/contrib/esmerald/decorator.py
--rw-r--r--   0        0        0     7836 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/contrib/esmerald/scheduler.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/events/__init__.py
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/events/base.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/events/constants.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/executors/__init__.py
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/executors/asyncio.py
--rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/executors/base.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/executors/debug.py
--rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/executors/pool.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/executors/types.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/schedulers/__init__.py
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/schedulers/asyncio.py
--rw-r--r--   0        0        0    40042 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/schedulers/base.py
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/schedulers/datastructures.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/schedulers/types.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/schedulers/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/stores/__init__.py
--rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/stores/base.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/stores/memory.py
--rw-r--r--   0        0        0     5094 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/stores/mongo.py
--rw-r--r--   0        0        0     5439 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/stores/redis.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/stores/types.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/tasks/__init__.py
--rw-r--r--   0        0        0    10031 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/tasks/base.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/tasks/types.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/triggers/__init__.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/triggers/base.py
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/triggers/combination.py
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/triggers/date.py
--rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/triggers/interval.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/triggers/types.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/triggers/cron/__init__.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/triggers/cron/constants.py
--rw-r--r--   0        0        0     9776 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/triggers/cron/expressions.py
--rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/triggers/cron/fields.py
--rw-r--r--   0        0        0    10010 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/triggers/cron/trigger.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 asyncz-0.2.0/asyncz/triggers/cron/types.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 asyncz-0.2.0/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 asyncz-0.2.0/LICENSE
--rw-r--r--   0        0        0     7221 2020-02-02 00:00:00.000000 asyncz-0.2.0/README.md
--rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 asyncz-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    10873 2020-02-02 00:00:00.000000 asyncz-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/__init__.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/_mapping.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/datastructures.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/enums.py
+-rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/py.typed
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/state.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/typing.py
+-rw-r--r--   0        0        0    11409 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/contrib/esmerald/__init__.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/contrib/esmerald/decorator.py
+-rw-r--r--   0        0        0     7860 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/contrib/esmerald/scheduler.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/events/__init__.py
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/events/base.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/events/constants.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/executors/__init__.py
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/executors/asyncio.py
+-rw-r--r--   0        0        0     7796 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/executors/base.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/executors/debug.py
+-rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/executors/pool.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/executors/types.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/schedulers/__init__.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/schedulers/asyncio.py
+-rw-r--r--   0        0        0    39976 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/schedulers/base.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/schedulers/datastructures.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/schedulers/types.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/schedulers/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/stores/__init__.py
+-rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/stores/base.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/stores/memory.py
+-rw-r--r--   0        0        0     5116 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/stores/mongo.py
+-rw-r--r--   0        0        0     5490 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/stores/redis.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/stores/types.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/tasks/__init__.py
+-rw-r--r--   0        0        0    10031 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/tasks/base.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/tasks/types.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/triggers/__init__.py
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/triggers/base.py
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/triggers/combination.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/triggers/date.py
+-rw-r--r--   0        0        0     4260 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/triggers/interval.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/triggers/types.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/triggers/cron/__init__.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/triggers/cron/constants.py
+-rw-r--r--   0        0        0    10456 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/triggers/cron/expressions.py
+-rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/triggers/cron/fields.py
+-rw-r--r--   0        0        0    10005 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/triggers/cron/trigger.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 asyncz-0.3.0/asyncz/triggers/cron/types.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 asyncz-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 asyncz-0.3.0/LICENSE
+-rw-r--r--   0        0        0     7231 2020-02-02 00:00:00.000000 asyncz-0.3.0/README.md
+-rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 asyncz-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    10934 2020-02-02 00:00:00.000000 asyncz-0.3.0/PKG-INFO
```

### Comparing `asyncz-0.2.0/asyncz/_mapping.py` & `asyncz-0.3.0/asyncz/_mapping.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.2.0/asyncz/datastructures.py` & `asyncz-0.3.0/asyncz/datastructures.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from datetime import datetime, timedelta, timezone, tzinfo
 from typing import TYPE_CHECKING, Any, Callable, List, Optional, Union
 
-from asyncz.typing import DictAny
 from pydantic import BaseModel
 
+from asyncz.typing import DictAny
+
 if TYPE_CHECKING:
     from asyncz.stores.types import StoreType
     from asyncz.triggers.types import TriggerType
 else:
     StoreType = Any
     TriggerType = Any
```

### Comparing `asyncz-0.2.0/asyncz/exceptions.py` & `asyncz-0.3.0/asyncz/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 class AsynczException(Exception):
     """
     Base exception for all Asyncz thrown error exceptions.
     """
 
     detail = None
 
-    def __init__(self, *args: Any, detail: str = ""):
+    def __init__(self, *args: Any, detail: str = "") -> None:
         if detail:
             self.detail = detail
         super().__init__(*(str(arg) for arg in args if arg), detail)
 
     def __repr__(self) -> str:
         if self.detail:
             return f"{self.__class__.__name__} - {self.detail}"
@@ -87,16 +87,16 @@
         detail = self.detail.format(id=_id, total=total)
         super().__init__(detail=detail)
 
 
 class SchedulerAlreadyRunningError(AsynczException):
     detail = "Scheduler is already running"
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.detail
 
 
 class SchedulerNotRunningError(AsynczException):
     detail = "Scheduler is not running"
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.detail
```

### Comparing `asyncz-0.2.0/asyncz/state.py` & `asyncz-0.3.0/asyncz/state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import inspect
 from typing import Any
 
-from asyncz.typing import DictAny
 from pydantic import BaseModel
 
+from asyncz.typing import DictAny
+
 object_setattr = object.__setattr__
 
 
 class BaseState(BaseModel):
     __slots__ = ["__weakref__"]
 
     def __setstate__(self, state: "DictAny") -> Any:
```

### Comparing `asyncz-0.2.0/asyncz/utils.py` & `asyncz-0.3.0/asyncz/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import inspect
 import re
 from asyncio import iscoroutinefunction
 from calendar import timegm
 from datetime import date, datetime, time, timedelta, tzinfo
 from functools import partial
-from typing import Any, Dict, Union
+from typing import Any, Callable, Union
 
-from asyncz.exceptions import AsynczException, AsynczLookupError
 from pytz import FixedOffset, timezone, utc
 
+from asyncz.exceptions import AsynczException, AsynczLookupError
+
 try:
     from threading import TIMEOUT_MAX
 except ImportError:
     TIMEOUT_MAX = 4294967
 
 BOOL_VALIDATION = {
     "true": ["true", "yes", "on", "y", "t", "1", True],
@@ -23,15 +24,15 @@
     r"(?P<year>\d{4})-(?P<month>\d{1,2})-(?P<day>\d{1,2})"
     r"(?:[ T](?P<hour>\d{1,2}):(?P<minute>\d{1,2}):(?P<second>\d{1,2})"
     r"(?:\.(?P<microsecond>\d{1,6}))?"
     r"(?P<timezone>Z|[+-]\d\d:\d\d)?)?$"
 )
 
 
-def repr_escape(string):
+def repr_escape(string: str) -> str:
     return string
 
 
 def to_int(value: Union[str, float]) -> int:
     """
     Safely converts a value to integer.
     """
@@ -77,29 +78,31 @@
                 "timezone name (such as Europe/London)."
             )
         return value
     if value is not None:
         raise TypeError("Expected tzinfo, got %s instead" % value.__class__.__name__)
 
 
-def to_datetime(value: Union[str, datetime], tz: tzinfo, arg_name: str) -> datetime:
+def to_datetime(
+    value: Union[str, datetime], tz: tzinfo, arg_name: str
+) -> Union[datetime, None, Any]:
     """
     Converts the given value to a timezone compatible aware datetime object.
 
     If a timezone aware datetime object is passed, it is returned unmodified.
     If a native datetime object is passed, it is given the specified timezone.
     If the input is a string, it is parsed as a datetime with the given timezone.
     """
     if not value or value is None:
-        return
+        return  # type: ignore
 
     if isinstance(value, datetime):
         _datetime = value
-    elif isinstance(value, date):
-        _datetime = datetime.combine(value, time())
+    elif isinstance(value, date):  # type: ignore
+        _datetime = datetime.combine(value, time())  # type: ignore
     elif isinstance(value, str):
         _value = DATE_REGEX.match(value)
 
         if not _value:
             raise AsynczException(detail="Invalid date string.")
 
         values = _value.groupdict()
@@ -109,15 +112,15 @@
             tz = utc
         elif tzname:
             hours, minutes = (int(x) for x in tzname[1:].split(":"))
             sign = 1 if tzname[0] == "+" else -1
             tz = FixedOffset(sign * (hours * 60 + minutes))
 
         values = {k: int(v or 0) for k, v in values.items()}
-        _datetime = datetime(**values)
+        _datetime = datetime(**values)  # type: ignore
     else:
         raise AsynczException(
             detail=f"Unsupported type for {arg_name}: {value.__class__.__name__}."
         )
 
     if _datetime.tzinfo is not None:
         return _datetime
@@ -130,15 +133,15 @@
 
     if isinstance(tz, str):
         tz = timezone(tz)
 
     return localize(_datetime, tz)
 
 
-def datetime_to_utc_timestamp(timeval: datetime):
+def datetime_to_utc_timestamp(timeval: datetime) -> Union[int, float]:
     """
     Converts a datetime instance to a timestamp.
     """
     if timeval is not None:
         return timegm(timeval.utctimetuple()) + timeval.microsecond / 1000000
 
 
@@ -146,15 +149,15 @@
     """
     Converts the given timestamp to a datetime instance.
     """
     if timestamp is not None:
         return datetime.fromtimestamp(timestamp, utc)
 
 
-def timedelta_seconds(delta: Any) -> Union[int, float]:
+def timedelta_seconds(delta: Any) -> Any:
     """
     Converts the given timedelta to seconds.
     """
     return delta.days * 24 * 60 * 60 + delta.seconds + delta.microseconds / 1000000.0
 
 
 def datetime_ceil(dateval: datetime) -> datetime:
@@ -166,15 +169,15 @@
     return dateval
 
 
 def datetime_repr(dateval: datetime) -> str:
     return dateval.strftime("%Y-%m-%d %H:%M:%S %Z") if dateval else "None"
 
 
-def get_callable_name(func: Any) -> str:
+def get_callable_name(func: Any) -> Any:
     """
     Returns the best available display name for the given function/callable.
     """
     # the easy case (on Python 3.3+)
     if hasattr(func, "__qualname__"):
         return func.__qualname__
 
@@ -182,17 +185,17 @@
     f_self = getattr(func, "__self__", None) or getattr(func, "im_self", None)
     if f_self and hasattr(func, "__name__"):
         f_class = f_self if inspect.isclass(f_self) else f_self.__class__
     else:
         f_class = getattr(func, "im_class", None)
 
     if f_class and hasattr(func, "__name__"):
-        return "%s.%s" % (f_class.__name__, func.__name__)
+        return "{}.{}".format(f_class.__name__, func.__name__)
 
-    if hasattr(func, "__call__"):
+    if hasattr(func, "__call__"):  # noqa
         if hasattr(func, "__name__"):
             return func.__name__
         return func.__class__.__name__
 
     raise TypeError("Unable to determine a name for %r -- maybe it is not a callable?" % func)
 
 
@@ -214,15 +217,15 @@
             module = obj.im_self.__module__
         elif hasattr(obj, "im_class") and obj.im_class:
             module = obj.im_class.__module__
         else:
             module = obj.__module__
     else:
         module = obj.__module__
-    return "%s:%s" % (module, name)
+    return "{}:{}".format(module, name)
 
 
 def ref_to_obj(ref: str) -> Any:
     """
     Returns the object pointed to by ``ref``.
     """
     if not isinstance(ref, str):
@@ -230,50 +233,54 @@
     if ":" not in ref:
         raise AsynczException("Invalid reference")
 
     modulename, rest = ref.split(":", 1)
     try:
         obj = __import__(modulename, fromlist=[rest])
     except ImportError:
-        raise AsynczLookupError("Error resolving reference %s: could not import module" % ref)
+        raise AsynczLookupError(
+            "Error resolving reference %s: could not import module" % ref
+        ) from None
 
     try:
         for name in rest.split("."):
             obj = getattr(obj, name)
         return obj
     except Exception:
-        raise AsynczLookupError("Error resolving reference %s: error looking up object" % ref)
+        raise AsynczLookupError(
+            "Error resolving reference %s: error looking up object" % ref
+        ) from None
 
 
-def maybe_ref(ref: str) -> Any:
+def maybe_ref(ref: Any) -> Any:
     """
     Returns the object that the given reference points to, if it is indeed a reference.
     If it is not a reference, the object is returned as-is.
     """
     if not isinstance(ref, str):
         return ref
     return ref_to_obj(ref)
 
 
-def check_callable_args(func, args: Any, kwargs: Dict[Any, Any]) -> None:
+def check_callable_args(func: Callable[..., Any], args: Any, kwargs: Any) -> None:
     """
     Ensures that the given callable can be called with the given arguments.
     """
     pos_kwargs_conflicts = []
     positional_only_kwargs = []
     unsatisfied_args = []
     unsatisfied_kwargs = []
     unmatched_args = list(args)
     unmatched_kwargs = list(kwargs)
     has_varargs = has_var_kwargs = False
 
     try:
         sig = inspect.signature(func, follow_wrapped=False)
     except ValueError as e:
-        raise AsynczException(detail=str(e))
+        raise AsynczException(detail=str(e)) from e
 
     for param in sig.parameters.values():
         if param.kind == param.POSITIONAL_OR_KEYWORD:
             if param.name in unmatched_kwargs and unmatched_args:
                 pos_kwargs_conflicts.append(param.name)
             elif unmatched_args:
                 del unmatched_args[0]
@@ -341,12 +348,12 @@
     return iscoroutinefunction(f)
 
 
 def normalize(value: datetime) -> datetime:
     return datetime.fromtimestamp(value.timestamp(), value.tzinfo)
 
 
-def localize(value: datetime, tzinfo: tzinfo) -> datetime:
+def localize(value: datetime, tzinfo: tzinfo) -> Any:
     if hasattr(tzinfo, "localize"):
         return tzinfo.localize(value)
 
     return normalize(value.replace(tzinfo=tzinfo))
```

### Comparing `asyncz-0.2.0/asyncz/contrib/esmerald/decorator.py` & `asyncz-0.3.0/asyncz/contrib/esmerald/decorator.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.2.0/asyncz/contrib/esmerald/scheduler.py` & `asyncz-0.3.0/asyncz/contrib/esmerald/scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 try:
     from esmerald.conf import settings
     from esmerald.exceptions import ImproperlyConfigured
     from esmerald.utils.module_loading import import_string
 except ImportError:
     raise ImportError(
         "Esmerald cannot be found. Please install it by running `pip install esmerald`."
-    )
+    ) from None
 
 if TYPE_CHECKING:
     from esmerald.applications import Esmerald
     from pydantic.typing import AnyCallable
 
 
 class EsmeraldScheduler:
@@ -83,15 +83,15 @@
 
             if not scheduled_task.is_enabled:
                 continue
 
             try:
                 scheduled_task.add_task(self.handler)
             except Exception as e:
-                raise ImproperlyConfigured(str(e))
+                raise ImproperlyConfigured(str(e)) from e
 
     def register_events(self, app: "Esmerald") -> None:
         """
         Registers the scheduler events in the Esmerald application.
         """
 
         @app.on_event("startup")
@@ -202,15 +202,15 @@
                 max_instances=self.max_intances,
                 next_run_time=self.next_run_time,
                 store=self.store,
                 executor=self.executor,
                 replace_existing=self.replace_existing,
             )
         except Exception as e:
-            raise ImproperlyConfigured(str(e))
+            raise ImproperlyConfigured(str(e)) from e
 
     def __call__(self, fn: "AnyCallable") -> None:
         """
         Tricking the object into think it's being instantiated by in reality
         is just returning itself.
         """
         self.fn = fn
```

### Comparing `asyncz-0.2.0/asyncz/events/base.py` & `asyncz-0.3.0/asyncz/events/base.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.2.0/asyncz/events/constants.py` & `asyncz-0.3.0/asyncz/events/constants.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.2.0/asyncz/executors/asyncio.py` & `asyncz-0.3.0/asyncz/executors/asyncio.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.2.0/asyncz/executors/base.py` & `asyncz-0.3.0/asyncz/executors/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 import traceback
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from datetime import datetime, timedelta
 from traceback import format_tb
 from typing import TYPE_CHECKING, Any, List, Optional, Union
 
+from loguru import logger
+from loguru._logger import Logger
+from pytz import utc
+
 from asyncz.events import TaskExecutionEvent
 from asyncz.events.constants import TASK_ERROR, TASK_EXECUTED, TASK_MISSED
 from asyncz.exceptions import MaximumInstancesError
 from asyncz.state import BaseStateExtra
-from loguru import logger
-from loguru._logger import Logger
-from pytz import utc
 
 if TYPE_CHECKING:
     from asyncz.tasks.types import TaskType
 
 
 class BaseExecutor(BaseStateExtra, ABC):
     """
```

### Comparing `asyncz-0.2.0/asyncz/executors/debug.py` & `asyncz-0.3.0/asyncz/executors/debug.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.2.0/asyncz/executors/pool.py` & `asyncz-0.3.0/asyncz/executors/pool.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.2.0/asyncz/schedulers/asyncio.py` & `asyncz-0.3.0/asyncz/schedulers/asyncio.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.2.0/asyncz/schedulers/base.py` & `asyncz-0.3.0/asyncz/schedulers/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import sys
 from abc import ABC, abstractmethod
 from datetime import datetime, timedelta
 from importlib import import_module
 from threading import RLock
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Union
 
+from loguru import logger
+from tzlocal import get_localzone
+
 from asyncz._mapping import AsynczObjectMapping
 from asyncz.events.base import SchedulerEvent, TaskEvent, TaskSubmissionEvent
 from asyncz.events.constants import (
     ALL_EVENTS,
     ALL_TASKS_REMOVED,
     EXECUTOR_ADDED,
     EXECUTOR_REMOVED,
@@ -34,29 +37,20 @@
 from asyncz.executors.base import BaseExecutor
 from asyncz.executors.pool import ThreadPoolExecutor
 from asyncz.stores.base import BaseStore
 from asyncz.stores.memory import MemoryStore
 from asyncz.tasks import Task
 from asyncz.triggers.base import BaseTrigger
 from asyncz.typing import undefined
-from asyncz.utils import (
-    TIMEOUT_MAX,
-    maybe_ref,
-    timedelta_seconds,
-    to_bool,
-    to_int,
-    to_timezone,
-)
-from loguru import logger
-from tzlocal import get_localzone
+from asyncz.utils import TIMEOUT_MAX, maybe_ref, timedelta_seconds, to_bool, to_int, to_timezone
 
 try:
     from collections.abc import MutableMapping
 except ImportError:
-    from collections import MutableMapping
+    from collections.abc import MutableMapping
 
 from asyncz.enums import PluginInstance, SchedulerState
 from asyncz.schedulers.datastructures import TaskDefaultStruct
 from asyncz.state import BaseStateExtra
 
 DictAny = Dict[Any, Any]
 
@@ -85,19 +79,19 @@
         state: current running state of the scheduler.
     """
 
     def __init__(self, global_config: Optional["DictAny"] = None, **kwargs: "DictAny") -> None:
         super().__init__(**kwargs)
         mapping = AsynczObjectMapping()
         self.global_config = global_config or {}
-        self.trigger_plugins = dict((k, v) for k, v in mapping.triggers.items())
+        self.trigger_plugins = dict(mapping.triggers.items())
         self.trigger_classes = {}
-        self.executor_plugins = dict((k, v) for k, v in mapping.executors.items())
+        self.executor_plugins = dict(mapping.executors.items())
         self.executor_classes = {}
-        self.store_plugins = dict((k, v) for k, v in mapping.stores.items())
+        self.store_plugins = dict(mapping.stores.items())
         self.store_classes = {}
         self.executors = {}
         self.executor_lock = self.create_lock()
         self.stores = {}
         self.store_lock = self.create_lock()
         self.listeners = []
         self.listeners_lock = self.create_lock()
@@ -132,19 +126,19 @@
         global_config = global_config or {}
 
         if self.state != SchedulerState.STATE_STOPPED:
             raise SchedulerAlreadyRunningError()
 
         if prefix:
             prefix_length = len(prefix)
-            global_config = dict(
-                (key[prefix_length:], value)
+            global_config = {
+                key[prefix_length:]: value
                 for key, value in global_config.items()
                 if key.startswith(prefix)
-            )
+            }
 
         config = {}
         for key, value in global_config.items():
             parts = key.split(".")
             parent = config
             key = parts.pop(0)
             while parts:
@@ -408,37 +402,35 @@
             max_instances: Maximum number of concurrently running instances allowed for this task.
             next_run_time: When to first run the task, regardless of the trigger (pass
                 None to add the task as paused).
             store: Alias of the task store to store the task in.
             executor: Alias of the executor to run the task with.
             replace_existing: True to replace an existing task with the same id (but retain the number of runs from the existing one).
         """
-        task_struct = dict(
-            trigger=self.create_trigger(trigger, trigger_args),
-            executor=executor,
-            fn=fn,
-            args=tuple(args) if args is not None else (),
-            kwargs=dict(kwargs) if kwargs is not None else {},
-            id=id,
-            name=name,
-            mistrigger_grace_time=mistrigger_grace_time,
-            coalesce=coalesce,
-            max_instances=max_instances,
-            next_run_time=next_run_time,
-        )
-        task_kwargs = dict(
-            (key, value) for key, value in task_struct.items() if value is not undefined
-        )
+        task_struct = {
+            "trigger": self.create_trigger(trigger, trigger_args),
+            "executor": executor,
+            "fn": fn,
+            "args": tuple(args) if args is not None else (),
+            "kwargs": dict(kwargs) if kwargs is not None else {},
+            "id": id,
+            "name": name,
+            "mistrigger_grace_time": mistrigger_grace_time,
+            "coalesce": coalesce,
+            "max_instances": max_instances,
+            "next_run_time": next_run_time,
+        }
+        task_kwargs = {key: value for key, value in task_struct.items() if value is not undefined}
         task = Task(self, **task_kwargs)
 
         with self.store_lock:
             if self.state == SchedulerState.STATE_STOPPED:
                 self.pending_tasks.append((task, store, replace_existing))
                 self.logger.info(
-                    f"Adding task tentatively. It will be properly scheduled when the scheduler starts."
+                    "Adding task tentatively. It will be properly scheduled when the scheduler starts."
                 )
             else:
                 self.real_add_task(task, store, replace_existing)
         return task
 
     def scheduled_task(
         self,
@@ -751,39 +743,39 @@
 
         Args:
             alias: The alias for the instance.
         """
         try:
             return self.executors[alias]
         except KeyError:
-            raise KeyError(f"No such executor: {alias}.")
+            raise KeyError(f"No such executor: {alias}.") from None
 
     def lookup_store(self, alias: str) -> "StoreType":
         """
         Returns the task store instance by the given name from the list of task stores that were
         added to this scheduler.
 
         Args:
             alias: The alias for the instance.
         """
         try:
             return self.stores[alias]
         except KeyError:
-            raise KeyError(f"No such store: {alias}.")
+            raise KeyError(f"No such store: {alias}.") from None
 
     def lookup_task(self, task_id: Union[str, int], store_alias: str) -> Any:
         """
         Finds a task by its ID.
 
         Args:
             task_id: The id of the task to lookup.
             alias: Alias of a task store to look in.
         """
         if self.state == SchedulerState.STATE_STOPPED:
-            for task, alias, replace_existing in self.pending_tasks:
+            for task, _, _ in self.pending_tasks:
                 if task.id == task_id:
                     return task, None
         else:
             for alias, store in self.stores.items():
                 if store_alias in (None, alias):
                     task = store.lookup_task(task_id)
                     if task is not None:
@@ -895,17 +887,17 @@
                 # plugin_cls = class_container[alias] = plugin_container[alias].load()
                 plugin_cls = class_container[alias] = self.resolve_load_plugin(
                     plugin_container[alias]
                 )
                 if not issubclass(plugin_cls, base_class):
                     raise TypeError(
                         f"The {format(_type)} entry point does not point to a {format(_type)} class."
-                    )
+                    ) from None
             else:
-                raise LookupError(f"No {_type} by the name '{alias}' was found.")
+                raise LookupError(f"No {_type} by the name '{alias}' was found.") from None
 
         return plugin_cls(**constructor_args)
 
     def create_trigger(self, trigger: "TriggerType", trigger_args: "DictAny") -> Any:
         """
         Creates a trigger.
         """
```

### Comparing `asyncz-0.2.0/asyncz/schedulers/datastructures.py` & `asyncz-0.3.0/asyncz/schedulers/datastructures.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from datetime import datetime
 from typing import Any, Callable, Optional, Union
 
+from pydantic import BaseModel
+
 from asyncz.triggers.types import TriggerType
 from asyncz.typing import DictAny, UndefinedType
-from pydantic import BaseModel
 
 
 class BaseStruct(BaseModel):
     class Config:
         arbitrary_types_allowed = True
```

### Comparing `asyncz-0.2.0/asyncz/stores/base.py` & `asyncz-0.3.0/asyncz/stores/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from abc import ABC, abstractmethod
 from datetime import datetime
 from typing import TYPE_CHECKING, Any, List, Optional, Union
 
+from loguru import logger
+
 from asyncz.state import BaseStateExtra
 from asyncz.typing import DictAny
-from loguru import logger
 
 if TYPE_CHECKING:
     from asyncz.tasks.types import TaskType
 
 
 class BaseStore(BaseStateExtra, ABC):
     """
```

### Comparing `asyncz-0.2.0/asyncz/stores/memory.py` & `asyncz-0.3.0/asyncz/stores/memory.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.2.0/asyncz/stores/mongo.py` & `asyncz-0.3.0/asyncz/stores/mongo.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import pickle
 from datetime import datetime
 from typing import Any, List, Optional, Union
 
 from asyncz.exceptions import ConflictIdError, TaskLookupError
+from asyncz.stores.base import BaseStore
 from asyncz.tasks import Task
 from asyncz.tasks.types import TaskType
-from asyncz.stores.base import BaseStore
 from asyncz.typing import DictAny
 from asyncz.utils import datetime_to_utc_timestamp, maybe_ref, utc_timestamp_to_datetime
 
 try:
     from bson.binary import Binary
     from pymongo import ASCENDING, MongoClient
     from pymongo.errors import DuplicateKeyError
 except ImportError:
-    raise ImportError("MongoDBStore requires pymongo to be installed")
+    raise ImportError("MongoDBStore requires pymongo to be installed") from None
 
 
 class MongoDBStore(BaseStore):
     """
     Stores tasks in a Mongo database instance. Any remaining kwargs are passing directly to the mongo client.
 
     Args:
@@ -71,15 +71,15 @@
         return task
 
     def get_due_tasks(self, now: datetime) -> List["Task"]:
         timestamp = datetime_to_utc_timestamp(now)
         return self.get_tasks({"next_run_time": {"$lte": timestamp}})
 
     def get_tasks(self, conditions: DictAny) -> List["Task"]:
-        tasks: List["Taskkk"] = []
+        tasks: List["Task"] = []
         failed_task_ids = []
 
         for document in self.collection.find(
             conditions, ["_id", "state"], sort=[("next_run_time", ASCENDING)]
         ):
             try:
                 tasks.append(self.rebuild_task(document["state"]))
@@ -112,15 +112,15 @@
                 {
                     "_id": task.id,
                     "next_run_time": datetime_to_utc_timestamp(task.next_run_time),
                     "state": Binary(pickle.dumps(task.__getstate__(), self.pickle_protocol)),
                 }
             )
         except DuplicateKeyError:
-            raise ConflictIdError(task.id)
+            raise ConflictIdError(task.id) from None
 
     def update_task(self, task: "TaskType"):
         updates = {
             "next_run_time": datetime_to_utc_timestamp(task.next_run_time),
             "state": Binary(pickle.dumps(task.__getstate__(), self.pickle_protocol)),
         }
         result = self.collection.update_one({"_id": task.id}, {"$set": updates})
@@ -135,8 +135,8 @@
     def remove_all_tasks(self):
         self.collection.delete_many({})
 
     def shutdown(self):
         self.client.close()
 
     def __repr__(self):
-        return "<%s (client=%s)>" % (self.__class__.__name__, self.client)
+        return "<{} (client={})>".format(self.__class__.__name__, self.client)
```

### Comparing `asyncz-0.2.0/asyncz/stores/redis.py` & `asyncz-0.3.0/asyncz/stores/redis.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import pickle
 from datetime import datetime
 from typing import Any, List, Optional, Union
 
+from pytz import utc
+
 from asyncz.exceptions import AsynczException, ConflictIdError, TaskLookupError
+from asyncz.stores.base import BaseStore
 from asyncz.tasks import Task
 from asyncz.tasks.types import TaskType
-from asyncz.stores.base import BaseStore
 from asyncz.typing import DictAny
 from asyncz.utils import datetime_to_utc_timestamp, utc_timestamp_to_datetime
-from pytz import utc
 
 try:
     from redis import Redis
 except ImportError:
-    raise ImportError("You must install redis to be able to use this store.")
+    raise ImportError("You must install redis to be able to use this store.") from None
 
 
 class RedisStore(BaseStore):
     """
     Stores tasks in a Redis instance. Any remaining kwargs are passing directly to the redis
     instance.
 
@@ -37,15 +38,17 @@
         pickle_protocol: Optional[int] = pickle.HIGHEST_PROTOCOL,
         **kwargs: DictAny,
     ):
         super().__init__(**kwargs)
         try:
             self.database = int(database)
         except (TypeError, ValueError):
-            raise AsynczException(f"The database value must be and int and got ({type(database)})")
+            raise AsynczException(
+                f"The database value must be and int and got ({type(database)})"
+            ) from None
 
         self.pickle_protocol = pickle_protocol
         self.tasks_key = tasks_key
         self.run_times_key = run_times_key
         self.redis = Redis(db=self.database, **kwargs)
 
     def lookup_task(self, task_id: Union[str, int]) -> "TaskType":
```

### Comparing `asyncz-0.2.0/asyncz/tasks/base.py` & `asyncz-0.3.0/asyncz/tasks/base.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.2.0/asyncz/triggers/base.py` & `asyncz-0.3.0/asyncz/triggers/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     from asyncz.triggers.types import TriggerType
 
 
 class BaseTrigger(BaseStateExtra, ABC):
     """
     Base model defining the protocol for every trigger.
     """
+
     alias: Optional[str] = None
 
     @abstractmethod
     def get_next_trigger_time(
         self, previous_time: datetime, now: Optional[datetime] = None
     ) -> Union[datetime, None]:
         """
```

### Comparing `asyncz-0.2.0/asyncz/triggers/combination.py` & `asyncz-0.3.0/asyncz/triggers/combination.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.2.0/asyncz/triggers/date.py` & `asyncz-0.3.0/asyncz/triggers/date.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from datetime import datetime, tzinfo
 from typing import Any, Dict, Optional, Union
 
+from tzlocal import get_localzone
+
 from asyncz.datastructures import DateState
 from asyncz.triggers.base import BaseTrigger
 from asyncz.typing import DictAny
 from asyncz.utils import datetime_repr, to_datetime, to_timezone
-from tzlocal import get_localzone
 
 
 class DateTrigger(BaseTrigger):
     """
     Triggers once on the given datetime. If run_at is left empty then the current time is used.
 
     Args:
@@ -46,11 +47,11 @@
         state = DateState(run_at=self.run_at)
         return state
 
     def __str__(self) -> str:
         return "date[%s]" % datetime_repr(self.run_at)
 
     def __repr__(self) -> str:
-        return "<%s (run_at='%s')>" % (
+        return "<{} (run_at='{}')>".format(
             self.__class__.__name__,
             datetime_repr(self.run_at),
         )
```

### Comparing `asyncz-0.2.0/asyncz/triggers/interval.py` & `asyncz-0.3.0/asyncz/triggers/interval.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 from datetime import datetime, timedelta, tzinfo
 from math import ceil
 from typing import Any, Dict, Optional, Union
 
+from tzlocal import get_localzone
+
 from asyncz.datastructures import IntervalState
 from asyncz.triggers.base import BaseTrigger
 from asyncz.typing import DictAny
-from asyncz.utils import (
-    datetime_repr,
-    normalize,
-    timedelta_seconds,
-    to_datetime,
-    to_timezone,
-)
-from tzlocal import get_localzone
+from asyncz.utils import datetime_repr, normalize, timedelta_seconds, to_datetime, to_timezone
 
 
 class IntervalTrigger(BaseTrigger):
     """
     Triggers on a specific intervals, starting on start_at if specified or datetime.now() + interval otherwise.
 
     Args:
@@ -111,12 +106,12 @@
     def __repr__(self) -> str:
         options = ["interval=%r" % self.interval, "start_at=%r" % datetime_repr(self.start_at)]
         if self.end_at:
             options.append("end_at=%r" % datetime_repr(self.end_at))
         if self.jitter:
             options.append("jitter=%s" % self.jitter)
 
-        return "<%s (%s, timezone='%s')>" % (
+        return "<{} ({}, timezone='{}')>".format(
             self.__class__.__name__,
             ", ".join(options),
             self.timezone,
         )
```

### Comparing `asyncz-0.2.0/asyncz/triggers/cron/constants.py` & `asyncz-0.3.0/asyncz/triggers/cron/constants.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.2.0/asyncz/triggers/cron/expressions.py` & `asyncz-0.3.0/asyncz/triggers/cron/expressions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 import re
 from calendar import monthrange
 from datetime import date, datetime
 from typing import TYPE_CHECKING, Any, ClassVar, Dict, Optional, Union
 
-from asyncz.triggers.cron.constants import (
-    MAX_VALUES,
-    MIN_VALUES,
-    MONTHS,
-    OPTIONS,
-    WEEKDAYS,
-)
-from asyncz.utils import to_int
 from pydantic import BaseModel
 
+from asyncz.triggers.cron.constants import MAX_VALUES, MIN_VALUES, MONTHS, OPTIONS, WEEKDAYS
+from asyncz.utils import to_int
+
 if TYPE_CHECKING:
     from asyncz.triggers.cron.types import FieldType
 
 
 class BaseExpression(BaseModel):
     class Config:
         arbitrary_types_allowed = True
@@ -30,41 +25,41 @@
     def __init__(self, step: Optional[Union[int, float]] = None, **kwargs: Dict[str, Any]):
         super().__init__(**kwargs)
         if step:
             self.step = to_int(step)
             if self.step == 0:
                 raise ValueError("Increment must be higher than 0.")
 
-    def validate_range(self, field_name: str):
+    def validate_range(self, field_name: str) -> None:
         value_range = MAX_VALUES[field_name] - MIN_VALUES[field_name]
         if self.step and self.step > value_range:
             raise ValueError(
                 f"The step value ({self.step}) is higher than the total range of the "
                 f"expression ({value_range})."
             )
 
-    def get_next_value(self, date: Union[date, datetime], field: "FieldType"):
-        start = field.get_value(date)
-        min_value = field.get_min(date)
-        max_value = field.get_max(date)
+    def get_next_value(self, date: Union[date, datetime], field: "FieldType") -> Any:
+        start = field.get_value(date)  # type: ignore
+        min_value = field.get_min(date)  # type: ignore
+        max_value = field.get_max(date)  # type: ignore
         start = max(start, min_value)
 
         if not self.step:
             next = start
         else:
             distance_to_next = (self.step - (start - min_value)) % self.step
-            next = start + distance_to_next
+            next = start + distance_to_next  # type: ignore
 
         if next <= max_value:
             return next
 
     def __eq__(self, other: Any) -> bool:
         return isinstance(other, self.__class__) and self.step == other.step
 
-    def __str__(self):
+    def __str__(self) -> str:
         if self.step:
             return "*/%d" % self.step
         return "*"
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}({self.step})"
 
@@ -80,25 +75,25 @@
         first: Union[str, float],
         last: Optional[Union[str, float]] = None,
         step: Optional[Union[int, float]] = None,
         **kwargs: Dict[str, Any],
     ):
         super().__init__(step=step, **kwargs)
         first = to_int(first)
-        last = to_int(last)
+        last = to_int(last)  # type: ignore
 
         if last is None and self.step is None:
             last = first
-        if last is not None and first > last:
+        if last is not None and first > last:  # type: ignore
             raise ValueError("The minimum value in a range must not be higher than the maximum.")
 
-        self.first = first
-        self.last = last
+        self.first: int = first
+        self.last: int = last
 
-    def validate_range(self, field_name: str):
+    def validate_range(self, field_name: str) -> None:
         super().validate_range(field_name)
 
         if self.first < MIN_VALUES[field_name]:
             raise ValueError(
                 f"The first value ({self.first}) is lower than the minimum value ({MIN_VALUES[field_name]})."
             )
 
@@ -111,37 +106,37 @@
 
         if self.step and self.step > value_range:
             raise ValueError(
                 f"The step value ({self.step}) is higher than the total range of the "
                 f"expression ({value_range})."
             )
 
-    def get_next_value(self, date: Union[date, datetime], field: "FieldType"):
-        start_value = field.get_value(date)
-        min_value = field.get_min(date)
-        max_value = field.get_max(date)
+    def get_next_value(self, date: Union[date, datetime], field: "FieldType") -> Union[int, None]:
+        start_value = field.get_value(date)  # type: ignore
+        min_value = field.get_min(date)  # type: ignore
+        max_value = field.get_max(date)  # type: ignore
 
         min_value = max(min_value, self.first)
         max_value = min(max_value, self.last) if self.last is not None else max_value
         next_value = max(min_value, start_value)
 
         if self.step:
             distance_to_next = (self.step - (next_value - min_value)) % self.step
-            next_value += distance_to_next
+            next_value += distance_to_next  # type: ignore
 
         return next_value if next_value <= max_value else None
 
-    def __eq__(self, other: Any):
+    def __eq__(self, other: Any) -> bool:
         return (
             isinstance(other, self.__class__)
             and self.first == other.first
             and self.last == other.last
         )
 
-    def __str__(self):
+    def __str__(self) -> str:
         if self.last != self.first and self.last is not None:
             range = "%d-%d" % (self.first, self.last)
         else:
             range = str(self.first)
 
         if self.step:
             return "%s/%d" % (range, self.step)
@@ -162,34 +157,40 @@
     )
     step: Optional[Union[int, float]]
 
     def __init__(
         self,
         first: Union[str, float],
         last: Optional[Union[str, float]] = None,
-        **kwargs: Dict[str, Any],
-    ):
+        **kwargs: Any,
+    ) -> None:
+        if isinstance(first, float):
+            first = str(first)
+
         try:
             first_number = MONTHS.index(first.lower()) + 1
         except ValueError:
-            raise ValueError(f"Invalid month name '{first}'.")
+            raise ValueError(f"Invalid month name '{first}'.") from None
 
         if not last:
             last_number = None
         else:
+            if isinstance(last, float):
+                last = str(last)
+
             try:
                 last_number = MONTHS.index(last.lower()) + 1
             except ValueError:
-                raise ValueError(f"Invalid month name '{last}'.")
+                raise ValueError(f"Invalid month name '{last}'.") from None
 
         super().__init__(first_number, last_number, **kwargs)
 
-    def __str__(self):
+    def __str__(self) -> str:
         if self.last != self.first and self.last is not None:
-            return "%s-%s" % (MONTHS[self.first - 1], MONTHS[self.last - 1])
+            return "{}-{}".format(MONTHS[self.first - 1], MONTHS[self.last - 1])
         return MONTHS[self.first - 1]
 
     def __repr__(self) -> str:
         args = ["'%s'" % MONTHS[self.first]]
         if self.last != self.first and self.last is not None:
             args.append("'%s'" % MONTHS[self.last - 1])
         return f"{self.__class__.__name__}({', '.join(args)})"
@@ -200,33 +201,39 @@
         r"(?P<first>[a-z]+)(?:-(?P<last>[a-z]+))?", re.IGNORECASE
     )
 
     def __init__(
         self,
         first: Union[str, float],
         last: Optional[Union[str, float]] = None,
-        **kwargs: Dict[str, Any],
+        **kwargs: Any,
     ):
+        if isinstance(first, float):
+            first = str(first)
+
         try:
             first_number = WEEKDAYS.index(first.lower())
         except ValueError:
-            raise ValueError(f"Invalid weekday name '{first}'.")
+            raise ValueError(f"Invalid weekday name '{first}'.") from None
 
         if not last:
             last_number = None
         else:
+            if isinstance(last, float):
+                last = str(last)
+
             try:
                 last_number = WEEKDAYS.index(last.lower())
             except ValueError:
-                raise ValueError(f"Invalid weekday name '{last}'")
+                raise ValueError(f"Invalid weekday name '{last}'") from None
         super().__init__(first_number, last_number, **kwargs)
 
-    def __str__(self):
+    def __str__(self) -> str:
         if self.last != self.first and self.last is not None:
-            return "%s-%s" % (WEEKDAYS[self.first], WEEKDAYS[self.last])
+            return "{}-{}".format(WEEKDAYS[self.first], WEEKDAYS[self.last])
         return WEEKDAYS[self.first]
 
     def __repr__(self) -> str:
         args = ["'%s'" % WEEKDAYS[self.first]]
         if self.last != self.first and self.last is not None:
             args.append("'%s'" % WEEKDAYS[self.last])
         return f"{self.__class__.__name__}({', '.join(args)})"
@@ -238,60 +245,62 @@
     )
 
     def __init__(self, option_name: str, weekday_name: str, **kwargs: Dict[str, Any]):
         super().__init__(step=None, **kwargs)
         try:
             self.option_number = OPTIONS.index(option_name.lower())
         except ValueError:
-            raise ValueError(f'Invalid weekday position "{option_name}".')
+            raise ValueError(f'Invalid weekday position "{option_name}".') from None
 
         try:
             self.weekday = WEEKDAYS.index(weekday_name.lower())
         except ValueError:
-            raise ValueError(f'Invalid weekday name "{weekday_name}".')
+            raise ValueError(f'Invalid weekday name "{weekday_name}".') from None
 
-    def get_next_value(self, date: Union[date, datetime], field: "FieldType"):
+    def get_next_value(  # type: ignore
+        self, date: Union[date, datetime], field: "FieldType"
+    ) -> Union[float, int]:
         first_day_wday, last_day = monthrange(date.year, date.month)
 
         first_hit_day = self.weekday - first_day_wday + 1
         if first_hit_day <= 0:
             first_hit_day += 7
 
         if self.option_number < 5:
             target_day = first_hit_day + self.option_number * 7
         else:
             target_day = first_hit_day + ((last_day - first_hit_day) // 7) * 7
 
         if target_day <= last_day and target_day >= date.day:
             return target_day
 
-    def __eq__(self, other: Any):
+    def __eq__(self, other: Any) -> bool:
         return (
             super().__eq__(other)
             and self.option_number == other.option_num
             and self.weekday == other.weekday
         )
 
-    def __str__(self):
-        return "%s %s" % (OPTIONS[self.option_number], WEEKDAYS[self.weekday])
+    def __str__(self) -> str:
+        return "{} {}".format(OPTIONS[self.option_number], WEEKDAYS[self.weekday])
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return (
             f"{self.__class__.__name__}('{OPTIONS[self.option_number]}"
             f"', '{WEEKDAYS[self.weekday]}')"
         )
 
 
 class LastDayOfMonthExpression(AllExpression):
     regex: ClassVar[re.Pattern] = re.compile(r"last", re.IGNORECASE)
 
-    def __init__(self, **kwargs: Dict[str, Any]):
+    def __init__(self, **kwargs: Dict[str, Any]) -> None:
         super().__init__(step=None, **kwargs)
 
-    def get_next_value(self, date: Union[date, datetime], field: "FieldType"):
+    def get_next_value(self, date: Union[date, datetime], field: "FieldType"):  # type: ignore
         return monthrange(date.year, date.month)[1]
 
-    def __str__(self):
+    def __str__(self) -> str:
         return "last"
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"{self.__class__.__name__}()"
```

### Comparing `asyncz-0.2.0/asyncz/triggers/cron/fields.py` & `asyncz-0.3.0/asyncz/triggers/cron/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import re
 from calendar import monthrange
 from datetime import datetime
 from typing import Any, Dict, List, Optional
 
-from asyncz.triggers.cron.constants import MAX_VALUES, MIN_VALUES
 from pydantic import BaseModel
 
-SEPARATOR = re.compile(" *, *")
-
+from asyncz.triggers.cron.constants import MAX_VALUES, MIN_VALUES
 from asyncz.triggers.cron.expressions import (
     AllExpression,
     LastDayOfMonthExpression,
     MonthRangeExpression,
     RangeExpression,
     WeekdayPositionExpression,
     WeekdayRangeExpression,
 )
 
+SEPARATOR = re.compile(" *, *")
+
 
 class BaseField(BaseModel):
     name: Optional[str]
     exprs: Optional[Any]
     is_default: Optional[bool]
     expressions: Optional[List[Any]]
     compilers: Optional[List[Any]]
@@ -79,25 +79,25 @@
                     compiled_expr.validate_range(self.name)
                 except ValueError as e:
                     message = "Error validating expression {!r}: {}".format(expr, e)
                     raise ValueError(message) from e
                 self.expressions.append(compiled_expr)
                 return
 
-        raise ValueError('Unrecognized expression "%s" for field "%s"' % (expr, self.name))
+        raise ValueError('Unrecognized expression "{}" for field "{}"'.format(expr, self.name))
 
     def __eq__(self, other):
         return isinstance(self, self.__class__) and self.expressions == other.expressions
 
     def __str__(self):
         expr_strings = (str(e) for e in self.expressions)
         return ",".join(expr_strings)
 
     def __repr__(self):
-        return "%s('%s', '%s')" % (self.__class__.__name__, self.name, self)
+        return "{}('{}', '{}')".format(self.__class__.__name__, self.name, self)
 
     class Config:
         arbitrary_types_allowed = True
 
 
 class WeekField(BaseField):
     def __init__(
```

### Comparing `asyncz-0.2.0/asyncz/triggers/cron/trigger.py` & `asyncz-0.3.0/asyncz/triggers/cron/trigger.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from datetime import datetime, timedelta, tzinfo
 from typing import Any, Dict, Optional, Union
 
+from tzlocal import get_localzone
+
 from asyncz.datastructures import CronState
 from asyncz.triggers.base import BaseTrigger
 from asyncz.triggers.cron.constants import DEFAULT_VALUES
 from asyncz.triggers.cron.fields import (
     BaseField,
     DayOfMonthField,
     DayOfWeekField,
@@ -16,15 +18,14 @@
     datetime_ceil,
     datetime_repr,
     localize,
     normalize,
     to_datetime,
     to_timezone,
 )
-from tzlocal import get_localzone
 
 
 class CronTrigger(BaseTrigger):
     """
     Triggers when the current time matches all specified time constraints. Very simlar to the way
     UNIX cron scheduler works.
 
@@ -113,19 +114,19 @@
         else:
             self.timezone = get_localzone()
 
         self.start_at = to_datetime(start_at, self.timezone, "start_at")
         self.end_at = to_datetime(end_at, self.timezone, "end_at")
         self.jitter = jitter
 
-        values = dict(
-            (key, value)
+        values = {
+            key: value
             for key, value in iter(locals().items())
             if key in self.field_names and value is not None
-        )
+        }
 
         self.fields = []
         assign_defaults = False
 
         for field_name in self.field_names:
             if field_name in values:
                 expressions = values.pop(field_name)
```

### Comparing `asyncz-0.2.0/LICENSE` & `asyncz-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncz-0.2.0/README.md` & `asyncz-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Asyncz
 
 <p align="center">
-  <a href="https://asyncz.tarsil.io"><img src="https://res.cloudinary.com/dymmond/image/upload/v1671461421/asyncz/asyncz-bg_bapqg1.png" alt='Asyncz'></a>
+  <a href="https://asyncz.tarsil.io"><img src="https://res.cloudinary.com/tarsild/image/upload/v1687363326/packages/asyncz/asyncz-new_wiyih8.png" alt='Asyncz'></a>
 </p>
 
 <p align="center">
     <em>🚀 The scheduler that simply works. 🚀</em>
 </p>
 
 <p align="center">
```

### Comparing `asyncz-0.2.0/PKG-INFO` & `asyncz-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: asyncz
-Version: 0.2.0
+Version: 0.3.0
 Summary: The scheduler that nobody wants but every application needs.
 Project-URL: Homepage, https://github.com/tarsil/asyncz
 Project-URL: Documentation, https://asyncz.tarsild.io/
 Project-URL: Changelog, https://asyncz.tarsild.io/release-notes/
 Project-URL: Funding, https://github.com/sponsors/tarsil
 Project-URL: Source, https://github.com/tarsil/asyncz
 Author-email: Tiago Silva <tiago.arasilva@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
-Keywords: api,apscheduler,asgi,cron,esmerald,fastapi,framework,http,machine learning,ml,openapi,pydantic,rest,scheduler,starlette,websocket
+Keywords: api,apscheduler,asgi,asyncz,cron,fastapi,framework,http,machine learning,ml,openapi,pydantic,rest,scheduler,starlette,websocket
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: AnyIO
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
@@ -34,15 +34,15 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: asyncio<4.0.0,>=3.4.3
 Requires-Dist: loguru<0.7.0,>=0.6.0
-Requires-Dist: pydantic<2.0.0,>=1.10.5
+Requires-Dist: pydantic<2.0.0,>=1.10.9
 Requires-Dist: pytz>=2022.6
 Requires-Dist: tzlocal<5.0,>=4.2
 Provides-Extra: all
 Requires-Dist: asyncio<4.0.0,>=3.4.3; extra == 'all'
 Requires-Dist: pydantic<2.0.0,>=1.10.5; extra == 'all'
 Requires-Dist: pytz>=2022.6; extra == 'all'
 Requires-Dist: tzlocal<5.0,>=4.2; extra == 'all'
@@ -69,20 +69,21 @@
 Requires-Dist: pymongo<5.0.0,>=4.3.3; extra == 'test'
 Requires-Dist: pytest-asyncio<1.0.0,>=0.19.0; extra == 'test'
 Requires-Dist: pytest-cov<5.0.0,>=2.12.0; extra == 'test'
 Requires-Dist: pytest-loguru<1,>=0.2.0; extra == 'test'
 Requires-Dist: pytest<8.0.0,>=7.1.3; extra == 'test'
 Requires-Dist: redis<5.0.0,>=4.4.0; extra == 'test'
 Requires-Dist: requests<3.0.0,>=2.27.0; extra == 'test'
+Requires-Dist: ruff<1.0.0,>=0.0.256; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Asyncz
 
 <p align="center">
-  <a href="https://asyncz.tarsil.io"><img src="https://res.cloudinary.com/dymmond/image/upload/v1671461421/asyncz/asyncz-bg_bapqg1.png" alt='Asyncz'></a>
+  <a href="https://asyncz.tarsil.io"><img src="https://res.cloudinary.com/tarsild/image/upload/v1687363326/packages/asyncz/asyncz-new_wiyih8.png" alt='Asyncz'></a>
 </p>
 
 <p align="center">
     <em>🚀 The scheduler that simply works. 🚀</em>
 </p>
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: asyncz Version: 0.2.0 Summary: The scheduler that
+Metadata-Version: 2.1 Name: asyncz Version: 0.3.0 Summary: The scheduler that
 nobody wants but every application needs. Project-URL: Homepage, https://
 github.com/tarsil/asyncz Project-URL: Documentation, https://asyncz.tarsild.io/
 Project-URL: Changelog, https://asyncz.tarsild.io/release-notes/ Project-URL:
 Funding, https://github.com/sponsors/tarsil Project-URL: Source, https://
 github.com/tarsil/asyncz Author-email: Tiago Silva
 arasilva@gmail.com> License-Expression: MIT License-File: LICENSE Keywords:
-api,apscheduler,asgi,cron,esmerald,fastapi,framework,http,machine
+api,apscheduler,asgi,asyncz,cron,fastapi,framework,http,machine
 learning,ml,openapi,pydantic,rest,scheduler,starlette,websocket Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Web Environment
 Classifier: Framework :: AnyIO Classifier: Framework :: AsyncIO Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Information
 Technology Classifier: Intended Audience :: System Administrators Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
 Internet Classifier: Topic :: Internet :: WWW/HTTP Classifier: Topic ::
 Internet :: WWW/HTTP :: HTTP Servers Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
 Software Development :: Libraries :: Application Frameworks Classifier: Topic
 :: Software Development :: Libraries :: Python Modules Classifier: Typing ::
 Typed Requires-Python: >=3.8 Requires-Dist: asyncio<4.0.0,>=3.4.3 Requires-
-Dist: loguru<0.7.0,>=0.6.0 Requires-Dist: pydantic<2.0.0,>=1.10.5 Requires-
+Dist: loguru<0.7.0,>=0.6.0 Requires-Dist: pydantic<2.0.0,>=1.10.9 Requires-
 Dist: pytz>=2022.6 Requires-Dist: tzlocal<5.0,>=4.2 Provides-Extra: all
 Requires-Dist: asyncio<4.0.0,>=3.4.3; extra == 'all' Requires-Dist:
 pydantic<2.0.0,>=1.10.5; extra == 'all' Requires-Dist: pytz>=2022.6; extra ==
 'all' Requires-Dist: tzlocal<5.0,>=4.2; extra == 'all' Provides-Extra: dev
 Requires-Dist: autoflake<3.0.0,>=1.4.0; extra == 'dev' Requires-Dist:
 black<23.0.0,>=22.10.0; extra == 'dev' Requires-Dist: flake8<7.0.0,>=3.8.3;
 extra == 'dev' Requires-Dist: isort<6.0.0,>=5.0.6; extra == 'dev' Requires-
@@ -42,16 +42,16 @@
 Requires-Dist: pyyaml<7.0.0,>=6.0; extra == 'doc' Provides-Extra: test
 Requires-Dist: esmerald==0.4.2; extra == 'test' Requires-Dist: mock>=4.0.3;
 extra == 'test' Requires-Dist: pymongo<5.0.0,>=4.3.3; extra == 'test' Requires-
 Dist: pytest-asyncio<1.0.0,>=0.19.0; extra == 'test' Requires-Dist: pytest-
 cov<5.0.0,>=2.12.0; extra == 'test' Requires-Dist: pytest-loguru<1,>=0.2.0;
 extra == 'test' Requires-Dist: pytest<8.0.0,>=7.1.3; extra == 'test' Requires-
 Dist: redis<5.0.0,>=4.4.0; extra == 'test' Requires-Dist:
-requests<3.0.0,>=2.27.0; extra == 'test' Description-Content-Type: text/
-markdown # Asyncz
+requests<3.0.0,>=2.27.0; extra == 'test' Requires-Dist: ruff<1.0.0,>=0.0.256;
+extra == 'test' Description-Content-Type: text/markdown # Asyncz
                                    [Asyncz]
                   ð The scheduler that simply works. ð
           [Test_Suite] [Package_version] [Supported_Python_versions]
 --- **Documentation**: [https://asyncz.tarsild.io](https://asyncz.tarsild.io)
 ð **Source Code**: [https://github.com/tarsil/asyncz](https://github.com/
 tarsil/asyncz) --- Asyncz is a scheduler for any ASGI application that needs to
 have those complicated scheduled operations with the best of what pydantic can
```


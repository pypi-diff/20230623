# Comparing `tmp/pydantic_xml-0.6.3.tar.gz` & `tmp/pydantic_xml-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_xml-0.6.3.tar", max compression
+gzip compressed data, was "pydantic_xml-0.7.0.tar", max compression
```

## Comparing `pydantic_xml-0.6.3.tar` & `pydantic_xml-0.7.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1211 2023-06-19 19:13:40.945762 pydantic_xml-0.6.3/LICENSE
--rw-r--r--   0        0        0     3182 2023-06-19 19:13:40.945762 pydantic_xml-0.6.3/README.rst
--rw-r--r--   0        0        0      599 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/__init__.py
--rw-r--r--   0        0        0      489 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/config.py
--rw-r--r--   0        0        0       80 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/element/__init__.py
--rw-r--r--   0        0        0    12576 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/element/element.py
--rw-r--r--   0        0        0      364 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/element/native/__init__.py
--rw-r--r--   0        0        0     1671 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/element/native/lxml.py
--rw-r--r--   0        0        0     1173 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/element/native/std.py
--rw-r--r--   0        0        0      569 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/errors.py
--rw-r--r--   0        0        0    11526 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/model.py
--rw-r--r--   0        0        0        0 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/py.typed
--rw-r--r--   0        0        0       73 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/serializers/__init__.py
--rw-r--r--   0        0        0     1445 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/serializers/encoder.py
--rw-r--r--   0        0        0      394 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/serializers/factories/__init__.py
--rw-r--r--   0        0        0     1898 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/serializers/factories/forwardref.py
--rw-r--r--   0        0        0     4612 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/serializers/factories/heterogeneous.py
--rw-r--r--   0        0        0     4337 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/serializers/factories/homogeneous.py
--rw-r--r--   0        0        0     4732 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/serializers/factories/mapping.py
--rw-r--r--   0        0        0     7057 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/serializers/factories/model.py
--rw-r--r--   0        0        0     4220 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/serializers/factories/primitive.py
--rw-r--r--   0        0        0     6555 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/serializers/factories/union.py
--rw-r--r--   0        0        0     3292 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/serializers/factories/wrapper.py
--rw-r--r--   0        0        0     7364 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/serializers/serializer.py
--rw-r--r--   0        0        0       48 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/typedefs.py
--rw-r--r--   0        0        0     2131 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pydantic_xml/utils.py
--rw-r--r--   0        0        0     1849 2023-06-19 19:13:40.949762 pydantic_xml-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     4687 1970-01-01 00:00:00.000000 pydantic_xml-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-06-23 20:11:44.107379 pydantic_xml-0.7.0/LICENSE
+-rw-r--r--   0        0        0     3182 2023-06-23 20:11:44.107379 pydantic_xml-0.7.0/README.rst
+-rw-r--r--   0        0        0      599 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/__init__.py
+-rw-r--r--   0        0        0      489 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/config.py
+-rw-r--r--   0        0        0       80 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/element/__init__.py
+-rw-r--r--   0        0        0    13091 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/element/element.py
+-rw-r--r--   0        0        0      374 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/element/native/__init__.py
+-rw-r--r--   0        0        0     1671 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/element/native/lxml.py
+-rw-r--r--   0        0        0     1173 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/element/native/std.py
+-rw-r--r--   0        0        0      569 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/errors.py
+-rw-r--r--   0        0        0    11708 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/model.py
+-rw-r--r--   0        0        0        0 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/py.typed
+-rw-r--r--   0        0        0       73 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/serializers/__init__.py
+-rw-r--r--   0        0        0     1445 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/serializers/encoder.py
+-rw-r--r--   0        0        0      394 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/serializers/factories/__init__.py
+-rw-r--r--   0        0        0     1898 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/serializers/factories/forwardref.py
+-rw-r--r--   0        0        0     4612 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/serializers/factories/heterogeneous.py
+-rw-r--r--   0        0        0     4337 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/serializers/factories/homogeneous.py
+-rw-r--r--   0        0        0     4732 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/serializers/factories/mapping.py
+-rw-r--r--   0        0        0     7057 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/serializers/factories/model.py
+-rw-r--r--   0        0        0     4220 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/serializers/factories/primitive.py
+-rw-r--r--   0        0        0     6693 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/serializers/factories/union.py
+-rw-r--r--   0        0        0     3292 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/serializers/factories/wrapper.py
+-rw-r--r--   0        0        0     7364 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/serializers/serializer.py
+-rw-r--r--   0        0        0       48 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/typedefs.py
+-rw-r--r--   0        0        0     2131 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/utils.py
+-rw-r--r--   0        0        0     1878 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     4687 1970-01-01 00:00:00.000000 pydantic_xml-0.7.0/PKG-INFO
```

### Comparing `pydantic_xml-0.6.3/LICENSE` & `pydantic_xml-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.3/README.rst` & `pydantic_xml-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.3/pydantic_xml/__init__.py` & `pydantic_xml-0.7.0/pydantic_xml/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.3/pydantic_xml/element/element.py` & `pydantic_xml-0.7.0/pydantic_xml/element/element.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import abc
 from enum import Enum
-from typing import Callable, Dict, Generic, List, Optional, Sequence, TypeVar
+from typing import Any, Callable, Dict, Generic, List, Optional, Sequence, TypeVar
 
 from pydantic_xml.typedefs import NsMap
 
 
 class XmlElementReader(abc.ABC):
     """
     Xml element data reader.
@@ -43,43 +43,43 @@
         Extracts all attribute from the xml element.
         All subsequent calls return `None`.
 
         :return: element attributes
         """
 
     @abc.abstractmethod
-    def pop_element(self, tag: str, search_mode: 'SearchMode') -> Optional['XmlElement']:
+    def pop_element(self, tag: str, search_mode: 'SearchMode') -> Optional['XmlElement[Any]']:
         """
         Extracts a sub-element from the xml element matching `tag`.
 
         :param tag: element tag
         :param search_mode: element search mode
         :return: sub-element
         """
 
     @abc.abstractmethod
-    def find_sub_element(self, path: Sequence[str], search_mode: 'SearchMode') -> Optional['XmlElement']:
+    def find_sub_element(self, path: Sequence[str], search_mode: 'SearchMode') -> Optional['XmlElement[Any]']:
         """
         Searches for an element at the provided path. If the element is not found returns `None`.
 
         :param path: path the element is searched at
         :param search_mode: element search mode
         :return: found element or `None`
         """
 
     @abc.abstractmethod
-    def create_snapshot(self) -> 'XmlElement':
+    def create_snapshot(self) -> 'XmlElement[Any]':
         """
         Creates a snapshot of the element. The snapshot can be modified not affecting the original one.
 
         :return: created snapshot
         """
 
     @abc.abstractmethod
-    def apply_snapshot(self, snapshot: 'XmlElement') -> None:
+    def apply_snapshot(self, snapshot: 'XmlElement[Any]') -> None:
         """
         Applies a snapshot to the current element.
         """
 
 
 class XmlElementWriter(abc.ABC):
     """
@@ -117,33 +117,33 @@
         """
         Sets xml element attributes.
 
         :param attributes: element attributes
         """
 
     @abc.abstractmethod
-    def append_element(self, element: 'XmlElement') -> None:
+    def append_element(self, element: 'XmlElement[Any]') -> None:
         """
         Appends a new sub-element to the xml element.
 
         :param element: sub-element to be added
         """
 
     @abc.abstractmethod
-    def make_element(self, tag: str, nsmap: Optional[NsMap]) -> 'XmlElement':
+    def make_element(self, tag: str, nsmap: Optional[NsMap]) -> 'XmlElement[Any]':
         """
         Creates an element of the current element type.
 
         :param tag: element tag
         :param nsmap: element namespace map
         :return: created element
         """
 
     @abc.abstractmethod
-    def find_element_or_create(self, tag: str, search_mode: 'SearchMode', nsmap: Optional[NsMap]) -> 'XmlElement':
+    def find_element_or_create(self, tag: str, search_mode: 'SearchMode', nsmap: Optional[NsMap]) -> 'XmlElement[Any]':
         """
         Searches for an element with the provided tag.
         If the element is found returns it otherwise creates a new one.
 
         :param tag: element tag to be found or created
         :param search_mode: element search mode
         :param nsmap: element namespace mapping
@@ -155,34 +155,36 @@
 
 
 class XmlElement(XmlElementReader, XmlElementWriter, Generic[NativeElement]):
     """
     Xml element.
     """
 
-    class State:
+    NativeElementInner = TypeVar('NativeElementInner')
+
+    class State(Generic[NativeElementInner]):
         __slots__ = ('text', 'attrib', 'elements', 'next_element_idx')
 
         def __init__(
                 self,
                 text: Optional[str],
                 attrib: Optional[Dict[str, str]],
-                elements: List['XmlElement'],
+                elements: List['XmlElement[XmlElement.NativeElementInner]'],
                 next_element_idx: int,
         ):
             self.text = text
             self.attrib = attrib
             self.elements = elements
             self.next_element_idx = next_element_idx
 
     __slots__ = ('_tag', '_nsmap')
 
     @classmethod
     @abc.abstractmethod
-    def from_native(cls, element: NativeElement) -> 'XmlElement':
+    def from_native(cls, element: NativeElement) -> 'XmlElement[NativeElement]':
         """
         Creates a instance of `XmlElement` from native element.
 
         :param element: native element
         :return: `XmlElement`
         """
 
@@ -195,15 +197,15 @@
         """
 
     def __init__(
             self,
             tag: str,
             text: Optional[str] = None,
             attributes: Optional[Dict[str, str]] = None,
-            elements: Optional[List['XmlElement']] = None,
+            elements: Optional[List['XmlElement[NativeElement]']] = None,
             nsmap: Optional[NsMap] = None,
     ):
         self._tag = tag
         self._nsmap = nsmap
         self._state = XmlElement.State(
             text=text,
             attrib=dict(attributes) if attributes is not None else None,
@@ -211,27 +213,27 @@
             next_element_idx=0,
         )
 
     @property
     def tag(self) -> str:
         return self._tag
 
-    def create_snapshot(self) -> 'XmlElement':
+    def create_snapshot(self) -> 'XmlElement[NativeElement]':
         element = self.__class__(
             tag=self._tag,
             text=self._state.text,
             attributes=dict(self._state.attrib) if self._state.attrib is not None else None,
             elements=[element.create_snapshot() for element in self._state.elements],
             nsmap=dict(self._nsmap) if self._nsmap is not None else None,
         )
         element._state.next_element_idx = self._state.next_element_idx
 
         return element
 
-    def apply_snapshot(self, snapshot: 'XmlElement') -> None:
+    def apply_snapshot(self, snapshot: 'XmlElement[NativeElement]') -> None:
         self._tag = snapshot._tag
         self._nsmap = snapshot._nsmap
         self._state.text = snapshot._state.text
         self._state.attrib = snapshot._state.attrib
         self._state.elements = snapshot._state.elements
         self._state.next_element_idx = snapshot._state.next_element_idx
 
@@ -249,53 +251,60 @@
             self._state.attrib = {}
 
         self._state.attrib[name] = value
 
     def set_attributes(self, attributes: Dict[str, str]) -> None:
         self._state.attrib = dict(attributes)
 
-    def append_element(self, element: 'XmlElement') -> None:
+    def append_element(self, element: 'XmlElement[NativeElement]') -> None:
         self._state.elements.append(element)
+        self._state.next_element_idx += 1
 
     def pop_text(self) -> Optional[str]:
         result, self._state.text = self._state.text, None
 
         return result
 
     def pop_attrib(self, name: str) -> Optional[str]:
         return self._state.attrib.pop(name, None) if self._state.attrib else None
 
     def pop_attributes(self) -> Optional[Dict[str, str]]:
         result, self._state.attrib = self._state.attrib, None
 
         return result
 
-    def pop_element(self, tag: str, search_mode: 'SearchMode') -> Optional['XmlElement']:
+    def pop_element(self, tag: str, search_mode: 'SearchMode') -> Optional['XmlElement[NativeElement]']:
         searcher = get_searcher(search_mode)
 
         return searcher(self._state, tag, False)
 
-    def find_sub_element(self, path: Sequence[str], search_mode: 'SearchMode') -> Optional['XmlElement']:
+    def find_sub_element(self, path: Sequence[str], search_mode: 'SearchMode') -> Optional['XmlElement[NativeElement]']:
         assert len(path) > 0, "path can't be empty"
 
         root, path = path[0], path[1:]
         element = self._find_element(root, search_mode)
         if element and path:
             return element.find_sub_element(path, search_mode)
 
         return element
 
-    def find_element_or_create(self, tag: str, search_mode: 'SearchMode', nsmap: Optional[NsMap]) -> 'XmlElement':
+    def find_element_or_create(
+            self,
+            tag: str,
+            search_mode: 'SearchMode',
+            nsmap: Optional[NsMap],
+    ) -> 'XmlElement[NativeElement]':
         if (sub_element := self._find_element(tag, search_mode)) is None:
             sub_element = self.make_element(tag=tag, nsmap=nsmap)
             self._state.elements.append(sub_element)
+            self._state.next_element_idx += 1
 
         return sub_element
 
-    def _find_element(self, tag: str, search_mode: 'SearchMode') -> Optional['XmlElement']:
+    def _find_element(self, tag: str, search_mode: 'SearchMode') -> Optional['XmlElement[NativeElement]']:
         searcher = get_searcher(search_mode)
 
         return searcher(self._state, tag, True)
 
 
 class SearchMode(str, Enum):
     """
@@ -307,61 +316,61 @@
     """
 
     STRICT = 'strict'
     ORDERED = 'ordered'
     UNORDERED = 'unordered'
 
 
-Searcher = Callable[[XmlElement.State, str, bool], Optional[XmlElement]]
+Searcher = Callable[[XmlElement.State[Any], str, bool], Optional[XmlElement]]
 
 
 def get_searcher(search_mode: SearchMode) -> Searcher:
     if search_mode == SearchMode.STRICT:
         return strict_search
     elif search_mode == SearchMode.ORDERED:
         return ordered_search
     elif search_mode == SearchMode.UNORDERED:
         return unordered_search
     else:
         raise AssertionError('unreachable')
 
 
-def strict_search(state: XmlElement.State, tag: str, look_behind: bool = False) -> Optional[XmlElement]:
+def strict_search(state: XmlElement.State[Any], tag: str, look_behind: bool = False) -> Optional[XmlElement[Any]]:
     """
     Searches for a sub-element sequentially one by one.
 
     :param state: element state
     :param tag: sub-element tag for be searched for
     :param look_behind: look for a previous element
     :return: found element or `None` if the element not found
     """
 
-    result: Optional['XmlElement'] = None
+    result: Optional[XmlElement[Any]] = None
 
     if look_behind and (result := _look_behind(state, tag)) is not None:
         return result
 
     if state.next_element_idx < len(state.elements) and state.elements[state.next_element_idx].tag == tag:
         result = state.elements[state.next_element_idx]
         state.next_element_idx += 1
 
     return result
 
 
-def ordered_search(state: XmlElement.State, tag: str, look_behind: bool = False) -> Optional[XmlElement]:
+def ordered_search(state: XmlElement.State[Any], tag: str, look_behind: bool = False) -> Optional[XmlElement[Any]]:
     """
     Searches for an element sequentially skipping unmatched ones.
 
     :param state: element state
     :param tag: sub-element tag for be searched for
     :param look_behind: look for a previous element
     :return: found element or `None` if the element not found
     """
 
-    result: Optional['XmlElement'] = None
+    result: Optional[XmlElement[Any]] = None
 
     if look_behind and (result := _look_behind(state, tag)) is not None:
         return result
 
     next_element_idx = state.next_element_idx
     while next_element_idx < len(state.elements):
         element = state.elements[next_element_idx]
@@ -371,25 +380,29 @@
             state.next_element_idx = next_element_idx
             result = element
             break
 
     return result
 
 
-def unordered_search(state: XmlElement.State, tag: str, look_behind: bool = False) -> Optional[XmlElement]:
+def unordered_search(
+        state: XmlElement.State[Any],
+        tag: str,
+        look_behind: bool = False,
+) -> Optional[XmlElement[Any]]:
     """
     Searches search for an element ignoring elements order.
 
     :param state: element state
     :param tag: sub-element tag for be searched for
     :param look_behind: look for a previous element
     :return: found element or `None` if the requested element not found
     """
 
-    result: Optional['XmlElement'] = None
+    result: Optional[XmlElement[Any]] = None
 
     if look_behind and (result := _look_behind(state, tag)) is not None:
         return result
 
     for idx in range(state.next_element_idx, len(state.elements)):
         element = state.elements[idx]
         if element.tag == tag:
@@ -398,14 +411,14 @@
             state.next_element_idx += 1
             result = element
             break
 
     return result
 
 
-def _look_behind(state: XmlElement.State, tag: str) -> Optional[XmlElement]:
+def _look_behind(state: XmlElement.State[Any], tag: str) -> Optional[XmlElement[Any]]:
     if state.next_element_idx != 0:
         candidate = state.elements[state.next_element_idx - 1]
         if candidate.tag == tag:
             return candidate
 
     return None
```

### Comparing `pydantic_xml-0.6.3/pydantic_xml/element/native/lxml.py` & `pydantic_xml-0.7.0/pydantic_xml/element/native/lxml.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.3/pydantic_xml/element/native/std.py` & `pydantic_xml-0.7.0/pydantic_xml/element/native/std.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.3/pydantic_xml/errors.py` & `pydantic_xml-0.7.0/pydantic_xml/errors.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.3/pydantic_xml/model.py` & `pydantic_xml-0.7.0/pydantic_xml/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import functools as ft
-from typing import Any, Callable, ClassVar, Dict, Optional, Tuple, Type, Union
+import typing
+from typing import Any, Callable, ClassVar, Dict, Optional, Tuple, Type, TypeVar, Union
 
 import pydantic as pd
 import pydantic.fields
 import pydantic.generics
 import pydantic.json
 
 from . import config, errors, serializers, utils
@@ -140,33 +141,37 @@
     def nsmap(self) -> Optional[NsMap]:
         return self._nsmap
 
 
 def attr(**kwargs: Any) -> Any:
     """
     Marks a pydantic field as an xml attribute.
-    Method parameters are identical to :py:class:`pydantic_xml.XmlAttributeInfo`.
+
+    :param kwargs: see :py:class:`pydantic_xml.XmlAttributeInfo`
     """
 
     return XmlAttributeInfo(**kwargs)
 
 
 def element(**kwargs: Any) -> Any:
     """
     Marks a pydantic field as an xml element.
-    Method parameters are identical to :py:class:`pydantic_xml.XmlElementInfo`.
+
+    :param kwargs: see :py:class:`pydantic_xml.XmlElementInfo`
     """
 
     return XmlElementInfo(**kwargs)
 
 
 def wrapped(*args: Any, **kwargs: Any) -> Any:
     """
     Marks a pydantic field as a wrapped xml entity.
-    Method parameters are identical to :py:class:`pydantic_xml.XmlWrapperInfo`.
+
+    :param args: see :py:class:`pydantic_xml.XmlWrapperInfo`
+    :param kwargs: see :py:class:`pydantic_xml.XmlWrapperInfo`
     """
 
     return XmlWrapperInfo(*args, **kwargs)
 
 
 class XmlModelMeta(pd.main.ModelMetaclass):
     """
@@ -195,14 +200,17 @@
                 xml_encoders.update(getattr(base.__config__, 'xml_encoders', {}))
 
         if self_config := namespace.get('Config'):
             xml_encoders.update(getattr(self_config, 'xml_encoders', {}))
             setattr(self_config, 'xml_encoders', xml_encoders)
 
 
+ModelT = TypeVar('ModelT', bound='BaseXmlModel')
+
+
 class BaseXmlModel(pd.BaseModel, metaclass=XmlModelMeta):
     """
     Base pydantic-xml model.
     """
 
     __xml_tag__: ClassVar[Optional[str]]
     __xml_ns__: ClassVar[Optional[str]]
@@ -260,34 +268,34 @@
     def update_forward_refs(cls, **kwargs: Any) -> None:
         super().update_forward_refs(**kwargs)
 
         if cls.__xml_serializer__ is not None:
             cls.__xml_serializer__.resolve_forward_refs()
 
     @classmethod
-    def from_xml_tree(cls, root: etree.Element) -> Optional['BaseXmlModel']:
+    def from_xml_tree(cls: Type[ModelT], root: etree.Element) -> ModelT:
         """
         Deserializes an xml element tree to an object of `cls` type.
 
         :param root: xml element to deserialize the object from
         :return: deserialized object
         """
 
         assert cls.__xml_serializer__ is not None, f"model {cls.__name__} is partially initialized"
 
         if root.tag == cls.__xml_serializer__.element_name:
-            obj = cls.__xml_serializer__.deserialize(XmlElement.from_native(root))
+            obj = typing.cast(ModelT, cls.__xml_serializer__.deserialize(XmlElement.from_native(root)))
             return obj
         else:
             raise errors.ParsingError(
                 f"root element not found (actual: {root.tag}, expected: {cls.__xml_serializer__.element_name})",
             )
 
     @classmethod
-    def from_xml(cls, source: Union[str, bytes]) -> Optional['BaseXmlModel']:
+    def from_xml(cls: Type[ModelT], source: Union[str, bytes]) -> ModelT:
         """
         Deserializes an xml string to an object of `cls` type.
 
         :param source: xml string
         :return: deserialized object
         """
 
@@ -331,14 +339,17 @@
         :param kwargs: additional xml serialization arguments
         :return: object xml representation
         """
 
         return etree.tostring(self.to_xml_tree(encoder=encoder, skip_empty=skip_empty), **kwargs)
 
 
+GenericModelT = TypeVar('GenericModelT', bound='BaseGenericXmlModel')
+
+
 class BaseGenericXmlModel(BaseXmlModel, pd.generics.GenericModel):
     """
     Base pydantic-xml generic model.
     """
 
     def __class_getitem__(cls, params: Union[Type[Any], Tuple[Type[Any], ...]]) -> Type[Any]:
         model = super().__class_getitem__(params)
@@ -356,15 +367,15 @@
         # checks that the model is not generic
         if not getattr(cls, '__concrete__', True):
             cls.__xml_serializer__ = None
         else:
             super().__init_serializer__()
 
     @classmethod
-    def from_xml_tree(cls, root: etree.Element) -> Optional['BaseXmlModel']:
+    def from_xml_tree(cls: Type[GenericModelT], root: etree.Element) -> GenericModelT:
         """
         Deserializes an xml element tree to an object of `cls` type.
 
         :param root: xml element to deserialize the object from
         :return: deserialized object
         """
```

### Comparing `pydantic_xml-0.6.3/pydantic_xml/serializers/encoder.py` & `pydantic_xml-0.7.0/pydantic_xml/serializers/encoder.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.3/pydantic_xml/serializers/factories/forwardref.py` & `pydantic_xml-0.7.0/pydantic_xml/serializers/factories/forwardref.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.3/pydantic_xml/serializers/factories/heterogeneous.py` & `pydantic_xml-0.7.0/pydantic_xml/serializers/factories/heterogeneous.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.3/pydantic_xml/serializers/factories/homogeneous.py` & `pydantic_xml-0.7.0/pydantic_xml/serializers/factories/homogeneous.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.3/pydantic_xml/serializers/factories/mapping.py` & `pydantic_xml-0.7.0/pydantic_xml/serializers/factories/mapping.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.3/pydantic_xml/serializers/factories/model.py` & `pydantic_xml-0.7.0/pydantic_xml/serializers/factories/model.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.3/pydantic_xml/serializers/factories/primitive.py` & `pydantic_xml-0.7.0/pydantic_xml/serializers/factories/primitive.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.3/pydantic_xml/serializers/factories/union.py` & `pydantic_xml-0.7.0/pydantic_xml/serializers/factories/union.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import dataclasses as dc
 import typing
 from typing import Any, List, Optional, Type
 
 import pydantic as pd
 
 import pydantic_xml as pxml
 from pydantic_xml import errors
@@ -66,15 +67,19 @@
                         model_field.name,
                         model_field.alias,
                         model_field.field_info,
                         sub_field,
                     ),
                 )
 
-                serializer = self._build_field_serializer(model, sub_field, ctx)
+                serializer = self._build_field_serializer(
+                    model,
+                    sub_field,
+                    dc.replace(ctx, parent_is_root=False),
+                )
                 assert isinstance(serializer, ModelSerializerFactory.ModelSerializer), "unexpected serializer type"
 
                 inner_serializers.append(serializer)
 
             self._inner_serializers = inner_serializers
 
         def serialize(
```

### Comparing `pydantic_xml-0.6.3/pydantic_xml/serializers/factories/wrapper.py` & `pydantic_xml-0.7.0/pydantic_xml/serializers/factories/wrapper.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.3/pydantic_xml/serializers/serializer.py` & `pydantic_xml-0.7.0/pydantic_xml/serializers/serializer.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.3/pydantic_xml/utils.py` & `pydantic_xml-0.7.0/pydantic_xml/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.6.3/pyproject.toml` & `pydantic_xml-0.7.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-xml"
-version = "0.6.3"
+version = "0.7.0"
 description = "pydantic xml extension"
 authors = ["Dmitry Pershin <dapper1291@gmail.com>"]
 license = "Unlicense"
 readme = "README.rst"
 homepage = "https://github.com/dapper91/pydantic-xml"
 repository = "https://github.com/dapper91/pydantic-xml"
 documentation = "https://github.com/dapper91/pydantic-xml"
@@ -49,14 +49,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 allow_redefinition = true
+disallow_any_generics = true
 disallow_incomplete_defs = true
 disallow_untyped_decorators = false
 disallow_untyped_defs = true
 no_implicit_optional = true
 show_error_codes = true
 strict_equality = true
 warn_unused_ignores = true
```

### Comparing `pydantic_xml-0.6.3/PKG-INFO` & `pydantic_xml-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-xml
-Version: 0.6.3
+Version: 0.7.0
 Summary: pydantic xml extension
 Home-page: https://github.com/dapper91/pydantic-xml
 License: Unlicense
 Keywords: pydantic,xml,serialization,deserialization,parsing,lxml
 Author: Dmitry Pershin
 Author-email: dapper1291@gmail.com
 Requires-Python: >=3.8,<4.0
```


# Comparing `tmp/hat_peg-0.5.6-cp38.cp39.cp310-none-any.whl.zip` & `tmp/hat_peg-0.5.7-cp310.cp311-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 10785 bytes, number of entries: 7
--rw-r--r--  2.0 unx    18897 b- defN 22-May-16 15:47 hat/peg.py
--rw-r--r--  2.0 unx    11358 b- defN 23-Feb-23 19:56 hat_peg-0.5.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     1827 b- defN 23-Feb-23 19:56 hat_peg-0.5.6.dist-info/METADATA
--rw-r--r--  2.0 unx      132 b- defN 23-Feb-23 19:56 hat_peg-0.5.6.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 23-Feb-23 19:56 hat_peg-0.5.6.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Feb-23 19:56 hat_peg-0.5.6.dist-info/zip-safe
-?rw-rw-r--  2.0 unx      541 b- defN 23-Feb-23 19:56 hat_peg-0.5.6.dist-info/RECORD
-7 files, 32760 bytes uncompressed, 9829 bytes compressed:  70.0%
+Zip file size: 10899 bytes, number of entries: 7
+-rw-r--r--  2.0 unx    18746 b- defN 23-Jun-23 20:29 hat/peg.py
+-rw-r--r--  2.0 unx    11358 b- defN 23-Jun-23 20:43 hat_peg-0.5.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2248 b- defN 23-Jun-23 20:43 hat_peg-0.5.7.dist-info/METADATA
+-rw-r--r--  2.0 unx      114 b- defN 23-Jun-23 20:43 hat_peg-0.5.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 23-Jun-23 20:43 hat_peg-0.5.7.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-23 20:43 hat_peg-0.5.7.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      541 b- defN 23-Jun-23 20:43 hat_peg-0.5.7.dist-info/RECORD
+7 files, 33012 bytes uncompressed, 9943 bytes compressed:  69.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: hat/peg.py
 Comment: 
 
-Filename: hat_peg-0.5.6.dist-info/LICENSE
+Filename: hat_peg-0.5.7.dist-info/LICENSE
 Comment: 
 
-Filename: hat_peg-0.5.6.dist-info/METADATA
+Filename: hat_peg-0.5.7.dist-info/METADATA
 Comment: 
 
-Filename: hat_peg-0.5.6.dist-info/WHEEL
+Filename: hat_peg-0.5.7.dist-info/WHEEL
 Comment: 
 
-Filename: hat_peg-0.5.6.dist-info/top_level.txt
+Filename: hat_peg-0.5.7.dist-info/top_level.txt
 Comment: 
 
-Filename: hat_peg-0.5.6.dist-info/zip-safe
+Filename: hat_peg-0.5.7.dist-info/zip-safe
 Comment: 
 
-Filename: hat_peg-0.5.6.dist-info/RECORD
+Filename: hat_peg-0.5.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hat/peg.py

```diff
@@ -90,41 +90,43 @@
 
     Node names are identifiers of parser's definitions and values
     are other nodes or string values representing matched `Literal`, `Class`
     or `Dot` leafs.
 
     """
     name: str
-    value: typing.List[typing.Union['Node', str]]
+    value: list[typing.Union['Node', str]]
 
 
-Action = typing.Callable[[Node, typing.List], typing.Any]
+Action: typing.TypeAlias = typing.Callable[[Node, list], typing.Any]
 """Action"""
 
 
 def walk_ast(node: Node,
-             actions: typing.Dict[str, Action],
-             default_action: typing.Optional[Action] = None
+             actions: dict[str, Action],
+             default_action: Action | None = None
              ) -> typing.Any:
     """Simple depth-first abstract syntax tree parser.
 
     Actions are key value pairs where keys represent node names and values
     are callables that should be called for appropriate node. Each callable
     receives matched node and list of results from recursively applying
     this function on child nodes. For nodes which name doesn't match any
     action, default action is used. If default action is not defined and node
     name doesn't match action, result is None and recursion is stopped.
 
     """
     action = actions.get(node.name, default_action)
     if not action:
         return
+
     children = [walk_ast(i, actions, default_action)
                 if isinstance(i, Node) else i
                 for i in node.value]
+
     return action(node, children)
 
 
 class Sequence(typing.NamedTuple):
     expressions: typing.List['Expression']
 
 
@@ -164,28 +166,29 @@
     values: typing.List[typing.Union[str, typing.Tuple[str, str]]]
 
 
 class Dot(typing.NamedTuple):
     pass
 
 
-Expression = typing.Union[Sequence, Choice, Not, And, OneOrMore, ZeroOrMore,
-                          Optional, Identifier, Literal, Class, Dot]
+Expression: typing.TypeAlias = (Sequence | Choice | Not | And | OneOrMore |
+                                ZeroOrMore | Optional | Identifier | Literal |
+                                Class | Dot)
 """Expression"""
 
 
 class MatchResult(typing.NamedTuple):
     """Match result
 
     Args:
         node: matched node or ``None`` if match failed
         rest: remaining input data
 
     """
-    node: typing.Optional[Node]
+    node: Node | None
     rest: str
 
 
 class MatchCallFrame(typing.NamedTuple):
     """Match call frame
 
     Args:
@@ -193,56 +196,56 @@
         data: input data
 
     """
     name: str
     data: str
 
 
-MatchCallStack = typing.Iterable[MatchCallFrame]
+MatchCallStack: typing.TypeAlias = typing.Iterable[MatchCallFrame]
 """Match call stack"""
 
 
-DebugCb = typing.Callable[[MatchResult, MatchCallStack], None]
+DebugCb: typing.TypeAlias = typing.Callable[[MatchResult, MatchCallStack],
+                                            None]
 """Debug callback"""
 
 
 class Grammar:
     """PEG Grammar.
 
     Args:
         definitions: grammar definitions
         starting: starting definition name
 
     """
 
     def __init__(self,
-                 definitions: typing.Union[str,
-                                           typing.Dict[str, Expression]],
+                 definitions: str | dict[str, Expression],
                  starting: str):
         if isinstance(definitions, str):
             ast = _peg_grammar.parse(definitions)
             definitions = walk_ast(ast, _peg_actions)
             definitions = {k: _reduce_expression(v)
                            for k, v in definitions.items()}
         self._definitions = definitions
         self._starting = starting
 
     @property
-    def definitions(self) -> typing.Dict[str, Expression]:
+    def definitions(self) -> dict[str, Expression]:
         """Definitions"""
         return self._definitions
 
     @property
     def starting(self) -> str:
         """Starting definition name"""
         return self._starting
 
     def parse(self,
               data: str,
-              debug_cb: typing.Optional[DebugCb] = None
+              debug_cb: DebugCb | None = None
               ) -> Node:
         """Parse input data.
 
         `debug_cb` is optional function which can be used for monitoring and
         debugging parse steps. It is called each time named definition
         is successfully or unsuccessfully matched. This function receives
         match result and match call stack.
@@ -266,15 +269,15 @@
     consumed = util.first(call_stack).data[:-len(result.rest)]
     print(success, stack)
     print('<<<', consumed)
     print('>>>', result.rest, flush=True)
 
 
 class _MatchCallStack(typing.NamedTuple):
-    frame: typing.Optional[MatchCallFrame]
+    frame: MatchCallFrame | None
     previous: typing.Optional['_MatchCallStack']
 
     def __iter__(self):
         current = self
         while current and current.frame:
             yield current.frame
             current = current.previous
@@ -622,16 +625,8 @@
                           chr(int(c[2:], 16))),
     'Hex': lambda n, c: c[0],
     'AND': lambda n, c: And,
     'NOT': lambda n, c: Not,
     'QUESTION': lambda n, c: Optional,
     'STAR': lambda n, c: ZeroOrMore,
     'PLUS': lambda n, c: OneOrMore,
-    'DOT': lambda n, c: Dot()
-}
-
-
-# HACK type alias
-util.register_type_alias('Action')
-util.register_type_alias('Expression')
-util.register_type_alias('MatchCallStack')
-util.register_type_alias('DebugCb')
+    'DOT': lambda n, c: Dot()}
```

## Comparing `hat_peg-0.5.6.dist-info/LICENSE` & `hat_peg-0.5.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `hat_peg-0.5.6.dist-info/METADATA` & `hat_peg-0.5.7.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,86 @@
 Metadata-Version: 2.1
 Name: hat-peg
-Version: 0.5.6
+Version: 0.5.7
 Summary: Hat PEG parser
 Home-page: https://github.com/hat-open/hat-peg
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: hat-util (~=0.6.7)
+Requires-Dist: hat-util (~=0.6.10)
 
-hat-peg - Python parsing expression grammar
-===========================================
+.. _online documentation: https://hat-peg.hat-open.com
+.. _git repository: https://github.com/hat-open/hat-peg.git
+.. _PyPI project: https://pypi.org/project/hat-peg
+.. _pydoit: https://pydoit.org
+.. _Hat Open: https://hat-open.com
+.. _Končar Digital: https://www.koncar.hr/en
 
-This library is part of Hat Open project - open-source framework of tools and
-libraries for developing applications used for remote monitoring, control and
-management of intelligent electronic devices such as IoT devices, PLCs,
-industrial automation or home automation systems.
 
-Development of Hat Open and associated repositories is sponsored by
-`Končar Digital <https://www.koncar.hr>`_.
+hat-peg - Python parsing expression grammar
+===========================================
 
 For more information see:
 
-    * hat-peg documentation - `<https://hat-peg.hat-open.com>`_
-    * hat-peg git repository - `<https://github.com/hat-open/hat-peg.git>`_
-    * Hat Open homepage - `<https://hat-open.com>`_
+* `online documentation`_
+* `git repository`_
 
-.. warning::
 
-    This project is currently in state of active development. Features,
-    functionality and API are unstable.
+Runtime requirements
+--------------------
+
+* python >=3.10
 
 
 Install
 -------
 
-::
+`hat-peg` is available as `PyPI project`_::
 
     $ pip install hat-peg
 
 
+Build
+-----
+
+Build tool used for `hat-peg` is `pydoit`_. It can be installed together
+with other python dependencies by running::
+
+    $ pip install -r requirements.pip.dev.txt
+
+For listing available doit tasks, use::
+
+    $ doit list
+
+Default task::
+
+    $ doit
+
+creates wheel package inside `build` directory.
+
+
+Hat Open
+--------
+
+`hat-peg` is part of `Hat Open`_ project - open-source framework of tools
+and libraries for developing applications used for remote monitoring, control
+and management of intelligent electronic devices such as IoT devices, PLCs,
+industrial automation or home automation systems.
+
+Development of Hat Open and associated repositories is sponsored by
+`Končar Digital`_.
+
+
 License
 -------
 
-Copyright 2020-2022 Hat Open AUTHORS
+Copyright 2020-2023 Hat Open AUTHORS
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```


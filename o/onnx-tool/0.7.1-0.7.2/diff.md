# Comparing `tmp/onnx-tool-0.7.1.tar.gz` & `tmp/onnx-tool-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnx-tool-0.7.1.tar", last modified: Tue Jun 20 15:43:34 2023, max compression
+gzip compressed data, was "onnx-tool-0.7.2.tar", last modified: Fri Jun 23 14:11:33 2023, max compression
```

## Comparing `onnx-tool-0.7.1.tar` & `onnx-tool-0.7.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 15:43:34.380592 onnx-tool-0.7.1/
--rw-rw-rw-   0        0        0     1092 2022-12-15 10:33:04.000000 onnx-tool-0.7.1/LICENSE
--rw-rw-rw-   0        0        0    10735 2023-06-20 15:43:34.380592 onnx-tool-0.7.1/PKG-INFO
--rw-rw-rw-   0        0        0    10276 2023-06-18 06:46:34.000000 onnx-tool-0.7.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 15:43:34.367696 onnx-tool-0.7.1/onnx_tool/
--rw-rw-rw-   0        0        0     7846 2023-06-19 15:21:47.000000 onnx-tool-0.7.1/onnx_tool/__init__.py
--rw-rw-rw-   0        0        0     3051 2023-06-18 06:46:34.000000 onnx-tool-0.7.1/onnx_tool/__main__.py
--rw-rw-rw-   0        0        0    16079 2023-06-19 15:20:56.000000 onnx-tool-0.7.1/onnx_tool/fusion.py
--rw-rw-rw-   0        0        0    56902 2023-06-20 15:34:51.000000 onnx-tool-0.7.1/onnx_tool/graph.py
--rw-rw-rw-   0        0        0      876 2023-06-19 15:20:56.000000 onnx-tool-0.7.1/onnx_tool/model.py
--rw-rw-rw-   0        0        0    73508 2023-06-18 06:46:34.000000 onnx-tool-0.7.1/onnx_tool/node.py
--rw-rw-rw-   0        0        0     6433 2023-06-18 06:46:34.000000 onnx-tool-0.7.1/onnx_tool/serialization.py
--rw-rw-rw-   0        0        0    15758 2023-06-18 06:46:34.000000 onnx-tool-0.7.1/onnx_tool/tensor.py
--rw-rw-rw-   0        0        0     3685 2023-06-20 15:38:47.000000 onnx-tool-0.7.1/onnx_tool/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-20 15:43:34.377186 onnx-tool-0.7.1/onnx_tool.egg-info/
--rw-rw-rw-   0        0        0    10735 2023-06-20 15:43:34.000000 onnx-tool-0.7.1/onnx_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      404 2023-06-20 15:43:34.000000 onnx-tool-0.7.1/onnx_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 15:43:34.000000 onnx-tool-0.7.1/onnx_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-06-20 15:43:34.000000 onnx-tool-0.7.1/onnx_tool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-20 15:43:34.000000 onnx-tool-0.7.1/onnx_tool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-06-20 15:43:33.000000 onnx-tool-0.7.1/onnx_tool.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-06-20 15:43:34.380592 onnx-tool-0.7.1/setup.cfg
--rw-rw-rw-   0        0        0      988 2023-06-20 15:38:55.000000 onnx-tool-0.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 14:11:33.945464 onnx-tool-0.7.2/
+-rw-rw-rw-   0        0        0     1092 2022-12-15 10:33:04.000000 onnx-tool-0.7.2/LICENSE
+-rw-rw-rw-   0        0        0    10735 2023-06-23 14:11:33.939957 onnx-tool-0.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0    10276 2023-06-18 06:46:34.000000 onnx-tool-0.7.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 14:11:33.934868 onnx-tool-0.7.2/onnx_tool/
+-rw-rw-rw-   0        0        0     7846 2023-06-19 15:21:47.000000 onnx-tool-0.7.2/onnx_tool/__init__.py
+-rw-rw-rw-   0        0        0     3051 2023-06-18 06:46:34.000000 onnx-tool-0.7.2/onnx_tool/__main__.py
+-rw-rw-rw-   0        0        0    16079 2023-06-19 15:20:56.000000 onnx-tool-0.7.2/onnx_tool/fusion.py
+-rw-rw-rw-   0        0        0    55538 2023-06-23 13:57:22.000000 onnx-tool-0.7.2/onnx_tool/graph.py
+-rw-rw-rw-   0        0        0      876 2023-06-19 15:20:56.000000 onnx-tool-0.7.2/onnx_tool/model.py
+-rw-rw-rw-   0        0        0    73508 2023-06-18 06:46:34.000000 onnx-tool-0.7.2/onnx_tool/node.py
+-rw-rw-rw-   0        0        0     6433 2023-06-18 06:46:34.000000 onnx-tool-0.7.2/onnx_tool/serialization.py
+-rw-rw-rw-   0        0        0    15758 2023-06-18 06:46:34.000000 onnx-tool-0.7.2/onnx_tool/tensor.py
+-rw-rw-rw-   0        0        0     3685 2023-06-23 14:10:10.000000 onnx-tool-0.7.2/onnx_tool/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-23 14:11:33.939957 onnx-tool-0.7.2/onnx_tool.egg-info/
+-rw-rw-rw-   0        0        0    10735 2023-06-23 14:11:33.000000 onnx-tool-0.7.2/onnx_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      404 2023-06-23 14:11:33.000000 onnx-tool-0.7.2/onnx_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 14:11:33.000000 onnx-tool-0.7.2/onnx_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-06-23 14:11:33.000000 onnx-tool-0.7.2/onnx_tool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-23 14:11:33.000000 onnx-tool-0.7.2/onnx_tool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-06-20 15:43:33.000000 onnx-tool-0.7.2/onnx_tool.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-06-23 14:11:33.945464 onnx-tool-0.7.2/setup.cfg
+-rw-rw-rw-   0        0        0      988 2023-06-23 14:10:10.000000 onnx-tool-0.7.2/setup.py
```

### Comparing `onnx-tool-0.7.1/LICENSE` & `onnx-tool-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `onnx-tool-0.7.1/PKG-INFO` & `onnx-tool-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnx-tool
-Version: 0.7.1
+Version: 0.7.2
 Summary: A tool for ONNX model:Rapid shape inference; Profile model; Compute Graph and Shape Engine; OPs fusion;Quantized models and sparse models are supported.
 Home-page: https://github.com/ThanatosShinji/onnx-tool
 Author: Luo Yu
 Author-email: luoyu888888@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: onnx-tool Version: 0.7.1 Summary: A tool for ONNX
+Metadata-Version: 2.1 Name: onnx-tool Version: 0.7.2 Summary: A tool for ONNX
 model:Rapid shape inference; Profile model; Compute Graph and Shape Engine; OPs
 fusion;Quantized models and sparse models are supported. Home-page: https://
 github.com/ThanatosShinji/onnx-tool Author: Luo Yu Author-email:
 luoyu888888@gmail.com License: MIT Classifier: Programming Language :: Python
 :: 3 Description-Content-Type: text/markdown License-File: LICENSE ç®ä½ä¸­æ
 # onnx-tool **A tool for ONNX model:** * *Rapid shape inference.* * *Profile
 model.* * *Constant_Folding.* * *Compute Graph and Shape Engine.* * *OPs
```

### Comparing `onnx-tool-0.7.1/README.md` & `onnx-tool-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `onnx-tool-0.7.1/onnx_tool/__init__.py` & `onnx-tool-0.7.2/onnx_tool/__init__.py`

 * *Files identical despite different names*

### Comparing `onnx-tool-0.7.1/onnx_tool/__main__.py` & `onnx-tool-0.7.2/onnx_tool/__main__.py`

 * *Files identical despite different names*

### Comparing `onnx-tool-0.7.1/onnx_tool/fusion.py` & `onnx-tool-0.7.2/onnx_tool/fusion.py`

 * *Files identical despite different names*

### Comparing `onnx-tool-0.7.1/onnx_tool/graph.py` & `onnx-tool-0.7.2/onnx_tool/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import copy
 import math
 import warnings
 
 import numpy
 import onnx
 
-import onnx_tool
 from .node import create_node
-from .tensor import get_attribute_data, Tensor, volume
 from .tensor import STATIC_TENSOR, DYNAMIC_TENSOR
+from .tensor import get_attribute_data, Tensor, volume
 from .utils import VERSION, tuple2str
 
 
 def __shape_of_initializer__(initial):
     shape = []
     # for nb in tensor.shape.dim
     for nb in initial.dims:
@@ -307,16 +306,15 @@
             for tensor in node.output:
                 if tensor not in self.producedby:
                     self.producedby[tensor] = []
                 self.producedby[tensor].append(node.name)
 
     def update_tensor_relations(self):
         self.__update_consumer_producer__()
-        self.dynamics=list(self.producedby.keys())
-
+        self.dynamics = list(self.producedby.keys())
 
     def __init_graph_from_onnxproto__(self, g, noderename):
         if g is None:
             return
         ncount = 0
         from .utils import timer
 
@@ -530,16 +528,16 @@
                         if con_node.input[i] == node.output[0]:
                             con_node.input[i] = indtensor
                             self.consumedby[indtensor].append(con)
                             break
             else:
                 for pro in self.producedby[indtensor]:
                     pro_node = self.nodemap[pro]
-                    assert(len(pro_node.output)==1)
-                    pro_node.output[0]=node.output[0]
+                    assert (len(pro_node.output) == 1)
+                    pro_node.output[0] = node.output[0]
 
     def fuse_subgraph_node_names(self, nodes: [str], nodeop: str, nodename: str, keep_attr=True):
         _inputs, _outputs = self.get_iotensors(nodes, remove_initials=False)
         newnode = onnx.helper.make_node(nodeop, _inputs, _outputs, name=nodename)
         count = 0
         if keep_attr:
             for node in nodes:
@@ -610,34 +608,34 @@
                 newnode.prevnodes.append(self.producedby[i])
         for o in _outputs:
             self.producedby[o] = [mainnode.name]
             if o in self.consumedby.keys():
                 newnode.nextnodes.append(self.consumedby[o])
         self.nodemap[mainnode.name] = newnode
 
-    def fuse_subgraph_iotensors(self, inputs: [], outputs: [], nodeop: str, name_prefix:str=None, keep_attr=True):
+    def fuse_subgraph_iotensors(self, inputs: [], outputs: [], nodeop: str, name_prefix: str = None, keep_attr=True):
         _, nodes, _ = self.__get_subnodes_byio__(inputs, outputs)
-        from .fusion import create_descs_from_nodenames,FusionPattern
-        descs=create_descs_from_nodenames(self,nodes)
+        from .fusion import create_descs_from_nodenames, FusionPattern
+        descs = create_descs_from_nodenames(self, nodes)
         pattern = FusionPattern(descs)
         nodesls = pattern.search_pattern(self)
-        for i,nodes in enumerate(nodesls):
-            name = name_prefix+'_'+str(i) if name_prefix is not None else nodes[0]
-            self.fuse_subgraph_node_names(nodes,nodeop,name,keep_attr)
+        for i, nodes in enumerate(nodesls):
+            name = name_prefix + '_' + str(i) if name_prefix is not None else nodes[0]
+            self.fuse_subgraph_node_names(nodes, nodeop, name, keep_attr)
 
     def get_onnxgraph_by_nodenames(self, nodenames):
         if len(nodenames):
             _inputs0, _outputs0 = self.get_iotensors(nodenames)
-            graph_level0 = self.reorder_nodes(nodenames, _inputs0)
+            graph_level0 = self.topsort_nodes(nodenames, _inputs0)
             subgraph = self.make_graph_onnx(graph_level0, 'subgraph', _inputs0, _outputs0)
             return subgraph
         return None
 
     def save_model(self, f: str, shape_only: bool = False, no_shape: bool = False, rawmodel: onnx.ModelProto = None):
-        if len(self.nodemap.keys())==0:
+        if len(self.nodemap.keys()) == 0:
             warnings.warn(f'Empty graph {f} to save')
             return
         graph = self.make_graph_onnx(self.nodemap.keys(), 'graph', self.input, self.output,
                                      with_initializer=not shape_only, with_shape_info=not no_shape)
         if graph is not None and f is not None:
             attr = {}
             attr['producer_name'] = 'onnx_tool'
@@ -681,85 +679,57 @@
                 if vinfo is None:
                     continue
                 value_infos.append(vinfo)
         graph = onnx.helper.make_graph(nodes=nodes, name=gname, inputs=inputs, outputs=outputs, initializer=initializer,
                                        value_info=value_infos)
         return graph
 
-    def __backwardsearch_node__(self,curnode,produced_by,consumed_by,produced,searched):
-        nodelist = []
-        node = self.nodemap[curnode]
-        searched.append(curnode)
-        for tname in node.input:
-            if tname in produced_by.keys() and tname not in produced:
-                nodelist.extend(self.__backwardsearch_node__(produced_by[tname], produced_by, consumed_by, produced, searched))
-
-
-        produced.extend(node.output)
-        nodelist +=[curnode]
-        return nodelist
-
-    def __forwardsearch_node__(self,curnode,produced_by,consumed_by,produced,searched):
-        nodelist=[]
-        backlist=[]
-        searched.append(curnode)
-        node = self.nodemap[curnode]
-        for tname in node.input:
-            if tname in produced_by.keys() and tname not in produced:
-                backlist.append(tname)
-        if len(backlist):
-            for tname in backlist:
-                nodelist.extend(self.__backwardsearch_node__(produced_by[tname], produced_by, consumed_by, produced,searched))
-
-        nodelist+=[curnode]
-
-        for tname in node.output:
-            produced.append(tname)
-        for tname in node.output:
-            if tname in consumed_by.keys():
-                for nextn in consumed_by[tname]:
-                    if nextn not in searched:
-                        nodelist.extend(self.__forwardsearch_node__(nextn,produced_by,consumed_by,produced,searched))
-        return nodelist
-
-    def reorder_nodes(self, node_names,input_names):
+    def topsort_nodes(self, node_names, input_names):
         # update
-        import sys
-        curlimit=sys.getrecursionlimit()
-        newlimit=len(node_names)*1 if len(node_names)*1 > curlimit else curlimit
-        sys.setrecursionlimit(newlimit+100) #TODO while version instead of recursion version
         produced_by = {}
         for name in node_names:
             node = self.nodemap[name]
             for tname in node.output:
                 produced_by[tname] = name
 
         consumed_by = {}
+        dependencies={}
         for name in node_names:
             node = self.nodemap[name]
+            count=0
             for tname in node.input:
                 if tname in produced_by.keys():
+                    count+=1
                     if tname in consumed_by.keys():
                         consumed_by[tname].append(name)
                     else:
                         consumed_by[tname] = [name]
+            dependencies[name]=count
 
-        produced = []
-        searched = []
         ordered_nodes = []
-        for input in input_names:
-            for cnode in self.consumedby[input]:
-                if cnode in searched:
-                    continue
-                ordered_nodes.extend(self.__forwardsearch_node__(cnode, produced_by, consumed_by, produced, searched))
-        sys.setrecursionlimit(curlimit)
+        queue =[]
+        while True:
+            for name in node_names:
+                if dependencies[name]==0:
+                    queue.append(name)
+                    ordered_nodes.append(name)
+                    dependencies[name]-=1
+            if len(queue)==0:
+                break
+            for name in queue:
+                node = self.nodemap[name]
+                for o in node.output:
+                    if o in consumed_by.keys():
+                        for con in consumed_by[o]:
+                            dependencies[con]-=1
+            queue.clear()
         return ordered_nodes
 
     def graph_reorder_nodes(self):
-        ordered_nodes=self.reorder_nodes(self.nodemap.keys(),self.input)
+        ordered_nodes = self.topsort_nodes(self.nodemap.keys(), self.input)
         new_map = {}
         for nname in ordered_nodes:
             new_map[nname] = self.nodemap[nname]
         self.nodemap = new_map
         self.update_tensor_relations()
 
     def get_iotensors(self, nodenames, remove_initials=True):
```

### Comparing `onnx-tool-0.7.1/onnx_tool/model.py` & `onnx-tool-0.7.2/onnx_tool/model.py`

 * *Files identical despite different names*

### Comparing `onnx-tool-0.7.1/onnx_tool/node.py` & `onnx-tool-0.7.2/onnx_tool/node.py`

 * *Files identical despite different names*

### Comparing `onnx-tool-0.7.1/onnx_tool/serialization.py` & `onnx-tool-0.7.2/onnx_tool/serialization.py`

 * *Files identical despite different names*

### Comparing `onnx-tool-0.7.1/onnx_tool/tensor.py` & `onnx-tool-0.7.2/onnx_tool/tensor.py`

 * *Files identical despite different names*

### Comparing `onnx-tool-0.7.1/onnx_tool/utils.py` & `onnx-tool-0.7.2/onnx_tool/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import time
 import warnings
 
-VERSION = "0.7.1"
+VERSION = "0.7.2"
 
 
 class timer():
     def __init__(self):
         self._startt = time.time()
 
     def start(self):
```

### Comparing `onnx-tool-0.7.1/onnx_tool.egg-info/PKG-INFO` & `onnx-tool-0.7.2/onnx_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnx-tool
-Version: 0.7.1
+Version: 0.7.2
 Summary: A tool for ONNX model:Rapid shape inference; Profile model; Compute Graph and Shape Engine; OPs fusion;Quantized models and sparse models are supported.
 Home-page: https://github.com/ThanatosShinji/onnx-tool
 Author: Luo Yu
 Author-email: luoyu888888@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: onnx-tool Version: 0.7.1 Summary: A tool for ONNX
+Metadata-Version: 2.1 Name: onnx-tool Version: 0.7.2 Summary: A tool for ONNX
 model:Rapid shape inference; Profile model; Compute Graph and Shape Engine; OPs
 fusion;Quantized models and sparse models are supported. Home-page: https://
 github.com/ThanatosShinji/onnx-tool Author: Luo Yu Author-email:
 luoyu888888@gmail.com License: MIT Classifier: Programming Language :: Python
 :: 3 Description-Content-Type: text/markdown License-File: LICENSE ç®ä½ä¸­æ
 # onnx-tool **A tool for ONNX model:** * *Rapid shape inference.* * *Profile
 model.* * *Constant_Folding.* * *Compute Graph and Shape Engine.* * *OPs
```

### Comparing `onnx-tool-0.7.1/setup.py` & `onnx-tool-0.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 readme = open("README.md", encoding="utf-8").read()
-VERSION = "0.7.1"
+VERSION = "0.7.2"
 
 requirements = [
     "onnx",
     "numpy",
     'tabulate'
 ]
```


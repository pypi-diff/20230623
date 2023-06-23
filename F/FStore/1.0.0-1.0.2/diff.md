# Comparing `tmp/FStore-1.0.0.tar.gz` & `tmp/FStore-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FStore-1.0.0.tar", last modified: Tue Aug 23 02:06:54 2022, max compression
+gzip compressed data, was "FStore-1.0.2.tar", last modified: Fri Jun 23 02:50:46 2023, max compression
```

## Comparing `FStore-1.0.0.tar` & `FStore-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 02:06:54.867393 FStore-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 02:06:54.863393 FStore-1.0.0/FStore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-08-23 02:06:54.000000 FStore-1.0.0/FStore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      250 2022-08-23 02:06:54.000000 FStore-1.0.0/FStore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-23 02:06:54.000000 FStore-1.0.0/FStore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-08-23 02:06:54.000000 FStore-1.0.0/FStore.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-08-23 02:06:54.000000 FStore-1.0.0/FStore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-08-23 02:06:44.000000 FStore-1.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-08-23 02:06:54.867393 FStore-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      331 2022-08-23 02:06:44.000000 FStore-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-23 02:06:54.867393 FStore-1.0.0/fstore/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-23 02:06:44.000000 FStore-1.0.0/fstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3216 2022-08-23 02:06:44.000000 FStore-1.0.0/fstore/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2913 2022-08-23 02:06:44.000000 FStore-1.0.0/fstore/binary_search_tree.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-23 02:06:54.867393 FStore-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      551 2022-08-23 02:06:44.000000 FStore-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:50:46.147256 FStore-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:50:46.147256 FStore-1.0.2/FStore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-23 02:50:46.000000 FStore-1.0.2/FStore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-23 02:50:46.000000 FStore-1.0.2/FStore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 02:50:46.000000 FStore-1.0.2/FStore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-23 02:50:46.000000 FStore-1.0.2/FStore.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 02:50:46.000000 FStore-1.0.2/FStore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-23 02:50:36.000000 FStore-1.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-23 02:50:46.147256 FStore-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-23 02:50:36.000000 FStore-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 02:50:46.147256 FStore-1.0.2/fstore/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 02:50:36.000000 FStore-1.0.2/fstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-06-23 02:50:36.000000 FStore-1.0.2/fstore/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-06-23 02:50:36.000000 FStore-1.0.2/fstore/binary_search_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 02:50:46.147256 FStore-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-23 02:50:36.000000 FStore-1.0.2/setup.py
```

### Comparing `FStore-1.0.0/FStore.egg-info/PKG-INFO` & `FStore-1.0.2/FStore.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: FStore
-Version: 1.0.0
+Version: 1.0.2
 Summary: Key-value store in Python
 Home-page: https://github.com/colin-m-davis/kvs
 Author: Colin Davis
 Author-email: colinmichaelsdavis@gmail.com
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # FStore
-A simple key-value store written in Python. 
+A simple key-value store written in Python.
+https://pypi.org/project/FStore/
 
 ## Usage
 Install FStore in your terminal with pip: `$ pip install fstore`
 
 Initialize a new FStore database: `$ fstore init [path/to/database]`
 
 Connect to an existing FStore database: `$ store init [path/to/database]`
```

### Comparing `FStore-1.0.0/LICENSE.txt` & `FStore-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `FStore-1.0.0/PKG-INFO` & `FStore-1.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: FStore
-Version: 1.0.0
+Version: 1.0.2
 Summary: Key-value store in Python
 Home-page: https://github.com/colin-m-davis/kvs
 Author: Colin Davis
 Author-email: colinmichaelsdavis@gmail.com
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # FStore
-A simple key-value store written in Python. 
+A simple key-value store written in Python.
+https://pypi.org/project/FStore/
 
 ## Usage
 Install FStore in your terminal with pip: `$ pip install fstore`
 
 Initialize a new FStore database: `$ fstore init [path/to/database]`
 
 Connect to an existing FStore database: `$ store init [path/to/database]`
```

### Comparing `FStore-1.0.0/fstore/__main__.py` & `FStore-1.0.2/fstore/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,16 +80,15 @@
 
             result = binary_search_tree.search(db.root, key)
 
             if result:
                 print(result)
             else:
                 print("(GET) Key not found")
-                
-        
+
         elif cmd == "put":
             key = input("(PUT) Key: ")
             val = input("(PUT) Value: ")
             db.root = binary_search_tree.insert(db.root, key, val)
 
         elif cmd == "del":
             key = input("(DEL) Key: ")
@@ -100,15 +99,15 @@
             
             db.save()
 
             break
 
         else:
             print("Not sure what you meant by that.")
-        
+
         cmd = None
 
 argsp = argsubparsers.add_parser("init", help="Initialize a new database.")
 argsp.add_argument("path", metavar="directory", nargs="?", default="./db", help="Location of database.")
 
 def cmd_init(args):
     db_init(args.path)
@@ -116,8 +115,8 @@
 argsp = argsubparsers.add_parser("connect", help="Connect to an existing database.")
 argsp.add_argument("path", metavar="directory", nargs="?", default="./db", help="Location of database.")
 
 def cmd_connect(args):
     db_connect(args.path)
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `FStore-1.0.0/fstore/binary_search_tree.py` & `FStore-1.0.2/fstore/binary_search_tree.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,71 +1,69 @@
 from collections import deque
 
-# Create a node
 class Node:
+    """tree element"""
     def __init__(self, key, val):
         self.key = key
         self.val = val
         self.left = None
         self.right = None
 
-# Search by key
 def search(root, key):
+    """search tree by key"""
     if not root:
-        return
+        return None
     if key < root.key:
         return search(root.left, key)
-    elif key > root.key:
+    if key > root.key:
         return search(root.right, key)
-    else:
-        return root.val
+    return root.val
 
-# Insert a node
 def insert(root, key, val):
-
+    """insert a node"""
     # Return a new node if the tree is empty
     if not root:
         return Node(key, val)
 
     # Traverse to the right place and insert the node
     if key < root.key:
         root.left = insert(root.left, key, val)
     else:
         root.right = insert(root.right, key, val)
 
     return root
 
-# Find the inorder successor
 def inorder_successor(root):
+    """find inorder successor"""
     current = root
 
-    while(current.left):
+    while current.left:
         current = current.left
 
     return current
 
-# Delete node
 def delete(root, key):
-    # Key is not in tree
+    """delete node"""
     if not root:
+        # Key is not in tree
         return root
 
     # Find the node to be deleted
     if key < root.key:
         root.left = delete(root.left, key)
-    elif(key > root.key):
+    elif key > root.key:
         root.right = delete(root.right, key)
     else:
         # If the node is with only one child or no child
         if root.left is None:
             temp = root.right
             root = None
             return temp
 
-        elif root.right is None:
+        if root.right is None:
             temp = root.left
             root = None
             return temp
 
         # If the node has two children,
         # place the inorder successor in position of the node to be deleted
         temp = inorder_successor(root.right)
@@ -73,19 +71,19 @@
         root.key = temp.key
 
         # Delete the inorder successor
         root.right = delete(root.right, temp.key)
 
     return root
 
-# Serialize tree to string
 def serialize(root):
+    """serialize tree to string"""
     if not root:
         return ""
-    
+
     result = ""
     q = deque()
     q.append(root)
     while len(q) > 0:
         cur = q.popleft()
         if cur:
             result += str(cur.key) + ":" + str(cur.val)
@@ -96,35 +94,35 @@
             if cur.right:
                 q.append(cur.right)
             else:
                 q.append(None)
         else:
             result += "NULL:NULL"
         result += ","
-    
+
     return result
 
-# Deserialize tree from string
 def deserialize(string):
+    """deserialize tree from string"""
     # Parse string into array of strings
     tmp = string.split(",")
     data = []
 
     for i in range(len(tmp)-1):
         # Separate strings into key-value pairs
         data.append(tmp[i].split(":"))
 
     return make(data)
 
-# Make tree from array of key-value pairs
 def make(elements):
+    """make tree from array of key-value pairs"""
     root = None
 
     for element in elements:
         key = element[0]
         val = element[1]
 
         # Skip over null nodes
         if key != "NULL":
             root = insert(root, key, val)
-        
+
     return root
```

### Comparing `FStore-1.0.0/setup.py` & `FStore-1.0.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='FStore',
-    version='1.0.0',
+    version='1.0.2',
     author='Colin Davis',
     author_email='colinmichaelsdavis@gmail.com',
     packages=find_packages(),
     url='https://github.com/colin-m-davis/kvs',
     license='LICENSE.txt',
     description='Key-value store in Python',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=[],
     entry_points = {
         'console_scripts': [
             'fstore = fstore.__main__:main'
         ]
     }
-)
+)
```


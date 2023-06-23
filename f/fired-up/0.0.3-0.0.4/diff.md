# Comparing `tmp/fired-up-0.0.3.tar.gz` & `tmp/fired-up-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fired-up-0.0.3.tar", last modified: Fri Jun 23 11:16:46 2023, max compression
+gzip compressed data, was "fired-up-0.0.4.tar", last modified: Fri Jun 23 13:46:10 2023, max compression
```

## Comparing `fired-up-0.0.3.tar` & `fired-up-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-06-23 11:16:46.260281 fired-up-0.0.3/
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-06-23 11:16:46.259401 fired-up-0.0.3/.github/
--rw-r--r--   0 xtof       (501) staff       (20)     4387 2023-06-23 10:53:42.000000 fired-up-0.0.3/.github/README.md
--rw-r--r--   0 xtof       (501) staff       (20)     1057 2023-06-22 20:12:57.000000 fired-up-0.0.3/LICENSE.txt
--rw-r--r--   0 xtof       (501) staff       (20)       77 2023-06-20 11:24:03.000000 fired-up-0.0.3/MANIFEST.in
--rw-r--r--   0 xtof       (501) staff       (20)     6070 2023-06-23 11:16:46.260173 fired-up-0.0.3/PKG-INFO
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-06-23 11:16:46.259513 fired-up-0.0.3/fired_up/
--rw-r--r--   0 xtof       (501) staff       (20)     2156 2023-06-23 11:14:56.000000 fired-up-0.0.3/fired_up/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-06-23 11:16:46.260015 fired-up-0.0.3/fired_up.egg-info/
--rw-r--r--   0 xtof       (501) staff       (20)     6070 2023-06-23 11:16:46.000000 fired-up-0.0.3/fired_up.egg-info/PKG-INFO
--rw-r--r--   0 xtof       (501) staff       (20)      230 2023-06-23 11:16:46.000000 fired-up-0.0.3/fired_up.egg-info/SOURCES.txt
--rw-r--r--   0 xtof       (501) staff       (20)        1 2023-06-23 11:16:46.000000 fired-up-0.0.3/fired_up.egg-info/dependency_links.txt
--rw-r--r--   0 xtof       (501) staff       (20)        5 2023-06-23 11:16:46.000000 fired-up-0.0.3/fired_up.egg-info/requires.txt
--rw-r--r--   0 xtof       (501) staff       (20)        9 2023-06-23 11:16:46.000000 fired-up-0.0.3/fired_up.egg-info/top_level.txt
--rw-r--r--   0 xtof       (501) staff       (20)       38 2023-06-23 11:16:46.260329 fired-up-0.0.3/setup.cfg
--rw-r--r--   0 xtof       (501) staff       (20)     1385 2023-06-22 20:20:12.000000 fired-up-0.0.3/setup.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-06-23 13:46:10.024715 fired-up-0.0.4/
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-06-23 13:46:10.023804 fired-up-0.0.4/.github/
+-rw-r--r--   0 xtof       (501) staff       (20)     5174 2023-06-23 13:44:41.000000 fired-up-0.0.4/.github/README.md
+-rw-r--r--   0 xtof       (501) staff       (20)     1057 2023-06-22 20:12:57.000000 fired-up-0.0.4/LICENSE.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       77 2023-06-20 11:24:03.000000 fired-up-0.0.4/MANIFEST.in
+-rw-r--r--   0 xtof       (501) staff       (20)     7177 2023-06-23 13:46:10.024601 fired-up-0.0.4/PKG-INFO
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-06-23 13:46:10.023921 fired-up-0.0.4/fired_up/
+-rw-r--r--   0 xtof       (501) staff       (20)     3043 2023-06-23 13:44:51.000000 fired-up-0.0.4/fired_up/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-06-23 13:46:10.024436 fired-up-0.0.4/fired_up.egg-info/
+-rw-r--r--   0 xtof       (501) staff       (20)     7177 2023-06-23 13:46:09.000000 fired-up-0.0.4/fired_up.egg-info/PKG-INFO
+-rw-r--r--   0 xtof       (501) staff       (20)      230 2023-06-23 13:46:10.000000 fired-up-0.0.4/fired_up.egg-info/SOURCES.txt
+-rw-r--r--   0 xtof       (501) staff       (20)        1 2023-06-23 13:46:09.000000 fired-up-0.0.4/fired_up.egg-info/dependency_links.txt
+-rw-r--r--   0 xtof       (501) staff       (20)        5 2023-06-23 13:46:09.000000 fired-up-0.0.4/fired_up.egg-info/requires.txt
+-rw-r--r--   0 xtof       (501) staff       (20)        9 2023-06-23 13:46:09.000000 fired-up-0.0.4/fired_up.egg-info/top_level.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       38 2023-06-23 13:46:10.024751 fired-up-0.0.4/setup.cfg
+-rw-r--r--   0 xtof       (501) staff       (20)     1385 2023-06-22 20:20:12.000000 fired-up-0.0.4/setup.py
```

### Comparing `fired-up-0.0.3/.github/README.md` & `fired-up-0.0.4/.github/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -146,7 +146,47 @@
 ```
 
 ```console
 % python examples/globals.py left write then right readwrite then left read
 right> left was here
 left> right was here too
 ```
+
+### Menus
+
+The FireUp class is kind of a Menu of Groups of Commands. You cal also nest Menus of your own:
+
+```python
+import json
+
+from fired_up import FiredUp, Menu, Group
+
+class Commands(Group):
+  def run(self):
+    print("Commands> running...")
+
+class SubCommands(Group):
+  def run(self):
+    print("SubCommands> running...")
+
+class SubSubCommands(Group):
+  def run(self):
+    print("SubSubCommands> running...")
+
+FiredUp(
+  commands=Commands,
+  submenu=Menu(
+    commands=SubCommands,
+    subsubmenu=Menu(
+      commands=SubSubCommands
+    )
+  )
+)
+```
+
+```console
+% python examples/nested.py commands run then submenu commands run then commands run then submenu subsubmenu commands run
+Commands> running...
+SubCommands> running...
+Commands> running...
+SubSubCommands> running...
+```
```

### Comparing `fired-up-0.0.3/LICENSE.txt` & `fired-up-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fired-up-0.0.3/PKG-INFO` & `fired-up-0.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fired-up
-Version: 0.0.3
+Version: 0.0.4
 Summary: conventions and supporting tools for using Fire in a more natural-ish language style
 Home-page: https://github.com/christophevg/fired-up
 Author: Christophe VG
 License: MIT
 Description: # Fired Up
         
         > conventions and supporting tools for using Fire in a more natural-ish style
@@ -154,13 +154,53 @@
         
         ```console
         % python examples/globals.py left write then right readwrite then left read
         right> left was here
         left> right was here too
         ```
         
+        ### Menus
+        
+        The FireUp class is kind of a Menu of Groups of Commands. You cal also nest Menus of your own:
+        
+        ```python
+        import json
+        
+        from fired_up import FiredUp, Menu, Group
+        
+        class Commands(Group):
+          def run(self):
+            print("Commands> running...")
+        
+        class SubCommands(Group):
+          def run(self):
+            print("SubCommands> running...")
+        
+        class SubSubCommands(Group):
+          def run(self):
+            print("SubSubCommands> running...")
+        
+        FiredUp(
+          commands=Commands,
+          submenu=Menu(
+            commands=SubCommands,
+            subsubmenu=Menu(
+              commands=SubSubCommands
+            )
+          )
+        )
+        ```
+        
+        ```console
+        % python examples/nested.py commands run then submenu commands run then commands run then submenu subsubmenu commands run
+        Commands> running...
+        SubCommands> running...
+        Commands> running...
+        SubSubCommands> running...
+        ```
+        
 Keywords: python fire DSL
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `fired-up-0.0.3/fired_up.egg-info/PKG-INFO` & `fired-up-0.0.4/fired_up.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fired-up
-Version: 0.0.3
+Version: 0.0.4
 Summary: conventions and supporting tools for using Fire in a more natural-ish language style
 Home-page: https://github.com/christophevg/fired-up
 Author: Christophe VG
 License: MIT
 Description: # Fired Up
         
         > conventions and supporting tools for using Fire in a more natural-ish style
@@ -154,13 +154,53 @@
         
         ```console
         % python examples/globals.py left write then right readwrite then left read
         right> left was here
         left> right was here too
         ```
         
+        ### Menus
+        
+        The FireUp class is kind of a Menu of Groups of Commands. You cal also nest Menus of your own:
+        
+        ```python
+        import json
+        
+        from fired_up import FiredUp, Menu, Group
+        
+        class Commands(Group):
+          def run(self):
+            print("Commands> running...")
+        
+        class SubCommands(Group):
+          def run(self):
+            print("SubCommands> running...")
+        
+        class SubSubCommands(Group):
+          def run(self):
+            print("SubSubCommands> running...")
+        
+        FiredUp(
+          commands=Commands,
+          submenu=Menu(
+            commands=SubCommands,
+            subsubmenu=Menu(
+              commands=SubSubCommands
+            )
+          )
+        )
+        ```
+        
+        ```console
+        % python examples/nested.py commands run then submenu commands run then commands run then submenu subsubmenu commands run
+        Commands> running...
+        SubCommands> running...
+        Commands> running...
+        SubSubCommands> running...
+        ```
+        
 Keywords: python fire DSL
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `fired-up-0.0.3/setup.py` & `fired-up-0.0.4/setup.py`

 * *Files identical despite different names*


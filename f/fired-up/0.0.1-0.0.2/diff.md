# Comparing `tmp/fired-up-0.0.1.tar.gz` & `tmp/fired-up-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fired-up-0.0.1.tar", last modified: Thu Jun 22 20:23:31 2023, max compression
+gzip compressed data, was "fired-up-0.0.2.tar", last modified: Fri Jun 23 10:54:50 2023, max compression
```

## Comparing `fired-up-0.0.1.tar` & `fired-up-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-06-22 20:23:31.194704 fired-up-0.0.1/
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-06-22 20:23:31.193836 fired-up-0.0.1/.github/
--rw-r--r--   0 xtof       (501) staff       (20)     3593 2023-06-22 20:16:57.000000 fired-up-0.0.1/.github/README.md
--rw-r--r--   0 xtof       (501) staff       (20)     1057 2023-06-22 20:12:57.000000 fired-up-0.0.1/LICENSE.txt
--rw-r--r--   0 xtof       (501) staff       (20)       77 2023-06-20 11:24:03.000000 fired-up-0.0.1/MANIFEST.in
--rw-r--r--   0 xtof       (501) staff       (20)     4964 2023-06-22 20:23:31.194600 fired-up-0.0.1/PKG-INFO
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-06-22 20:23:31.193944 fired-up-0.0.1/fired_up/
--rw-r--r--   0 xtof       (501) staff       (20)     1896 2023-06-22 20:18:54.000000 fired-up-0.0.1/fired_up/__init__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-06-22 20:23:31.194440 fired-up-0.0.1/fired_up.egg-info/
--rw-r--r--   0 xtof       (501) staff       (20)     4964 2023-06-22 20:23:31.000000 fired-up-0.0.1/fired_up.egg-info/PKG-INFO
--rw-r--r--   0 xtof       (501) staff       (20)      230 2023-06-22 20:23:31.000000 fired-up-0.0.1/fired_up.egg-info/SOURCES.txt
--rw-r--r--   0 xtof       (501) staff       (20)        1 2023-06-22 20:23:31.000000 fired-up-0.0.1/fired_up.egg-info/dependency_links.txt
--rw-r--r--   0 xtof       (501) staff       (20)        5 2023-06-22 20:23:31.000000 fired-up-0.0.1/fired_up.egg-info/requires.txt
--rw-r--r--   0 xtof       (501) staff       (20)        9 2023-06-22 20:23:31.000000 fired-up-0.0.1/fired_up.egg-info/top_level.txt
--rw-r--r--   0 xtof       (501) staff       (20)       38 2023-06-22 20:23:31.194738 fired-up-0.0.1/setup.cfg
--rw-r--r--   0 xtof       (501) staff       (20)     1385 2023-06-22 20:20:12.000000 fired-up-0.0.1/setup.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-06-23 10:54:50.250022 fired-up-0.0.2/
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-06-23 10:54:50.249140 fired-up-0.0.2/.github/
+-rw-r--r--   0 xtof       (501) staff       (20)     4387 2023-06-23 10:53:42.000000 fired-up-0.0.2/.github/README.md
+-rw-r--r--   0 xtof       (501) staff       (20)     1057 2023-06-22 20:12:57.000000 fired-up-0.0.2/LICENSE.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       77 2023-06-20 11:24:03.000000 fired-up-0.0.2/MANIFEST.in
+-rw-r--r--   0 xtof       (501) staff       (20)     6070 2023-06-23 10:54:50.249919 fired-up-0.0.2/PKG-INFO
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-06-23 10:54:50.249242 fired-up-0.0.2/fired_up/
+-rw-r--r--   0 xtof       (501) staff       (20)     2156 2023-06-23 10:47:08.000000 fired-up-0.0.2/fired_up/__init__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-06-23 10:54:50.249754 fired-up-0.0.2/fired_up.egg-info/
+-rw-r--r--   0 xtof       (501) staff       (20)     6070 2023-06-23 10:54:50.000000 fired-up-0.0.2/fired_up.egg-info/PKG-INFO
+-rw-r--r--   0 xtof       (501) staff       (20)      230 2023-06-23 10:54:50.000000 fired-up-0.0.2/fired_up.egg-info/SOURCES.txt
+-rw-r--r--   0 xtof       (501) staff       (20)        1 2023-06-23 10:54:50.000000 fired-up-0.0.2/fired_up.egg-info/dependency_links.txt
+-rw-r--r--   0 xtof       (501) staff       (20)        5 2023-06-23 10:54:50.000000 fired-up-0.0.2/fired_up.egg-info/requires.txt
+-rw-r--r--   0 xtof       (501) staff       (20)        9 2023-06-23 10:54:50.000000 fired-up-0.0.2/fired_up.egg-info/top_level.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       38 2023-06-23 10:54:50.250056 fired-up-0.0.2/setup.cfg
+-rw-r--r--   0 xtof       (501) staff       (20)     1385 2023-06-22 20:20:12.000000 fired-up-0.0.2/setup.py
```

### Comparing `fired-up-0.0.1/.github/README.md` & `fired-up-0.0.2/.github/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -7,14 +7,20 @@
 [![Built with PyPi Template](https://img.shields.io/badge/PyPi_Template-v0.2.0-blue.svg)](https://github.com/christophevg/pypi-template)
 
 
 ## A command line DSL using Fire
 
 `Fire` is a fun module that allows for providing a quick and beautiful command line interface on top of a Python module. `Fired Up` adds some baseclasses and conventions to make this experience even more fun, by adding the possibility to chain multiple top-level commands/classes, using a shared clipboard.
 
+### Minimal Survival Command
+
+```console
+% pip install fired-up
+```
+
 ### An example
 
 With `Fired Up` it is possible to run a command like this:
 
 ```console
 % python examples/hello.py generate a_reversed_list 1,a,2,b then dump as_json
 [
@@ -90,24 +96,57 @@
 ```
 
 > I'm not happy yet with the required changes, so improvements will be imminent ;-)
 
 For now, it runs the same and offers improved chaining possibilities:
 
 ```conole
-% PYTHONPATH=. python examples/fire-group.py ingestion run
+% python examples/fire-group.py ingestion run
 Ingesting! Nom nom nom...
-% PYTHONPATH=. python examples/fire-group.py digestion run
+% python examples/fire-group.py digestion run
 Burp!
-% PYTHONPATH=. python examples/fire-group.py digestion status
+% python examples/fire-group.py digestion status
 Satiated.
-% PYTHONPATH=. python examples/fire-group.py ingestion run then digestion run status
+% python examples/fire-group.py ingestion run then digestion run status
 Satiated.
-% PYTHONPATH=. python examples/fire-group.py --all ingestion run then digestion run status
+% python examples/fire-group.py --all ingestion run then digestion run status
 Ingesting! Nom nom nom...
 Burp!
 Satiated.
-% PYTHONPATH=. python examples/fire-group.py --all ingestion run then digestion volume 2 run status
+% python examples/fire-group.py --all ingestion run then digestion volume 2 run status
 Ingesting! Nom nom nom...
 Burp! Burp!
 Satiated.
 ```
+
+### Globals and Arguments
+
+Besides the versioned clipboard, you can also use globals and pass arguments to the constructors of the Groups:
+
+```python
+from fired_up import FiredUp, Group
+
+class Left(Group):
+  def __init__(self, write, *args, **kwargs):
+    super().__init__(*args, **kwargs)
+    self._write = write
+
+  def write(self):
+    if self._write:
+      self.globals["message"] = "left was here"
+
+  def read(self):
+    print("left>", self.globals["message"])
+
+class Right(Group):
+  def readwrite(self):
+    print("right>", self.globals["message"])
+    self.globals["message"] = "right was here too"
+
+FiredUp(left=(Left, { "write" : True }), right=Right)
+```
+
+```console
+% python examples/globals.py left write then right readwrite then left read
+right> left was here
+left> right was here too
+```
```

### Comparing `fired-up-0.0.1/LICENSE.txt` & `fired-up-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fired-up-0.0.1/PKG-INFO` & `fired-up-0.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fired-up
-Version: 0.0.1
+Version: 0.0.2
 Summary: conventions and supporting tools for using Fire in a more natural-ish language style
 Home-page: https://github.com/christophevg/fired-up
 Author: Christophe VG
 License: MIT
 Description: # Fired Up
         
         > conventions and supporting tools for using Fire in a more natural-ish style
@@ -14,14 +14,20 @@
         [![Built with PyPi Template](https://img.shields.io/badge/PyPi_Template-v0.2.0-blue.svg)](https://github.com/christophevg/pypi-template)
         
         
         ## A command line DSL using Fire
         
         `Fire` is a fun module that allows for providing a quick and beautiful command line interface on top of a Python module. `Fired Up` adds some baseclasses and conventions to make this experience even more fun, by adding the possibility to chain multiple top-level commands/classes, using a shared clipboard.
         
+        ### Minimal Survival Command
+        
+        ```console
+        % pip install fired-up
+        ```
+        
         ### An example
         
         With `Fired Up` it is possible to run a command like this:
         
         ```console
         % python examples/hello.py generate a_reversed_list 1,a,2,b then dump as_json
         [
@@ -97,31 +103,64 @@
         ```
         
         > I'm not happy yet with the required changes, so improvements will be imminent ;-)
         
         For now, it runs the same and offers improved chaining possibilities:
         
         ```conole
-        % PYTHONPATH=. python examples/fire-group.py ingestion run
+        % python examples/fire-group.py ingestion run
         Ingesting! Nom nom nom...
-        % PYTHONPATH=. python examples/fire-group.py digestion run
+        % python examples/fire-group.py digestion run
         Burp!
-        % PYTHONPATH=. python examples/fire-group.py digestion status
+        % python examples/fire-group.py digestion status
         Satiated.
-        % PYTHONPATH=. python examples/fire-group.py ingestion run then digestion run status
+        % python examples/fire-group.py ingestion run then digestion run status
         Satiated.
-        % PYTHONPATH=. python examples/fire-group.py --all ingestion run then digestion run status
+        % python examples/fire-group.py --all ingestion run then digestion run status
         Ingesting! Nom nom nom...
         Burp!
         Satiated.
-        % PYTHONPATH=. python examples/fire-group.py --all ingestion run then digestion volume 2 run status
+        % python examples/fire-group.py --all ingestion run then digestion volume 2 run status
         Ingesting! Nom nom nom...
         Burp! Burp!
         Satiated.
         ```
         
+        ### Globals and Arguments
+        
+        Besides the versioned clipboard, you can also use globals and pass arguments to the constructors of the Groups:
+        
+        ```python
+        from fired_up import FiredUp, Group
+        
+        class Left(Group):
+          def __init__(self, write, *args, **kwargs):
+            super().__init__(*args, **kwargs)
+            self._write = write
+        
+          def write(self):
+            if self._write:
+              self.globals["message"] = "left was here"
+        
+          def read(self):
+            print("left>", self.globals["message"])
+        
+        class Right(Group):
+          def readwrite(self):
+            print("right>", self.globals["message"])
+            self.globals["message"] = "right was here too"
+        
+        FiredUp(left=(Left, { "write" : True }), right=Right)
+        ```
+        
+        ```console
+        % python examples/globals.py left write then right readwrite then left read
+        right> left was here
+        left> right was here too
+        ```
+        
 Keywords: python fire DSL
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `fired-up-0.0.1/fired_up/__init__.py` & `fired-up-0.0.2/fired_up/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 """
 
   conventions and supporting tools for using Fire in a more natural-ish
   language style
 
 """
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 
 import sys
 import functools
 
 import fire
 
 class Group():
   """
   
   baseclass for command groups
   
   """
-  def __init__(self, _shared=None, _exit=None):
-    self._shared = _shared
-    self._exit   = _exit
+  def __init__(self, _clipboard=None, _exit=None, _globals=None):
+    self.globals    = _globals
+    self._clipboard = _clipboard
+    self._exit      = _exit
 
   def then(self):
-    # next(self._shared)
+    # next(self._clipboard)
     return self._exit
 
   def copy(self, value, name="default"):
-    self._shared[name] = value
+    self._clipboard[name] = value
     return self
 
   def paste(self, name="default"):
-    return self._shared[name]
+    return self._clipboard[name]
 
 def keep(method):
   @functools.wraps(method)
   def wrapper(self, *args, **kwargs):
     result = method(self, *args, **kwargs)
     self.copy(result)
     if result:
-      next(self._shared)
+      next(self._clipboard)
     return self
   return wrapper
 
 class Clipboards():
   """
   
   simple multi-clipboard support
@@ -67,24 +68,34 @@
 
   def __str__(self):
     return str(self._boards)
 
 if "--all" in sys.argv:
   sys.argv.remove("--all")
   def paste_result(obj):
-    return [board["default"] for board in obj._shared._boards[:-1] ]
+    return [board["default"] for board in obj._clipboard._boards[:-1] ]
 else:
   def paste_result(obj):
     return obj.paste()
 
 class FiredUp(Group):
-  def __init__(self, name=None, *args, **kwargs):
-    self._shared = Clipboards()
+  def __init__(self, name=None, **kwargs):
+    self._globals = {}
+    self._clipboard  = Clipboards()
     for group, clazz in kwargs.items():
+      if type(clazz) is tuple:
+        clazz, args = clazz
+      else:
+        args = {}
       for attr in clazz.__dict__:
         if callable(getattr(clazz, attr)) and attr != "__init__":
           setattr(clazz, attr, keep(getattr(clazz, attr)))
-      self.__dict__[group] = clazz(_shared=self._shared, _exit=self)
+      self.__dict__[group] = clazz(
+        _globals=self._globals,
+        _clipboard=self._clipboard,
+        _exit=self,
+        **args
+      )
     try:
       fire.Fire(self, name=name, serialize=paste_result)
     except KeyboardInterrupt:
       pass
```

### Comparing `fired-up-0.0.1/fired_up.egg-info/PKG-INFO` & `fired-up-0.0.2/fired_up.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fired-up
-Version: 0.0.1
+Version: 0.0.2
 Summary: conventions and supporting tools for using Fire in a more natural-ish language style
 Home-page: https://github.com/christophevg/fired-up
 Author: Christophe VG
 License: MIT
 Description: # Fired Up
         
         > conventions and supporting tools for using Fire in a more natural-ish style
@@ -14,14 +14,20 @@
         [![Built with PyPi Template](https://img.shields.io/badge/PyPi_Template-v0.2.0-blue.svg)](https://github.com/christophevg/pypi-template)
         
         
         ## A command line DSL using Fire
         
         `Fire` is a fun module that allows for providing a quick and beautiful command line interface on top of a Python module. `Fired Up` adds some baseclasses and conventions to make this experience even more fun, by adding the possibility to chain multiple top-level commands/classes, using a shared clipboard.
         
+        ### Minimal Survival Command
+        
+        ```console
+        % pip install fired-up
+        ```
+        
         ### An example
         
         With `Fired Up` it is possible to run a command like this:
         
         ```console
         % python examples/hello.py generate a_reversed_list 1,a,2,b then dump as_json
         [
@@ -97,31 +103,64 @@
         ```
         
         > I'm not happy yet with the required changes, so improvements will be imminent ;-)
         
         For now, it runs the same and offers improved chaining possibilities:
         
         ```conole
-        % PYTHONPATH=. python examples/fire-group.py ingestion run
+        % python examples/fire-group.py ingestion run
         Ingesting! Nom nom nom...
-        % PYTHONPATH=. python examples/fire-group.py digestion run
+        % python examples/fire-group.py digestion run
         Burp!
-        % PYTHONPATH=. python examples/fire-group.py digestion status
+        % python examples/fire-group.py digestion status
         Satiated.
-        % PYTHONPATH=. python examples/fire-group.py ingestion run then digestion run status
+        % python examples/fire-group.py ingestion run then digestion run status
         Satiated.
-        % PYTHONPATH=. python examples/fire-group.py --all ingestion run then digestion run status
+        % python examples/fire-group.py --all ingestion run then digestion run status
         Ingesting! Nom nom nom...
         Burp!
         Satiated.
-        % PYTHONPATH=. python examples/fire-group.py --all ingestion run then digestion volume 2 run status
+        % python examples/fire-group.py --all ingestion run then digestion volume 2 run status
         Ingesting! Nom nom nom...
         Burp! Burp!
         Satiated.
         ```
         
+        ### Globals and Arguments
+        
+        Besides the versioned clipboard, you can also use globals and pass arguments to the constructors of the Groups:
+        
+        ```python
+        from fired_up import FiredUp, Group
+        
+        class Left(Group):
+          def __init__(self, write, *args, **kwargs):
+            super().__init__(*args, **kwargs)
+            self._write = write
+        
+          def write(self):
+            if self._write:
+              self.globals["message"] = "left was here"
+        
+          def read(self):
+            print("left>", self.globals["message"])
+        
+        class Right(Group):
+          def readwrite(self):
+            print("right>", self.globals["message"])
+            self.globals["message"] = "right was here too"
+        
+        FiredUp(left=(Left, { "write" : True }), right=Right)
+        ```
+        
+        ```console
+        % python examples/globals.py left write then right readwrite then left read
+        right> left was here
+        left> right was here too
+        ```
+        
 Keywords: python fire DSL
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `fired-up-0.0.1/setup.py` & `fired-up-0.0.2/setup.py`

 * *Files identical despite different names*


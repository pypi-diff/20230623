# Comparing `tmp/clearconf-0.2.tar.gz` & `tmp/clearconf-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clearconf-0.2.tar", max compression
+gzip compressed data, was "clearconf-0.3.tar", max compression
```

## Comparing `clearconf-0.2.tar` & `clearconf-0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0        0 2022-09-27 07:32:12.000000 clearconf-0.2/README.md
--rw-r--r--   0        0        0       37 2023-03-09 11:05:52.349840 clearconf-0.2/clearconf/__init__.py
--rw-r--r--   0        0        0     1745 2023-03-09 10:40:27.689995 clearconf-0.2/clearconf/assets/example_conf.py
--rw-r--r--   0        0        0      968 2023-03-09 10:43:17.689976 clearconf-0.2/clearconf/assets/init.py
--rw-r--r--   0        0        0      213 2023-03-09 10:40:27.689995 clearconf-0.2/clearconf/assets/stub_conf.py
--rw-r--r--   0        0        0     5433 2023-03-07 15:58:21.118270 clearconf-0.2/clearconf/base_config.py
--rw-r--r--   0        0        0        0 2022-09-27 06:44:08.000000 clearconf-0.2/clearconf/cli/__init__.py
--rw-r--r--   0        0        0      930 2023-03-09 10:45:19.289963 clearconf-0.2/clearconf/cli/defaults.py
--rw-r--r--   0        0        0     1729 2023-03-09 10:41:59.379984 clearconf-0.2/clearconf/cli/main.py
--rw-r--r--   0        0        0        0 2023-03-07 17:46:25.227838 clearconf-0.2/clearconf/utils/__init__.py
--rw-r--r--   0        0        0      746 2023-03-09 10:37:23.100013 clearconf-0.2/clearconf/utils/conf.py
--rw-r--r--   0        0        0      917 2023-03-08 15:22:36.900532 clearconf-0.2/clearconf/utils/file.py
--rw-r--r--   0        0        0      509 2023-03-09 10:37:23.090013 clearconf-0.2/clearconf/utils/stdout.py
--rw-r--r--   0        0        0      357 2023-03-09 11:08:02.509830 clearconf-0.2/pyproject.toml
--rw-r--r--   0        0        0      469 1970-01-01 00:00:00.000000 clearconf-0.2/PKG-INFO
+-rw-r--r--   0        0        0     2786 2023-06-22 21:13:09.616037 clearconf-0.3/README.md
+-rw-r--r--   0        0        0       37 2023-06-22 21:13:09.616037 clearconf-0.3/clearconf/__init__.py
+-rw-r--r--   0        0        0     1745 2023-06-22 21:13:09.626037 clearconf-0.3/clearconf/assets/example_conf.py
+-rw-r--r--   0        0        0      968 2023-06-22 21:13:09.626037 clearconf-0.3/clearconf/assets/init.py
+-rw-r--r--   0        0        0      213 2023-06-22 21:13:09.626037 clearconf-0.3/clearconf/assets/stub_conf.py
+-rw-r--r--   0        0        0     5801 2023-06-22 21:55:36.506018 clearconf-0.3/clearconf/base_config.py
+-rw-r--r--   0        0        0        0 2023-06-22 21:13:09.626037 clearconf-0.3/clearconf/cli/__init__.py
+-rw-r--r--   0        0        0      930 2023-06-22 21:13:09.626037 clearconf-0.3/clearconf/cli/defaults.py
+-rw-r--r--   0        0        0     1729 2023-06-22 21:13:09.626037 clearconf-0.3/clearconf/cli/main.py
+-rw-r--r--   0        0        0        0 2023-06-22 21:13:09.626037 clearconf-0.3/clearconf/utils/__init__.py
+-rw-r--r--   0        0        0      746 2023-06-22 21:13:09.626037 clearconf-0.3/clearconf/utils/conf.py
+-rw-r--r--   0        0        0      917 2023-06-22 21:13:09.626037 clearconf-0.3/clearconf/utils/file.py
+-rw-r--r--   0        0        0      509 2023-06-22 21:13:09.626037 clearconf-0.3/clearconf/utils/stdout.py
+-rw-r--r--   0        0        0      721 2023-06-22 22:05:46.806016 clearconf-0.3/pyproject.toml
+-rw-r--r--   0        0        0     3522 1970-01-01 00:00:00.000000 clearconf-0.3/PKG-INFO
```

### Comparing `clearconf-0.2/clearconf/assets/example_conf.py` & `clearconf-0.3/clearconf/assets/example_conf.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.2/clearconf/assets/init.py` & `clearconf-0.3/clearconf/assets/init.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.2/clearconf/base_config.py` & `clearconf-0.3/clearconf/base_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import __main__
 import collections
 import inspect
 import json
 from pathlib import Path
 
 
-class BaseConfig:
+class Watcher(type):
+    def __init__(cls, name, bases, clsdict):
+        if len(cls.mro()) > 2:
+            cls._subclass()
+        super(Watcher, cls).__init__(name, bases, clsdict)
 
-    @classmethod
-    def init(cls):
-        cls._subclass()
+class BaseConfig(metaclass=Watcher):
 
     @classmethod
     def to_json(cls):
         return json.dumps(cls.to_dict())
 
     @classmethod
     def to_dict(cls):
@@ -42,14 +44,16 @@
                     if type(attr).__name__ == 'function':
                         if attr.__name__ == '<lambda>':
                             funcString = str(inspect.getsourcelines(attr)[0])
                             res[k] = funcString.strip("['\\n']").split(" = ")[1]
                         else:
                             res[k] = f'function : {attr.__name__}'
                     elif attr.__module__.split('.')[0] == '__main__' or 'config' in attr.__module__:
+                        if len(attr.mro()) >= 5: # when a config class is subclassed to use it directly
+                            k = attr.mro()[3].__name__ 
                         res[k] = attr.to_dict()
                     else:
                         # End up here if attr is not a class defined inside module.
                         # e.g. built-in types, functions, etc.
                         if type(attr).__name__ == 'type':
                             name = attr.__name__
                         else:
@@ -109,14 +113,17 @@
                     else:
                         res.append(f'{attr.__module__}.{attr.__name__}')
                 # If it's not a class save it. This is done for basic types.
                 # Could cause problems with complex objects
                 else:
                     res.append(attr)
         return res
+    
+    def get_cfg(self):
+        return self.__class__
 
     def __getattribute__(self, item):
         return object.__getattribute__(self, item)
 
 
 def flatten(d, parent_key='', sep='.'):
     items = []
```

### Comparing `clearconf-0.2/clearconf/cli/defaults.py` & `clearconf-0.3/clearconf/cli/defaults.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.2/clearconf/cli/main.py` & `clearconf-0.3/clearconf/cli/main.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.2/clearconf/utils/conf.py` & `clearconf-0.3/clearconf/utils/conf.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.2/clearconf/utils/file.py` & `clearconf-0.3/clearconf/utils/file.py`

 * *Files identical despite different names*


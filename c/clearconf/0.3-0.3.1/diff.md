# Comparing `tmp/clearconf-0.3.tar.gz` & `tmp/clearconf-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clearconf-0.3.tar", max compression
+gzip compressed data, was "clearconf-0.3.1.tar", max compression
```

## Comparing `clearconf-0.3.tar` & `clearconf-0.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     2786 2023-06-22 21:13:09.616037 clearconf-0.3/README.md
--rw-r--r--   0        0        0       37 2023-06-22 21:13:09.616037 clearconf-0.3/clearconf/__init__.py
--rw-r--r--   0        0        0     1745 2023-06-22 21:13:09.626037 clearconf-0.3/clearconf/assets/example_conf.py
--rw-r--r--   0        0        0      968 2023-06-22 21:13:09.626037 clearconf-0.3/clearconf/assets/init.py
--rw-r--r--   0        0        0      213 2023-06-22 21:13:09.626037 clearconf-0.3/clearconf/assets/stub_conf.py
--rw-r--r--   0        0        0     5801 2023-06-22 21:55:36.506018 clearconf-0.3/clearconf/base_config.py
--rw-r--r--   0        0        0        0 2023-06-22 21:13:09.626037 clearconf-0.3/clearconf/cli/__init__.py
--rw-r--r--   0        0        0      930 2023-06-22 21:13:09.626037 clearconf-0.3/clearconf/cli/defaults.py
--rw-r--r--   0        0        0     1729 2023-06-22 21:13:09.626037 clearconf-0.3/clearconf/cli/main.py
--rw-r--r--   0        0        0        0 2023-06-22 21:13:09.626037 clearconf-0.3/clearconf/utils/__init__.py
--rw-r--r--   0        0        0      746 2023-06-22 21:13:09.626037 clearconf-0.3/clearconf/utils/conf.py
--rw-r--r--   0        0        0      917 2023-06-22 21:13:09.626037 clearconf-0.3/clearconf/utils/file.py
--rw-r--r--   0        0        0      509 2023-06-22 21:13:09.626037 clearconf-0.3/clearconf/utils/stdout.py
--rw-r--r--   0        0        0      721 2023-06-22 22:05:46.806016 clearconf-0.3/pyproject.toml
--rw-r--r--   0        0        0     3522 1970-01-01 00:00:00.000000 clearconf-0.3/PKG-INFO
+-rw-r--r--   0        0        0     2786 2023-06-22 21:13:09.616037 clearconf-0.3.1/README.md
+-rw-r--r--   0        0        0       37 2023-06-22 21:13:09.616037 clearconf-0.3.1/clearconf/__init__.py
+-rw-r--r--   0        0        0     1745 2023-06-22 21:13:09.626037 clearconf-0.3.1/clearconf/assets/example_conf.py
+-rw-r--r--   0        0        0      968 2023-06-22 21:13:09.626037 clearconf-0.3.1/clearconf/assets/init.py
+-rw-r--r--   0        0        0      213 2023-06-22 21:13:09.626037 clearconf-0.3.1/clearconf/assets/stub_conf.py
+-rw-r--r--   0        0        0     5834 2023-06-22 22:22:44.826005 clearconf-0.3.1/clearconf/base_config.py
+-rw-r--r--   0        0        0        0 2023-06-22 21:13:09.626037 clearconf-0.3.1/clearconf/cli/__init__.py
+-rw-r--r--   0        0        0      930 2023-06-22 21:13:09.626037 clearconf-0.3.1/clearconf/cli/defaults.py
+-rw-r--r--   0        0        0     1729 2023-06-22 21:13:09.626037 clearconf-0.3.1/clearconf/cli/main.py
+-rw-r--r--   0        0        0        0 2023-06-22 21:13:09.626037 clearconf-0.3.1/clearconf/utils/__init__.py
+-rw-r--r--   0        0        0      746 2023-06-22 21:13:09.626037 clearconf-0.3.1/clearconf/utils/conf.py
+-rw-r--r--   0        0        0      917 2023-06-22 21:13:09.626037 clearconf-0.3.1/clearconf/utils/file.py
+-rw-r--r--   0        0        0      509 2023-06-22 21:13:09.626037 clearconf-0.3.1/clearconf/utils/stdout.py
+-rw-r--r--   0        0        0      723 2023-06-22 22:26:28.545992 clearconf-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3524 1970-01-01 00:00:00.000000 clearconf-0.3.1/PKG-INFO
```

### Comparing `clearconf-0.3/README.md` & `clearconf-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `clearconf-0.3/clearconf/assets/example_conf.py` & `clearconf-0.3.1/clearconf/assets/example_conf.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.3/clearconf/assets/init.py` & `clearconf-0.3.1/clearconf/assets/init.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.3/clearconf/base_config.py` & `clearconf-0.3.1/clearconf/base_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         # This removes variables from superclasses
         for i in range(3, len(target.__mro__) - 1):
             # The if allows inheritance between configs but I guess there are better solutions
             if 'configs' not in target.__mro__[i].__module__:
                 target_attr = target_attr - set(dir(target.__mro__[i]))
 
         for k in target_attr:
-            if not k.startswith('_') and k not in ['to_dict', 'to_json', 'to_list', 'init', 'to_flat_dict']:
+            if not k.startswith('_') and k not in ['to_dict', 'to_json', 'to_list', 'init', 'to_flat_dict', 'get_cfg']:
                 attr = getattr(target, k)
 
                 # If it's a module get inside
                 if hasattr(attr, '__module__'):
 
                     # If it's a class inside config, get inside it,
                     # else just log module and name in the dict as a string.
@@ -68,15 +68,15 @@
     @classmethod
     def _subclass(cls):
 
         target = cls
 
         res = {}
         for k in dir(target):
-            if not k.startswith('_') and k not in ['to_dict', 'to_json', 'to_list', 'init', 'to_flat_dict']:
+            if not k.startswith('_') and k not in ['to_dict', 'to_json', 'to_list', 'init', 'to_flat_dict', 'get_cfg']:
                 attr = getattr(target, k)
                 # If it's a class inside config, get inside it,
                 # else just log module and name in the dict as a string
                 if hasattr(attr, '__module__') and type(attr).__name__ != 'function':
 
                     # if we are executing the config the module is __main__. If we are importing it is config
                     # Not ideal but config could be anywhere in the name
@@ -99,15 +99,15 @@
 
     @classmethod
     def to_list(cls):
         target = cls
 
         res = []
         for k in dir(target):
-            if not k.startswith('_') and k not in ['to_dict', 'to_json', 'to_list', 'init', 'to_flat_dict']:
+            if not k.startswith('_') and k not in ['to_dict', 'to_json', 'to_list', 'init', 'to_flat_dict', 'get_cfg']:
                 attr = getattr(target, k)
                 # If it's a class inside config, get inside it,
                 # else just log module and name in the dict as a string
                 if type(attr) == type:
                     if attr.__module__.split('.')[0] in ['configs', '__main__']:
                         res.append(attr.to_list())
                     else:
```

### Comparing `clearconf-0.3/clearconf/cli/defaults.py` & `clearconf-0.3.1/clearconf/cli/defaults.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.3/clearconf/cli/main.py` & `clearconf-0.3.1/clearconf/cli/main.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.3/clearconf/utils/conf.py` & `clearconf-0.3.1/clearconf/utils/conf.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.3/clearconf/utils/file.py` & `clearconf-0.3.1/clearconf/utils/file.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.3/pyproject.toml` & `clearconf-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clearconf"
-version = "0.3"
+version = "0.3.1"
 description = "ClearConf is a library created to support easy and manageble python configuration. It consists in a CLI tool to manage the configuration directory, and in a python class (BaseConfig) which adds additional functionalities to a configuration class."
 authors = ["andrearosasco <andrea.rosasco@iit.it>"]
 homepage = "https://github.com/andrearosasco/clearconf"
 repository = "https://github.com/andrearosasco/clearconf"
 readme = "README.md"
```

### Comparing `clearconf-0.3/PKG-INFO` & `clearconf-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clearconf
-Version: 0.3
+Version: 0.3.1
 Summary: ClearConf is a library created to support easy and manageble python configuration. It consists in a CLI tool to manage the configuration directory, and in a python class (BaseConfig) which adds additional functionalities to a configuration class.
 Home-page: https://github.com/andrearosasco/clearconf
 Author: andrearosasco
 Author-email: andrea.rosasco@iit.it
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```


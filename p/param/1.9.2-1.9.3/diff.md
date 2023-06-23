# Comparing `tmp/param-1.9.2.tar.gz` & `tmp/param-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/param-1.9.2.tar", last modified: Tue Oct  8 14:06:10 2019, max compression
+gzip compressed data, was "dist/param-1.9.3.tar", last modified: Sun Jan 26 20:58:49 2020, max compression
```

## Comparing `param-1.9.2.tar` & `param-1.9.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 14:06:10.000000 param-1.9.2/
--rw-rw-r--   0 travis    (2000) travis    (2000)      141 2019-10-08 14:05:43.000000 param-1.9.2/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     1499 2019-10-08 14:05:43.000000 param-1.9.2/LICENSE.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     2912 2019-10-08 14:06:10.000000 param-1.9.2/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 14:06:10.000000 param-1.9.2/numbergen/
--rw-rw-r--   0 travis    (2000) travis    (2000)    26699 2019-10-08 14:05:43.000000 param-1.9.2/numbergen/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      334 2019-10-08 14:06:10.000000 param-1.9.2/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 14:06:10.000000 param-1.9.2/param.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2912 2019-10-08 14:06:10.000000 param-1.9.2/param.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-10-08 14:06:10.000000 param-1.9.2/param.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       16 2019-10-08 14:06:10.000000 param-1.9.2/param.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      309 2019-10-08 14:06:10.000000 param-1.9.2/param.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       40 2019-10-08 14:06:10.000000 param-1.9.2/param.egg-info/requires.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-10-08 14:06:10.000000 param-1.9.2/param/
--rw-rw-r--   0 travis    (2000) travis    (2000)    12582 2019-10-08 14:05:43.000000 param-1.9.2/param/ipython.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    30509 2019-10-08 14:05:43.000000 param-1.9.2/param/version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    70076 2019-10-08 14:05:43.000000 param-1.9.2/param/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   110255 2019-10-08 14:05:43.000000 param-1.9.2/param/parameterized.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       64 2019-10-08 14:06:09.000000 param-1.9.2/param/.version
--rw-rw-r--   0 travis    (2000) travis    (2000)     1502 2019-10-08 14:05:43.000000 param-1.9.2/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     2203 2019-10-08 14:05:43.000000 param-1.9.2/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-26 20:58:49.000000 param-1.9.3/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      141 2020-01-26 20:58:23.000000 param-1.9.3/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1499 2020-01-26 20:58:23.000000 param-1.9.3/LICENSE.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2912 2020-01-26 20:58:49.000000 param-1.9.3/PKG-INFO
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-26 20:58:48.000000 param-1.9.3/numbergen/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26699 2020-01-26 20:58:23.000000 param-1.9.3/numbergen/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      334 2020-01-26 20:58:49.000000 param-1.9.3/setup.cfg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-26 20:58:49.000000 param-1.9.3/param.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2912 2020-01-26 20:58:48.000000 param-1.9.3/param.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-01-26 20:58:48.000000 param-1.9.3/param.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       16 2020-01-26 20:58:48.000000 param-1.9.3/param.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      309 2020-01-26 20:58:48.000000 param-1.9.3/param.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       40 2020-01-26 20:58:48.000000 param-1.9.3/param.egg-info/requires.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-26 20:58:49.000000 param-1.9.3/param/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12582 2020-01-26 20:58:23.000000 param-1.9.3/param/ipython.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30509 2020-01-26 20:58:23.000000 param-1.9.3/param/version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    70242 2020-01-26 20:58:23.000000 param-1.9.3/param/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   110255 2020-01-26 20:58:23.000000 param-1.9.3/param/parameterized.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       64 2020-01-26 20:58:48.000000 param-1.9.3/param/.version
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1502 2020-01-26 20:58:23.000000 param-1.9.3/README.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2203 2020-01-26 20:58:23.000000 param-1.9.3/setup.py
```

### Comparing `param-1.9.2/LICENSE.txt` & `param-1.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `param-1.9.2/PKG-INFO` & `param-1.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: param
-Version: 1.9.2
+Version: 1.9.3
 Summary: Declarative Python programming using Parameters.
 Home-page: http://ioam.github.com/param/
 Author: IOAM
 Author-email: developers@topographica.org
 Maintainer: IOAM
 Maintainer-email: developers@topographica.org
 License: BSD
```

### Comparing `param-1.9.2/numbergen/__init__.py` & `param-1.9.3/numbergen/__init__.py`

 * *Files identical despite different names*

### Comparing `param-1.9.2/param.egg-info/PKG-INFO` & `param-1.9.3/param.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: param
-Version: 1.9.2
+Version: 1.9.3
 Summary: Declarative Python programming using Parameters.
 Home-page: http://ioam.github.com/param/
 Author: IOAM
 Author-email: developers@topographica.org
 Maintainer: IOAM
 Maintainer-email: developers@topographica.org
 License: BSD
```

### Comparing `param-1.9.2/param/ipython.py` & `param-1.9.3/param/ipython.py`

 * *Files identical despite different names*

### Comparing `param-1.9.2/param/version.py` & `param-1.9.3/param/version.py`

 * *Files identical despite different names*

### Comparing `param-1.9.2/param/__init__.py` & `param-1.9.3/param/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1288,15 +1288,15 @@
                                       instantiate=instantiate,
                                       compute_default_fn=compute_default_fn,
                                       check_on_set=check_on_set,
                                       allow_None=allow_None, **params)
 
 class ClassSelector(SelectorBase):
     """
-    Parameter whose value is a specified class or an instance of that class.
+    Parameter allowing selection of either a subclass or an instance of a given set of classes.
     By default, requires an instance, but if is_instance=False, accepts a class instead.
     Both class and instance values respect the instantiate slot, though it matters only
     for is_instance=True.
     """
 
     __slots__ = ['class_','is_instance']
 
@@ -1331,16 +1331,19 @@
 
         (I.e. return {name: <class>} for all classes that are
         concrete_descendents() of self.class_.)
 
         Only classes from modules that have been imported are added
         (see concrete_descendents()).
         """
-        classes = concrete_descendents(self.class_)
-        d=OrderedDict((name,class_) for name,class_ in classes.items())
+        classes = self.class_ if isinstance(self.class_, tuple) else (self.class_,)
+        all_classes = {}
+        for cls in classes:
+            all_classes.update(concrete_descendents(cls))
+        d=OrderedDict((name,class_) for name,class_ in all_classes.items())
         if self.allow_None:
             d['None']=None
         return d
 
 
 class List(Parameter):
     """
```

### Comparing `param-1.9.2/param/parameterized.py` & `param-1.9.3/param/parameterized.py`

 * *Files identical despite different names*

### Comparing `param-1.9.2/README.rst` & `param-1.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `param-1.9.2/setup.py` & `param-1.9.3/setup.py`

 * *Files identical despite different names*


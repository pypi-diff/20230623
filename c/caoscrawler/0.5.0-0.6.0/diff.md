# Comparing `tmp/caoscrawler-0.5.0.tar.gz` & `tmp/caoscrawler-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caoscrawler-0.5.0.tar", last modified: Tue Mar 28 12:56:50 2023, max compression
+gzip compressed data, was "caoscrawler-0.6.0.tar", last modified: Fri Jun 23 14:28:38 2023, max compression
```

## Comparing `caoscrawler-0.5.0.tar` & `caoscrawler-0.6.0.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-03-28 12:56:50.696446 caoscrawler-0.5.0/
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    34459 2022-04-20 13:57:35.000000 caoscrawler-0.5.0/LICENSE
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3035 2023-03-28 12:56:50.696446 caoscrawler-0.5.0/PKG-INFO
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     2598 2023-01-30 14:52:30.000000 caoscrawler-0.5.0/README.md
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      920 2023-03-28 12:56:50.696446 caoscrawler-0.5.0/setup.cfg
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      206 2022-04-20 13:57:35.000000 caoscrawler-0.5.0/setup.py
-drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-03-28 12:56:50.693113 caoscrawler-0.5.0/src/
-drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-03-28 12:56:50.696446 caoscrawler-0.5.0/src/caoscrawler/
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      154 2023-03-28 12:52:28.000000 caoscrawler-0.5.0/src/caoscrawler/__init__.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     1235 2022-10-11 13:45:05.000000 caoscrawler-0.5.0/src/caoscrawler/authorize.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     2785 2023-03-22 13:07:35.000000 caoscrawler-0.5.0/src/caoscrawler/cfood-schema.yml
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    43362 2023-03-22 13:07:35.000000 caoscrawler-0.5.0/src/caoscrawler/converters.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    51779 2023-03-28 12:52:28.000000 caoscrawler-0.5.0/src/caoscrawler/crawl.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     2450 2023-03-28 12:52:28.000000 caoscrawler-0.5.0/src/caoscrawler/debug_tree.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     2083 2023-03-22 13:07:35.000000 caoscrawler-0.5.0/src/caoscrawler/default_converters.yml
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2022-10-11 13:45:05.000000 caoscrawler-0.5.0/src/caoscrawler/extension-converters-config-schema.yml
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     6385 2023-03-22 13:07:35.000000 caoscrawler-0.5.0/src/caoscrawler/identifiable.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    19443 2023-03-24 09:41:17.000000 caoscrawler-0.5.0/src/caoscrawler/identifiable_adapters.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     2530 2023-01-30 14:52:30.000000 caoscrawler-0.5.0/src/caoscrawler/identified_cache.py
-drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-03-28 12:56:50.696446 caoscrawler-0.5.0/src/caoscrawler/macros/
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)       71 2022-10-11 13:45:05.000000 caoscrawler-0.5.0/src/caoscrawler/macros/__init__.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     5198 2023-01-30 14:52:30.000000 caoscrawler-0.5.0/src/caoscrawler/macros/macro_yaml_object.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    18147 2023-03-28 12:52:28.000000 caoscrawler-0.5.0/src/caoscrawler/scanner.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3203 2022-10-11 13:45:05.000000 caoscrawler-0.5.0/src/caoscrawler/stores.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     4255 2023-01-30 14:52:30.000000 caoscrawler-0.5.0/src/caoscrawler/structure_elements.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     1250 2022-10-11 13:45:05.000000 caoscrawler-0.5.0/src/caoscrawler/utils.py
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3296 2023-03-28 12:52:28.000000 caoscrawler-0.5.0/src/caoscrawler/version.py
-drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-03-28 12:56:50.696446 caoscrawler-0.5.0/src/caoscrawler.egg-info/
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3035 2023-03-28 12:56:50.000000 caoscrawler-0.5.0/src/caoscrawler.egg-info/PKG-INFO
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      872 2023-03-28 12:56:50.000000 caoscrawler-0.5.0/src/caoscrawler.egg-info/SOURCES.txt
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        1 2023-03-28 12:56:50.000000 caoscrawler-0.5.0/src/caoscrawler.egg-info/dependency_links.txt
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)       58 2023-03-28 12:56:50.000000 caoscrawler-0.5.0/src/caoscrawler.egg-info/entry_points.txt
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      151 2023-03-28 12:56:50.000000 caoscrawler-0.5.0/src/caoscrawler.egg-info/requires.txt
--rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)       12 2023-03-28 12:56:50.000000 caoscrawler-0.5.0/src/caoscrawler.egg-info/top_level.txt
+drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-06-23 14:28:38.842576 caoscrawler-0.6.0/
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    34459 2022-01-21 09:13:50.000000 caoscrawler-0.6.0/LICENSE
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3035 2023-06-23 14:28:38.842576 caoscrawler-0.6.0/PKG-INFO
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     2598 2023-06-23 14:27:16.000000 caoscrawler-0.6.0/README.md
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      919 2023-06-23 14:28:38.842576 caoscrawler-0.6.0/setup.cfg
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      206 2022-01-21 09:13:50.000000 caoscrawler-0.6.0/setup.py
+drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-06-23 14:28:38.842576 caoscrawler-0.6.0/src/
+drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-06-23 14:28:38.842576 caoscrawler-0.6.0/src/caoscrawler/
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      154 2023-06-23 14:27:16.000000 caoscrawler-0.6.0/src/caoscrawler/__init__.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     1235 2022-10-11 13:56:19.000000 caoscrawler-0.6.0/src/caoscrawler/authorize.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     2785 2023-06-23 14:27:16.000000 caoscrawler-0.6.0/src/caoscrawler/cfood-schema.yml
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     1246 2023-06-23 14:27:16.000000 caoscrawler-0.6.0/src/caoscrawler/config.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    43266 2023-06-23 14:27:16.000000 caoscrawler-0.6.0/src/caoscrawler/converters.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    61468 2023-06-23 14:27:16.000000 caoscrawler-0.6.0/src/caoscrawler/crawl.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     2450 2023-06-23 14:27:16.000000 caoscrawler-0.6.0/src/caoscrawler/debug_tree.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     2083 2023-06-23 14:27:16.000000 caoscrawler-0.6.0/src/caoscrawler/default_converters.yml
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2022-10-11 13:56:19.000000 caoscrawler-0.6.0/src/caoscrawler/extension-converters-config-schema.yml
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     6385 2023-06-23 14:27:16.000000 caoscrawler-0.6.0/src/caoscrawler/identifiable.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    20053 2023-06-23 14:27:16.000000 caoscrawler-0.6.0/src/caoscrawler/identifiable_adapters.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     2530 2023-06-23 14:27:16.000000 caoscrawler-0.6.0/src/caoscrawler/identified_cache.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     2950 2023-06-23 14:27:16.000000 caoscrawler-0.6.0/src/caoscrawler/logging.py
+drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-06-23 14:28:38.842576 caoscrawler-0.6.0/src/caoscrawler/macros/
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)       71 2022-10-11 13:56:19.000000 caoscrawler-0.6.0/src/caoscrawler/macros/__init__.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     5198 2023-06-23 14:27:16.000000 caoscrawler-0.6.0/src/caoscrawler/macros/macro_yaml_object.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)    17476 2023-06-23 14:27:16.000000 caoscrawler-0.6.0/src/caoscrawler/scanner.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3203 2022-10-11 13:56:19.000000 caoscrawler-0.6.0/src/caoscrawler/stores.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     4255 2023-06-23 14:27:16.000000 caoscrawler-0.6.0/src/caoscrawler/structure_elements.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     1250 2022-10-11 13:56:19.000000 caoscrawler-0.6.0/src/caoscrawler/utils.py
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3296 2023-06-23 14:27:16.000000 caoscrawler-0.6.0/src/caoscrawler/version.py
+drwxr-xr-x   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        0 2023-06-23 14:28:38.842576 caoscrawler-0.6.0/src/caoscrawler.egg-info/
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)     3035 2023-06-23 14:28:38.000000 caoscrawler-0.6.0/src/caoscrawler.egg-info/PKG-INFO
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      925 2023-06-23 14:28:38.000000 caoscrawler-0.6.0/src/caoscrawler.egg-info/SOURCES.txt
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)        1 2023-06-23 14:28:38.000000 caoscrawler-0.6.0/src/caoscrawler.egg-info/dependency_links.txt
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)       58 2023-06-23 14:28:38.000000 caoscrawler-0.6.0/src/caoscrawler.egg-info/entry_points.txt
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)      150 2023-06-23 14:28:38.000000 caoscrawler-0.6.0/src/caoscrawler.egg-info/requires.txt
+-rw-r--r--   0 fspreck_indiscale  (1001) fspreck_indiscale  (1001)       12 2023-06-23 14:28:38.000000 caoscrawler-0.6.0/src/caoscrawler.egg-info/top_level.txt
```

### Comparing `caoscrawler-0.5.0/LICENSE` & `caoscrawler-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `caoscrawler-0.5.0/PKG-INFO` & `caoscrawler-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caoscrawler
-Version: 0.5.0
+Version: 0.6.0
 Summary: A new crawler for caosdb
 Author: Alexander Schlemmer
 Author-email: alexander.schlemmer@ds.mpg.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `caoscrawler-0.5.0/README.md` & `caoscrawler-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `caoscrawler-0.5.0/setup.cfg` & `caoscrawler-0.6.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = caoscrawler
-version = 0.5.0
+version = 0.6.0
 author = Alexander Schlemmer
 author_email = alexander.schlemmer@ds.mpg.de
 description = A new crawler for caosdb
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
@@ -14,15 +14,15 @@
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.7
 install_requires = 
 	importlib-resources
-	caosdb >= 0.11.0
+	caosdb > 0.11.2
 	caosadvancedtools >= 0.7.0
 	yaml-header-tools >= 0.2.1
 	pyyaml
 	odfpy #make optional
 	pandas
 	importlib_metadata;python_version<'3.8'
```

### Comparing `caoscrawler-0.5.0/src/caoscrawler/authorize.py` & `caoscrawler-0.6.0/src/caoscrawler/authorize.py`

 * *Files identical despite different names*

### Comparing `caoscrawler-0.5.0/src/caoscrawler/cfood-schema.yml` & `caoscrawler-0.6.0/src/caoscrawler/cfood-schema.yml`

 * *Files identical despite different names*

### Comparing `caoscrawler-0.5.0/src/caoscrawler/converters.py` & `caoscrawler-0.6.0/src/caoscrawler/converters.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,18 +111,19 @@
     """To be raised if contents of an element to be converted are invalid."""
 
     def __init__(self, msg):
         self.message = msg
 
 
 def create_path_value(func):
-    """decorator for create_values functions that adds a value containing the path
+    """Decorator for create_values functions that adds a value containing the path.
 
     should be used for StructureElement that are associated with file system objects that have a
     path, like File or Directory.
+
     """
 
     def inner(self, values: GeneralStore, element: StructureElement):
         func(self, values=values, element=element)
         values.update({self.name + ".path": element.path})
     return inner
 
@@ -151,30 +152,36 @@
                 return values[varname]
 
     propvalue_template = CrawlerTemplate(propvalue)
     return propvalue_template.safe_substitute(**values.get_storage())
 
 
 def handle_value(value: Union[dict, str, list], values: GeneralStore):
-    """
-    determines whether the given value needs to set a property, be added to an existing value (create a list) or
+    """Determine whether the given value needs to set a property, be added to an existing value (create a list) or
     add as an additional property (multiproperty).
 
     Variable names (starting with a "$") are replaced by the corresponding value stored in the
     `values` GeneralStore.
 
-    Parameters:
-    - value: if str, the value to be interpreted. E.g. "4", "hallo" or "$a" etc.
-             if dict, must have keys "value" and "collection_mode". The returned tuple is directly
-             created from the corresponding values.
-             if list, each element is checked for replacement and the resulting list will be used
-             as (list) value for the property
-    Returns a tuple:
-    - the final value of the property; variable names contained in `values` are replaced.
-    - the collection mode (can be single, list or multiproperty)
+Parameters
+----------
+
+value:
+  - if str, the value to be interpreted. E.g. "4", "hallo" or "$a" etc.
+  - if dict, must have keys "value" and "collection_mode". The returned tuple is directly
+    created from the corresponding values.
+  - if list, each element is checked for replacement and the resulting list will be used
+    as (list) value for the property
+
+Returns
+-------
+
+out: tuple
+  - the final value of the property; variable names contained in `values` are replaced.
+  - the collection mode (can be single, list or multiproperty)
     """
     # @review Florian Spreckelsen 2022-05-13
 
     if type(value) == dict:
         if "value" not in value:
             # TODO: how do we handle this case? Just ignore?
             #       or disallow?
@@ -298,17 +305,15 @@
                 var_replaced_parent = replace_variables(parent, values)
                 if not has_parent(c_record, var_replaced_parent):
                     c_record.add_parent(var_replaced_parent)
     return keys_modified
 
 
 class Converter(object, metaclass=ABCMeta):
-    """
-    Converters treat StructureElements contained in the hierarchical sturcture.
-    """
+    """Converters treat StructureElements contained in the hierarchical sturcture."""
 
     def __init__(self, definition: dict, name: str, converter_registry: dict):
         self.definition = definition
         self.name = name
 
         # Used to store usage information for debugging:
         self.metadata: dict[str, set[str]] = {
@@ -411,25 +416,25 @@
         """
         pass
 
     @staticmethod
     def _debug_matching_template(name: str, regexp: list[str], matched: list[str],
                                  result: Optional[dict]):
         """ Template for the debugging output for the match function """
-        msg = "\n--------" + name + "-----------"
+        msg = "\n--------" + name + "-----------\n"
         for re, ma in zip(regexp, matched):
-            msg += "matching against:\n" + re
-            msg += "matching:\n" + ma
-            msg += "---------"
+            msg += "matching against:\n" + re + "\n"
+            msg += "matching:\n" + ma + "\n"
+            msg += "---------\n"
         if result is None:
             msg += "No match"
         else:
-            msg += "Matched groups:"
+            msg += "Matched groups:\n"
             msg += str(result)
-        msg += "----------------------------------------"
+        msg += "----------------------------------------\n"
         logger.debug(msg)
 
     @staticmethod
     def debug_matching(kind=None):
         def debug_matching_decorator(func):
             """
             decorator for the match function of Converters that implements debug for the match of
@@ -531,17 +536,15 @@
             elif os.path.isfile(path):
                 children.append(File(name, path))
 
         return children
 
 
 class SimpleFileConverter(Converter):
-    """
-    Just a file, ignore the contents.
-    """
+    """Just a file, ignore the contents."""
 
     def typecheck(self, element: StructureElement):
         return isinstance(element, File)
 
     def create_children(self, generalStore: GeneralStore, element: StructureElement):
         return list()
 
@@ -564,17 +567,15 @@
     def __init__(self, *args, **kwargs):
         warnings.warn(DeprecationWarning(
             "This class is depricated. Please use SimpleFileConverter."))
         super().__init__(*args, **kwargs)
 
 
 class MarkdownFileConverter(SimpleFileConverter):
-    """
-    reads the yaml header of markdown files (if a such a header exists).
-    """
+    """Read the yaml header of markdown files (if a such a header exists)."""
 
     def create_children(self, generalStore: GeneralStore, element: StructureElement):
         # TODO: See comment on types and inheritance
         if not isinstance(element, File):
             raise RuntimeError("A markdown file is needed to create children.")
 
         try:
@@ -600,15 +601,15 @@
                 raise RuntimeError(
                     "Header entry {} has incompatible type.".format(name))
         return children
 
 
 def convert_basic_element(element: Union[list, dict, bool, int, float, str, None], name=None,
                           msg_prefix=""):
-    """converts basic Python objects to the corresponding StructureElements """
+    """Convert basic Python objects to the corresponding StructureElements"""
     if isinstance(element, list):
         return ListElement(name, element)
     elif isinstance(element, dict):
         return DictElement(name, element)
     elif isinstance(element, bool):
         return BooleanElement(name, element)
     elif isinstance(element, int):
@@ -624,20 +625,24 @@
     else:
         raise NotImplementedError(
             msg_prefix + f"The object that has an unexpected type: {type(element)}\n"
             f"The object is:\n{str(element)}")
 
 
 def validate_against_json_schema(instance, schema_resource: Union[dict, str]):
-    """validates given ``instance`` against given ``schema_resource``.
+    """Validate given ``instance`` against given ``schema_resource``.
+
+Parameters
+----------
+
+instance:
+  Instance to be validated, typically ``dict`` but can be ``list``, ``str``, etc.
 
-    Args:
-        instance: instance to be validated, typically ``dict`` but can be ``list``, ``str``, etc.
-        schema_resource: Either a path to the JSON file containing the schema or a  ``dict`` with
-        the schema
+schema_resource:
+  Either a path to the JSON file containing the schema or a  ``dict`` with the schema.
     """
     if isinstance(schema_resource, dict):
         schema = schema_resource
     elif isinstance(schema_resource, str):
         with open(schema_resource, 'r') as json_file:
             schema = json.load(json_file)
     else:
@@ -748,23 +753,27 @@
             name=element.name + "_child_dict",
             msg_prefix="The YAML File contained content that was parsed to a Python object"
             " with an unexpected type.")
         return [structure_element]
 
 
 def match_name_and_value(definition, name, value):
-    """
-    takes match definitions from the definition argument and applies regular expressiion to name
-    and possibly value
+    """Take match definitions from the definition argument and apply regular expression to name and
+    possibly value
 
     one of the keys 'match_name' and "match' needs to be available in definition
     'match_value' is optional
 
-    Returns None, if match_name or match lead to no match. Otherwise, returns a dictionary with the
-        matched groups, possibly including matches from using match_value
+Returns
+-------
+
+out:
+  None, if match_name or match lead to no match. Otherwise, returns a dictionary with the
+  matched groups, possibly including matches from using match_value
+
     """
     if "match_name" in definition:
         if "match" in definition:
             raise RuntimeError(f"Do not supply both, 'match_name' and 'match'.")
 
         m1 = re.match(definition["match_name"], name)
         if m1 is None:
@@ -792,19 +801,19 @@
     values = dict()
     values.update(m1)
     values.update(m2)
     return values
 
 
 class _AbstractScalarValueElementConverter(Converter):
-    """
-    A base class for all converters that have a scalar value that can be matched using a regular
+    """A base class for all converters that have a scalar value that can be matched using a regular
     expression.
 
     values must have one of the following type: str, bool, int, float
+
     """
 
     default_matches = {
         "accept_text": False,
         "accept_bool": False,
         "accept_int": False,
         "accept_float": False,
@@ -836,23 +845,22 @@
                 and not isinstance(element, BooleanElement)
                 and not isinstance(element, IntegerElement)
                 and not isinstance(element, FloatElement)):
             raise ValueError("create_children was called with wrong type of StructureElement")
         return match_name_and_value(self.definition, element.name, element.value)
 
     def _typecheck(self, element: StructureElement, allowed_matches: dict):
-        """
-        returns whether the type of StructureElement is accepted.
+        """Return whether the type of StructureElement is accepted.
 
-        Parameters:
-        element: StructureElement, the element that is checked
-        allowed_matches: Dict, a dictionary that defines what types are allowed. It must have the
-                         keys 'accept_text', 'accept_bool', 'accept_int', and 'accept_float'.
+        Parameters: element: StructureElement, the element that is checked allowed_matches: Dict, a
+        dictionary that defines what types are allowed. It must have the keys 'accept_text',
+        'accept_bool', 'accept_int', and 'accept_float'.
 
         returns:  whether or not the converter allows the type of element
+
         """
         if (bool(allowed_matches["accept_text"]) and isinstance(element, TextElement)):
             return True
         elif (bool(allowed_matches["accept_bool"]) and isinstance(element, BooleanElement)):
             return True
         elif (bool(allowed_matches["accept_int"]) and isinstance(element, IntegerElement)):
             return True
@@ -991,22 +999,22 @@
     def __init__(self, *args, **kwargs):
         warnings.warn(DeprecationWarning(
             "This class is depricated. Please use ListElementConverter."))
         super().__init__(*args, **kwargs)
 
 
 class TableConverter(Converter):
-    """
-    This converter reads tables in different formats line by line and
+    """This converter reads tables in different formats line by line and
     allows matching the corresponding rows.
 
     The subtree generated by the table converter consists of DictElements, each being
     a row. The corresponding header elements will become the dictionary keys.
 
     The rows can be matched using a DictElementConverter.
+
     """
     @abstractmethod
     def get_options(self):
         """
         This method needs to be overwritten by the specific table converter to provide
         information about the possible options.
         """
@@ -1096,20 +1104,20 @@
         for index, row in table.iterrows():
             child_elements.append(
                 DictElement(str(index), row.to_dict()))
         return child_elements
 
 
 class DateElementConverter(TextElementConverter):
-    """
-    allows to convert different text formats of dates to Python date objects.
+    """allows to convert different text formats of dates to Python date objects.
 
     The text to be parsed must be contained in the "date" group. The format string can be supplied
     under "dateformat" in the Converter definition. The library used is datetime so see its
     documentation for information on how to create the format string.
+
     """
 
     def match(self, element: StructureElement):
         matches = super().match(element)
         if matches is not None and "date" in matches:
             matches.update({"date": datetime.datetime.strptime(
                 matches["date"],
```

### Comparing `caoscrawler-0.5.0/src/caoscrawler/crawl.py` & `caoscrawler-0.6.0/src/caoscrawler/crawl.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,76 +34,82 @@
 import argparse
 import importlib
 import logging
 import os
 import sys
 import uuid
 import warnings
-import yaml
-
 from argparse import RawTextHelpFormatter
 from collections import defaultdict
 from copy import deepcopy
+from datetime import datetime
 from enum import Enum
-from importlib_resources import files
-from jsonschema import validate
 from typing import Any, Optional, Type, Union
 
 import caosdb as db
-
-from caosadvancedtools.utils import create_entity_link
-from caosadvancedtools.cache import UpdateCache, Cache
+import yaml
+from caosadvancedtools.cache import Cache, UpdateCache
 from caosadvancedtools.crawler import Crawler as OldCrawler
-from caosdb.apiutils import (compare_entities, EntityMergeConflictError,
+from caosadvancedtools.serverside.helper import send_mail
+from caosadvancedtools.utils import create_entity_link
+from caosdb.apiutils import (EntityMergeConflictError, compare_entities,
                              merge_entities)
+from caosdb.cached import cache_clear, cached_get_entity_by
 from caosdb.common.datatype import is_reference
+from caosdb.exceptions import EmptyUniqueQueryError
+from importlib_resources import files
+from jsonschema import validate
 
-from .converters import Converter, DirectoryConverter, ConverterValidationError
+from .config import get_config_setting
+from .converters import Converter, ConverterValidationError, DirectoryConverter
+from .debug_tree import DebugTree
 from .identifiable import Identifiable
-from .identifiable_adapters import (IdentifiableAdapter,
-                                    LocalStorageIdentifiableAdapter,
-                                    CaosDBIdentifiableAdapter)
+from .identifiable_adapters import (CaosDBIdentifiableAdapter,
+                                    IdentifiableAdapter,
+                                    LocalStorageIdentifiableAdapter)
 from .identified_cache import IdentifiedCache
+from .logging import configure_server_side_logging
 from .macros import defmacro_constructor, macro_constructor
+from .scanner import (create_converter_registry, initialize_converters,
+                      load_definition, scan_directory, scan_structure_elements)
 from .stores import GeneralStore, RecordStore
-from .structure_elements import StructureElement, Directory, NoneElement
+from .structure_elements import Directory, NoneElement, StructureElement
 from .version import check_cfood_version
 
-from .scanner import (scan_directory,
-                      load_definition,
-                      create_converter_registry,
-                      initialize_converters,
-                      scan_structure_elements)
-from .debug_tree import DebugTree
-
 logger = logging.getLogger(__name__)
 
 SPECIAL_PROPERTIES_STRICT = ("description", "name", "id", "path")
 SPECIAL_PROPERTIES_NOT_STRICT = ("file", "checksum", "size")
 
 # Register the macro functions from the submodule:
 yaml.SafeLoader.add_constructor("!defmacro", defmacro_constructor)
 yaml.SafeLoader.add_constructor("!macro", macro_constructor)
 
 
+class ForbiddenTransaction(Exception):
+    pass
+
+
 def check_identical(record1: db.Entity, record2: db.Entity, ignore_id=False):
-    """
-    This function uses compare_entities to check whether to entities are identical
-    in a quite complex fashion:
-    - If one of the entities has additional parents or additional properties -> not identical
-    - If the value of one of the properties differs -> not identical
-    - If datatype, importance or unit are reported different for a property by compare_entities
-      return "not_identical" only if these attributes are set explicitely by record1.
-      Ignore the difference otherwise.
-    - If description, name, id or path appear in list of differences -> not identical.
-    - If file, checksum, size appear -> Only different, if explicitely set by record1.
-
-    record1 serves as the reference, so datatype, importance and unit checks are carried
-    out using the attributes from record1. In that respect, the function is not symmetrical
-    in its arguments.
+    """Check whether two entities are identical.
+
+This function uses compare_entities to check whether two entities are identical
+in a quite complex fashion:
+
+- If one of the entities has additional parents or additional properties -> not identical
+- If the value of one of the properties differs -> not identical
+- If datatype, importance or unit are reported different for a property by compare_entities
+   return "not_identical" only if these attributes are set explicitely by record1.
+   Ignore the difference otherwise.
+- If description, name, id or path appear in list of differences -> not identical.
+- If file, checksum, size appear -> Only different, if explicitely set by record1.
+
+record1 serves as the reference, so datatype, importance and unit checks are carried
+out using the attributes from record1. In that respect, the function is not symmetrical
+in its arguments.
     """
     comp = compare_entities(record1, record2)
 
     if ignore_id:
         if "id" in comp[0]:
             del comp[0]["id"]
         if "id" in comp[1]:
@@ -209,15 +215,18 @@
         self._crawled_data = None
 
         # The following caches store records, where we checked whether they exist on the remote
         # server. Since, it is important to know whether they exist or not, we store them into two
         # different caches.
         self.remote_existing_cache = IdentifiedCache()
         self.remote_missing_cache = IdentifiedCache()
+        # TODO does it make sense to have this as member variable?
         self.securityMode = securityMode
+        # TODO does it make sense to have this as member variable(run_id)?
+        self.generate_run_id()
 
         self.identifiableAdapter: IdentifiableAdapter = LocalStorageIdentifiableAdapter()
         if identifiableAdapter is not None:
             self.identifiableAdapter = identifiableAdapter
 
         if debug is not None:
             warnings.warn(DeprecationWarning(
@@ -387,30 +396,31 @@
             if (isinstance(p.value, list)):
                 lst = []
                 for el in p.value:
                     if (isinstance(el, db.Entity) and el.id is None):
                         cached = self.get_from_any_cache(
                             self.identifiableAdapter.get_identifiable(el, referencing_entities))
                         if cached is None:
-                            raise RuntimeError("Not in cache.")
+                            lst.append(el)
+                            continue
                         if not check_identical(cached, el, True):
                             if isinstance(p.value, db.File):
                                 if p.value.path != cached.path:
                                     raise RuntimeError("Not identical.")
                             else:
                                 raise RuntimeError("Not identical.")
                         lst.append(cached)
                     else:
                         lst.append(el)
                 p.value = lst
             if (isinstance(p.value, db.Entity) and p.value.id is None):
                 cached = self.get_from_any_cache(
                     self.identifiableAdapter.get_identifiable(p.value, referencing_entities))
                 if cached is None:
-                    raise RuntimeError("Not in cache.")
+                    continue
                 if not check_identical(cached, p.value, True):
                     if isinstance(p.value, db.File):
                         if p.value.path != cached.path:
                             raise RuntimeError("Not identical.")
                     else:
                         raise RuntimeError("Not identical.")
                 p.value = cached
@@ -559,15 +569,18 @@
                 # 1. Can it be identified via an ID?
                 elif record.id is not None:
                     to_be_updated.append(record)
                     self.add_to_remote_existing_cache(record, identifiable)
                     del flat[i]
                 # 2. Can it be identified via a path?
                 elif record.path is not None:
-                    existing = self._get_entity_by_path(record.path)
+                    try:
+                        existing = cached_get_entity_by(path=record.path)
+                    except EmptyUniqueQueryError:
+                        existing = None
                     if existing is None:
                         to_be_inserted.append(record)
                         self.add_to_remote_missing_cache(record, identifiable)
                         del flat[i]
                     else:
                         record.id = existing.id
                         # TODO check the following copying of _size and _checksum
@@ -618,16 +631,25 @@
                     del flat[i]
                     resolved_references = True
 
             for record in flat:
                 self.replace_references_with_cached(record, referencing_entities)
 
         if len(flat) > 0:
+            circle = self.detect_circular_dependency(flat)
+            if circle is None:
+                logger.error("Failed, but found NO circular dependency. The data is as follows:"
+                             + str(self.compact_entity_list_representation(flat)))
+            else:
+                logger.error("Found circular dependency (Note that this might include references "
+                             "that are not identifying properties): "
+                             + self.compact_entity_list_representation(circle))
             raise RuntimeError(
-                "Could not resolve all Entity references. Circular Dependency?")
+                f"Could not finish split_into_inserts_and_updates. Circular dependency: "
+                f"{circle is not None}")
 
         return to_be_inserted, to_be_updated
 
     def replace_entities_with_ids(self, rec: db.Record):
         for el in rec.properties:
             if isinstance(el.value, db.Entity):
                 if el.value.id is not None:
@@ -635,14 +657,63 @@
             elif isinstance(el.value, list):
                 for index, val in enumerate(el.value):
                     if isinstance(val, db.Entity):
                         if val.id is not None:
                             el.value[index] = val.id
 
     @staticmethod
+    def compact_entity_list_representation(circle):
+        """ a more readable representation than the standard xml representation
+
+        TODO this can be removed once the yaml format representation is in pylib
+        """
+        text = "\n--------\n"
+        for el in circle:
+            if el.name is not None:
+                text += f"{el.name}\n"
+            text += f"{[el.name for el in el.parents]}\n"
+            props = {p.name: p.value for p in el.properties}
+            text += f"{props}\n"
+
+        return text + "--------\n"
+
+    @staticmethod
+    def detect_circular_dependency(flat: list[db.Entity]):
+        """
+        Detects whether there are circular references in the given entity list and returns a list
+        where the entities are ordered according to the chain of references (and only the entities
+        contained in the circle are included. Returns None if no circular dependency is found.
+
+        TODO: for the sake of detecting problems for split_into_inserts_and_updates we should only
+        consider references that are identifying properties.
+        """
+        circle = [flat[0]]
+        closed = False
+        while not closed:
+            current = circle[-1]
+            added_to_circle = False
+            for p in current.properties:
+                if isinstance(p.value, list):
+                    for pval in p.value:
+                        if pval in flat:
+                            if pval in circle:
+                                closed = True
+                            circle.append(pval)
+                            added_to_circle = True
+                else:
+                    if p.value in flat:
+                        if p.value in circle:
+                            closed = True
+                        circle.append(p.value)
+                        added_to_circle = True
+            if not added_to_circle:
+                return None
+        return circle
+
+    @staticmethod
     def _merge_properties_from_remote(
             crawled_data: list[db.Record],
             identified_records: list[db.Record]
     ):
         """Merge entity representation that was created by crawling the data with remotely found
         identified records s.th. new properties and property values are updated correctly but
         additional properties are not overwritten.
@@ -714,15 +785,15 @@
         if they are not updated first.
         """
         logger.debug("=== Going to execute parent updates ===")
         Crawler.set_ids_and_datatype_of_parents_and_properties(to_be_updated)
         parent_updates = db.Container()
 
         for entity in to_be_updated:
-            old_entity = Crawler._get_entity_by_id(entity.id)
+            old_entity = cached_get_entity_by(eid=entity.id)
 
             # Check whether the parents have been changed and add them if missing
             # in the old entity:
             changes_made = False
             for parent in entity.parents:
                 found = False
                 for old_parent in old_entity.parents:
@@ -744,35 +815,20 @@
                 update_cache.insert(parent_updates, run_id)
                 logger.info("Some entities need to be updated because they are missing a parent "
                             "RecordType. The update was NOT executed due to the chosen security "
                             "mode. This might lead to a failure of inserts that follow.")
                 logger.info(parent_updates)
 
     @staticmethod
-    def _get_entity_by_name(name):
-        return db.Entity(name=name).retrieve()
-
-    @staticmethod
-    def _get_entity_by_path(path):
-        try:
-            return db.execute_query(f"FIND FILE WHICH IS STORED AT '{path}'", unique=True)
-        except db.exceptions.EmptyUniqueQueryError:
-            return None
-
-    @staticmethod
-    def _get_entity_by_id(id):
-        return db.Entity(id=id).retrieve()
-
-    @staticmethod
     def execute_inserts_in_list(to_be_inserted, securityMode,
                                 run_id: Optional[uuid.UUID] = None,
                                 unique_names=True):
         for record in to_be_inserted:
             for prop in record.properties:
-                entity = Crawler._get_entity_by_name(prop.name)
+                entity = cached_get_entity_by(name=prop.name)
                 _resolve_datatype(prop, entity)
         logger.debug("INSERT")
         logger.debug(to_be_inserted)
         if len(to_be_inserted) > 0:
             if securityMode.value > SecurityMode.RETRIEVE.value:
                 db.Container().extend(to_be_inserted).insert(unique=unique_names)
             elif run_id is not None:
@@ -780,18 +836,18 @@
                 update_cache.insert(to_be_inserted, run_id, insert=True)
 
     @staticmethod
     def set_ids_and_datatype_of_parents_and_properties(rec_list):
         for record in rec_list:
             for parent in record.parents:
                 if parent.id is None:
-                    parent.id = Crawler._get_entity_by_name(parent.name).id
+                    parent.id = cached_get_entity_by(name=parent.name).id
             for prop in record.properties:
                 if prop.id is None:
-                    entity = Crawler._get_entity_by_name(prop.name)
+                    entity = cached_get_entity_by(name=prop.name)
                     prop.id = entity.id
                     _resolve_datatype(prop, entity)
 
     @staticmethod
     def execute_updates_in_list(to_be_updated, securityMode,
                                 run_id: Optional[uuid.UUID] = None,
                                 unique_names=True):
@@ -801,62 +857,110 @@
         if len(to_be_updated) > 0:
             if securityMode.value > SecurityMode.INSERT.value:
                 db.Container().extend(to_be_updated).update(unique=unique_names)
             elif run_id is not None:
                 update_cache = UpdateCache()
                 update_cache.insert(to_be_updated, run_id)
 
+    @staticmethod
+    def check_whether_parent_exists(records: list[db.Entity], parents: list[str]):
+        """ returns a list of all records in `records` that have a parent that is in `parents`"""
+        problems = []
+        for rec in records:
+            for parent in rec.parents:
+                if parent.name in parents:
+                    problems.append(rec)
+        return problems
+
     def synchronize(self,
                     commit_changes: bool = True,
                     unique_names: bool = True,
                     crawled_data: Optional[list[db.Record]] = None,
+                    no_insert_RTs: Optional[list[str]] = None,
+                    no_update_RTs: Optional[list[str]] = None,
+                    path_for_authorized_run: Optional[str] = "",
                     ):
         """
         This function applies several stages:
         1) Retrieve identifiables for all records in crawled_data.
         2) Compare crawled_data with existing records.
         3) Insert and update records based on the set of identified differences.
 
         This function makes use of an IdentifiableAdapter which is used to retrieve
         register and retrieve identifiables.
 
         if commit_changes is True, the changes are synchronized to the CaosDB server.
         For debugging in can be useful to set this to False.
 
-        Return the final to_be_inserted and to_be_updated as tuple.
+        Parameters
+        ----------
+        no_insert_RTs : list[str], optional
+            list of RecordType names. Records that have one of those RecordTypes
+            as parent will not be inserted
+        no_update_RTs : list[str], optional
+            list of RecordType names. Records that have one of those RecordTypes
+            as parent will not be updated
+        path_for_authorized_run : str, optional
+            only used if there are changes that need authorization before being
+            applied. The form for rerunning the crawler with the authorization
+            of these changes will be generated with this path. See
+            ``caosadvancedtools.crawler.Crawler.save_form`` for more info about
+            the authorization form.
+
+        Returns
+        -------
+        inserts and updates
+            the final to_be_inserted and to_be_updated as tuple.
         """
         if crawled_data is None:
             warnings.warn(DeprecationWarning(
                 "Calling synchronize without the data to be synchronized is depricated. Please "
                 "use for example the Scanner to create this data."))
             crawled_data = self.crawled_data
 
-        self.generate_run_id()
-
         to_be_inserted, to_be_updated = self.split_into_inserts_and_updates(crawled_data)
         referencing_entities = self.create_reference_mapping(to_be_updated + to_be_inserted)
 
-        # TODO: refactoring of typo
         for el in to_be_updated:
             # all entity objects are replaced by their IDs except for the not yet inserted ones
             self.replace_entities_with_ids(el)
 
-        identified_records = [
-            self.identifiableAdapter.retrieve_identified_record_for_record(record,
-                                                                           referencing_entities)
-            for record in to_be_updated]
+        identified_records = []
+        for record in to_be_updated:
+            if record.id is not None:
+                # TODO: use cache here?
+                identified_records.append(cached_get_entity_by(eid=record.id))
+            else:
+                raise Exception("Please report a bug: At this stage all records to be updated"
+                                " should have an ID")
         # Merge with existing data to prevent unwanted overwrites
         to_be_updated = self._merge_properties_from_remote(to_be_updated, identified_records)
         # remove unnecessary updates from list by comparing the target records
         # to the existing ones
         to_be_updated = self.remove_unnecessary_updates(to_be_updated, identified_records)
 
+        if no_insert_RTs:
+            ins_problems = self.check_whether_parent_exists(to_be_inserted, no_insert_RTs)
+        else:
+            ins_problems = []
+        if no_update_RTs:
+            upd_problems = self.check_whether_parent_exists(to_be_updated, no_update_RTs)
+        else:
+            upd_problems = []
+        if len(ins_problems) > 0 or len(upd_problems) > 0:
+            raise ForbiddenTransaction(
+                "One or more Records that have a parent which is excluded from inserts or updates."
+                f"\nRecords excluded from inserts have the following RecordTypes:\n{[el.parents[0].name for el in ins_problems]}"
+                f"\nRecords excluded from updates have the following RecordTypes:\n{[el.parents[0].name for el in upd_problems]}"
+            )
+
         logger.info(f"Going to insert {len(to_be_inserted)} Entities and update "
                     f"{len(to_be_updated)} Entities.")
         if commit_changes:
+            cache_clear()
             self.execute_parent_updates_in_list(to_be_updated, securityMode=self.securityMode,
                                                 run_id=self.run_id, unique_names=unique_names)
             logger.info(f"Added parent RecordTypes where necessary.")
             self.execute_inserts_in_list(
                 to_be_inserted, self.securityMode, self.run_id, unique_names=unique_names)
             logger.info(f"Executed inserts:\n"
                         + self.create_entity_summary(to_be_inserted))
@@ -865,22 +969,20 @@
             logger.info(f"Executed updates:\n"
                         + self.create_entity_summary(to_be_updated))
 
         update_cache = UpdateCache()
         pending_inserts = update_cache.get_inserts(self.run_id)
         if pending_inserts:
             Crawler.inform_about_pending_changes(
-                # TODO crawled_directory is no longer available
-                pending_inserts, self.run_id, "missing crawled_directory")
+                pending_inserts, self.run_id, path_for_authorized_run)
 
         pending_updates = update_cache.get_updates(self.run_id)
         if pending_updates:
             Crawler.inform_about_pending_changes(
-                # TODO crawled_directory is no longer available
-                pending_updates, self.run_id, "missing crawled_directory")
+                pending_updates, self.run_id, path_for_authorized_run)
 
         return (to_be_inserted, to_be_updated)
 
     @staticmethod
     def create_entity_summary(entities: list[db.Entity]):
         """ Creates a summary string reprensentation of a list of entities."""
         parents = {}
@@ -898,17 +1000,15 @@
 
             output = output[:-2] + "\n"
         return output
 
     @staticmethod
     def inform_about_pending_changes(pending_changes, run_id, path, inserts=False):
         # Sending an Email with a link to a form to authorize updates is
-        # only done in SSS mode
-
-        if "SHARED_DIR" in os.environ:
+        if get_config_setting("send_crawler_notifications"):
             filename = OldCrawler.save_form(
                 [el[3] for el in pending_changes], path, run_id)
             OldCrawler.send_mail([el[3] for el in pending_changes], filename)
 
         for i, el in enumerate(pending_changes):
 
             logger.debug(
@@ -968,14 +1068,158 @@
         # paths["converters_usage"] = [self.debug_build_usage_tree(
         #     cv) for cv in self.debug_converters]
 
         with open(filename, "w") as f:
             f.write(yaml.dump(paths, sort_keys=False))
 
 
+def _create_status_record(logfile_url, run_id):
+    """Insert a CrawlerRun Record
+
+    CrawlerRun Records are used to have a (somewhat) persistent feedback from crawler runs that
+    are easyly accessible by users.
+    """
+    if get_config_setting("create_crawler_status_records"):
+        (db.Record()
+            .add_parent('CrawlerRun')
+            .add_property('logfile', logfile_url)
+            .add_property('status', "RUNNING")
+            .add_property('run_id', run_id)
+            .add_property('started', datetime.now().isoformat())
+         .insert())
+
+
+def _update_status_record(run_id, n_inserts, n_updates, status):
+    """Update the CrawlerRun Record
+
+    The Record is identified using the run_id. The status is changed and some information about the
+    run is added.
+    """
+    if get_config_setting("create_crawler_status_records"):
+        cr_rec = db.execute_query(f"FIND RECORD CrawlerRun WITH run_id={run_id}", unique=True)
+        cr_rec.get_property('status').value = status
+        (cr_rec
+            .add_property(db.execute_query(
+                f"FIND Property with name='number_of_inserted_entities'", unique=True).id,
+                n_inserts)
+            .add_property(
+                db.execute_query(f"FIND Property with name='number_of_updated_entities'",
+                                 unique=True).id, n_updates)
+            .add_property(
+                db.execute_query(f"FIND Property with name='finished'",
+                                 unique=True).id, datetime.now().isoformat()))
+        cr_rec.update()
+
+
+def _notify_about_inserts_and_updates(n_inserts, n_updates, logfile, run_id):
+    """send an email notification
+
+    Only if there were inserts or updates.
+
+    The email contains some basic information and a link to the log and the CrawlerRun Record.
+    """
+    if not get_config_setting("send_crawler_notifications"):
+        return
+    if n_inserts == 0 and n_updates == 0:
+        return
+    text = f"""Dear Curator,
+the CaosDB Crawler successfully crawled the data and
+- inserted {n_inserts} new Entities and
+- updated {n_updates} existing Entities.
+
+"""
+
+    if get_config_setting("create_crawler_status_records"):
+        domain = get_config_setting("public_host_url")
+        text += ("You can checkout the CrawlerRun Record for more information:\n"
+                 f"{domain}/Entity/?P=0L10&query=find%20crawlerrun%20with%20run_id=%27{run_id}%27\n\n")
+    text += (f"You can download the logfile here:\n{domain}/Shared/" + logfile)
+    send_mail(
+        from_addr=get_config_setting("sendmail_from_address"),
+        to=get_config_setting("sendmail_to_address"),
+        subject="Crawler Update",
+        body=text)
+
+
+def _treat_deprecated_prefix(prefix, remove_prefix):
+    """notify about deprecation and use given value"""
+    if prefix != "":
+        warnings.warn(DeprecationWarning("The prefix argument is deprecated and will be removed "
+                                         "in the future. Please use `remove_prefix` instead."))
+        if remove_prefix is not None:
+            raise ValueError("Please do not supply the (deprecated) `prefix` and the "
+                             "`remove_prefix` argument at the same time. Only use "
+                             "`remove_prefix` instead.")
+        return prefix
+    return remove_prefix
+
+
+def _fix_file_paths(crawled_data, add_prefix, remove_prefix):
+    """adjust the path according to add_/remove_prefix
+
+    Also remove the `file` attribute from File entities (because inserts need currently be done
+    by loadfiles.
+    """
+    for elem in crawled_data:
+        if isinstance(elem, db.File):
+            # correct the file path:
+            # elem.file = os.path.join(args.path, elem.file)
+            if remove_prefix:
+                if elem.path.startswith(remove_prefix):
+                    elem.path = elem.path[len(remove_prefix):]
+                else:
+                    raise RuntimeError("Prefix shall be removed from file path but the path "
+                                       "does not start with the prefix:"
+                                       f"\n{remove_prefix}\n{elem.path}")
+            if add_prefix:
+                elem.path = add_prefix + elem.path
+            elem.file = None
+            # TODO: as long as the new file backend is not finished
+            #       we are using the loadFiles function to insert symlinks.
+            #       Therefore, I am setting the files to None here.
+            #       Otherwise, the symlinks in the database would be replaced
+            #       by uploads of the files which we currently do not want to happen.
+
+
+def _check_record_types(crawled_data):
+    """Check for all parents in crawled_data whether they exists
+
+    raise Error if it does not
+    """
+    rtsfinder = dict()
+
+    for elem in crawled_data:
+        # Check whether all needed RecordTypes exist:
+        if len(elem.parents) > 0:
+            for parent in elem.parents:
+                if parent.name in rtsfinder:
+                    continue
+
+                rt = db.RecordType(name=parent.name)
+                try:
+                    rt.retrieve()
+                    rtsfinder[parent.name] = True
+                except db.TransactionError:
+                    rtsfinder[parent.name] = False
+
+    notfound = [k for k, v in rtsfinder.items() if not v]
+    if len(notfound) > 0:
+        raise RuntimeError("Missing RecordTypes: {}". format(", ".join(notfound)))
+
+
+def _store_dry_run_data(ins, upd):
+    """write insets and updates to a file """
+    inserts = [str(i) for i in ins]
+    updates = [str(i) for i in upd]
+    with open("dry.yml", "w") as f:
+        f.write(yaml.dump({
+            "insert": inserts,
+            "update": updates}))
+
+
 def crawler_main(crawled_directory_path: str,
                  cfood_file_name: str,
                  identifiables_definition_file: Optional[str] = None,
                  debug: bool = False,
                  provenance_file: Optional[str] = None,
                  dry_run: bool = False,
                  prefix: str = "",
@@ -992,15 +1236,15 @@
     crawled_directory_path : str
         path to be crawled
     cfood_file_name : str
         filename of the cfood to be used
     identifiables_definition_file : str
         filename of an identifiable definition yaml file
     debug : bool
-        whether or not to run in debug mode
+        DEPRECATED, whether or not to run in debug mode
     provenance_file : str
         provenance information will be stored in a file with given filename
     dry_run : bool
         do not commit any chnages to the server
     prefix : str
         DEPRECATED, remove the given prefix from file paths
     securityMode : int
@@ -1016,90 +1260,68 @@
         add the given prefix to file paths
 
     Returns
     -------
     return_value : int
         0 if successful
     """
-    crawler = Crawler(securityMode=securityMode)
     try:
+        crawler = Crawler(securityMode=securityMode)
+
+        # setup logging and reporting if serverside execution
+        if "SHARED_DIR" in os.environ:
+            userlog_public, htmluserlog_public, debuglog_public = configure_server_side_logging()
+            _create_status_record(
+                get_config_setting("public_host_url") + "/Shared/" + htmluserlog_public, crawler.run_id)
 
         debug_tree = DebugTree()
         crawled_data = scan_directory(
             crawled_directory_path, cfood_file_name, restricted_path, debug_tree=debug_tree)
+        _fix_file_paths(crawled_data, add_prefix, remove_prefix)
+        _check_record_types(crawled_data)
+
+        if provenance_file is not None and debug:
+            crawler.save_debug_data(debug_tree=debug_tree, filename=provenance_file)
+
+        if identifiables_definition_file is not None:
+            ident = CaosDBIdentifiableAdapter()
+            ident.load_from_yaml_definition(identifiables_definition_file)
+            crawler.identifiableAdapter = ident
+
+        remove_prefix = _treat_deprecated_prefix(prefix, remove_prefix)
+
+        if dry_run:
+            inserts, updates = crawler.synchronize(commit_changes=False, crawled_data=crawled_data)
+            _store_dry_run_data(inserts, updates)
+        else:
+            inserts, updates = crawler.synchronize(commit_changes=True, unique_names=unique_names,
+                                                   crawled_data=crawled_data,
+                                                   path_for_authorized_run=crawled_directory_path)
+            if "SHARED_DIR" in os.environ:
+                _notify_about_inserts_and_updates(len(inserts), len(updates), userlog_public,
+                                                  crawler.run_id)
+                _update_status_record(crawler.run_id, len(inserts), len(updates), status="OK")
+        return 0
+    except ForbiddenTransaction as err:
+        logger.error(err)
+        _update_status_record(crawler.run_id, 0, 0, status="FAILED")
+        return 1
     except ConverterValidationError as err:
         logger.error(err)
+        _update_status_record(crawler.run_id, 0, 0, status="FAILED")
         return 1
-    if provenance_file is not None and debug:
-        crawler.save_debug_data(debug_tree, provenance_file)
-
-    if identifiables_definition_file is not None:
-        ident = CaosDBIdentifiableAdapter()
-        ident.load_from_yaml_definition(identifiables_definition_file)
-        crawler.identifiableAdapter = ident
-
-    if prefix != "":
-        warnings.warn(DeprecationWarning("The prefix argument is deprecated and will be removed "
-                                         "in the future. Please use `remove_prefix` instead."))
-        if remove_prefix is not None:
-            raise ValueError("Please do not supply the (deprecated) `prefix` and the "
-                             "`remove_prefix` argument at the same time. Only use "
-                             "`remove_prefix` instead.")
-        remove_prefix = prefix
+    except Exception as err:
+        logger.debug(err)
 
-    if dry_run:
-        ins, upd = crawler.synchronize(commit_changes=False, crawled_data=crawled_data)
-        inserts = [str(i) for i in ins]
-        updates = [str(i) for i in upd]
-        with open("dry.yml", "w") as f:
-            f.write(yaml.dump({
-                "insert": inserts,
-                "update": updates}))
-    else:
-        rtsfinder = dict()
-        for elem in crawled_data:
-            if isinstance(elem, db.File):
-                # correct the file path:
-                # elem.file = os.path.join(args.path, elem.file)
-                if remove_prefix:
-                    if elem.path.startswith(remove_prefix):
-                        elem.path = elem.path[len(remove_prefix):]
-                    else:
-                        raise RuntimeError("Prefix shall be removed from file path but the path "
-                                           "does not start with the prefix:"
-                                           f"\n{remove_prefix}\n{elem.path}")
-                if add_prefix:
-                    elem.path = add_prefix + elem.path
-                elem.file = None
-                # TODO: as long as the new file backend is not finished
-                #       we are using the loadFiles function to insert symlinks.
-                #       Therefore, I am setting the files to None here.
-                #       Otherwise, the symlinks in the database would be replaced
-                #       by uploads of the files which we currently do not want to happen.
-
-            # Check whether all needed RecordTypes exist:
-            if len(elem.parents) > 0:
-                for parent in elem.parents:
-                    if parent.name in rtsfinder:
-                        continue
-
-                    rt = db.RecordType(name=parent.name)
-                    try:
-                        rt.retrieve()
-                        rtsfinder[parent.name] = True
-                    except db.TransactionError:
-                        rtsfinder[parent.name] = False
-        notfound = [k for k, v in rtsfinder.items() if not v]
-        if len(notfound) > 0:
-            raise RuntimeError("Missing RecordTypes: {}".
-                               format(", ".join(notfound)))
-
-        crawler.synchronize(commit_changes=True, unique_names=unique_names,
-                            crawled_data=crawled_data)
-    return 0
+        if "SHARED_DIR" in os.environ:
+            domain = get_config_setting("public_host_url")
+            logger.error("Unexpected Error: Please tell your administrator about this and provide the"
+                         f" following path.\n{domain}/Shared/" + debuglog_public)
+        _update_status_record(crawler.run_id, 0, 0, status="FAILED")
+        return 1
 
 
 def parse_args():
     parser = argparse.ArgumentParser(description=__doc__,
                                      formatter_class=RawTextHelpFormatter)
     parser.add_argument("cfood_file_name",
                         help="Path name of the cfood yaml file to be used.")
```

### Comparing `caoscrawler-0.5.0/src/caoscrawler/debug_tree.py` & `caoscrawler-0.6.0/src/caoscrawler/debug_tree.py`

 * *Files identical despite different names*

### Comparing `caoscrawler-0.5.0/src/caoscrawler/default_converters.yml` & `caoscrawler-0.6.0/src/caoscrawler/default_converters.yml`

 * *Files identical despite different names*

### Comparing `caoscrawler-0.5.0/src/caoscrawler/identifiable.py` & `caoscrawler-0.6.0/src/caoscrawler/identifiable.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         if properties is not None and 'name' in [k.lower() for k in properties.keys()]:
             raise ValueError("Please use the separete 'name' keyword instead of the properties "
                              "dict for name")
         self.record_id = record_id
         self.path = path
         self.record_type = record_type
         self.name = name
-        if name is "":
+        if name == "":
             self.name = None
         self.properties: dict = {}
         if properties is not None:
             self.properties = properties
         self.backrefs: list[Union[int, db.Entity]] = []
         if backrefs is not None:
             self.backrefs = backrefs
```

### Comparing `caoscrawler-0.5.0/src/caoscrawler/identifiable_adapters.py` & `caoscrawler-0.6.0/src/caoscrawler/identifiable_adapters.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 # ** end header
 #
 
 from __future__ import annotations
 import yaml
 
 from datetime import datetime
+from caosdb.cached import cached_get_entity_by
 from typing import Any
 from .identifiable import Identifiable
 import caosdb as db
 import logging
 from abc import abstractmethod, ABCMeta
 from .utils import has_parent
 
@@ -62,66 +63,70 @@
         # replace single quotes, otherwise they may break the queries
         return value.replace("\'", "\\'")
     else:
         return str(value)
 
 
 class IdentifiableAdapter(metaclass=ABCMeta):
-    """
-    Base class for identifiable adapters.
+    """Base class for identifiable adapters.
+
+Some terms:
 
-    Some terms:
-    - Registered identifiable is the definition of an identifiable which is:
-      - A record type as the parent
-      - A list of properties
-      - A list of referenced by statements
+- Registered identifiable is the definition of an identifiable which is:
+    - A record type as the parent
+    - A list of properties
+    - A list of referenced by statements
+- Identifiable is the concrete identifiable, e.g. the Record based on
+    the registered identifiable with all the values filled in.
+- Identified record is the result of retrieving a record based on the
+    identifiable from the database.
 
-    - Identifiable is the concrete identifiable, e.g. the Record based on
-      the registered identifiable with all the values filled in.
+General question to clarify:
 
-    - Identified record is the result of retrieving a record based on the
-      identifiable from the database.
+- Do we want to support multiple identifiables per RecordType?
+- Current implementation supports only one identifiable per RecordType.
 
-    General question to clarify:
-    Do we want to support multiple identifiables per RecordType?
-    Current implementation supports only one identifiable per RecordType.
+The list of referenced by statements is currently not implemented.
 
-    The list of referenced by statements is currently not implemented.
+The IdentifiableAdapter can be used to retrieve the three above mentioned objects (registred
+identifiabel, identifiable and identified record) for a Record.
 
-    The IdentifiableAdapter can be used to retrieve the three above mentioned objects (registred
-    identifiabel, identifiable and identified record) for a Record.
     """
 
     @staticmethod
     def create_query_for_identifiable(ident: Identifiable):
         """
         This function is taken from the old crawler:
         caosdb-advanced-user-tools/src/caosadvancedtools/crawler.py
 
         uses the properties of ident to create a query that can determine
         whether the required record already exists.
         """
 
         query_string = "FIND RECORD "
         if ident.record_type is not None:
-            query_string += ident.record_type
+            query_string += f"'{ident.record_type}'"
         for ref in ident.backrefs:
             eid = ref
             if isinstance(ref, db.Entity):
                 eid = ref.id
             query_string += (" WHICH IS REFERENCED BY " + str(eid) + " AND")
 
         query_string += " WITH "
 
         if ident.name is not None:
-            query_string += "name='{}'".format(ident.name)
+            query_string += "name='{}'".format(convert_value(ident.name))
             if len(ident.properties) > 0:
                 query_string += " AND "
 
         query_string += IdentifiableAdapter.create_property_query(ident)
+        if query_string.endswith(" AND WITH "):
+            query_string = query_string[:-len(" AND WITH ")]
+        if query_string.endswith(" AND "):
+            query_string = query_string[:-len(" AND ")]
         return query_string
 
     @staticmethod
     def create_property_query(entity: Identifiable):
         query_string = ""
         for pname, pvalue in entity.properties.items():
             if pvalue is None:
@@ -185,20 +190,22 @@
         if referencing_entities is None:
             referencing_entities = {}
 
         property_name_list_A = []
         property_name_list_B = []
         identifiable_props = {}
         identifiable_backrefs = []
+        name_is_identifying_property = False
 
         if registered_identifiable is not None:
             # fill the values:
             for prop in registered_identifiable.properties:
                 if prop.name == "name":
                     # The name can be an identifiable, but it isn't a property
+                    name_is_identifying_property = True
                     continue
                 # problem: what happens with multi properties?
                 # case A: in the registered identifiable
                 # case B: in the identifiable
 
                 # TODO: similar to the Identifiable class, Registred Identifiable should be a
                 # separate class too
@@ -238,15 +245,15 @@
 
         # use the RecordType of the registred Identifiable if it exists
         # We do not use parents of Record because it might have multiple
         return Identifiable(
             record_id=record.id,
             record_type=(registered_identifiable.parents[0].name
                          if registered_identifiable else None),
-            name=record.name,
+            name=record.name if name_is_identifying_property else None,
             properties=identifiable_props,
             path=record.path,
             backrefs=identifiable_backrefs
         )
 
     @abstractmethod
     def retrieve_identified_record_for_identifiable(self, identifiable: Identifiable):
@@ -256,29 +263,29 @@
         This function will return None if there is either no identifiable registered
         or no corresponding identified record in the database for a given record.
 
         Warning: this function is not expected to work correctly for file identifiables.
         """
         pass
 
-    # TODO: remove side effect
-    # TODO: use ID if record has one?
     def retrieve_identified_record_for_record(self, record: db.Record, referencing_entities=None):
         """
         This function combines all functionality of the IdentifierAdapter by
         returning the identifiable after having checked for an appropriate
         registered identifiable.
 
         In case there was no appropriate registered identifiable or no identifiable could
         be found return value is None.
         """
-        identifiable = self.get_identifiable(record, referencing_entities=referencing_entities)
+        if record.path is not None:
+            return cached_get_entity_by(path=record.path)
+        if record.id is not None:
+            return cached_get_entity_by(eid=record.id)
 
-        if identifiable.path is not None:
-            return self.get_file(identifiable)
+        identifiable = self.get_identifiable(record, referencing_entities=referencing_entities)
 
         return self.retrieve_identified_record_for_identifiable(identifiable)
 
 
 class LocalStorageIdentifiableAdapter(IdentifiableAdapter):
     """
     Identifiable adapter which can be used for unit tests.
@@ -418,19 +425,19 @@
     """
     Identifiable adapter which can be used for production.
     """
 
     # TODO: don't store registered identifiables locally
 
     def __init__(self):
-        self._registered_identifiables = dict()
+        self._registered_identifiables = {}
 
     def load_from_yaml_definition(self, path: str):
         """Load identifiables defined in a yaml file"""
-        with open(path, 'r') as yaml_f:
+        with open(path, 'r', encoding="utf-8") as yaml_f:
             identifiable_data = yaml.safe_load(yaml_f)
 
         for key, value in identifiable_data.items():
             rt = db.RecordType().add_parent(key)
             for prop_name in value:
                 if isinstance(prop_name, str):
                     rt.add_property(name=prop_name)
@@ -442,14 +449,18 @@
 
             self.register_identifiable(key, rt)
 
     def register_identifiable(self, name: str, definition: db.RecordType):
         self._registered_identifiables[name] = definition
 
     def get_file(self, identifiable: Identifiable):
+        # TODO is this needed for Identifiable?
+        # or can we get rid of this function?
+        if isinstance(identifiable, db.Entity):
+            return cached_get_entity_by(path=identifiable)
         if identifiable.path is None:
             raise RuntimeError("Path must not be None for File retrieval.")
         candidates = db.execute_query("FIND File which is stored at '{}'".format(
             identifiable.path))
         if len(candidates) > 1:
             raise RuntimeError("Identifiable was not defined unambigiously.")
         if len(candidates) == 0:
```

### Comparing `caoscrawler-0.5.0/src/caoscrawler/identified_cache.py` & `caoscrawler-0.6.0/src/caoscrawler/identified_cache.py`

 * *Files identical despite different names*

### Comparing `caoscrawler-0.5.0/src/caoscrawler/macros/macro_yaml_object.py` & `caoscrawler-0.6.0/src/caoscrawler/macros/macro_yaml_object.py`

 * *Files identical despite different names*

### Comparing `caoscrawler-0.5.0/src/caoscrawler/scanner.py` & `caoscrawler-0.6.0/src/caoscrawler/scanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,52 +22,37 @@
 # along with this program. If not, see <https://www.gnu.org/licenses/>.
 #
 # ** end header
 #
 
 """
 This is the scanner, the original "_crawl" function from crawl.py.
-This is just the functionality, that extracts data from the file system.
+
+This is just the functionality that extracts data from the file system.
 """
 
 from __future__ import annotations
 
-import argparse
 import importlib
 import logging
 import os
-import sys
 import warnings
 import yaml
 
-from argparse import RawTextHelpFormatter
-from collections import defaultdict
-from copy import deepcopy
-from enum import Enum
 from importlib_resources import files
 from jsonschema import validate
 from typing import Any, Optional, Type, Union
 
 import caosdb as db
+from .converters import Converter
 
-from caosadvancedtools.cache import UpdateCache, Cache
-from caosadvancedtools.crawler import Crawler as OldCrawler
-from caosdb.apiutils import (compare_entities, EntityMergeConflictError,
-                             merge_entities)
-from caosdb.common.datatype import is_reference
-
-from .converters import Converter, DirectoryConverter, ConverterValidationError
-
-from .macros import defmacro_constructor, macro_constructor
-from .stores import Store, GeneralStore, RecordStore
-from .structure_elements import StructureElement, Directory, NoneElement
+from .stores import GeneralStore, RecordStore
+from .structure_elements import StructureElement, Directory
 from .version import check_cfood_version
 
-from caosdb.high_level_api import convert_to_python_object
-
 from .debug_tree import DebugTree
 
 logger = logging.getLogger(__name__)
 
 
 def load_definition(crawler_definition_path: str):
     """
@@ -230,33 +215,36 @@
             general_store: Optional[GeneralStore] = None,
             record_store: Optional[RecordStore] = None,
             structure_elements_path: Optional[list[str]] = None,
             converters_path: Optional[list[str]] = None,
             restricted_path: Optional[list[str]] = None,
             crawled_data: Optional[list[db.Record]] = None,
             debug_tree: Optional[DebugTree] = None):
-    """
-    Crawl a list of StructureElements and apply any matching converters.
+    """Crawl a list of StructureElements and apply any matching converters.
 
     Formerly known as "_crawl".
 
     items: structure_elements (e.g. files and folders on one level on the hierarchy)
+
     converters: locally defined converters for
-                        treating structure elements. A locally defined converter could be
-                        one that is only valid for a specific subtree of the originally
-                        cralwed StructureElement structure.
+        treating structure elements. A locally defined converter could be
+        one that is only valid for a specific subtree of the originally
+        cralwed StructureElement structure.
+
     general_store and record_store: This recursion of the crawl function should only operate on
                                   copies of the global stores of the Crawler object.
+
     restricted_path: optional, list of strings, traverse the data tree only along the given
                      path. For example, when a directory contains files a, b and c and b is
                      given in restricted_path, a and c will be ignroed by the crawler.
                      When the end of the given path is reached, traverse the full tree as
                      normal. The first element of the list provided by restricted_path should
                      be the name of the StructureElement at this level, i.e. denoting the
                      respective element in the items argument.
+
     """
     # This path_found variable stores wether the path given by restricted_path was found in the
     # data tree
     path_found = False
     if restricted_path is not None and len(restricted_path) == 0:
         restricted_path = None
```

### Comparing `caoscrawler-0.5.0/src/caoscrawler/stores.py` & `caoscrawler-0.6.0/src/caoscrawler/stores.py`

 * *Files identical despite different names*

### Comparing `caoscrawler-0.5.0/src/caoscrawler/structure_elements.py` & `caoscrawler-0.6.0/src/caoscrawler/structure_elements.py`

 * *Files identical despite different names*

### Comparing `caoscrawler-0.5.0/src/caoscrawler/utils.py` & `caoscrawler-0.6.0/src/caoscrawler/utils.py`

 * *Files identical despite different names*

### Comparing `caoscrawler-0.5.0/src/caoscrawler/version.py` & `caoscrawler-0.6.0/src/caoscrawler/version.py`

 * *Files identical despite different names*

### Comparing `caoscrawler-0.5.0/src/caoscrawler.egg-info/PKG-INFO` & `caoscrawler-0.6.0/src/caoscrawler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caoscrawler
-Version: 0.5.0
+Version: 0.6.0
 Summary: A new crawler for caosdb
 Author: Alexander Schlemmer
 Author-email: alexander.schlemmer@ds.mpg.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `caoscrawler-0.5.0/src/caoscrawler.egg-info/SOURCES.txt` & `caoscrawler-0.6.0/src/caoscrawler.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 src/caoscrawler/__init__.py
 src/caoscrawler/authorize.py
 src/caoscrawler/cfood-schema.yml
+src/caoscrawler/config.py
 src/caoscrawler/converters.py
 src/caoscrawler/crawl.py
 src/caoscrawler/debug_tree.py
 src/caoscrawler/default_converters.yml
 src/caoscrawler/extension-converters-config-schema.yml
 src/caoscrawler/identifiable.py
 src/caoscrawler/identifiable_adapters.py
 src/caoscrawler/identified_cache.py
+src/caoscrawler/logging.py
 src/caoscrawler/scanner.py
 src/caoscrawler/stores.py
 src/caoscrawler/structure_elements.py
 src/caoscrawler/utils.py
 src/caoscrawler/version.py
 src/caoscrawler.egg-info/PKG-INFO
 src/caoscrawler.egg-info/SOURCES.txt
```


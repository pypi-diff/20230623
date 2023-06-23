# Comparing `tmp/cabinet-2023.6.23.1.tar.gz` & `tmp/cabinet-2023.6.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cabinet-2023.6.23.1.tar", last modified: Fri Jun 23 21:03:24 2023, max compression
+gzip compressed data, was "cabinet-2023.6.8.1.tar", last modified: Fri Jun  9 04:30:15 2023, max compression
```

## Comparing `cabinet-2023.6.23.1.tar` & `cabinet-2023.6.8.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-23 21:03:24.257041 cabinet-2023.6.23.1/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     1090 2023-06-17 20:33:55.000000 cabinet-2023.6.23.1/LICENSE
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     6862 2023-06-23 21:03:24.257041 cabinet-2023.6.23.1/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     6510 2023-06-22 20:53:24.000000 cabinet-2023.6.23.1/README.md
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       98 2023-03-06 04:41:10.000000 cabinet-2023.6.23.1/pyproject.toml
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      750 2023-06-23 21:03:24.257041 cabinet-2023.6.23.1/setup.cfg
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-23 21:03:24.253041 cabinet-2023.6.23.1/src/
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-23 21:03:24.257041 cabinet-2023.6.23.1/src/cabinet/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       80 2023-06-09 04:30:03.000000 cabinet-2023.6.23.1/src/cabinet/__init__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       69 2023-05-31 04:50:50.000000 cabinet-2023.6.23.1/src/cabinet/__main__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    30129 2023-06-23 21:02:04.000000 cabinet-2023.6.23.1/src/cabinet/cabinet.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     3687 2023-04-16 16:59:23.000000 cabinet-2023.6.23.1/src/cabinet/mail.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-23 21:03:24.257041 cabinet-2023.6.23.1/src/cabinet.egg-info/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     6862 2023-06-23 21:03:24.000000 cabinet-2023.6.23.1/src/cabinet.egg-info/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      333 2023-06-23 21:03:24.000000 cabinet-2023.6.23.1/src/cabinet.egg-info/SOURCES.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-06-23 21:03:24.000000 cabinet-2023.6.23.1/src/cabinet.egg-info/dependency_links.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       41 2023-06-23 21:03:24.000000 cabinet-2023.6.23.1/src/cabinet.egg-info/entry_points.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2023-06-23 21:03:24.000000 cabinet-2023.6.23.1/src/cabinet.egg-info/top_level.txt
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-23 21:03:24.257041 cabinet-2023.6.23.1/test/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     5868 2023-05-31 04:52:07.000000 cabinet-2023.6.23.1/test/test___init__.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-09 04:30:15.960220 cabinet-2023.6.8.1/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    11357 2023-03-06 03:35:41.000000 cabinet-2023.6.8.1/LICENSE
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     6579 2023-06-09 04:30:15.960220 cabinet-2023.6.8.1/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     6228 2023-05-31 04:52:07.000000 cabinet-2023.6.8.1/README.md
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       98 2023-03-06 04:41:10.000000 cabinet-2023.6.8.1/pyproject.toml
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      750 2023-06-09 04:30:15.960220 cabinet-2023.6.8.1/setup.cfg
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-09 04:30:15.960220 cabinet-2023.6.8.1/src/
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-09 04:30:15.960220 cabinet-2023.6.8.1/src/cabinet/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       80 2023-06-09 04:30:03.000000 cabinet-2023.6.8.1/src/cabinet/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       69 2023-05-31 04:50:50.000000 cabinet-2023.6.8.1/src/cabinet/__main__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    26147 2023-06-09 04:29:47.000000 cabinet-2023.6.8.1/src/cabinet/cabinet.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     3687 2023-04-16 16:59:23.000000 cabinet-2023.6.8.1/src/cabinet/mail.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-09 04:30:15.960220 cabinet-2023.6.8.1/src/cabinet.egg-info/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     6579 2023-06-09 04:30:15.000000 cabinet-2023.6.8.1/src/cabinet.egg-info/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      333 2023-06-09 04:30:15.000000 cabinet-2023.6.8.1/src/cabinet.egg-info/SOURCES.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-06-09 04:30:15.000000 cabinet-2023.6.8.1/src/cabinet.egg-info/dependency_links.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       41 2023-06-09 04:30:15.000000 cabinet-2023.6.8.1/src/cabinet.egg-info/entry_points.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2023-06-09 04:30:15.000000 cabinet-2023.6.8.1/src/cabinet.egg-info/top_level.txt
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-09 04:30:15.960220 cabinet-2023.6.8.1/test/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     5868 2023-05-31 04:52:07.000000 cabinet-2023.6.8.1/test/test___init__.py
```

### Comparing `cabinet-2023.6.23.1/PKG-INFO` & `cabinet-2023.6.8.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cabinet
-Version: 2023.6.23.1
+Version: 2023.6.8.1
 Summary: Easily manage data storage and logging across repos
 Home-page: https://github.com/tylerjwoodfin/cabinet
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -41,21 +41,20 @@
 
 Options:
   -h, --help              Show this help message and exit
   --configure, -config    Configure
   --edit, -e              Edit the settings.json file
   --edit-file, -ef        Edit a specific file
   --no-create             (for -ef) Do not create file if it does not exist
-  --get, -g               Get a property from settings.json
-  --put, -p               Put a property into settings.json
-  --remove, -rm           Removes a property from settings.json
-  --get-file              Returns the file specified
+  --get, -g [GET ...]     Get a property from settings.json
+  --put PUT [PUT ...]     Put a property into settings.json
+  --get-file GET_FILE     Get file
   --strip                 (for --get-file) Whether to strip file content whitespace
   --log, -l               Log a message to the default location
-  --level                 (for -l) Log level [debug, info, warn, error, critical]
+  --level LOG_LEVEL       (for -l) Log level [debug, info, warn, error, critical]
   -v, --version           show version number and exit
 
 Mail:
   --mail                Sends an email
   --subject SUBJECT, -s SUBJECT
                         Email subject
   --body BODY, -b BODY  Email body
@@ -136,15 +135,16 @@
 cab = Cabinet()
 
 cab.put("employee", "Tyler", "salary", 7.25)
 ```
 
 or terminal:
 ```
-cabinet -p employee Tyler salary 7.25
+# warning - from the terminal, numeric values in cabinet are stored as strings
+cabinet -p employer Tyler salary 7.25
 ```
 
 results in this structure in settings.json:
 ```
 {
     "employee": {
         "Tyler": {
@@ -171,39 +171,14 @@
 ```
 
 results in:
 ```
 7.25
 ```
 
-### `remove`
-
-python:
-```
-from cabinet import Cabinet
-
-cab = Cabinet()
-
-cab.remove("employee", "Tyler", "salary")
-```
-
-or terminal:
-```
-cabinet -rm employee Tyler salary
-```
-
-results in this structure in settings.json:
-```
-{
-    "employee": {
-        "tyler": {}
-    }
-}
-```
-
 ### `edit_file`
 
 python:
 ```
 from cabinet import Cabinet
 
 cab = Cabinet()
@@ -262,19 +237,19 @@
 cab.log("Connection timed out") # defaults to 'info' if no level is set
 cab.log("This function hit a breakpoint", level="debug")
 cab.log("Looks like the server is on fire", level="critical")
 cab.log("This is fine", level="info")
 
 # writes to a file named LOG_TEMPERATURE
 
-cab.log("30", log_name="LOG_TEMPERATURE")
+cab.log("30", logName="LOG_TEMPERATURE")
 
 # writes to a file named LOG_TEMPERATURE in /home/{username}/weather
 
-cab.log("30", log_name="LOG_TEMPERATURE", file_path="/home/{username}/weather")
+cab.log("30", logName="LOG_TEMPERATURE", filePath="/home/{username}/weather")
 
     # format
     # 2021-12-29 19:29:27,896 — INFO — 30
 
 ```
 
 terminal:
```

### Comparing `cabinet-2023.6.23.1/README.md` & `cabinet-2023.6.8.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -29,21 +29,20 @@
 
 Options:
   -h, --help              Show this help message and exit
   --configure, -config    Configure
   --edit, -e              Edit the settings.json file
   --edit-file, -ef        Edit a specific file
   --no-create             (for -ef) Do not create file if it does not exist
-  --get, -g               Get a property from settings.json
-  --put, -p               Put a property into settings.json
-  --remove, -rm           Removes a property from settings.json
-  --get-file              Returns the file specified
+  --get, -g [GET ...]     Get a property from settings.json
+  --put PUT [PUT ...]     Put a property into settings.json
+  --get-file GET_FILE     Get file
   --strip                 (for --get-file) Whether to strip file content whitespace
   --log, -l               Log a message to the default location
-  --level                 (for -l) Log level [debug, info, warn, error, critical]
+  --level LOG_LEVEL       (for -l) Log level [debug, info, warn, error, critical]
   -v, --version           show version number and exit
 
 Mail:
   --mail                Sends an email
   --subject SUBJECT, -s SUBJECT
                         Email subject
   --body BODY, -b BODY  Email body
@@ -124,15 +123,16 @@
 cab = Cabinet()
 
 cab.put("employee", "Tyler", "salary", 7.25)
 ```
 
 or terminal:
 ```
-cabinet -p employee Tyler salary 7.25
+# warning - from the terminal, numeric values in cabinet are stored as strings
+cabinet -p employer Tyler salary 7.25
 ```
 
 results in this structure in settings.json:
 ```
 {
     "employee": {
         "Tyler": {
@@ -159,39 +159,14 @@
 ```
 
 results in:
 ```
 7.25
 ```
 
-### `remove`
-
-python:
-```
-from cabinet import Cabinet
-
-cab = Cabinet()
-
-cab.remove("employee", "Tyler", "salary")
-```
-
-or terminal:
-```
-cabinet -rm employee Tyler salary
-```
-
-results in this structure in settings.json:
-```
-{
-    "employee": {
-        "tyler": {}
-    }
-}
-```
-
 ### `edit_file`
 
 python:
 ```
 from cabinet import Cabinet
 
 cab = Cabinet()
@@ -250,19 +225,19 @@
 cab.log("Connection timed out") # defaults to 'info' if no level is set
 cab.log("This function hit a breakpoint", level="debug")
 cab.log("Looks like the server is on fire", level="critical")
 cab.log("This is fine", level="info")
 
 # writes to a file named LOG_TEMPERATURE
 
-cab.log("30", log_name="LOG_TEMPERATURE")
+cab.log("30", logName="LOG_TEMPERATURE")
 
 # writes to a file named LOG_TEMPERATURE in /home/{username}/weather
 
-cab.log("30", log_name="LOG_TEMPERATURE", file_path="/home/{username}/weather")
+cab.log("30", logName="LOG_TEMPERATURE", filePath="/home/{username}/weather")
 
     # format
     # 2021-12-29 19:29:27,896 — INFO — 30
 
 ```
 
 terminal:
```

### Comparing `cabinet-2023.6.23.1/setup.cfg` & `cabinet-2023.6.8.1/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [metadata]
 name = cabinet
-version = 2023.06.23.1
+version = 2023.06.08.1
 author = Tyler Woodfin
 author_email = feedback@tyler.cloud
 description = Easily manage data storage and logging across repos
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tylerjwoodfin/cabinet
 project_urls = 
-bug tracker = https://github.com/tylerjwoodfin/cabinet/issues
+Bug Tracker = https://github.com/tylerjwoodfin/cabinet/issues
 py_modules = ["cabinet"]
 classifiers = 
-programming language = : Python :: 3
-license = : OSI Approved :: MIT License
-operating system = : OS Independent
+Programming Language = : Python :: 3
+License = : OSI Approved :: MIT License
+Operating System = : OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.6
```

### Comparing `cabinet-2023.6.23.1/src/cabinet/cabinet.py` & `cabinet-2023.6.8.1/src/cabinet/cabinet.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 """
 
 import os
 import json
 import pathlib
 import logging
 import sys
-import ast
 import argparse
 from datetime import date
 from typing import Optional
 import importlib.metadata
 from .mail import Mail
 
 
@@ -304,29 +303,18 @@
         file_handler.setFormatter(log_format)
 
         logger.addHandler(file_handler)
         return logger
 
     def _ifprint(self, message: str, is_print: bool):
         """
-        Prints the message if `print` is true.
+        Prints a string if `print` is true.
         """
-
-        # check for valid JSON
-        try:
-            json.loads(message)
-            if is_print:
-                print(json.dumps(message, indent=2))
-        except TypeError:
-            if is_print:
-                print(json.dumps(message, indent=2))
-        except json.JSONDecodeError:
-            if is_print:
-                print(message)
-            return message
+        if is_print:
+            print(message)
 
     def configure(self):
         """
         Configures the Cabinet instance based on command line arguments or user input.
         """
 
         message = f"""
@@ -456,128 +444,54 @@
                 File must be in the `path_cabinet` folder.
                 Default: 'settings.json'
 
         Returns:
             The value that was put into the property.
         """
 
-        def parse_arg(value):
-            """
-            Infer the value type (e.g. 2 will not be parsed as a string)
-            """
-            if value == "null":
-                return None
-            try:
-                return int(value)
-            except ValueError:
-                try:
-                    return float(value)
-                except ValueError:
-                    if value.lower() == 'true':
-                        return True
-                    if value.lower() == 'false':
-                        return False
-                    try:
-                        return ast.literal_eval(value)
-                    except (SyntaxError, ValueError):
-                        return value
-            except TypeError:
-                # 'dict' objects or similar can just return original value
-                return value
-
         path_full = f"{self.path_cabinet}/{file_name}"
 
         maximum_attribute_index = 0
         attribute_max_attribute_index = attribute
 
         if not value:
-            value = parse_arg(attribute[-1])
+            value = attribute[-1]
             maximum_attribute_index = -1
             attribute_max_attribute_index = attribute[:maximum_attribute_index]
 
         _settings = self.settings_json if file_name == 'settings.json' else json.load(
             open(path_full, encoding="utf8"))
 
+        # iterate through entire JSON object and replace 2nd to last attribute with value
+
         partition = _settings
 
         for index, item in enumerate(attribute_max_attribute_index):
             if item not in partition:
                 try:
                     partition[item] = value if index == len(
                         attribute) + maximum_attribute_index - 1 else {}
                     partition = partition[item]
                     self.log(
-                        f"Adding key: {{'{item}': {partition}}} \
-to \"{attribute_max_attribute_index[index-1] if index > 0 else path_full}\"",
+                        f"Adding new key '{item}' to {partition if index > 0 else path_full}",
                         is_quiet=self.new_setup)
                 except TypeError as error:
-                    self.log((f"{error}\n\n{' -> '.join(attribute[:-2])} ",
-                              "is currently a string, so it cannot \
-be treated as an object with multiple properties."), level="error")
-            elif not isinstance(partition[item], str):
+                    self.log(f"{error}\n\n{attribute[index-1]} is currently a string, so it cannot \
+be treated as an object with multiple properties.", level="error")
+            else:
                 if index == len(attribute) + maximum_attribute_index - 1:
                     partition[item] = value
                 else:
                     partition = partition[item]
-            else:
-                self.log(f"{' -> '.join(attribute[:-2])} is currently a string, so it cannot \
-be treated as an object with multiple properties.", level="error")
-                exit(-1)
-
-        with open(path_full, 'w+', encoding="utf8") as file:
-            json.dump(_settings, file, indent=4)
-
-        self.log(
-            f"{' -> '.join(attribute[:-1])} set to {value}",
-            level='info', is_quiet=not is_print)
-
-        return value
-
-    def remove(self, *attribute, file_name='settings.json', is_print=False):
-        """
-        Removes a property from a JSON file (default name: settings.json).
-
-        Args:
-            *attribute (str): A series of keys in the JSON object
-                to identify the location of the property.
-            file_name (str): The name of the JSON file to remove the property from.
-                File must be in the `path_cabinet` folder.
-                Default: 'settings.json'
-
-        Returns:
-            The value that was removed from the property.
-            If the property doesn't exist, None is returned.
-        """
-        path_full = f"{self.path_cabinet}/{file_name}"
-
-        _settings = self.settings_json if file_name == 'settings.json' else json.load(
-            open(path_full, encoding="utf8"))
-
-        partition = _settings
-
-        for index, item in enumerate(attribute):
-            if item not in partition:
-                self.log(
-                    (f"Key '{item}' does not exist in"
-                     f" \"{attribute[:index] if index > 0 else path_full}\""),
-                    level="warning")
-                return None
-            elif index == len(attribute) - 1:
-                value = partition[item]
-                del partition[item]
-            else:
-                partition = partition[item]
 
         with open(path_full, 'w+', encoding="utf8") as file:
             json.dump(_settings, file, indent=4)
 
-        self.log(
-            f"{' -> '.join(attribute)} removed.",
-            level='info', is_quiet=not is_print)
-
+        self._ifprint(
+            f"{' -> '.join(attribute[:-1])} set to {value}", is_print)
         return value
 
     def get_file_as_array(self, item: str, file_path=None, strip: bool = True,
                           ignore_not_found: bool = False):
         """
         Reads a file and returns its contents as a list of lines.
         The file is assumed to be encoded in UTF-8.
@@ -711,46 +625,30 @@
         cabinet edit <file path/name, optional; default: settings.json>
     """
 
     cab = Cabinet()
     package_name = sys.modules[__name__].__package__.split('.')[0]
     version = importlib.metadata.version(package_name)
 
-    class ValidatePutArgs(argparse.Action):
-        """
-        Custom argparse action to validate the number of arguments for the --put option.
-        Ensures that a minimum of 2 arguments are provided.
-        """
-
-        def __call__(self, parser, namespace, values, option_string=None):
-            if len(values) < 2:
-                if len(values) == 1 and values[0] == 'ut':
-                    print("I think you meant to use '--put' or '-p'.\n")
-                parser.error(
-                    f"At least 2 arguments are required for {option_string}")
-            setattr(namespace, self.dest, values)
-
     parser = argparse.ArgumentParser(
         description=f"Cabinet ({version})")
 
     parser.add_argument('--configure', '-config', dest='configure',
                         action='store_true', help='Configure')
     parser.add_argument('--edit', '-e', dest='edit', action='store_true',
                         help='Edit the settings.json file')
     parser.add_argument('--edit-file', '-ef', type=str, dest='edit_file',
                         help='Edit a specific file')
     parser.add_argument('--no-create', dest='create',
                         action='store_false',
                         help='(for -ef) Do not create file if it does not exist')
     parser.add_argument('--get', '-g', dest='get', nargs='+',
                         help='Get a property from settings.json')
-    parser.add_argument('--put', '-p', dest='put', nargs='+', action=ValidatePutArgs,
+    parser.add_argument('--put', '-p', dest='put', nargs='+',
                         help='Put a property into settings.json')
-    parser.add_argument('--remove', '-rm', dest='remove',
-                        nargs='+', help='Remove a property from settings.json')
     parser.add_argument('--get-file', dest='get_file',
                         type=str, help='Get file')
     parser.add_argument('--strip', dest='strip', action='store_false',
                         help='(for --get-file) Whether to strip file content whitespace')
     parser.add_argument('--log', '-l', type=str,
                         dest='log', help='Log a message to the default location')
     parser.add_argument('--level', type=str, dest='log_level',
@@ -779,17 +677,14 @@
         cab.edit_file(file_path=args.edit_file,
                       create_if_not_exist=args.create)
     elif args.get:
         cab.get(is_print=True, *args.get)
     elif args.put:
         attribute_values = args.put
         cab.put(*attribute_values, is_print=True)
-    elif args.remove:
-        attribute_values = args.remove
-        cab.remove(*attribute_values, is_print=True)
     elif args.get_file:
         cab.get_file_as_array(item=args.get_file,
                               file_path=None, strip=args.strip)
     elif args.log:
         cab.log(message=args.log, level=args.log_level)
     elif args.mail:
         to_addr = None
```

### Comparing `cabinet-2023.6.23.1/src/cabinet/mail.py` & `cabinet-2023.6.8.1/src/cabinet/mail.py`

 * *Files identical despite different names*

### Comparing `cabinet-2023.6.23.1/src/cabinet.egg-info/PKG-INFO` & `cabinet-2023.6.8.1/src/cabinet.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cabinet
-Version: 2023.6.23.1
+Version: 2023.6.8.1
 Summary: Easily manage data storage and logging across repos
 Home-page: https://github.com/tylerjwoodfin/cabinet
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -41,21 +41,20 @@
 
 Options:
   -h, --help              Show this help message and exit
   --configure, -config    Configure
   --edit, -e              Edit the settings.json file
   --edit-file, -ef        Edit a specific file
   --no-create             (for -ef) Do not create file if it does not exist
-  --get, -g               Get a property from settings.json
-  --put, -p               Put a property into settings.json
-  --remove, -rm           Removes a property from settings.json
-  --get-file              Returns the file specified
+  --get, -g [GET ...]     Get a property from settings.json
+  --put PUT [PUT ...]     Put a property into settings.json
+  --get-file GET_FILE     Get file
   --strip                 (for --get-file) Whether to strip file content whitespace
   --log, -l               Log a message to the default location
-  --level                 (for -l) Log level [debug, info, warn, error, critical]
+  --level LOG_LEVEL       (for -l) Log level [debug, info, warn, error, critical]
   -v, --version           show version number and exit
 
 Mail:
   --mail                Sends an email
   --subject SUBJECT, -s SUBJECT
                         Email subject
   --body BODY, -b BODY  Email body
@@ -136,15 +135,16 @@
 cab = Cabinet()
 
 cab.put("employee", "Tyler", "salary", 7.25)
 ```
 
 or terminal:
 ```
-cabinet -p employee Tyler salary 7.25
+# warning - from the terminal, numeric values in cabinet are stored as strings
+cabinet -p employer Tyler salary 7.25
 ```
 
 results in this structure in settings.json:
 ```
 {
     "employee": {
         "Tyler": {
@@ -171,39 +171,14 @@
 ```
 
 results in:
 ```
 7.25
 ```
 
-### `remove`
-
-python:
-```
-from cabinet import Cabinet
-
-cab = Cabinet()
-
-cab.remove("employee", "Tyler", "salary")
-```
-
-or terminal:
-```
-cabinet -rm employee Tyler salary
-```
-
-results in this structure in settings.json:
-```
-{
-    "employee": {
-        "tyler": {}
-    }
-}
-```
-
 ### `edit_file`
 
 python:
 ```
 from cabinet import Cabinet
 
 cab = Cabinet()
@@ -262,19 +237,19 @@
 cab.log("Connection timed out") # defaults to 'info' if no level is set
 cab.log("This function hit a breakpoint", level="debug")
 cab.log("Looks like the server is on fire", level="critical")
 cab.log("This is fine", level="info")
 
 # writes to a file named LOG_TEMPERATURE
 
-cab.log("30", log_name="LOG_TEMPERATURE")
+cab.log("30", logName="LOG_TEMPERATURE")
 
 # writes to a file named LOG_TEMPERATURE in /home/{username}/weather
 
-cab.log("30", log_name="LOG_TEMPERATURE", file_path="/home/{username}/weather")
+cab.log("30", logName="LOG_TEMPERATURE", filePath="/home/{username}/weather")
 
     # format
     # 2021-12-29 19:29:27,896 — INFO — 30
 
 ```
 
 terminal:
```

### Comparing `cabinet-2023.6.23.1/test/test___init__.py` & `cabinet-2023.6.8.1/test/test___init__.py`

 * *Files identical despite different names*


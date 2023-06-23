# Comparing `tmp/skeletonkey-0.1.0.tar.gz` & `tmp/skeletonkey-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skeletonkey-0.1.0.tar", last modified: Tue May 16 00:30:55 2023, max compression
+gzip compressed data, was "skeletonkey-0.1.1.tar", last modified: Fri Jun 23 20:08:30 2023, max compression
```

## Comparing `skeletonkey-0.1.0.tar` & `skeletonkey-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 sizemol  (77241) grp.csci.Faculty (71145)        0 2023-05-16 00:30:54.970136 skeletonkey-0.1.0/
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     1071 2023-05-01 03:35:36.000000 skeletonkey-0.1.0/LICENSE
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     4304 2023-05-16 00:30:54.950135 skeletonkey-0.1.0/PKG-INFO
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     3814 2023-05-01 05:00:51.000000 skeletonkey-0.1.0/README.md
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)       38 2023-05-16 00:30:54.986137 skeletonkey-0.1.0/setup.cfg
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)      717 2023-05-16 00:30:42.000000 skeletonkey-0.1.0/setup.py
-drwxr-xr-x   0 sizemol  (77241) grp.csci.Faculty (71145)        0 2023-05-16 00:30:54.502113 skeletonkey-0.1.0/skeletonkey/
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)      562 2023-05-01 04:36:26.000000 skeletonkey-0.1.0/skeletonkey/__init__.py
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     8060 2023-05-01 05:05:03.000000 skeletonkey-0.1.0/skeletonkey/config.py
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     4658 2023-05-01 04:36:26.000000 skeletonkey-0.1.0/skeletonkey/core.py
-drwxr-xr-x   0 sizemol  (77241) grp.csci.Faculty (71145)        0 2023-05-16 00:30:54.846130 skeletonkey-0.1.0/skeletonkey.egg-info/
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     4304 2023-05-16 00:30:52.000000 skeletonkey-0.1.0/skeletonkey.egg-info/PKG-INFO
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)      232 2023-05-16 00:30:52.000000 skeletonkey-0.1.0/skeletonkey.egg-info/SOURCES.txt
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)        1 2023-05-16 00:30:52.000000 skeletonkey-0.1.0/skeletonkey.egg-info/dependency_links.txt
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)       12 2023-05-16 00:30:52.000000 skeletonkey-0.1.0/skeletonkey.egg-info/top_level.txt
+drwxr-xr-x   0 sizemol  (77241) grp.csci.Faculty (71145)        0 2023-06-23 20:08:30.091232 skeletonkey-0.1.1/
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     1071 2023-05-01 03:35:36.000000 skeletonkey-0.1.1/LICENSE
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     4304 2023-06-23 20:08:30.079231 skeletonkey-0.1.1/PKG-INFO
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     3814 2023-05-01 05:00:51.000000 skeletonkey-0.1.1/README.md
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)       38 2023-06-23 20:08:30.155235 skeletonkey-0.1.1/setup.cfg
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)      758 2023-06-23 20:07:35.000000 skeletonkey-0.1.1/setup.py
+drwxr-xr-x   0 sizemol  (77241) grp.csci.Faculty (71145)        0 2023-06-23 20:08:29.827219 skeletonkey-0.1.1/skeletonkey/
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)      562 2023-05-01 04:36:26.000000 skeletonkey-0.1.1/skeletonkey/__init__.py
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)    10442 2023-06-23 19:57:18.000000 skeletonkey-0.1.1/skeletonkey/config.py
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     4684 2023-06-23 19:41:37.000000 skeletonkey-0.1.1/skeletonkey/core.py
+drwxr-xr-x   0 sizemol  (77241) grp.csci.Faculty (71145)        0 2023-06-23 20:08:30.035229 skeletonkey-0.1.1/skeletonkey.egg-info/
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     4304 2023-06-23 20:08:28.000000 skeletonkey-0.1.1/skeletonkey.egg-info/PKG-INFO
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)      266 2023-06-23 20:08:28.000000 skeletonkey-0.1.1/skeletonkey.egg-info/SOURCES.txt
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)        1 2023-06-23 20:08:28.000000 skeletonkey-0.1.1/skeletonkey.egg-info/dependency_links.txt
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)       14 2023-06-23 20:08:28.000000 skeletonkey-0.1.1/skeletonkey.egg-info/requires.txt
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)       12 2023-06-23 20:08:28.000000 skeletonkey-0.1.1/skeletonkey.egg-info/top_level.txt
```

### Comparing `skeletonkey-0.1.0/LICENSE` & `skeletonkey-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `skeletonkey-0.1.0/PKG-INFO` & `skeletonkey-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skeletonkey
-Version: 0.1.0
+Version: 0.1.1
 Summary: A bare-bones configuration managment tool.
 Home-page: https://github.com/sizemore0125/skeletonkey
 Author: Logan Sizemore
 Author-email: sizemore0125@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `skeletonkey-0.1.0/README.md` & `skeletonkey-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `skeletonkey-0.1.0/setup.py` & `skeletonkey-0.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="skeletonkey",
-    version="0.1.0",
+    version="0.1.1",
     description="A bare-bones configuration managment tool.",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sizemore0125/skeletonkey",
     author="Logan Sizemore",
     author_email="sizemore0125@gmail.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.7",
+    install_requires=["pyYAML>=3.0.0"],
 )
```

### Comparing `skeletonkey-0.1.0/skeletonkey/__init__.py` & `skeletonkey-0.1.1/skeletonkey/__init__.py`

 * *Files identical despite different names*

### Comparing `skeletonkey-0.1.0/skeletonkey/config.py` & `skeletonkey-0.1.1/skeletonkey/config.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import argparse
 import inspect
 import os
 from typing import List
 
 import yaml
 
+
 def find_yaml_path(file_path: str) -> str:
     """
     Given a file path, this function checks if a YAML file exists with either
     '.yml' or '.yaml' extension, and returns the correct path.
 
     Args:
         file_path (str): The file path without extension or with either '.yml' or '.yaml' extension.
@@ -26,41 +27,45 @@
         str: The correct file path with the existing extension.
 
     Raises:
         FileNotFoundError: If no YAML file is found with either extension.
     """
     base_path, ext = os.path.splitext(file_path)
 
-    yml_path = base_path + '.yml'
-    yaml_path = base_path + '.yaml'
+    yml_path = base_path + ".yml"
+    yaml_path = base_path + ".yaml"
 
     if os.path.isfile(yml_path):
         return yml_path
     elif os.path.isfile(yaml_path):
         return yaml_path
     else:
-        raise FileNotFoundError(f"No YAML file found with either '.yml' or '.yaml' extension for path: {base_path}")
+        raise FileNotFoundError(
+            f"No YAML file found with either '.yml' or '.yaml' extension for path: {base_path}. You may have mistakenly specified an absolute path."
+        )
+
 
 def open_yaml(path: str) -> dict:
     """
     Read and parse the YAML file located at the given path.
-    
+
     Args:
         path (str): The file path to the YAML file.
-        
+
     Returns:
         dict: A dictionary representing the YAML content.
     """
     path = find_yaml_path(path)
-    with open(os.path.expanduser(path), 'r') as handle:
+    with open(os.path.expanduser(path), "r") as handle:
         return yaml.safe_load(handle)
 
-def dict_to_path(dictionary: dict, parent_key='', sep='/') -> List[str]:
+
+def dict_to_path(dictionary: dict, parent_key="", sep="/") -> List[str]:
     """
-    Flatten a nested dictionary into a single-level dictionary by concatenating 
+    Flatten a nested dictionary into a single-level dictionary by concatenating
     nested keys using a specified separator.
 
     Args:
         dictionary (dict): The nested dictionary to be flattened.
         parent_key (str): The initial parent key, default is an empty string.
         sep (str): The separator used to concatenate nested keys, default is '/'.
 
@@ -83,33 +88,35 @@
                     items.extend(sublist_items)
                 else:
                     # If the item is not a dictionary, append it to the key
                     items.append(os.path.join(new_key, item))
         else:
             # If the value is neither a dictionary nor a list, add it to the items
             items.append(os.path.join(new_key, value))
-            
+
     return items
 
+
 def add_yaml_extension(path: str) -> str:
     """
     Append the '.yaml' extension to a given path if it doesn't already have it.
 
     Args:
         path (str): The input file path or name.
 
     Returns:
         str: The modified file path or name with the '.yaml' extension added.
     """
-    yaml_extention1 = '.yaml'
-    yaml_extention2 = '.yml'
+    yaml_extention1 = ".yaml"
+    yaml_extention2 = ".yml"
     if not path.endswith(yaml_extention1) and not path.endswith(yaml_extention2):
         path += yaml_extention1
     return path
-    
+
+
 def get_default_yaml_paths_from_dict(default_yaml: dict) -> List[str]:
     """
     Process a nested dictionary of default YAML file paths, flattening the
     dictionary, converting it to a list of paths, and ensuring each path has
     a '.yaml' extension.
 
     Args:
@@ -118,59 +125,135 @@
     Returns:
         List[str]: A list of processed and validated default YAML file paths.
     """
     default_yaml = dict_to_path(default_yaml)
     default_yaml = [add_yaml_extension(filename) for filename in default_yaml]
     return default_yaml
 
-def load_yaml_config(config_path: str, config_name: str, default_keyword: str = "defaults") ->  dict:
+
+def get_default_args_from_dict(config_path: str, default_yaml: dict) -> dict:
+    """
+    Load a YAML default configuration files in dict format and returns a dictionary of args.
+
+    Args:
+        config_path (str): The file path to the YAML configuration file.
+        default_yml (dict): A dictionary data structure representing the paths to many
+            YAML configuration files.
+
+    Returns:
+        dict: The updated configuration dictionary."""
+    yaml_paths = get_default_yaml_paths_from_dict(default_yaml)
+    default_configs = [
+        open_yaml(os.path.join(config_path, yaml_path)) for yaml_path in yaml_paths
+    ]
+    default_config = {
+        key: value
+        for config_dict in default_configs
+        if config_dict
+        for key, value in config_dict.items()
+    }
+    return default_config
+
+
+def get_default_args_from_path(config_path: str, default_yaml: str) -> dict:
+    """
+    Load a YAML default configuration files and returns a dictionary of args.
+
+    Args:
+        config_path (str): The file path to the YAML base configuration file.
+        default_yml (str): The relative path to to the default YAML subconfiguration file.
+
+    Returns:
+        dict: The updated configuration dictionary.
+    """
+    default_yaml = add_yaml_extension(default_yaml)
+    default_config_path = os.path.join(config_path, default_yaml)
+    default_config = open_yaml(default_config_path)
+    return default_config
+
+
+def load_yaml_config(
+    config_path: str, config_name: str, default_keyword: str = "defaults"
+) -> dict:
     """
     Load a YAML configuration file and update it with default configurations.
 
     Args:
-        path (str): The file path to the YAML configuration file.
+        config_path (str): The file path to the YAML configuration file.
+        config_name (str): The name of the YAML configuration file.
         default_keyword (str): The keyword used to identify default configurations
             in the YAML file. Defaults to "defaults".
 
     Returns:
         dict: The updated configuration dictionary.
     """
     path = os.path.join(config_path, config_name)
     config = open_yaml(path)
-    
+
     if default_keyword in config:
-        for default_yaml in config[default_keyword]:
-            if isinstance(default_yaml, str):
-                default_yaml = add_yaml_extension(default_yaml)
-                default_config = open_yaml(os.path.join(config_path, default_yaml))
-            elif isinstance(default_yaml, dict):
-                yaml_paths = get_default_yaml_paths_from_dict(default_yaml)
-                default_configs = [open_yaml(os.path.join(config_path, yaml_path)) for yaml_path in yaml_paths]
-                default_config = {key: value for config_dict in default_configs for key, value in config_dict.items()}
-            config.update((key, value) for key, value in default_config.items() if key not in config)
+        default_path_dict = config[default_keyword]
+        if isinstance(default_path_dict, dict):
+            default_config = get_default_args_from_dict(config_path, default_path_dict)
+
+            if default_config:
+                config.update(
+                    (key, value)
+                    for key, value in default_config.items()
+                    if key not in config
+                )
+        else:
+            for default_yaml in default_path_dict:
+                if isinstance(default_yaml, dict):
+                    default_config = get_default_args_from_dict(
+                        config_path, default_yaml
+                    )
+
+                elif isinstance(default_yaml, str):
+                    default_config = get_default_args_from_path(
+                        config_path, default_yaml
+                    )
+
+                if default_config:
+                    config.update(
+                        (key, value)
+                        for key, value in default_config.items()
+                        if key not in config
+                    )
+        del config[default_keyword]
 
     return config
 
-def add_args_from_dict(arg_parser: argparse.ArgumentParser, config: dict, prefix='') -> None:
+
+def add_args_from_dict(
+    arg_parser: argparse.ArgumentParser, config: dict, prefix=""
+) -> None:
     """
-    Add arguments to an ArgumentParser instance using key-value pairs from a 
+    Add arguments to an ArgumentParser instance using key-value pairs from a
     configuration dictionary. If the dictionary contains a nested dictionary, the
     argument will be added as --key.key value.
     Args:
         arg_parser (argparse.ArgumentParser): The ArgumentParser instance to which
                                               arguments will be added.
         config (dict): A dictionary containing key-value pairs representing
                        the arguments and their default values.
         prefix (str, optional): The prefix string for nested keys. Defaults to ''.
     """
     for key, value in config.items():
         if isinstance(value, dict):
-            add_args_from_dict(arg_parser, value, f'{prefix}{key}.')
+            add_args_from_dict(arg_parser, value, f"{prefix}{key}.")
         else:
-            arg_parser.add_argument(f"--{prefix}{key}", default=value, type=type(value))
+            if key.startswith("$") and key[1:] in os.environ:
+                env_var = os.environ[key[1:]]
+                arg_parser.add_argument(
+                    f"--{prefix}{key[1:]}", default=env_var, type=type(env_var)
+                )
+            else:
+                arg_parser.add_argument(
+                    f"--{prefix}{key}", default=value, type=type(value)
+                )
 
 
 def dict_to_namespace(dictionary: dict) -> argparse.Namespace:
     """
     Convert a dictionary to an argparse.Namespace object recursively.
 
     Args:
@@ -201,8 +284,8 @@
         current_dict = nested_dict
         for sub_key in keys[:-1]:
             if sub_key not in current_dict:
                 current_dict[sub_key] = {}
             current_dict = current_dict[sub_key]
         current_dict[keys[-1]] = value
 
-    return dict_to_namespace(nested_dict)
+    return dict_to_namespace(nested_dict)
```

### Comparing `skeletonkey-0.1.0/skeletonkey/core.py` & `skeletonkey-0.1.1/skeletonkey/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 import argparse
 import functools
 import inspect
 import os
 import sys
 from typing import Callable, Optional, Type, Any, Dict
 
-from .config import load_yaml_config, add_args_from_dict, add_yaml_extension, namespace_to_nested_namespace
+from .config import (
+    load_yaml_config,
+    add_args_from_dict,
+    add_yaml_extension,
+    namespace_to_nested_namespace,
+)
 
 
 def get_config_dir_path(config_path: str) -> str:
     """
     Convert a given relative or absolute config file path to its absolute directory path.
 
     Args:
@@ -34,14 +39,15 @@
             config_path = config_path[len("../") :]
             path_from_main = os.path.dirname(path_from_main)
 
         # Create absolute path.
         config_path = os.path.join(path_from_main, config_path)
     return config_path
 
+
 def unlock(config_name: str, config_path: Optional[str] = None) -> Callable:
     """
     Create a decorator for parsing and injecting configuration arguments into a
     main function from a YAML file.
 
     Args:
         config_name (str): The name of the YAML configuration file.
@@ -98,16 +104,16 @@
 def instantiate(namespace: argparse.Namespace) -> Any:
     """
     Instantiate a class object using a dictionary of keyword arguments.
     The dictionary should contain the keys "_kwargs_" and "_target_" to
     specify the class to instantiate and its arguments.
 
     Args:
-        namespace (argparse.Namespace): A Namespace object containing the key "_kwargs_" 
-            to specify the class and its arguments, along with any additional keyword 
+        namespace (argparse.Namespace): A Namespace object containing the key "_kwargs_"
+            to specify the class and its arguments, along with any additional keyword
             arguments for the class.
 
     Returns:
         Any: An instance of the specified class.
 
     Raises:
         AssertionError: If the class is missing specific parameters.
```

### Comparing `skeletonkey-0.1.0/skeletonkey.egg-info/PKG-INFO` & `skeletonkey-0.1.1/skeletonkey.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skeletonkey
-Version: 0.1.0
+Version: 0.1.1
 Summary: A bare-bones configuration managment tool.
 Home-page: https://github.com/sizemore0125/skeletonkey
 Author: Logan Sizemore
 Author-email: sizemore0125@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```


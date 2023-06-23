# Comparing `tmp/pymince-2.8.0.tar.gz` & `tmp/pymince-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymince-2.8.0.tar", last modified: Fri Jun 16 07:56:25 2023, max compression
+gzip compressed data, was "pymince-2.9.0.tar", last modified: Fri Jun 23 15:31:21 2023, max compression
```

## Comparing `pymince-2.8.0.tar` & `pymince-2.9.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:56:25.247122 pymince-2.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-16 07:56:05.000000 pymince-2.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    40149 2023-06-16 07:56:25.247122 pymince-2.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    39326 2023-06-16 07:56:05.000000 pymince-2.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:56:25.247122 pymince-2.8.0/pymince/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-16 07:56:05.000000 pymince-2.8.0/pymince/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-16 07:56:05.000000 pymince-2.8.0/pymince/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-16 07:56:05.000000 pymince-2.8.0/pymince/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-16 07:56:05.000000 pymince-2.8.0/pymince/boolean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-06-16 07:56:05.000000 pymince-2.8.0/pymince/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-06-16 07:56:05.000000 pymince-2.8.0/pymince/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-16 07:56:05.000000 pymince-2.8.0/pymince/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-06-16 07:56:05.000000 pymince-2.8.0/pymince/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)    13535 2023-06-16 07:56:05.000000 pymince-2.8.0/pymince/iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-06-16 07:56:05.000000 pymince-2.8.0/pymince/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-06-16 07:56:05.000000 pymince-2.8.0/pymince/jsonlines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-16 07:56:05.000000 pymince-2.8.0/pymince/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-16 07:56:05.000000 pymince-2.8.0/pymince/std.py
--rw-r--r--   0 runner    (1001) docker     (123)    10125 2023-06-16 07:56:05.000000 pymince-2.8.0/pymince/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-16 07:56:05.000000 pymince-2.8.0/pymince/warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-16 07:56:05.000000 pymince-2.8.0/pymince/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:56:25.247122 pymince-2.8.0/pymince.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    40149 2023-06-16 07:56:25.000000 pymince-2.8.0/pymince.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-16 07:56:25.000000 pymince-2.8.0/pymince.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 07:56:25.000000 pymince-2.8.0/pymince.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 07:56:25.000000 pymince-2.8.0/pymince.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 07:56:25.000000 pymince-2.8.0/pymince.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-06-16 07:56:05.000000 pymince-2.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 07:56:25.247122 pymince-2.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-16 07:56:05.000000 pymince-2.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:31:21.766707 pymince-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-23 15:31:03.000000 pymince-2.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    41661 2023-06-23 15:31:21.766707 pymince-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    40838 2023-06-23 15:31:03.000000 pymince-2.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:31:21.766707 pymince-2.9.0/pymince/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-23 15:31:03.000000 pymince-2.9.0/pymince/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-23 15:31:03.000000 pymince-2.9.0/pymince/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-23 15:31:03.000000 pymince-2.9.0/pymince/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-23 15:31:03.000000 pymince-2.9.0/pymince/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-06-23 15:31:03.000000 pymince-2.9.0/pymince/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-06-23 15:31:03.000000 pymince-2.9.0/pymince/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-23 15:31:03.000000 pymince-2.9.0/pymince/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-06-23 15:31:03.000000 pymince-2.9.0/pymince/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13535 2023-06-23 15:31:03.000000 pymince-2.9.0/pymince/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-06-23 15:31:03.000000 pymince-2.9.0/pymince/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-06-23 15:31:03.000000 pymince-2.9.0/pymince/jsonlines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-23 15:31:03.000000 pymince-2.9.0/pymince/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-23 15:31:03.000000 pymince-2.9.0/pymince/std.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10125 2023-06-23 15:31:03.000000 pymince-2.9.0/pymince/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-23 15:31:03.000000 pymince-2.9.0/pymince/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-23 15:31:03.000000 pymince-2.9.0/pymince/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:31:21.766707 pymince-2.9.0/pymince.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    41661 2023-06-23 15:31:21.000000 pymince-2.9.0/pymince.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-23 15:31:21.000000 pymince-2.9.0/pymince.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 15:31:21.000000 pymince-2.9.0/pymince.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 15:31:21.000000 pymince-2.9.0/pymince.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-23 15:31:21.000000 pymince-2.9.0/pymince.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-06-23 15:31:03.000000 pymince-2.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 15:31:21.766707 pymince-2.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-06-23 15:31:03.000000 pymince-2.9.0/setup.py
```

### Comparing `pymince-2.8.0/LICENSE` & `pymince-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymince-2.8.0/PKG-INFO` & `pymince-2.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymince
-Version: 2.8.0
+Version: 2.9.0
 Summary: Python shredded utilities
 Home-page: https://github.com/rmoralespp/pymince
 Author: rmoralespp
 Author-email: rmoralespp@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -55,16 +55,16 @@
 | **algorithm.py** |[*fibonacci*](#fibonacci), [*luhn*](#luhn), [*sieve_of_eratosthenes*](#sieve_of_eratosthenes)|
 | **boolean.py** |[*string2bool*](#string2bool)|
 | **dates.py** |[*IsoWeekDay*](#IsoWeekDay), [*WeekDay*](#WeekDay), [*irange*](#irange), [*string2year*](#string2year)|
 | **dictionary.py** |[*DigestGetter*](#DigestGetter), [*all_true_values*](#all_true_values), [*find_leaf_value*](#find_leaf_value), [*from_objects*](#from_objects), [*frozendict*](#frozendict), [*tree*](#tree)|
 | **file.py** |[*decompress*](#decompress), [*ensure_directory*](#ensure_directory), [*get_valid_filename*](#get_valid_filename), [*is_empty_directory*](#is_empty_directory), [*match_from_zip*](#match_from_zip), [*replace_extension*](#replace_extension)|
 | **functional.py** |[*caller*](#caller), [*classproperty*](#classproperty), [*identity*](#identity), [*once*](#once), [*pipe*](#pipe), [*retry_if_errors*](#retry_if_errors), [*retry_if_none*](#retry_if_none), [*set_attributes*](#set_attributes), [*suppress*](#suppress)|
 | **iterator.py** |[*all_distinct*](#all_distinct), [*all_equal*](#all_equal), [*all_equals*](#all_equals), [*all_identical*](#all_identical), [*centroid*](#centroid), [*consume*](#consume), [*grouper*](#grouper), [*ibool*](#ibool), [*in_all*](#in_all), [*in_any*](#in_any), [*ipush*](#ipush), [*mul*](#mul), [*only_one*](#only_one), [*pad_end*](#pad_end), [*pad_start*](#pad_start), [*partition*](#partition), [*replacer*](#replacer), [*splitter*](#splitter), [*sub*](#sub), [*truediv*](#truediv), [*uniquer*](#uniquer), [*uniques*](#uniques)|
-| **json.py** |[*JSONEncoder*](#JSONEncoder), [*dump_from_csv*](#dump_from_csv), [*dump_into*](#dump_into), [*dump_into_zip*](#dump_into_zip), [*idump_into*](#idump_into), [*idump_lines*](#idump_lines), [*load_from*](#load_from), [*load_from_zip*](#load_from_zip)|
-| **jsonlines.py** |[*dump*](#dump), [*dump_into*](#dump_into), [*dumper*](#dumper), [*dumps*](#dumps), [*load*](#load), [*load_from*](#load_from)|
+| **json.py** |[*JSONEncoder*](#JSONEncoder), [*dump_from_csv*](#dump_from_csv), [*dump_into*](#dump_into), [*dump_into_zip*](#dump_into_zip), [*idump_fork*](#idump_fork), [*idump_into*](#idump_into), [*idump_lines*](#idump_lines), [*load_from*](#load_from), [*load_from_zip*](#load_from_zip)|
+| **jsonlines.py** |[*dump*](#dump), [*dump_fork*](#dump_fork), [*dump_into*](#dump_into), [*dumper*](#dumper), [*dumps*](#dumps), [*load*](#load), [*load_from*](#load_from)|
 | **logging.py** |[*StructuredFormatter*](#StructuredFormatter), [*timed_block*](#timed_block)|
 | **std.py** |[*bind_json_std*](#bind_json_std)|
 | **text.py** |[*are_anagram*](#are_anagram), [*fullstr*](#fullstr), [*get_random_secret*](#get_random_secret), [*get_random_string*](#get_random_string), [*is_binary*](#is_binary), [*is_email_address*](#is_email_address), [*is_int*](#is_int), [*is_negative_int*](#is_negative_int), [*is_palindrome*](#is_palindrome), [*is_payment_card*](#is_payment_card), [*is_percentage*](#is_percentage), [*is_positive_int*](#is_positive_int), [*is_roman*](#is_roman), [*is_url*](#is_url), [*multireplace*](#multireplace), [*multireplacer*](#multireplacer), [*normalize_newlines*](#normalize_newlines), [*remove_decimal_zeros*](#remove_decimal_zeros), [*remove_number_commas*](#remove_number_commas), [*replace*](#replace)|
 | **warnings.py** |[*deprecated*](#deprecated)|
 | **xml.py** |[*iterparse*](#iterparse)|
 
 #### algorithm.py
@@ -970,14 +970,38 @@
 Dump JSON into the zip archive under the name arcname.
 
 Examples:
     from pymince.json import dump_into_zip
 
     dump_into_zip("archive.zip", "foo.json", {"key": "value"})
 ```
+##### idump_fork
+```
+idump_fork(path_items, encoding='utf-8', dump_if_empty=True, **dumps_kwargs)
+
+Incrementally dumps different groups of elements into
+the indicated JSON file.
+*** Useful to reduce memory consumption ***
+
+:param Iterable[file_path, Iterable[dict]] path_items: group items by file path
+:param encoding: 'utf-8' by default.
+:param bool dump_if_empty: If false, don't create an empty file.
+:param dumps_kwargs: json.dumps kwargs.
+
+Examples:
+    from pymince.json import idump_fork
+
+    path_items = (
+        ("num.json", ({"value": 1}, {"value": 2})),
+        ("num.json", ({"value": 3},)),
+        ("foo.json", ({"a": "1"}, {"b": 2})),
+        ("baz.json", ()),
+    )
+    idump_fork(iter(path_items))
+```
 ##### idump_into
 ```
 idump_into(filename, iterable, encoding='utf-8', **kwargs)
 
 Dump an iterable incrementally into a JSON file
 using the "utf-8" encoding.
 The result will always be an array with the elements of the iterable.
@@ -1039,14 +1063,38 @@
 Example:
     from pymince.jsonlines import dump
 
     data = ({'foo': 1}, {'bar': 2})
     with open('myfile.jsonl', mode='w', encoding ='utf-8') as file:
         dump(iter(data), file)
 ```
+##### dump_fork
+```
+dump_fork(path_items, encoding='utf-8', dump_if_empty=True, **kwargs)
+
+Incrementally dumps different groups of elements into
+the indicated `jsonlines` file.
+*** Useful to reduce memory consumption ***
+
+:param Iterable[file_path, Iterable[dict]] path_items: group items by file path
+:param encoding: 'utf-8' by default.
+:param bool dump_if_empty: If false, don't create an empty `jsonlines` file.
+:param kwargs: json.dumps kwargs.
+
+Examples:
+    from pymince.jsonlines import dump_fork
+
+    path_items = (
+        ("num.jsonl", ({"value": 1}, {"value": 2})),
+        ("num.jsonl", ({"value": 3},)),
+        ("foo.jsonl", ({"a": "1"}, {"b": 2})),
+        ("baz.jsonl", ()),
+    )
+    dump_fork(iter(path_items))
+```
 ##### dump_into
 ```
 dump_into(filename, iterable, encoding='utf-8', **kwargs)
 
 Dump iterable to a `jsonlines` file.
 
 Example:
```

### Comparing `pymince-2.8.0/README.md` & `pymince-2.9.0/pymince.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: pymince
+Version: 2.9.0
+Summary: Python shredded utilities
+Home-page: https://github.com/rmoralespp/pymince
+Author: rmoralespp
+Author-email: rmoralespp@gmail.com
+License: MIT
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Internet
+Classifier: Topic :: Utilities
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # pymince
 
 [![CI](https://github.com/rmoralespp/pymince/workflows/CI/badge.svg)](https://github.com/rmoralespp/pymince/actions?query=event%3Arelease+workflow%3ACI)
 [![pypi](https://img.shields.io/pypi/v/pymince.svg)](https://pypi.python.org/pypi/pymince)
 [![versions](https://img.shields.io/pypi/pyversions/pymince.svg)](https://github.com/rmoralespp/pymince)
 [![codecov](https://codecov.io/gh/rmoralespp/pymince/branch/main/graph/badge.svg)](https://app.codecov.io/gh/rmoralespp/pymince)
 [![license](https://img.shields.io/github/license/rmoralespp/pymince.svg)](https://github.com/rmoralespp/pymince/blob/main/LICENSE)
@@ -32,16 +55,16 @@
 | **algorithm.py** |[*fibonacci*](#fibonacci), [*luhn*](#luhn), [*sieve_of_eratosthenes*](#sieve_of_eratosthenes)|
 | **boolean.py** |[*string2bool*](#string2bool)|
 | **dates.py** |[*IsoWeekDay*](#IsoWeekDay), [*WeekDay*](#WeekDay), [*irange*](#irange), [*string2year*](#string2year)|
 | **dictionary.py** |[*DigestGetter*](#DigestGetter), [*all_true_values*](#all_true_values), [*find_leaf_value*](#find_leaf_value), [*from_objects*](#from_objects), [*frozendict*](#frozendict), [*tree*](#tree)|
 | **file.py** |[*decompress*](#decompress), [*ensure_directory*](#ensure_directory), [*get_valid_filename*](#get_valid_filename), [*is_empty_directory*](#is_empty_directory), [*match_from_zip*](#match_from_zip), [*replace_extension*](#replace_extension)|
 | **functional.py** |[*caller*](#caller), [*classproperty*](#classproperty), [*identity*](#identity), [*once*](#once), [*pipe*](#pipe), [*retry_if_errors*](#retry_if_errors), [*retry_if_none*](#retry_if_none), [*set_attributes*](#set_attributes), [*suppress*](#suppress)|
 | **iterator.py** |[*all_distinct*](#all_distinct), [*all_equal*](#all_equal), [*all_equals*](#all_equals), [*all_identical*](#all_identical), [*centroid*](#centroid), [*consume*](#consume), [*grouper*](#grouper), [*ibool*](#ibool), [*in_all*](#in_all), [*in_any*](#in_any), [*ipush*](#ipush), [*mul*](#mul), [*only_one*](#only_one), [*pad_end*](#pad_end), [*pad_start*](#pad_start), [*partition*](#partition), [*replacer*](#replacer), [*splitter*](#splitter), [*sub*](#sub), [*truediv*](#truediv), [*uniquer*](#uniquer), [*uniques*](#uniques)|
-| **json.py** |[*JSONEncoder*](#JSONEncoder), [*dump_from_csv*](#dump_from_csv), [*dump_into*](#dump_into), [*dump_into_zip*](#dump_into_zip), [*idump_into*](#idump_into), [*idump_lines*](#idump_lines), [*load_from*](#load_from), [*load_from_zip*](#load_from_zip)|
-| **jsonlines.py** |[*dump*](#dump), [*dump_into*](#dump_into), [*dumper*](#dumper), [*dumps*](#dumps), [*load*](#load), [*load_from*](#load_from)|
+| **json.py** |[*JSONEncoder*](#JSONEncoder), [*dump_from_csv*](#dump_from_csv), [*dump_into*](#dump_into), [*dump_into_zip*](#dump_into_zip), [*idump_fork*](#idump_fork), [*idump_into*](#idump_into), [*idump_lines*](#idump_lines), [*load_from*](#load_from), [*load_from_zip*](#load_from_zip)|
+| **jsonlines.py** |[*dump*](#dump), [*dump_fork*](#dump_fork), [*dump_into*](#dump_into), [*dumper*](#dumper), [*dumps*](#dumps), [*load*](#load), [*load_from*](#load_from)|
 | **logging.py** |[*StructuredFormatter*](#StructuredFormatter), [*timed_block*](#timed_block)|
 | **std.py** |[*bind_json_std*](#bind_json_std)|
 | **text.py** |[*are_anagram*](#are_anagram), [*fullstr*](#fullstr), [*get_random_secret*](#get_random_secret), [*get_random_string*](#get_random_string), [*is_binary*](#is_binary), [*is_email_address*](#is_email_address), [*is_int*](#is_int), [*is_negative_int*](#is_negative_int), [*is_palindrome*](#is_palindrome), [*is_payment_card*](#is_payment_card), [*is_percentage*](#is_percentage), [*is_positive_int*](#is_positive_int), [*is_roman*](#is_roman), [*is_url*](#is_url), [*multireplace*](#multireplace), [*multireplacer*](#multireplacer), [*normalize_newlines*](#normalize_newlines), [*remove_decimal_zeros*](#remove_decimal_zeros), [*remove_number_commas*](#remove_number_commas), [*replace*](#replace)|
 | **warnings.py** |[*deprecated*](#deprecated)|
 | **xml.py** |[*iterparse*](#iterparse)|
 
 #### algorithm.py
@@ -947,14 +970,38 @@
 Dump JSON into the zip archive under the name arcname.
 
 Examples:
     from pymince.json import dump_into_zip
 
     dump_into_zip("archive.zip", "foo.json", {"key": "value"})
 ```
+##### idump_fork
+```
+idump_fork(path_items, encoding='utf-8', dump_if_empty=True, **dumps_kwargs)
+
+Incrementally dumps different groups of elements into
+the indicated JSON file.
+*** Useful to reduce memory consumption ***
+
+:param Iterable[file_path, Iterable[dict]] path_items: group items by file path
+:param encoding: 'utf-8' by default.
+:param bool dump_if_empty: If false, don't create an empty file.
+:param dumps_kwargs: json.dumps kwargs.
+
+Examples:
+    from pymince.json import idump_fork
+
+    path_items = (
+        ("num.json", ({"value": 1}, {"value": 2})),
+        ("num.json", ({"value": 3},)),
+        ("foo.json", ({"a": "1"}, {"b": 2})),
+        ("baz.json", ()),
+    )
+    idump_fork(iter(path_items))
+```
 ##### idump_into
 ```
 idump_into(filename, iterable, encoding='utf-8', **kwargs)
 
 Dump an iterable incrementally into a JSON file
 using the "utf-8" encoding.
 The result will always be an array with the elements of the iterable.
@@ -1016,14 +1063,38 @@
 Example:
     from pymince.jsonlines import dump
 
     data = ({'foo': 1}, {'bar': 2})
     with open('myfile.jsonl', mode='w', encoding ='utf-8') as file:
         dump(iter(data), file)
 ```
+##### dump_fork
+```
+dump_fork(path_items, encoding='utf-8', dump_if_empty=True, **kwargs)
+
+Incrementally dumps different groups of elements into
+the indicated `jsonlines` file.
+*** Useful to reduce memory consumption ***
+
+:param Iterable[file_path, Iterable[dict]] path_items: group items by file path
+:param encoding: 'utf-8' by default.
+:param bool dump_if_empty: If false, don't create an empty `jsonlines` file.
+:param kwargs: json.dumps kwargs.
+
+Examples:
+    from pymince.jsonlines import dump_fork
+
+    path_items = (
+        ("num.jsonl", ({"value": 1}, {"value": 2})),
+        ("num.jsonl", ({"value": 3},)),
+        ("foo.jsonl", ({"a": "1"}, {"b": 2})),
+        ("baz.jsonl", ()),
+    )
+    dump_fork(iter(path_items))
+```
 ##### dump_into
 ```
 dump_into(filename, iterable, encoding='utf-8', **kwargs)
 
 Dump iterable to a `jsonlines` file.
 
 Example:
```

### Comparing `pymince-2.8.0/pymince/algorithm.py` & `pymince-2.9.0/pymince/algorithm.py`

 * *Files identical despite different names*

### Comparing `pymince-2.8.0/pymince/boolean.py` & `pymince-2.9.0/pymince/boolean.py`

 * *Files identical despite different names*

### Comparing `pymince-2.8.0/pymince/dates.py` & `pymince-2.9.0/pymince/dates.py`

 * *Files identical despite different names*

### Comparing `pymince-2.8.0/pymince/dictionary.py` & `pymince-2.9.0/pymince/dictionary.py`

 * *Files identical despite different names*

### Comparing `pymince-2.8.0/pymince/file.py` & `pymince-2.9.0/pymince/file.py`

 * *Files identical despite different names*

### Comparing `pymince-2.8.0/pymince/functional.py` & `pymince-2.9.0/pymince/functional.py`

 * *Files identical despite different names*

### Comparing `pymince-2.8.0/pymince/iterator.py` & `pymince-2.9.0/pymince/iterator.py`

 * *Files identical despite different names*

### Comparing `pymince-2.8.0/pymince/json.py` & `pymince-2.9.0/pymince/json.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import dataclasses
 import datetime
 import decimal
 import functools
 import itertools
 import json
 import operator
+import os
 import textwrap
 import uuid
 import zipfile
 
 dumps = functools.partial(json.dumps, ensure_ascii=False)
 dump = functools.partial(json.dump, ensure_ascii=False)
 ENCODING = "utf-8"
@@ -155,14 +156,76 @@
         dump_into("foo.json", it)
     """
 
     with open(filename, mode="w", encoding=encoding) as f:
         f.writelines(idump_lines(iterable, **kwargs))
 
 
+def idump_fork(path_items, encoding=ENCODING, dump_if_empty=True, **dumps_kwargs):
+    """
+    Incrementally dumps different groups of elements into
+    the indicated JSON file.
+    *** Useful to reduce memory consumption ***
+
+    :param Iterable[file_path, Iterable[dict]] path_items: group items by file path
+    :param encoding: 'utf-8' by default.
+    :param bool dump_if_empty: If false, don't create an empty file.
+    :param dumps_kwargs: json.dumps kwargs.
+
+    Examples:
+        from pymince.json import idump_fork
+
+        path_items = (
+            ("num.json", ({"value": 1}, {"value": 2})),
+            ("num.json", ({"value": 3},)),
+            ("foo.json", ({"a": "1"}, {"b": 2})),
+            ("baz.json", ()),
+        )
+        idump_fork(iter(path_items))
+    """
+
+    def get_dumper(dst):
+        nothing = True
+        with open(dst, mode="w", encoding=encoding) as fd:
+            write = fd.write
+            write("[\n")
+            try:
+                while True:
+                    obj = yield
+                    if nothing:
+                        nothing = False
+                    else:
+                        write(",\n")
+                    write(textwrap.indent(encode(obj), prefix))
+            except GeneratorExit:
+                write("]") if nothing else write("\n]")
+
+        if nothing and not dump_if_empty:
+            os.unlink(dst)
+
+    encode = functools.partial(dumps, **dumps_kwargs)
+    indent = dumps_kwargs.get("indent")
+    prefix = " " * indent if indent else ""
+
+    dumpers = dict()
+    for path, items in path_items:
+        if path in dumpers:
+            dumper = dumpers[path]
+        else:
+            dumper = get_dumper(path)
+            dumper.send(None)
+            dumpers[path] = dumper
+
+        for item in items:
+            dumper.send(item)
+    # Cleanup
+    for dumper in dumpers.values():
+        dumper.close()
+
+
 class JSONEncoder(json.JSONEncoder):
     """
     JSON encoder that handles additional types compared
     to `json.JSONEncoder`
 
     - `datetime` and `date` are serialized to strings according to the isoformat.
     - `decimal.Decimal` is serialized to a string.
```

### Comparing `pymince-2.8.0/pymince/jsonlines.py` & `pymince-2.9.0/pymince/jsonlines.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 Useful functions for working with JSON lines data as described:
 - http://ndjson.org/
 - https://jsonlines.org/
 """
 
 import functools
 import json
+import os
 
 import pymince._constants
 
 empty = pymince._constants.empty
 dumps_line = functools.partial(json.dumps, ensure_ascii=False)
 utf_8 = pymince._constants.utf_8
 new_line = "\n"
@@ -68,14 +69,71 @@
         dump_into("myfile.jsonl", iter(data))
     """
 
     with open(filename, mode="w", encoding=encoding) as f:
         dump(iterable, f, **kwargs)
 
 
+def dump_fork(path_items, encoding=utf_8, dump_if_empty=True, **kwargs):
+    """
+    Incrementally dumps different groups of elements into
+    the indicated `jsonlines` file.
+    *** Useful to reduce memory consumption ***
+
+    :param Iterable[file_path, Iterable[dict]] path_items: group items by file path
+    :param encoding: 'utf-8' by default.
+    :param bool dump_if_empty: If false, don't create an empty `jsonlines` file.
+    :param kwargs: json.dumps kwargs.
+
+    Examples:
+        from pymince.jsonlines import dump_fork
+
+        path_items = (
+            ("num.jsonl", ({"value": 1}, {"value": 2})),
+            ("num.jsonl", ({"value": 3},)),
+            ("foo.jsonl", ({"a": "1"}, {"b": 2})),
+            ("baz.jsonl", ()),
+        )
+        dump_fork(iter(path_items))
+    """
+
+    def get_writer(dst):
+        nothing = True
+        with open(dst, mode="w", encoding=encoding) as fd:
+            try:
+                while True:
+                    obj = yield
+                    if nothing:
+                        nothing = False
+                    else:
+                        fd.write(new_line)
+                    fd.write(encoder(obj))
+            except GeneratorExit:
+                pass
+        if nothing and not dump_if_empty:
+            os.unlink(dst)
+
+    encoder = functools.partial(dumps_line, **kwargs)
+    writers = dict()
+
+    for path, items in path_items:
+        if path in writers:
+            writer = writers[path]
+        else:
+            writer = get_writer(path)
+            writer.send(None)
+            writers[path] = writer
+
+        for item in items:
+            writer.send(item)
+    # Cleanup
+    for writer in writers.values():
+        writer.close()
+
+
 def load(fp, **kwargs):
     """
     Returns iterable from a file formatted as JSON lines.
 
     :param fp: file-like object
     :param kwargs: `json.loads` kwargs
     :rtype: Iterable[str]
```

### Comparing `pymince-2.8.0/pymince/logging.py` & `pymince-2.9.0/pymince/logging.py`

 * *Files identical despite different names*

### Comparing `pymince-2.8.0/pymince/std.py` & `pymince-2.9.0/pymince/std.py`

 * *Files identical despite different names*

### Comparing `pymince-2.8.0/pymince/text.py` & `pymince-2.9.0/pymince/text.py`

 * *Files identical despite different names*

### Comparing `pymince-2.8.0/pymince/warnings.py` & `pymince-2.9.0/pymince/warnings.py`

 * *Files identical despite different names*

### Comparing `pymince-2.8.0/pymince/xml.py` & `pymince-2.9.0/pymince/xml.py`

 * *Files identical despite different names*

### Comparing `pymince-2.8.0/pymince.egg-info/PKG-INFO` & `pymince-2.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: pymince
-Version: 2.8.0
-Summary: Python shredded utilities
-Home-page: https://github.com/rmoralespp/pymince
-Author: rmoralespp
-Author-email: rmoralespp@gmail.com
-License: MIT
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Internet
-Classifier: Topic :: Utilities
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # pymince
 
 [![CI](https://github.com/rmoralespp/pymince/workflows/CI/badge.svg)](https://github.com/rmoralespp/pymince/actions?query=event%3Arelease+workflow%3ACI)
 [![pypi](https://img.shields.io/pypi/v/pymince.svg)](https://pypi.python.org/pypi/pymince)
 [![versions](https://img.shields.io/pypi/pyversions/pymince.svg)](https://github.com/rmoralespp/pymince)
 [![codecov](https://codecov.io/gh/rmoralespp/pymince/branch/main/graph/badge.svg)](https://app.codecov.io/gh/rmoralespp/pymince)
 [![license](https://img.shields.io/github/license/rmoralespp/pymince.svg)](https://github.com/rmoralespp/pymince/blob/main/LICENSE)
@@ -55,16 +32,16 @@
 | **algorithm.py** |[*fibonacci*](#fibonacci), [*luhn*](#luhn), [*sieve_of_eratosthenes*](#sieve_of_eratosthenes)|
 | **boolean.py** |[*string2bool*](#string2bool)|
 | **dates.py** |[*IsoWeekDay*](#IsoWeekDay), [*WeekDay*](#WeekDay), [*irange*](#irange), [*string2year*](#string2year)|
 | **dictionary.py** |[*DigestGetter*](#DigestGetter), [*all_true_values*](#all_true_values), [*find_leaf_value*](#find_leaf_value), [*from_objects*](#from_objects), [*frozendict*](#frozendict), [*tree*](#tree)|
 | **file.py** |[*decompress*](#decompress), [*ensure_directory*](#ensure_directory), [*get_valid_filename*](#get_valid_filename), [*is_empty_directory*](#is_empty_directory), [*match_from_zip*](#match_from_zip), [*replace_extension*](#replace_extension)|
 | **functional.py** |[*caller*](#caller), [*classproperty*](#classproperty), [*identity*](#identity), [*once*](#once), [*pipe*](#pipe), [*retry_if_errors*](#retry_if_errors), [*retry_if_none*](#retry_if_none), [*set_attributes*](#set_attributes), [*suppress*](#suppress)|
 | **iterator.py** |[*all_distinct*](#all_distinct), [*all_equal*](#all_equal), [*all_equals*](#all_equals), [*all_identical*](#all_identical), [*centroid*](#centroid), [*consume*](#consume), [*grouper*](#grouper), [*ibool*](#ibool), [*in_all*](#in_all), [*in_any*](#in_any), [*ipush*](#ipush), [*mul*](#mul), [*only_one*](#only_one), [*pad_end*](#pad_end), [*pad_start*](#pad_start), [*partition*](#partition), [*replacer*](#replacer), [*splitter*](#splitter), [*sub*](#sub), [*truediv*](#truediv), [*uniquer*](#uniquer), [*uniques*](#uniques)|
-| **json.py** |[*JSONEncoder*](#JSONEncoder), [*dump_from_csv*](#dump_from_csv), [*dump_into*](#dump_into), [*dump_into_zip*](#dump_into_zip), [*idump_into*](#idump_into), [*idump_lines*](#idump_lines), [*load_from*](#load_from), [*load_from_zip*](#load_from_zip)|
-| **jsonlines.py** |[*dump*](#dump), [*dump_into*](#dump_into), [*dumper*](#dumper), [*dumps*](#dumps), [*load*](#load), [*load_from*](#load_from)|
+| **json.py** |[*JSONEncoder*](#JSONEncoder), [*dump_from_csv*](#dump_from_csv), [*dump_into*](#dump_into), [*dump_into_zip*](#dump_into_zip), [*idump_fork*](#idump_fork), [*idump_into*](#idump_into), [*idump_lines*](#idump_lines), [*load_from*](#load_from), [*load_from_zip*](#load_from_zip)|
+| **jsonlines.py** |[*dump*](#dump), [*dump_fork*](#dump_fork), [*dump_into*](#dump_into), [*dumper*](#dumper), [*dumps*](#dumps), [*load*](#load), [*load_from*](#load_from)|
 | **logging.py** |[*StructuredFormatter*](#StructuredFormatter), [*timed_block*](#timed_block)|
 | **std.py** |[*bind_json_std*](#bind_json_std)|
 | **text.py** |[*are_anagram*](#are_anagram), [*fullstr*](#fullstr), [*get_random_secret*](#get_random_secret), [*get_random_string*](#get_random_string), [*is_binary*](#is_binary), [*is_email_address*](#is_email_address), [*is_int*](#is_int), [*is_negative_int*](#is_negative_int), [*is_palindrome*](#is_palindrome), [*is_payment_card*](#is_payment_card), [*is_percentage*](#is_percentage), [*is_positive_int*](#is_positive_int), [*is_roman*](#is_roman), [*is_url*](#is_url), [*multireplace*](#multireplace), [*multireplacer*](#multireplacer), [*normalize_newlines*](#normalize_newlines), [*remove_decimal_zeros*](#remove_decimal_zeros), [*remove_number_commas*](#remove_number_commas), [*replace*](#replace)|
 | **warnings.py** |[*deprecated*](#deprecated)|
 | **xml.py** |[*iterparse*](#iterparse)|
 
 #### algorithm.py
@@ -970,14 +947,38 @@
 Dump JSON into the zip archive under the name arcname.
 
 Examples:
     from pymince.json import dump_into_zip
 
     dump_into_zip("archive.zip", "foo.json", {"key": "value"})
 ```
+##### idump_fork
+```
+idump_fork(path_items, encoding='utf-8', dump_if_empty=True, **dumps_kwargs)
+
+Incrementally dumps different groups of elements into
+the indicated JSON file.
+*** Useful to reduce memory consumption ***
+
+:param Iterable[file_path, Iterable[dict]] path_items: group items by file path
+:param encoding: 'utf-8' by default.
+:param bool dump_if_empty: If false, don't create an empty file.
+:param dumps_kwargs: json.dumps kwargs.
+
+Examples:
+    from pymince.json import idump_fork
+
+    path_items = (
+        ("num.json", ({"value": 1}, {"value": 2})),
+        ("num.json", ({"value": 3},)),
+        ("foo.json", ({"a": "1"}, {"b": 2})),
+        ("baz.json", ()),
+    )
+    idump_fork(iter(path_items))
+```
 ##### idump_into
 ```
 idump_into(filename, iterable, encoding='utf-8', **kwargs)
 
 Dump an iterable incrementally into a JSON file
 using the "utf-8" encoding.
 The result will always be an array with the elements of the iterable.
@@ -1039,14 +1040,38 @@
 Example:
     from pymince.jsonlines import dump
 
     data = ({'foo': 1}, {'bar': 2})
     with open('myfile.jsonl', mode='w', encoding ='utf-8') as file:
         dump(iter(data), file)
 ```
+##### dump_fork
+```
+dump_fork(path_items, encoding='utf-8', dump_if_empty=True, **kwargs)
+
+Incrementally dumps different groups of elements into
+the indicated `jsonlines` file.
+*** Useful to reduce memory consumption ***
+
+:param Iterable[file_path, Iterable[dict]] path_items: group items by file path
+:param encoding: 'utf-8' by default.
+:param bool dump_if_empty: If false, don't create an empty `jsonlines` file.
+:param kwargs: json.dumps kwargs.
+
+Examples:
+    from pymince.jsonlines import dump_fork
+
+    path_items = (
+        ("num.jsonl", ({"value": 1}, {"value": 2})),
+        ("num.jsonl", ({"value": 3},)),
+        ("foo.jsonl", ({"a": "1"}, {"b": 2})),
+        ("baz.jsonl", ()),
+    )
+    dump_fork(iter(path_items))
+```
 ##### dump_into
 ```
 dump_into(filename, iterable, encoding='utf-8', **kwargs)
 
 Dump iterable to a `jsonlines` file.
 
 Example:
```

### Comparing `pymince-2.8.0/pyproject.toml` & `pymince-2.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pymince-2.8.0/setup.py` & `pymince-2.9.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,19 +5,27 @@
 
 
 def read(filename):
     with open(filename, encoding="utf-8") as f:
         return f.read()
 
 
+def get_long_description():
+    blocks = (
+        read("README.md"),
+        # Fixme read("CHANGELOG.md"),
+    )
+    return "\n".join(blocks)
+
+
 setup(
     name=__title__,
     version=__version__,
     description="Python shredded utilities",
-    long_description=read("README.md"),
+    long_description=get_long_description(),
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
```


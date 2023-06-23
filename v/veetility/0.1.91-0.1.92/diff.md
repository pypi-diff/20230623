# Comparing `tmp/veetility-0.1.91.tar.gz` & `tmp/veetility-0.1.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veetility-0.1.91.tar", last modified: Fri Jun 23 10:21:12 2023, max compression
+gzip compressed data, was "veetility-0.1.92.tar", last modified: Fri Jun 23 10:57:32 2023, max compression
```

## Comparing `veetility-0.1.91.tar` & `veetility-0.1.92.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-06-23 10:21:12.470429 veetility-0.1.91/
--rw-r--r--   0 willbutler   (502) staff       (20)     3538 2023-06-23 10:21:12.470221 veetility-0.1.91/PKG-INFO
--rw-r--r--   0 willbutler   (502) staff       (20)     2881 2023-02-28 17:30:34.000000 veetility-0.1.91/README.md
--rw-r--r--   0 willbutler   (502) staff       (20)       38 2023-06-23 10:21:12.470494 veetility-0.1.91/setup.cfg
--rw-r--r--   0 willbutler   (502) staff       (20)     1438 2023-06-23 10:21:05.000000 veetility-0.1.91/setup.py
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-06-23 10:21:12.465452 veetility-0.1.91/tests/
--rw-r--r--   0 willbutler   (502) staff       (20)     1892 2023-04-09 19:51:45.000000 veetility-0.1.91/tests/test_best_fuzzy_match_dict.py
--rw-r--r--   0 willbutler   (502) staff       (20)     2471 2023-04-09 19:42:01.000000 veetility-0.1.91/tests/test_identify_match_multi_cols.py
--rw-r--r--   0 willbutler   (502) staff       (20)     1588 2023-04-09 18:45:40.000000 veetility-0.1.91/tests/test_prepare_string_matching.py
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-06-23 10:21:12.468936 veetility-0.1.91/veetility/
--rw-r--r--   0 willbutler   (502) staff       (20)        0 2023-02-28 17:30:34.000000 veetility-0.1.91/veetility/__init__.py
--rw-r--r--   0 willbutler   (502) staff       (20)    17689 2023-06-12 11:29:12.000000 veetility-0.1.91/veetility/cleaning_functions.py
--rw-r--r--   0 willbutler   (502) staff       (20)     7088 2023-05-23 14:51:46.000000 veetility-0.1.91/veetility/generic_functions.py
--rw-r--r--   0 willbutler   (502) staff       (20)     2465 2023-03-03 12:20:14.000000 veetility-0.1.91/veetility/point_to_point_regressor.py
--rw-r--r--   0 willbutler   (502) staff       (20)    30599 2023-06-23 10:20:51.000000 veetility-0.1.91/veetility/quality_assessments.py
--rw-r--r--   0 willbutler   (502) staff       (20)    11585 2023-05-23 16:42:13.000000 veetility-0.1.91/veetility/snowflake.py
--rw-r--r--   0 willbutler   (502) staff       (20)    53597 2023-06-12 19:20:06.000000 veetility-0.1.91/veetility/utility_functions.py
--rw-r--r--   0 willbutler   (502) staff       (20)     2411 2023-05-05 13:50:17.000000 veetility-0.1.91/veetility/v_lift.py
--rw-r--r--   0 willbutler   (502) staff       (20)     6007 2023-06-12 15:35:11.000000 veetility-0.1.91/veetility/view_through_rate.py
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-06-23 10:21:12.469934 veetility-0.1.91/veetility.egg-info/
--rw-r--r--   0 willbutler   (502) staff       (20)     3538 2023-06-23 10:21:12.000000 veetility-0.1.91/veetility.egg-info/PKG-INFO
--rw-r--r--   0 willbutler   (502) staff       (20)      557 2023-06-23 10:21:12.000000 veetility-0.1.91/veetility.egg-info/SOURCES.txt
--rw-r--r--   0 willbutler   (502) staff       (20)        1 2023-06-23 10:21:12.000000 veetility-0.1.91/veetility.egg-info/dependency_links.txt
--rw-r--r--   0 willbutler   (502) staff       (20)       97 2023-06-23 10:21:12.000000 veetility-0.1.91/veetility.egg-info/requires.txt
--rw-r--r--   0 willbutler   (502) staff       (20)       10 2023-06-23 10:21:12.000000 veetility-0.1.91/veetility.egg-info/top_level.txt
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-06-23 10:57:32.495826 veetility-0.1.92/
+-rw-r--r--   0 willbutler   (502) staff       (20)     3538 2023-06-23 10:57:32.495613 veetility-0.1.92/PKG-INFO
+-rw-r--r--   0 willbutler   (502) staff       (20)     2881 2023-02-28 17:30:34.000000 veetility-0.1.92/README.md
+-rw-r--r--   0 willbutler   (502) staff       (20)       38 2023-06-23 10:57:32.495879 veetility-0.1.92/setup.cfg
+-rw-r--r--   0 willbutler   (502) staff       (20)     1438 2023-06-23 10:57:23.000000 veetility-0.1.92/setup.py
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-06-23 10:57:32.490158 veetility-0.1.92/tests/
+-rw-r--r--   0 willbutler   (502) staff       (20)     1892 2023-04-09 19:51:45.000000 veetility-0.1.92/tests/test_best_fuzzy_match_dict.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     2471 2023-04-09 19:42:01.000000 veetility-0.1.92/tests/test_identify_match_multi_cols.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     1588 2023-04-09 18:45:40.000000 veetility-0.1.92/tests/test_prepare_string_matching.py
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-06-23 10:57:32.494067 veetility-0.1.92/veetility/
+-rw-r--r--   0 willbutler   (502) staff       (20)        0 2023-02-28 17:30:34.000000 veetility-0.1.92/veetility/__init__.py
+-rw-r--r--   0 willbutler   (502) staff       (20)    17689 2023-06-12 11:29:12.000000 veetility-0.1.92/veetility/cleaning_functions.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     7088 2023-05-23 14:51:46.000000 veetility-0.1.92/veetility/generic_functions.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     2465 2023-03-03 12:20:14.000000 veetility-0.1.92/veetility/point_to_point_regressor.py
+-rw-r--r--   0 willbutler   (502) staff       (20)    30693 2023-06-23 10:56:40.000000 veetility-0.1.92/veetility/quality_assessments.py
+-rw-r--r--   0 willbutler   (502) staff       (20)    11585 2023-05-23 16:42:13.000000 veetility-0.1.92/veetility/snowflake.py
+-rw-r--r--   0 willbutler   (502) staff       (20)    53597 2023-06-12 19:20:06.000000 veetility-0.1.92/veetility/utility_functions.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     2411 2023-05-05 13:50:17.000000 veetility-0.1.92/veetility/v_lift.py
+-rw-r--r--   0 willbutler   (502) staff       (20)     6007 2023-06-12 15:35:11.000000 veetility-0.1.92/veetility/view_through_rate.py
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-06-23 10:57:32.495376 veetility-0.1.92/veetility.egg-info/
+-rw-r--r--   0 willbutler   (502) staff       (20)     3538 2023-06-23 10:57:32.000000 veetility-0.1.92/veetility.egg-info/PKG-INFO
+-rw-r--r--   0 willbutler   (502) staff       (20)      557 2023-06-23 10:57:32.000000 veetility-0.1.92/veetility.egg-info/SOURCES.txt
+-rw-r--r--   0 willbutler   (502) staff       (20)        1 2023-06-23 10:57:32.000000 veetility-0.1.92/veetility.egg-info/dependency_links.txt
+-rw-r--r--   0 willbutler   (502) staff       (20)       97 2023-06-23 10:57:32.000000 veetility-0.1.92/veetility.egg-info/requires.txt
+-rw-r--r--   0 willbutler   (502) staff       (20)       10 2023-06-23 10:57:32.000000 veetility-0.1.92/veetility.egg-info/top_level.txt
```

### Comparing `veetility-0.1.91/PKG-INFO` & `veetility-0.1.92/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veetility
-Version: 0.1.91
+Version: 0.1.92
 Summary: Demo library
 Home-page: 
 Author: Vaynermedia
 Author-email: will.butler@vaynermedia.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `veetility-0.1.91/README.md` & `veetility-0.1.92/README.md`

 * *Files identical despite different names*

### Comparing `veetility-0.1.91/setup.py` & `veetility-0.1.92/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="veetility",
-    version="0.1.91",
+    version="0.1.92",
     description="Demo library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="Vaynermedia",
     author_email="will.butler@vaynermedia.com",
     license="MIT",
```

### Comparing `veetility-0.1.91/tests/test_best_fuzzy_match_dict.py` & `veetility-0.1.92/tests/test_best_fuzzy_match_dict.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.91/tests/test_identify_match_multi_cols.py` & `veetility-0.1.92/tests/test_identify_match_multi_cols.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.91/tests/test_prepare_string_matching.py` & `veetility-0.1.92/tests/test_prepare_string_matching.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.91/veetility/cleaning_functions.py` & `veetility-0.1.92/veetility/cleaning_functions.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.91/veetility/generic_functions.py` & `veetility-0.1.92/veetility/generic_functions.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.91/veetility/point_to_point_regressor.py` & `veetility-0.1.92/veetility/point_to_point_regressor.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.91/veetility/quality_assessments.py` & `veetility-0.1.92/veetility/quality_assessments.py`

 * *Files 0% similar despite different names*

```diff
@@ -435,24 +435,26 @@
         key_values_conv_cols = [x.replace(' Key', '') for x in naming_convention.columns if ' Key' in x]
 
         def remove_empties_from_list(input_list):
             '''Obtaining a list of keys from the tracker sheet column often results in multiple empty
                 strings, this function removes them from the list'''
             return list(filter(lambda x: x != '', input_list))
 
-        def return_value(string, tag, acceptable_values):
+        def return_value(string, tag, acceptable_values=None):
             """This checks for each campaign, group_name or ad_name string, for a certain tag e.g.'pl'
             whether the tag is even present and if so whether a correct value is present"""
             search_string = f'{start_char}{tag}{middle_char}(.*?){end_char}'
             search_result = re.search(search_string, string + '_') #add a underscore at so search string has an endpoint to find
             if search_result == None:
                 return 'NoKey'
             elif search_result.group(1).strip(' ') == '':
                 return 'NoKey'
             else:
+                if acceptable_values == None:
+                    return "CorrectKeyPresent"
                 if search_result.group(1).upper() in acceptable_values:
                     return "Correct"
                 else:
                     return 'Incorrect Value'
 
         
         for level in conv_level_tuple:
@@ -463,13 +465,13 @@
             for label,tag in level[0].items():
                 #For each label and tag in the required set 
                 if label in key_values_conv_cols:
                     acceptable_values= remove_empties_from_list(naming_convention[label+' Key'].str.upper().unique().tolist())
                     output_df[f'{label} ("{tag}")'] = output_df[level[1]].apply(lambda x: return_value(x, tag, acceptable_values))
                     checking_cols.append(f'{label} ("{tag}")')
                 else:
-                    output_df[f'{label} ("{tag}")'] = output_df[level[1]].apply(lambda x: return_value(x, tag, []))
+                    output_df[f'{label} ("{tag}")'] = output_df[level[1]].apply(lambda x: return_value(x, tag))
                     checking_cols.append(f'{label} ("{tag}")')
                 
             output_df = output_df.sort_values(by=checking_cols, ascending=False)
             self.util.write_to_gsheet(workbook_name = gsheet_name, sheet_name= level[2], df = output_df)
```

### Comparing `veetility-0.1.91/veetility/snowflake.py` & `veetility-0.1.92/veetility/snowflake.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.91/veetility/utility_functions.py` & `veetility-0.1.92/veetility/utility_functions.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.91/veetility/v_lift.py` & `veetility-0.1.92/veetility/v_lift.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.91/veetility/view_through_rate.py` & `veetility-0.1.92/veetility/view_through_rate.py`

 * *Files identical despite different names*

### Comparing `veetility-0.1.91/veetility.egg-info/PKG-INFO` & `veetility-0.1.92/veetility.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veetility
-Version: 0.1.91
+Version: 0.1.92
 Summary: Demo library
 Home-page: 
 Author: Vaynermedia
 Author-email: will.butler@vaynermedia.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `veetility-0.1.91/veetility.egg-info/SOURCES.txt` & `veetility-0.1.92/veetility.egg-info/SOURCES.txt`

 * *Files identical despite different names*


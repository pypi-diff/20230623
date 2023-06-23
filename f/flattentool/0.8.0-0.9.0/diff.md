# Comparing `tmp/flattentool-0.8.0.tar.gz` & `tmp/flattentool-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flattentool-0.8.0.tar", last modified: Wed Jul 31 16:25:32 2019, max compression
+gzip compressed data, was "dist/flattentool-0.9.0.tar", last modified: Tue Oct 22 09:40:37 2019, max compression
```

## Comparing `flattentool-0.8.0.tar` & `flattentool-0.9.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-07-31 16:25:32.000000 flattentool-0.8.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-07-31 16:25:32.000000 flattentool-0.8.0/flattentool.egg-info/
--rw-r--r--   0 root         (0) root         (0)      465 2019-07-31 16:25:32.000000 flattentool-0.8.0/flattentool.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2019-07-31 16:25:32.000000 flattentool-0.8.0/flattentool.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2019-07-31 16:25:32.000000 flattentool-0.8.0/flattentool.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      337 2019-07-31 16:25:32.000000 flattentool-0.8.0/flattentool.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       70 2019-07-31 16:25:32.000000 flattentool-0.8.0/flattentool.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)      662 2019-07-31 16:24:40.000000 flattentool-0.8.0/setup.py
--rw-rw-r--   0 root         (0) root         (0)       70 2019-07-31 16:25:32.000000 flattentool-0.8.0/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)       68 2018-06-05 09:56:09.000000 flattentool-0.8.0/flatten-tool
--rw-r--r--   0 root         (0) root         (0)      337 2019-07-31 16:25:32.000000 flattentool-0.8.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-07-31 16:25:32.000000 flattentool-0.8.0/flattentool/
--rw-rw-r--   0 root         (0) root         (0)    12206 2019-07-31 15:52:24.000000 flattentool-0.8.0/flattentool/cli.py
--rw-rw-r--   0 root         (0) root         (0)    38773 2019-07-31 15:52:24.000000 flattentool-0.8.0/flattentool/input.py
--rw-rw-r--   0 root         (0) root         (0)      140 2018-06-05 09:56:09.000000 flattentool-0.8.0/flattentool/exceptions.py
--rw-rw-r--   0 root         (0) root         (0)     5440 2018-11-22 10:31:53.000000 flattentool-0.8.0/flattentool/sort_xml.py
--rw-rw-r--   0 root         (0) root         (0)     1166 2018-11-22 10:31:53.000000 flattentool-0.8.0/flattentool/lib.py
--rw-rw-r--   0 root         (0) root         (0)     3551 2019-07-26 19:18:27.000000 flattentool-0.8.0/flattentool/output.py
--rw-rw-r--   0 root         (0) root         (0)      795 2018-06-05 09:56:09.000000 flattentool-0.8.0/flattentool/sheet.py
--rw-rw-r--   0 root         (0) root         (0)     3409 2018-11-22 10:31:53.000000 flattentool-0.8.0/flattentool/xml_output.py
--rw-rw-r--   0 root         (0) root         (0)    14233 2019-07-31 15:52:24.000000 flattentool-0.8.0/flattentool/schema.py
--rw-rw-r--   0 root         (0) root         (0)    18053 2019-07-31 15:52:24.000000 flattentool-0.8.0/flattentool/json_input.py
--rw-rw-r--   0 root         (0) root         (0)    11232 2019-07-31 15:52:24.000000 flattentool-0.8.0/flattentool/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3038 2018-06-05 09:56:09.000000 flattentool-0.8.0/README.md
+drwxr-xr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2019-10-22 09:40:37.000000 flattentool-0.9.0/
+drwxr-xr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2019-10-22 09:40:37.000000 flattentool-0.9.0/flattentool.egg-info/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        1 2019-10-22 09:40:37.000000 flattentool-0.9.0/flattentool.egg-info/dependency_links.txt
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)       12 2019-10-22 09:40:37.000000 flattentool-0.9.0/flattentool.egg-info/top_level.txt
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      465 2019-10-22 09:40:37.000000 flattentool-0.9.0/flattentool.egg-info/SOURCES.txt
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      337 2019-10-22 09:40:37.000000 flattentool-0.9.0/flattentool.egg-info/PKG-INFO
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)       70 2019-10-22 09:40:37.000000 flattentool-0.9.0/flattentool.egg-info/requires.txt
+-rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)      662 2019-09-24 14:40:03.000000 flattentool-0.9.0/setup.py
+-rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)     3038 2019-09-05 17:47:56.000000 flattentool-0.9.0/README.md
+-rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)      337 2019-10-22 09:40:37.000000 flattentool-0.9.0/PKG-INFO
+drwxr-xr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2019-10-22 09:40:37.000000 flattentool-0.9.0/flattentool/
+-rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)    38773 2019-08-13 11:46:36.000000 flattentool-0.9.0/flattentool/input.py
+-rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)    18053 2019-08-13 11:46:36.000000 flattentool-0.9.0/flattentool/json_input.py
+-rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)     5440 2019-03-13 06:29:15.000000 flattentool-0.9.0/flattentool/sort_xml.py
+-rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)    12206 2019-08-13 11:46:36.000000 flattentool-0.9.0/flattentool/cli.py
+-rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)     3551 2019-03-13 06:29:15.000000 flattentool-0.9.0/flattentool/output.py
+-rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)    11232 2019-08-13 11:46:36.000000 flattentool-0.9.0/flattentool/__init__.py
+-rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)    14233 2019-08-13 11:46:36.000000 flattentool-0.9.0/flattentool/schema.py
+-rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)     3449 2019-09-11 10:03:01.000000 flattentool-0.9.0/flattentool/xml_output.py
+-rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)     1166 2019-03-13 06:29:15.000000 flattentool-0.9.0/flattentool/lib.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      140 2017-03-20 13:35:36.000000 flattentool-0.9.0/flattentool/exceptions.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      795 2016-06-07 18:27:14.000000 flattentool-0.9.0/flattentool/sheet.py
+-rwxr-xr-x   0 bjwebb    (1000) bjwebb    (1000)       68 2015-11-19 17:51:31.000000 flattentool-0.9.0/flatten-tool
+-rw-r--r--   0 bjwebb    (1000) bjwebb    (1000)       70 2019-10-22 09:40:37.000000 flattentool-0.9.0/setup.cfg
```

### Comparing `flattentool-0.8.0/setup.py` & `flattentool-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 install_requires = ['jsonref', 'schema', 'openpyxl>=2.6', 'six', 'pytz', 'xmltodict', 'lxml']
 
 if sys.version < '3':
     install_requires.append('unicodecsv')
 
 setup(
     name='flattentool',
-    version='0.8.0',
+    version='0.9.0',
     author='Open Data Services',
     author_email='code@opendataservices.coop',
     packages=['flattentool'],
     scripts=['flatten-tool'],
     url='https://github.com/OpenDataServices/flatten-tool',
     license='MIT',
     description='Tools for generating CSV and other flat versions of the structured data',
```

### Comparing `flattentool-0.8.0/flattentool/cli.py` & `flattentool-0.9.0/flattentool/cli.py`

 * *Files identical despite different names*

### Comparing `flattentool-0.8.0/flattentool/input.py` & `flattentool-0.9.0/flattentool/input.py`

 * *Files identical despite different names*

### Comparing `flattentool-0.8.0/flattentool/sort_xml.py` & `flattentool-0.9.0/flattentool/sort_xml.py`

 * *Files identical despite different names*

### Comparing `flattentool-0.8.0/flattentool/lib.py` & `flattentool-0.9.0/flattentool/lib.py`

 * *Files identical despite different names*

### Comparing `flattentool-0.8.0/flattentool/output.py` & `flattentool-0.9.0/flattentool/output.py`

 * *Files identical despite different names*

### Comparing `flattentool-0.8.0/flattentool/sheet.py` & `flattentool-0.9.0/flattentool/sheet.py`

 * *Files identical despite different names*

### Comparing `flattentool-0.8.0/flattentool/xml_output.py` & `flattentool-0.9.0/flattentool/xml_output.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,10 +82,10 @@
         for element in root:
             sort_element(element, schema_dict)
     if xml_comment is None:
         xml_comment = 'XML generated by flatten-tool'
     comment = ET.Comment(xml_comment)
     root.insert(0, comment)
     if USING_LXML:
-        return ET.tostring(root, pretty_print=True)
+        return ET.tostring(root, pretty_print=True, xml_declaration=True, encoding='utf-8')
     else:
         return ET.tostring(root)
```

### Comparing `flattentool-0.8.0/flattentool/schema.py` & `flattentool-0.9.0/flattentool/schema.py`

 * *Files identical despite different names*

### Comparing `flattentool-0.8.0/flattentool/json_input.py` & `flattentool-0.9.0/flattentool/json_input.py`

 * *Files identical despite different names*

### Comparing `flattentool-0.8.0/flattentool/__init__.py` & `flattentool-0.9.0/flattentool/__init__.py`

 * *Files identical despite different names*

### Comparing `flattentool-0.8.0/README.md` & `flattentool-0.9.0/README.md`

 * *Files identical despite different names*


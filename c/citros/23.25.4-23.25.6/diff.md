# Comparing `tmp/citros-23.25.4.tar.gz` & `tmp/citros-23.25.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citros-23.25.4.tar", last modified: Thu Jun 22 22:01:12 2023, max compression
+gzip compressed data, was "citros-23.25.6.tar", last modified: Thu Jun 22 22:27:13 2023, max compression
```

## Comparing `citros-23.25.4.tar` & `citros-23.25.6.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:01:12.386602 citros-23.25.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-22 22:00:56.000000 citros-23.25.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-06-22 22:01:12.386602 citros-23.25.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-06-22 22:00:56.000000 citros-23.25.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:01:12.382602 citros-23.25.4/bin/
--rw-r--r--   0 runner    (1001) docker     (123)    17661 2023-06-22 22:00:56.000000 citros-23.25.4/bin/citros
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:01:12.382602 citros-23.25.4/citros/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-22 22:00:56.000000 citros-23.25.4/citros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19027 2023-06-22 22:00:56.000000 citros-23.25.4/citros/citros.py
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-06-22 22:00:56.000000 citros-23.25.4/citros/citros_bag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-22 22:00:56.000000 citros-23.25.4/citros/citros_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-06-22 22:00:56.000000 citros-23.25.4/citros/citros_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-06-22 22:00:56.000000 citros-23.25.4/citros/citros_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8429 2023-06-22 22:00:56.000000 citros-23.25.4/citros/citros_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-22 22:00:56.000000 citros-23.25.4/citros/citros_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:01:12.386602 citros-23.25.4/citros/launches/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-22 22:00:56.000000 citros-23.25.4/citros/launches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12322 2023-06-22 22:00:56.000000 citros-23.25.4/citros/launches/launch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:01:12.386602 citros-23.25.4/citros/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-22 22:00:56.000000 citros-23.25.4/citros/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-22 22:00:56.000000 citros-23.25.4/citros/logger/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-22 22:00:56.000000 citros-23.25.4/citros/logger/logger_pg_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:01:12.386602 citros-23.25.4/citros/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-22 22:00:56.000000 citros-23.25.4/citros/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-22 22:00:56.000000 citros-23.25.4/citros/parsers/parser_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20601 2023-06-22 22:00:56.000000 citros-23.25.4/citros/parsers/parser_ros2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:01:12.386602 citros-23.25.4/citros/rosbag/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-22 22:00:56.000000 citros-23.25.4/citros/rosbag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-22 22:00:56.000000 citros-23.25.4/citros/rosbag/reader_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-22 22:00:56.000000 citros-23.25.4/citros/rosbag/reader_mcap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-06-22 22:00:56.000000 citros-23.25.4/citros/rosbag/reader_sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:01:12.382602 citros-23.25.4/citros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-06-22 22:01:12.000000 citros-23.25.4/citros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-22 22:01:12.000000 citros-23.25.4/citros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 22:01:12.000000 citros-23.25.4/citros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-22 22:01:12.000000 citros-23.25.4/citros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-22 22:01:12.000000 citros-23.25.4/citros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-22 22:00:56.000000 citros-23.25.4/citros_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 22:01:12.386602 citros-23.25.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-22 22:00:56.000000 citros-23.25.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:01:12.386602 citros-23.25.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-06-22 22:00:56.000000 citros-23.25.4/tests/test_parse_makefile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-06-22 22:00:56.000000 citros-23.25.4/tests/test_parse_setup_py.py
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-22 22:00:56.000000 citros-23.25.4/tests/test_parse_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:27:13.126909 citros-23.25.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-22 22:26:58.000000 citros-23.25.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-06-22 22:27:13.126909 citros-23.25.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-06-22 22:26:58.000000 citros-23.25.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:27:13.122909 citros-23.25.6/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)    17661 2023-06-22 22:26:58.000000 citros-23.25.6/bin/citros
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:27:13.122909 citros-23.25.6/citros/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-22 22:26:58.000000 citros-23.25.6/citros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19027 2023-06-22 22:26:58.000000 citros-23.25.6/citros/citros.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-06-22 22:26:58.000000 citros-23.25.6/citros/citros_bag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-22 22:26:58.000000 citros-23.25.6/citros/citros_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-06-22 22:26:58.000000 citros-23.25.6/citros/citros_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-06-22 22:26:58.000000 citros-23.25.6/citros/citros_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8429 2023-06-22 22:26:58.000000 citros-23.25.6/citros/citros_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-22 22:26:58.000000 citros-23.25.6/citros/citros_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:27:13.122909 citros-23.25.6/citros/launches/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-22 22:26:58.000000 citros-23.25.6/citros/launches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12322 2023-06-22 22:26:58.000000 citros-23.25.6/citros/launches/launch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:27:13.126909 citros-23.25.6/citros/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-22 22:26:58.000000 citros-23.25.6/citros/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-22 22:26:58.000000 citros-23.25.6/citros/logger/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-22 22:26:58.000000 citros-23.25.6/citros/logger/logger_pg_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:27:13.126909 citros-23.25.6/citros/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-22 22:26:58.000000 citros-23.25.6/citros/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-22 22:26:58.000000 citros-23.25.6/citros/parsers/parser_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20601 2023-06-22 22:26:58.000000 citros-23.25.6/citros/parsers/parser_ros2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:27:13.126909 citros-23.25.6/citros/rosbag/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-22 22:26:58.000000 citros-23.25.6/citros/rosbag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-22 22:26:58.000000 citros-23.25.6/citros/rosbag/reader_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-22 22:26:58.000000 citros-23.25.6/citros/rosbag/reader_mcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-06-22 22:26:58.000000 citros-23.25.6/citros/rosbag/reader_sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:27:13.122909 citros-23.25.6/citros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-06-22 22:27:13.000000 citros-23.25.6/citros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-22 22:27:13.000000 citros-23.25.6/citros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 22:27:13.000000 citros-23.25.6/citros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-22 22:27:13.000000 citros-23.25.6/citros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-22 22:27:13.000000 citros-23.25.6/citros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-22 22:26:58.000000 citros-23.25.6/citros_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 22:27:13.126909 citros-23.25.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-22 22:26:58.000000 citros-23.25.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 22:27:13.126909 citros-23.25.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-06-22 22:26:58.000000 citros-23.25.6/tests/test_parse_makefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-06-22 22:26:58.000000 citros-23.25.6/tests/test_parse_setup_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-22 22:26:58.000000 citros-23.25.6/tests/test_parse_xml.py
```

### Comparing `citros-23.25.4/LICENSE` & `citros-23.25.6/LICENSE`

 * *Files identical despite different names*

### Comparing `citros-23.25.4/PKG-INFO` & `citros-23.25.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citros
-Version: 23.25.4
+Version: 23.25.6
 Summary: A cli entrypoint for the citros system.
 Home-page: http://pypi.python.org/pypi/citros_cli/
 Author: vovacooper
 Author-email: vova@lulav.space
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `citros-23.25.4/README.md` & `citros-23.25.6/README.md`

 * *Files identical despite different names*

### Comparing `citros-23.25.4/bin/citros` & `citros-23.25.6/bin/citros`

 * *Files identical despite different names*

### Comparing `citros-23.25.4/citros/__init__.py` & `citros-23.25.6/citros/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.25.4/citros/citros.py` & `citros-23.25.6/citros/citros.py`

 * *Files identical despite different names*

### Comparing `citros-23.25.4/citros/citros_bag.py` & `citros-23.25.6/citros/citros_bag.py`

 * *Files identical despite different names*

### Comparing `citros-23.25.4/citros/citros_batch.py` & `citros-23.25.6/citros/citros_batch.py`

 * *Files identical despite different names*

### Comparing `citros-23.25.4/citros/citros_events.py` & `citros-23.25.6/citros/citros_events.py`

 * *Files identical despite different names*

### Comparing `citros-23.25.4/citros/citros_integration.py` & `citros-23.25.6/citros/citros_integration.py`

 * *Files identical despite different names*

### Comparing `citros-23.25.4/citros/citros_params.py` & `citros-23.25.6/citros/citros_params.py`

 * *Files identical despite different names*

### Comparing `citros-23.25.4/citros/citros_utils.py` & `citros-23.25.6/citros/citros_utils.py`

 * *Files identical despite different names*

### Comparing `citros-23.25.4/citros/launches/__init__.py` & `citros-23.25.6/citros/launches/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.25.4/citros/launches/launch.py` & `citros-23.25.6/citros/launches/launch.py`

 * *Files identical despite different names*

### Comparing `citros-23.25.4/citros/logger/__init__.py` & `citros-23.25.6/citros/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.25.4/citros/logger/logger.py` & `citros-23.25.6/citros/logger/logger.py`

 * *Files identical despite different names*

### Comparing `citros-23.25.4/citros/logger/logger_pg_handler.py` & `citros-23.25.6/citros/logger/logger_pg_handler.py`

 * *Files identical despite different names*

### Comparing `citros-23.25.4/citros/parsers/__init__.py` & `citros-23.25.6/citros/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.25.4/citros/parsers/parser_ros2.py` & `citros-23.25.6/citros/parsers/parser_ros2.py`

 * *Files identical despite different names*

### Comparing `citros-23.25.4/citros/rosbag/__init__.py` & `citros-23.25.6/citros/rosbag/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.25.4/citros/rosbag/reader_base.py` & `citros-23.25.6/citros/rosbag/reader_base.py`

 * *Files identical despite different names*

### Comparing `citros-23.25.4/citros/rosbag/reader_mcap.py` & `citros-23.25.6/citros/rosbag/reader_mcap.py`

 * *Files identical despite different names*

### Comparing `citros-23.25.4/citros/rosbag/reader_sqlite.py` & `citros-23.25.6/citros/rosbag/reader_sqlite.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,13 @@
                 bytes_wrote = buffer.write(row + '\n')
                 size = size + bytes_wrote
                 # 10MB chunks max
                 if size >= CHUNK_SIZE:                    
                     yield buffer
                     buffer, size = StringIO(), 0
             
-            # upload topic by topic so it one topic has an error it wont effect the whole bag. 
-            if size >= CHUNK_SIZE:                    
-                yield buffer
-                buffer, size = StringIO(), 0
+            # upload topic by topic so it one topic has an error it wont effect the whole bag.             
+            yield buffer
+            buffer, size = StringIO(), 0
                     
         # return the rest of the file.
         yield buffer
```

### Comparing `citros-23.25.4/citros.egg-info/PKG-INFO` & `citros-23.25.6/citros.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citros
-Version: 23.25.4
+Version: 23.25.6
 Summary: A cli entrypoint for the citros system.
 Home-page: http://pypi.python.org/pypi/citros_cli/
 Author: vovacooper
 Author-email: vova@lulav.space
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `citros-23.25.4/citros.egg-info/SOURCES.txt` & `citros-23.25.6/citros.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `citros-23.25.4/setup.py` & `citros-23.25.6/setup.py`

 * *Files identical despite different names*

### Comparing `citros-23.25.4/tests/test_parse_makefile.py` & `citros-23.25.6/tests/test_parse_makefile.py`

 * *Files identical despite different names*

### Comparing `citros-23.25.4/tests/test_parse_setup_py.py` & `citros-23.25.6/tests/test_parse_setup_py.py`

 * *Files identical despite different names*

### Comparing `citros-23.25.4/tests/test_parse_xml.py` & `citros-23.25.6/tests/test_parse_xml.py`

 * *Files identical despite different names*

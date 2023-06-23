# Comparing `tmp/spark-board-0.0.2.tar.gz` & `tmp/spark-board-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/spark-board/spark-board/dist/.tmp-efa9nfb_/spark-board-0.0.2.tar", last modified: Fri Jun 23 04:28:48 2023, max compression
+gzip compressed data, was "/home/runner/work/spark-board/spark-board/dist/.tmp-cfq5h83o/spark-board-0.0.3.tar", last modified: Fri Jun 23 04:36:02 2023, max compression
```

## Comparing `spark-board-0.0.2.tar` & `spark-board-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 04:28:48.000000 spark-board-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-23 04:28:30.000000 spark-board-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-23 04:28:48.000000 spark-board-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-23 04:28:30.000000 spark-board-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 04:28:30.000000 spark-board-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 04:28:48.000000 spark-board-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-23 04:28:30.000000 spark-board-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 04:28:48.000000 spark-board-0.0.2/spark_board/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-23 04:28:30.000000 spark-board-0.0.2/spark_board/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-06-23 04:28:30.000000 spark-board-0.0.2/spark_board/html.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 04:28:48.000000 spark-board-0.0.2/spark_board/plan_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-23 04:28:30.000000 spark-board-0.0.2/spark_board/plan_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-23 04:28:30.000000 spark-board-0.0.2/spark_board/plan_extractor/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-23 04:28:30.000000 spark-board-0.0.2/spark_board/plan_extractor/dag_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-23 04:28:30.000000 spark-board-0.0.2/spark_board/plan_extractor/py4j_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-06-23 04:28:30.000000 spark-board-0.0.2/spark_board/plan_extractor/transformation_node_builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-23 04:28:30.000000 spark-board-0.0.2/spark_board/plan_extractor/transformations_dag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 04:28:48.000000 spark-board-0.0.2/spark_board.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-23 04:28:48.000000 spark-board-0.0.2/spark_board.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-23 04:28:48.000000 spark-board-0.0.2/spark_board.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 04:28:48.000000 spark-board-0.0.2/spark_board.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-23 04:28:48.000000 spark-board-0.0.2/spark_board.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-23 04:28:48.000000 spark-board-0.0.2/spark_board.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 04:36:02.000000 spark-board-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-23 04:35:44.000000 spark-board-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-23 04:36:02.000000 spark-board-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-23 04:35:44.000000 spark-board-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 04:35:44.000000 spark-board-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 04:36:02.000000 spark-board-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-23 04:35:44.000000 spark-board-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 04:36:02.000000 spark-board-0.0.3/spark_board/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-23 04:35:44.000000 spark-board-0.0.3/spark_board/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-06-23 04:35:44.000000 spark-board-0.0.3/spark_board/html.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 04:36:02.000000 spark-board-0.0.3/spark_board/plan_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-23 04:35:44.000000 spark-board-0.0.3/spark_board/plan_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-23 04:35:44.000000 spark-board-0.0.3/spark_board/plan_extractor/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-23 04:35:44.000000 spark-board-0.0.3/spark_board/plan_extractor/dag_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-23 04:35:44.000000 spark-board-0.0.3/spark_board/plan_extractor/py4j_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-06-23 04:35:44.000000 spark-board-0.0.3/spark_board/plan_extractor/transformation_node_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-23 04:35:44.000000 spark-board-0.0.3/spark_board/plan_extractor/transformations_dag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 04:36:02.000000 spark-board-0.0.3/spark_board.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-23 04:36:02.000000 spark-board-0.0.3/spark_board.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-23 04:36:02.000000 spark-board-0.0.3/spark_board.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 04:36:02.000000 spark-board-0.0.3/spark_board.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-23 04:36:02.000000 spark-board-0.0.3/spark_board.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-23 04:36:02.000000 spark-board-0.0.3/spark_board.egg-info/top_level.txt
```

### Comparing `spark-board-0.0.2/LICENSE` & `spark-board-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spark-board-0.0.2/PKG-INFO` & `spark-board-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-board
-Version: 0.0.2
+Version: 0.0.3
 Summary: Interactive visualization of Spark jobs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `spark-board-0.0.2/README.md` & `spark-board-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `spark-board-0.0.2/setup.py` & `spark-board-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 README = (this_directory / "README.md").read_text()
 
 
 setup(
     name="spark-board",
-    version="0.0.2",
+    version="0.0.3",
     authors=[
         {"name": "Axel Lijdens", "email": "alijdens@fi.uba.ar"},
         {"name": "Ezequiel Werner", "email": "ewerner@fi.uba.ar"},
     ],
     description="Interactive visualization of Spark jobs",
     long_description_content_type="text/markdown",
     long_description=README,
```

### Comparing `spark-board-0.0.2/spark_board/html.py` & `spark-board-0.0.3/spark_board/html.py`

 * *Files identical despite different names*

### Comparing `spark-board-0.0.2/spark_board/plan_extractor/dag.py` & `spark-board-0.0.3/spark_board/plan_extractor/dag.py`

 * *Files identical despite different names*

### Comparing `spark-board-0.0.2/spark_board/plan_extractor/dag_builder.py` & `spark-board-0.0.3/spark_board/plan_extractor/dag_builder.py`

 * *Files identical despite different names*

### Comparing `spark-board-0.0.2/spark_board/plan_extractor/transformation_node_builders.py` & `spark-board-0.0.3/spark_board/plan_extractor/transformation_node_builders.py`

 * *Files identical despite different names*

### Comparing `spark-board-0.0.2/spark_board/plan_extractor/transformations_dag.py` & `spark-board-0.0.3/spark_board/plan_extractor/transformations_dag.py`

 * *Files identical despite different names*

### Comparing `spark-board-0.0.2/spark_board.egg-info/PKG-INFO` & `spark-board-0.0.3/spark_board.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-board
-Version: 0.0.2
+Version: 0.0.3
 Summary: Interactive visualization of Spark jobs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `spark-board-0.0.2/spark_board.egg-info/SOURCES.txt` & `spark-board-0.0.3/spark_board.egg-info/SOURCES.txt`

 * *Files identical despite different names*


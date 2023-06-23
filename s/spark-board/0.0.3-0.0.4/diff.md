# Comparing `tmp/spark-board-0.0.3.tar.gz` & `tmp/spark-board-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/spark-board/spark-board/dist/.tmp-cfq5h83o/spark-board-0.0.3.tar", last modified: Fri Jun 23 04:36:02 2023, max compression
+gzip compressed data, was "/home/runner/work/spark-board/spark-board/dist/.tmp-rri_qphi/spark-board-0.0.4.tar", last modified: Fri Jun 23 04:48:38 2023, max compression
```

## Comparing `spark-board-0.0.3.tar` & `spark-board-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 04:36:02.000000 spark-board-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-23 04:35:44.000000 spark-board-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-23 04:36:02.000000 spark-board-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-23 04:35:44.000000 spark-board-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 04:35:44.000000 spark-board-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 04:36:02.000000 spark-board-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-23 04:35:44.000000 spark-board-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 04:36:02.000000 spark-board-0.0.3/spark_board/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-23 04:35:44.000000 spark-board-0.0.3/spark_board/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-06-23 04:35:44.000000 spark-board-0.0.3/spark_board/html.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 04:36:02.000000 spark-board-0.0.3/spark_board/plan_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-23 04:35:44.000000 spark-board-0.0.3/spark_board/plan_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-23 04:35:44.000000 spark-board-0.0.3/spark_board/plan_extractor/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-23 04:35:44.000000 spark-board-0.0.3/spark_board/plan_extractor/dag_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-23 04:35:44.000000 spark-board-0.0.3/spark_board/plan_extractor/py4j_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-06-23 04:35:44.000000 spark-board-0.0.3/spark_board/plan_extractor/transformation_node_builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-23 04:35:44.000000 spark-board-0.0.3/spark_board/plan_extractor/transformations_dag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 04:36:02.000000 spark-board-0.0.3/spark_board.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-23 04:36:02.000000 spark-board-0.0.3/spark_board.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-23 04:36:02.000000 spark-board-0.0.3/spark_board.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 04:36:02.000000 spark-board-0.0.3/spark_board.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-23 04:36:02.000000 spark-board-0.0.3/spark_board.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-23 04:36:02.000000 spark-board-0.0.3/spark_board.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 04:48:38.000000 spark-board-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-23 04:48:17.000000 spark-board-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-23 04:48:38.000000 spark-board-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-23 04:48:17.000000 spark-board-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 04:48:17.000000 spark-board-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 04:48:38.000000 spark-board-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-23 04:48:17.000000 spark-board-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 04:48:38.000000 spark-board-0.0.4/spark_board/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-23 04:48:17.000000 spark-board-0.0.4/spark_board/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-06-23 04:48:17.000000 spark-board-0.0.4/spark_board/html.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 04:48:38.000000 spark-board-0.0.4/spark_board/plan_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-23 04:48:17.000000 spark-board-0.0.4/spark_board/plan_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-23 04:48:17.000000 spark-board-0.0.4/spark_board/plan_extractor/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-23 04:48:17.000000 spark-board-0.0.4/spark_board/plan_extractor/dag_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-23 04:48:17.000000 spark-board-0.0.4/spark_board/plan_extractor/py4j_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-06-23 04:48:17.000000 spark-board-0.0.4/spark_board/plan_extractor/transformation_node_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-23 04:48:17.000000 spark-board-0.0.4/spark_board/plan_extractor/transformations_dag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 04:48:38.000000 spark-board-0.0.4/spark_board/ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 04:48:38.000000 spark-board-0.0.4/spark_board/ui/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-23 04:48:31.000000 spark-board-0.0.4/spark_board/ui/assets/filter-baaad4cd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-23 04:48:31.000000 spark-board-0.0.4/spark_board/ui/assets/group-daa83ef9.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-06-23 04:48:31.000000 spark-board-0.0.4/spark_board/ui/assets/index-c952fe44.css
+-rw-r--r--   0 runner    (1001) docker     (123)   471497 2023-06-23 04:48:31.000000 spark-board-0.0.4/spark_board/ui/assets/index-d2bd27be.js
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-23 04:48:31.000000 spark-board-0.0.4/spark_board/ui/assets/join-cbb2d651.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    33550 2023-06-23 04:48:31.000000 spark-board-0.0.4/spark_board/ui/assets/logo-c54f7abe.png
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-23 04:48:31.000000 spark-board-0.0.4/spark_board/ui/assets/project-5fbb0573.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-23 04:48:31.000000 spark-board-0.0.4/spark_board/ui/assets/sort-7864cb74.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-23 04:48:31.000000 spark-board-0.0.4/spark_board/ui/assets/table-1441493a.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    21357 2023-06-23 04:48:31.000000 spark-board-0.0.4/spark_board/ui/assets/union-e6640cdd.png
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-23 04:48:31.000000 spark-board-0.0.4/spark_board/ui/assets/upload-4f5382f0.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-23 04:48:32.000000 spark-board-0.0.4/spark_board/ui/assets/upper-limit-2af54b76.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-06-23 04:48:31.000000 spark-board-0.0.4/spark_board/ui/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 04:48:38.000000 spark-board-0.0.4/spark_board.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-23 04:48:38.000000 spark-board-0.0.4/spark_board.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-23 04:48:38.000000 spark-board-0.0.4/spark_board.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 04:48:38.000000 spark-board-0.0.4/spark_board.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-23 04:48:38.000000 spark-board-0.0.4/spark_board.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-23 04:48:38.000000 spark-board-0.0.4/spark_board.egg-info/top_level.txt
```

### Comparing `spark-board-0.0.3/LICENSE` & `spark-board-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spark-board-0.0.3/PKG-INFO` & `spark-board-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-board
-Version: 0.0.3
+Version: 0.0.4
 Summary: Interactive visualization of Spark jobs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `spark-board-0.0.3/README.md` & `spark-board-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `spark-board-0.0.3/setup.py` & `spark-board-0.0.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,31 +4,32 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 README = (this_directory / "README.md").read_text()
 
 
 setup(
     name="spark-board",
-    version="0.0.3",
+    version="0.0.4",
     authors=[
         {"name": "Axel Lijdens", "email": "alijdens@fi.uba.ar"},
         {"name": "Ezequiel Werner", "email": "ewerner@fi.uba.ar"},
     ],
     description="Interactive visualization of Spark jobs",
     long_description_content_type="text/markdown",
     long_description=README,
-    readme="README.md",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">3.6",
     install_requires=[
         "pyspark>3",
     ],
     packages=[package for package in find_packages() if package.startswith("spark_board")],
     # this is required to include the static web files that show the spark-board UI in the
-    # spark_board/ui directory thiss directory is created during the deployment process and
-    # contains the compiled spark-board-ui react application
-    include_package_data=True,
+    # final package. This directory is created during the deployment process and contains
+    # the compiled spark-board-ui react application
+    package_data={
+        "spark_board": ["ui/**/*"],
+    },
 )
```

### Comparing `spark-board-0.0.3/spark_board/html.py` & `spark-board-0.0.4/spark_board/html.py`

 * *Files identical despite different names*

### Comparing `spark-board-0.0.3/spark_board/plan_extractor/dag.py` & `spark-board-0.0.4/spark_board/plan_extractor/dag.py`

 * *Files identical despite different names*

### Comparing `spark-board-0.0.3/spark_board/plan_extractor/dag_builder.py` & `spark-board-0.0.4/spark_board/plan_extractor/dag_builder.py`

 * *Files identical despite different names*

### Comparing `spark-board-0.0.3/spark_board/plan_extractor/transformation_node_builders.py` & `spark-board-0.0.4/spark_board/plan_extractor/transformation_node_builders.py`

 * *Files identical despite different names*

### Comparing `spark-board-0.0.3/spark_board/plan_extractor/transformations_dag.py` & `spark-board-0.0.4/spark_board/plan_extractor/transformations_dag.py`

 * *Files identical despite different names*

### Comparing `spark-board-0.0.3/spark_board.egg-info/PKG-INFO` & `spark-board-0.0.4/spark_board.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-board
-Version: 0.0.3
+Version: 0.0.4
 Summary: Interactive visualization of Spark jobs
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```


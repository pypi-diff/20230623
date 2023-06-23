# Comparing `tmp/SmartDriveML-0.0.8.tar.gz` & `tmp/SmartDriveML-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SmartDriveML-0.0.8.tar", last modified: Fri Jun 23 19:18:28 2023, max compression
+gzip compressed data, was "SmartDriveML-0.0.9.tar", last modified: Fri Jun 23 19:22:04 2023, max compression
```

## Comparing `SmartDriveML-0.0.8.tar` & `SmartDriveML-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 19:18:28.676080 SmartDriveML-0.0.8/
--rw-rw-rw-   0        0        0     1790 2023-06-23 19:18:28.676080 SmartDriveML-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-23 19:18:28.644838 SmartDriveML-0.0.8/SmartDriveML/
--rw-rw-rw-   0        0        0      238 2023-06-23 19:14:37.000000 SmartDriveML-0.0.8/SmartDriveML/MainCode.py
--rw-rw-rw-   0        0        0        0 2023-06-23 19:18:10.000000 SmartDriveML-0.0.8/SmartDriveML/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-23 19:18:28.676080 SmartDriveML-0.0.8/SmartDriveML.egg-info/
--rw-rw-rw-   0        0        0     1790 2023-06-23 19:18:28.000000 SmartDriveML-0.0.8/SmartDriveML.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-06-23 19:18:28.000000 SmartDriveML-0.0.8/SmartDriveML.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 19:18:28.000000 SmartDriveML-0.0.8/SmartDriveML.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-23 19:18:28.000000 SmartDriveML-0.0.8/SmartDriveML.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-23 19:18:28.000000 SmartDriveML-0.0.8/SmartDriveML.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 19:18:28.676080 SmartDriveML-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     2988 2023-06-23 19:18:22.000000 SmartDriveML-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 19:22:04.717977 SmartDriveML-0.0.9/
+-rw-rw-rw-   0        0        0     1790 2023-06-23 19:22:04.717977 SmartDriveML-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-23 19:22:04.717977 SmartDriveML-0.0.9/SmartDriveML.egg-info/
+-rw-rw-rw-   0        0        0     1790 2023-06-23 19:22:04.000000 SmartDriveML-0.0.9/SmartDriveML.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      187 2023-06-23 19:22:04.000000 SmartDriveML-0.0.9/SmartDriveML.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 19:22:04.000000 SmartDriveML-0.0.9/SmartDriveML.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-23 19:22:04.000000 SmartDriveML-0.0.9/SmartDriveML.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 19:22:04.000000 SmartDriveML-0.0.9/SmartDriveML.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 19:22:04.717977 SmartDriveML-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2988 2023-06-23 19:21:47.000000 SmartDriveML-0.0.9/setup.py
```

### Comparing `SmartDriveML-0.0.8/PKG-INFO` & `SmartDriveML-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmartDriveML
-Version: 0.0.8
+Version: 0.0.9
 Summary: SmartDriveML: Driving Industrial Projects with Affordable ML Solutions, Frameworks and Cloud Choices
 Home-page: UNKNOWN
 Author: Hrishikesh Thakurdesai
 Author-email: hrishikesh.thakurdesai.92@gmail.com
 License: UNKNOWN
 Keywords: python,machine learning,pyspark,cloud
 Platform: UNKNOWN
```

### Comparing `SmartDriveML-0.0.8/SmartDriveML.egg-info/PKG-INFO` & `SmartDriveML-0.0.9/SmartDriveML.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmartDriveML
-Version: 0.0.8
+Version: 0.0.9
 Summary: SmartDriveML: Driving Industrial Projects with Affordable ML Solutions, Frameworks and Cloud Choices
 Home-page: UNKNOWN
 Author: Hrishikesh Thakurdesai
 Author-email: hrishikesh.thakurdesai.92@gmail.com
 License: UNKNOWN
 Keywords: python,machine learning,pyspark,cloud
 Platform: UNKNOWN
```

### Comparing `SmartDriveML-0.0.8/setup.py` & `SmartDriveML-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'SmartDriveML: Driving Industrial Projects with Affordable ML Solutions, Frameworks and Cloud Choices'
 LONG_DESCRIPTION = 'SmartDriveML is a state-of-the-art Python library created to revolutionize the way industries drive projects using machine learning. This advanced application serves as a comprehensive tool, assisting users in making informed decisions regarding cloud service providers, framework selection, and project feasibility, all while maintaining a cost-effective approach. One of the core functionalities of SmartDriveML is its ability to compare costs among various cloud service providers. By leveraging its integrated algorithms and extensive data on cloud service pricing, this tool enables users to evaluate the financial implications of different providers such as AWS or Azure. With this crucial information at their disposal, industries can optimize their budget allocation, ensuring that their machine learning projects remain economically viable. Another essential feature of SmartDriveML is its framework analysis capability. The library provides comprehensive insights into popular frameworks like Pandas and PySpark, aiding users in choosing the most suitable option for their specific project requirements. By considering factors such as data volume, computational needs, and ease of implementation, SmartDriveML helps industries make informed decisions that align with their objectives and resource constraints. Moreover, SmartDriveML goes beyond cost and framework analysis by providing essential functions for exploratory data analysis and executing fundamental machine learning algorithms on sample datasets. These functions enable users to assess the potential of their projects, allowing them to evaluate whether machine learning can effectively drive their initiatives. By providing this accessible yet powerful toolset, SmartDriveML empowers industries to make data-driven decisions and confidently embark on machine learning-driven projects.'
 
 # Setting up
 setup(
     name="SmartDriveML",
     version=VERSION,
```


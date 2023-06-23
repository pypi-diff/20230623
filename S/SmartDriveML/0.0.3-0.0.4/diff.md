# Comparing `tmp/SmartDriveML-0.0.3.tar.gz` & `tmp/SmartDriveML-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SmartDriveML-0.0.3.tar", last modified: Fri Jun 23 15:42:43 2023, max compression
+gzip compressed data, was "SmartDriveML-0.0.4.tar", last modified: Fri Jun 23 19:00:43 2023, max compression
```

## Comparing `SmartDriveML-0.0.3.tar` & `SmartDriveML-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 15:42:43.650757 SmartDriveML-0.0.3/
--rw-rw-rw-   0        0        0     1790 2023-06-23 15:42:43.635140 SmartDriveML-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-23 15:42:43.619510 SmartDriveML-0.0.3/SmartDriveML/
--rw-rw-rw-   0        0        0      141 2023-06-23 15:20:45.000000 SmartDriveML-0.0.3/SmartDriveML/MainCode.py
--rw-rw-rw-   0        0        0       15 2023-06-23 15:40:10.000000 SmartDriveML-0.0.3/SmartDriveML/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-23 15:42:43.635140 SmartDriveML-0.0.3/SmartDriveML.egg-info/
--rw-rw-rw-   0        0        0     1790 2023-06-23 15:42:43.000000 SmartDriveML-0.0.3/SmartDriveML.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-06-23 15:42:43.000000 SmartDriveML-0.0.3/SmartDriveML.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 15:42:43.000000 SmartDriveML-0.0.3/SmartDriveML.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-23 15:42:43.000000 SmartDriveML-0.0.3/SmartDriveML.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-23 15:42:43.000000 SmartDriveML-0.0.3/SmartDriveML.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 15:42:43.650757 SmartDriveML-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     2988 2023-06-23 15:42:29.000000 SmartDriveML-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 19:00:43.676637 SmartDriveML-0.0.4/
+-rw-rw-rw-   0        0        0     1790 2023-06-23 19:00:43.676637 SmartDriveML-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-23 19:00:43.645390 SmartDriveML-0.0.4/SmartDriveML/
+-rw-rw-rw-   0        0        0       30 2023-06-23 19:00:17.000000 SmartDriveML-0.0.4/SmartDriveML/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 19:00:43.661024 SmartDriveML-0.0.4/SmartDriveML.egg-info/
+-rw-rw-rw-   0        0        0     1790 2023-06-23 19:00:43.000000 SmartDriveML-0.0.4/SmartDriveML.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2023-06-23 19:00:43.000000 SmartDriveML-0.0.4/SmartDriveML.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 19:00:43.000000 SmartDriveML-0.0.4/SmartDriveML.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-23 19:00:43.000000 SmartDriveML-0.0.4/SmartDriveML.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-23 19:00:43.000000 SmartDriveML-0.0.4/SmartDriveML.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 19:00:43.676637 SmartDriveML-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     2988 2023-06-23 19:00:28.000000 SmartDriveML-0.0.4/setup.py
```

### Comparing `SmartDriveML-0.0.3/PKG-INFO` & `SmartDriveML-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmartDriveML
-Version: 0.0.3
+Version: 0.0.4
 Summary: SmartDriveML: Driving Industrial Projects with Affordable ML Solutions, Frameworks and Cloud Choices
 Home-page: UNKNOWN
 Author: Hrishikesh Thakurdesai
 Author-email: hrishikesh.thakurdesai.92@gmail.com
 License: UNKNOWN
 Keywords: python,machine learning,pyspark,cloud
 Platform: UNKNOWN
```

### Comparing `SmartDriveML-0.0.3/SmartDriveML.egg-info/PKG-INFO` & `SmartDriveML-0.0.4/SmartDriveML.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmartDriveML
-Version: 0.0.3
+Version: 0.0.4
 Summary: SmartDriveML: Driving Industrial Projects with Affordable ML Solutions, Frameworks and Cloud Choices
 Home-page: UNKNOWN
 Author: Hrishikesh Thakurdesai
 Author-email: hrishikesh.thakurdesai.92@gmail.com
 License: UNKNOWN
 Keywords: python,machine learning,pyspark,cloud
 Platform: UNKNOWN
```

### Comparing `SmartDriveML-0.0.3/setup.py` & `SmartDriveML-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'SmartDriveML: Driving Industrial Projects with Affordable ML Solutions, Frameworks and Cloud Choices'
 LONG_DESCRIPTION = 'SmartDriveML is a state-of-the-art Python library created to revolutionize the way industries drive projects using machine learning. This advanced application serves as a comprehensive tool, assisting users in making informed decisions regarding cloud service providers, framework selection, and project feasibility, all while maintaining a cost-effective approach. One of the core functionalities of SmartDriveML is its ability to compare costs among various cloud service providers. By leveraging its integrated algorithms and extensive data on cloud service pricing, this tool enables users to evaluate the financial implications of different providers such as AWS or Azure. With this crucial information at their disposal, industries can optimize their budget allocation, ensuring that their machine learning projects remain economically viable. Another essential feature of SmartDriveML is its framework analysis capability. The library provides comprehensive insights into popular frameworks like Pandas and PySpark, aiding users in choosing the most suitable option for their specific project requirements. By considering factors such as data volume, computational needs, and ease of implementation, SmartDriveML helps industries make informed decisions that align with their objectives and resource constraints. Moreover, SmartDriveML goes beyond cost and framework analysis by providing essential functions for exploratory data analysis and executing fundamental machine learning algorithms on sample datasets. These functions enable users to assess the potential of their projects, allowing them to evaluate whether machine learning can effectively drive their initiatives. By providing this accessible yet powerful toolset, SmartDriveML empowers industries to make data-driven decisions and confidently embark on machine learning-driven projects.'
 
 # Setting up
 setup(
     name="SmartDriveML",
     version=VERSION,
```


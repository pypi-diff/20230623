# Comparing `tmp/SmartDriveML-0.0.5.tar.gz` & `tmp/SmartDriveML-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SmartDriveML-0.0.5.tar", last modified: Fri Jun 23 19:04:54 2023, max compression
+gzip compressed data, was "SmartDriveML-0.0.6.tar", last modified: Fri Jun 23 19:10:15 2023, max compression
```

## Comparing `SmartDriveML-0.0.5.tar` & `SmartDriveML-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 19:04:54.716468 SmartDriveML-0.0.5/
--rw-rw-rw-   0        0        0     1790 2023-06-23 19:04:54.700844 SmartDriveML-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-23 19:04:54.685219 SmartDriveML-0.0.5/SmartDriveML/
--rw-rw-rw-   0        0        0       30 2023-06-23 19:00:17.000000 SmartDriveML-0.0.5/SmartDriveML/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-23 19:04:54.700844 SmartDriveML-0.0.5/SmartDriveML.egg-info/
--rw-rw-rw-   0        0        0     1790 2023-06-23 19:04:54.000000 SmartDriveML-0.0.5/SmartDriveML.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2023-06-23 19:04:54.000000 SmartDriveML-0.0.5/SmartDriveML.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 19:04:54.000000 SmartDriveML-0.0.5/SmartDriveML.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-23 19:04:54.000000 SmartDriveML-0.0.5/SmartDriveML.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-23 19:04:54.000000 SmartDriveML-0.0.5/SmartDriveML.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 19:04:54.716468 SmartDriveML-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     2988 2023-06-23 19:04:40.000000 SmartDriveML-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 19:10:15.509321 SmartDriveML-0.0.6/
+-rw-rw-rw-   0        0        0     1790 2023-06-23 19:10:15.509321 SmartDriveML-0.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-23 19:10:15.493723 SmartDriveML-0.0.6/SmartDriveML/
+-rw-rw-rw-   0        0        0      141 2023-06-23 15:20:45.000000 SmartDriveML-0.0.6/SmartDriveML/MainCode.py
+-rw-rw-rw-   0        0        0       31 2023-06-23 19:09:33.000000 SmartDriveML-0.0.6/SmartDriveML/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 19:10:15.509321 SmartDriveML-0.0.6/SmartDriveML.egg-info/
+-rw-rw-rw-   0        0        0     1790 2023-06-23 19:10:15.000000 SmartDriveML-0.0.6/SmartDriveML.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-06-23 19:10:15.000000 SmartDriveML-0.0.6/SmartDriveML.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 19:10:15.000000 SmartDriveML-0.0.6/SmartDriveML.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-23 19:10:15.000000 SmartDriveML-0.0.6/SmartDriveML.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-23 19:10:15.000000 SmartDriveML-0.0.6/SmartDriveML.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 19:10:15.509321 SmartDriveML-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     2988 2023-06-23 19:10:00.000000 SmartDriveML-0.0.6/setup.py
```

### Comparing `SmartDriveML-0.0.5/PKG-INFO` & `SmartDriveML-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmartDriveML
-Version: 0.0.5
+Version: 0.0.6
 Summary: SmartDriveML: Driving Industrial Projects with Affordable ML Solutions, Frameworks and Cloud Choices
 Home-page: UNKNOWN
 Author: Hrishikesh Thakurdesai
 Author-email: hrishikesh.thakurdesai.92@gmail.com
 License: UNKNOWN
 Keywords: python,machine learning,pyspark,cloud
 Platform: UNKNOWN
```

### Comparing `SmartDriveML-0.0.5/SmartDriveML.egg-info/PKG-INFO` & `SmartDriveML-0.0.6/SmartDriveML.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SmartDriveML
-Version: 0.0.5
+Version: 0.0.6
 Summary: SmartDriveML: Driving Industrial Projects with Affordable ML Solutions, Frameworks and Cloud Choices
 Home-page: UNKNOWN
 Author: Hrishikesh Thakurdesai
 Author-email: hrishikesh.thakurdesai.92@gmail.com
 License: UNKNOWN
 Keywords: python,machine learning,pyspark,cloud
 Platform: UNKNOWN
```

### Comparing `SmartDriveML-0.0.5/setup.py` & `SmartDriveML-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'SmartDriveML: Driving Industrial Projects with Affordable ML Solutions, Frameworks and Cloud Choices'
 LONG_DESCRIPTION = 'SmartDriveML is a state-of-the-art Python library created to revolutionize the way industries drive projects using machine learning. This advanced application serves as a comprehensive tool, assisting users in making informed decisions regarding cloud service providers, framework selection, and project feasibility, all while maintaining a cost-effective approach. One of the core functionalities of SmartDriveML is its ability to compare costs among various cloud service providers. By leveraging its integrated algorithms and extensive data on cloud service pricing, this tool enables users to evaluate the financial implications of different providers such as AWS or Azure. With this crucial information at their disposal, industries can optimize their budget allocation, ensuring that their machine learning projects remain economically viable. Another essential feature of SmartDriveML is its framework analysis capability. The library provides comprehensive insights into popular frameworks like Pandas and PySpark, aiding users in choosing the most suitable option for their specific project requirements. By considering factors such as data volume, computational needs, and ease of implementation, SmartDriveML helps industries make informed decisions that align with their objectives and resource constraints. Moreover, SmartDriveML goes beyond cost and framework analysis by providing essential functions for exploratory data analysis and executing fundamental machine learning algorithms on sample datasets. These functions enable users to assess the potential of their projects, allowing them to evaluate whether machine learning can effectively drive their initiatives. By providing this accessible yet powerful toolset, SmartDriveML empowers industries to make data-driven decisions and confidently embark on machine learning-driven projects.'
 
 # Setting up
 setup(
     name="SmartDriveML",
     version=VERSION,
```


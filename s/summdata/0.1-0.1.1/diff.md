# Comparing `tmp/summdata-0.1.tar.gz` & `tmp/summdata-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "summdata-0.1.tar", last modified: Tue May  9 16:18:30 2023, max compression
+gzip compressed data, was "summdata-0.1.1.tar", last modified: Fri Jun 23 18:57:34 2023, max compression
```

## Comparing `summdata-0.1.tar` & `summdata-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 isabellevea   (501) staff       (20)        0 2023-05-09 16:18:30.160219 summdata-0.1/
--rw-r--r--   0 isabellevea   (501) staff       (20)       78 2023-05-09 16:18:30.159972 summdata-0.1/PKG-INFO
--rw-r--r--   0 isabellevea   (501) staff       (20)       38 2023-05-09 16:18:30.160288 summdata-0.1/setup.cfg
--rw-r--r--   0 isabellevea   (501) staff       (20)      164 2023-05-09 16:17:23.000000 summdata-0.1/setup.py
-drwxr-xr-x   0 isabellevea   (501) staff       (20)        0 2023-05-09 16:18:30.158683 summdata-0.1/summdata/
--rw-r--r--   0 isabellevea   (501) staff       (20)     2362 2023-05-09 16:17:23.000000 summdata-0.1/summdata/SummaryContinuous.py
--rw-r--r--   0 isabellevea   (501) staff       (20)     1046 2023-05-05 17:55:12.000000 summdata-0.1/summdata/SummaryStatistics.py
--rw-r--r--   0 isabellevea   (501) staff       (20)       42 2023-05-04 16:44:09.000000 summdata-0.1/summdata/__init__.py
--rw-r--r--   0 isabellevea   (501) staff       (20)        0 2023-05-09 16:17:23.000000 summdata-0.1/summdata/example.py
-drwxr-xr-x   0 isabellevea   (501) staff       (20)        0 2023-05-09 16:18:30.159748 summdata-0.1/summdata.egg-info/
--rw-r--r--   0 isabellevea   (501) staff       (20)       78 2023-05-09 16:18:30.000000 summdata-0.1/summdata.egg-info/PKG-INFO
--rw-r--r--   0 isabellevea   (501) staff       (20)      268 2023-05-09 16:18:30.000000 summdata-0.1/summdata.egg-info/SOURCES.txt
--rw-r--r--   0 isabellevea   (501) staff       (20)        1 2023-05-09 16:18:30.000000 summdata-0.1/summdata.egg-info/dependency_links.txt
--rw-r--r--   0 isabellevea   (501) staff       (20)        1 2023-05-04 16:52:52.000000 summdata-0.1/summdata.egg-info/not-zip-safe
--rw-r--r--   0 isabellevea   (501) staff       (20)        9 2023-05-09 16:18:30.000000 summdata-0.1/summdata.egg-info/top_level.txt
+drwxr-xr-x   0 isabellevea   (501) staff       (20)        0 2023-06-23 18:57:34.096847 summdata-0.1.1/
+-rw-r--r--   0 isabellevea   (501) staff       (20)      145 2023-06-23 18:57:34.096629 summdata-0.1.1/PKG-INFO
+-rw-r--r--   0 isabellevea   (501) staff       (20)     1969 2023-06-23 18:56:17.000000 summdata-0.1.1/README.md
+-rw-r--r--   0 isabellevea   (501) staff       (20)       38 2023-06-23 18:57:34.096907 summdata-0.1.1/setup.cfg
+-rw-r--r--   0 isabellevea   (501) staff       (20)      247 2023-06-23 18:53:17.000000 summdata-0.1.1/setup.py
+drwxr-xr-x   0 isabellevea   (501) staff       (20)        0 2023-06-23 18:57:34.095217 summdata-0.1.1/summdata/
+-rw-r--r--   0 isabellevea   (501) staff       (20)     2324 2023-06-23 18:41:13.000000 summdata-0.1.1/summdata/SummaryContinuous.py
+-rw-r--r--   0 isabellevea   (501) staff       (20)     1046 2023-05-05 17:55:12.000000 summdata-0.1.1/summdata/SummaryStatistics.py
+-rw-r--r--   0 isabellevea   (501) staff       (20)       42 2023-05-04 16:44:09.000000 summdata-0.1.1/summdata/__init__.py
+-rw-r--r--   0 isabellevea   (501) staff       (20)      376 2023-05-09 17:49:34.000000 summdata-0.1.1/summdata/example.py
+drwxr-xr-x   0 isabellevea   (501) staff       (20)        0 2023-06-23 18:57:34.096379 summdata-0.1.1/summdata.egg-info/
+-rw-r--r--   0 isabellevea   (501) staff       (20)      145 2023-06-23 18:57:34.000000 summdata-0.1.1/summdata.egg-info/PKG-INFO
+-rw-r--r--   0 isabellevea   (501) staff       (20)      278 2023-06-23 18:57:34.000000 summdata-0.1.1/summdata.egg-info/SOURCES.txt
+-rw-r--r--   0 isabellevea   (501) staff       (20)        1 2023-06-23 18:57:34.000000 summdata-0.1.1/summdata.egg-info/dependency_links.txt
+-rw-r--r--   0 isabellevea   (501) staff       (20)        1 2023-05-04 16:52:52.000000 summdata-0.1.1/summdata.egg-info/not-zip-safe
+-rw-r--r--   0 isabellevea   (501) staff       (20)        9 2023-06-23 18:57:34.000000 summdata-0.1.1/summdata.egg-info/top_level.txt
```

### Comparing `summdata-0.1/summdata/SummaryContinuous.py` & `summdata-0.1.1/summdata/SummaryContinuous.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,16 @@
 import math
 import matplotlib.pyplot as plt
 from collections import Counter
 from .SummaryStatistics import SummaryStatistics
 
 
 class Continuous(SummaryStatistics):
-	"""What does this function do
-
-
-	Attributes:
 	
 
-
-
-	"""
-
 	def __init__(self, mu =0, sigma =1):
 		SummaryStatistics.__init__(self, mu, sigma)
 
 	def show_length(self):
 		""" This function returns the length of the data set
 
 		Args: 
@@ -91,24 +83,24 @@
 			None
 		
 		Returns: 
 			float: mode of the data presented as a list
 	
 		"""
 					
-		uniq_values = []
-		mode_values = []
+		counter = 0
+		num = self.data[0]
+
 		for i in self.data:
-			if i not in uniq_values:
-				uniq_values.append(i)
-			else:
-				mode_values.append(i)
-		self.mode = set(mode_values)
-		
+			current_frequency = self.data.count(i)
+			if (current_frequency > counter):
+				counter = current_frequency
+				num = i
 
+		self.mode = num
 
 		return self.mode
 
 
 
 	def calculate_stdev(self, sample=True):
```

### Comparing `summdata-0.1/summdata/SummaryStatistics.py` & `summdata-0.1.1/summdata/SummaryStatistics.py`

 * *Files identical despite different names*


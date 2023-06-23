# Comparing `tmp/pp_project_pkg-1.0.202306201419-py3-none-any.whl.zip` & `tmp/pp_project_pkg-1.0.202306231241-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 10488 bytes, number of entries: 13
--rw-rw-r--  2.0 unx       71 b- defN 23-Jun-06 14:15 pp_project_pkg/__init__.py
--rw-rw-r--  2.0 unx     4766 b- defN 23-Jun-20 12:40 pp_project_pkg/linear_train.py
--rw-rw-r--  2.0 unx      577 b- defN 23-Jun-06 14:14 pp_project_pkg/newsvendor.py
--rw-rw-r--  2.0 unx     7115 b- defN 23-Jun-06 15:26 pp_project_pkg/pp_tables.py
--rw-rw-r--  2.0 unx     6657 b- defN 23-Jun-20 14:19 pp_project_pkg/utils.py
--rw-rw-r--  2.0 unx      396 b- defN 23-Jun-20 14:19 pp_project_pkg/version.py
--rw-rw-r--  2.0 unx     4602 b- defN 23-Jun-20 09:33 pp_project_pkg/wrangling.py
--rwxrwxr-x  2.0 unx       65 b- defN 23-Jun-06 09:53 pp_project_pkg-1.0.202306201419.data/scripts/get_tables.py
--rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-06 15:48 pp_project_pkg-1.0.202306201419.data/scripts/pp_project_run.py
--rw-rw-r--  2.0 unx      191 b- defN 23-Jun-20 14:19 pp_project_pkg-1.0.202306201419.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-20 14:19 pp_project_pkg-1.0.202306201419.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-20 14:19 pp_project_pkg-1.0.202306201419.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1182 b- defN 23-Jun-20 14:19 pp_project_pkg-1.0.202306201419.dist-info/RECORD
-13 files, 27045 bytes uncompressed, 8466 bytes compressed:  68.7%
+Zip file size: 10665 bytes, number of entries: 13
+-rw-rw-r--  2.0 unx       71 b- defN 23-Jun-07 11:24 pp_project_pkg/__init__.py
+-rw-rw-r--  2.0 unx     5335 b- defN 23-Jun-23 12:39 pp_project_pkg/linear_train.py
+-rw-rw-r--  2.0 unx      577 b- defN 23-Jun-07 11:24 pp_project_pkg/newsvendor.py
+-rw-rw-r--  2.0 unx     7115 b- defN 23-Jun-07 11:24 pp_project_pkg/pp_tables.py
+-rw-rw-r--  2.0 unx     6657 b- defN 23-Jun-23 12:39 pp_project_pkg/utils.py
+-rw-rw-r--  2.0 unx      396 b- defN 23-Jun-23 12:41 pp_project_pkg/version.py
+-rw-rw-r--  2.0 unx     4602 b- defN 23-Jun-18 22:21 pp_project_pkg/wrangling.py
+-rwxrwxr-x  2.0 unx       65 b- defN 23-Jun-02 12:43 pp_project_pkg-1.0.202306231241.data/scripts/get_tables.py
+-rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-07 11:24 pp_project_pkg-1.0.202306231241.data/scripts/pp_project_run.py
+-rw-rw-r--  2.0 unx      191 b- defN 23-Jun-23 12:41 pp_project_pkg-1.0.202306231241.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-23 12:41 pp_project_pkg-1.0.202306231241.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-Jun-23 12:41 pp_project_pkg-1.0.202306231241.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1182 b- defN 23-Jun-23 12:41 pp_project_pkg-1.0.202306231241.dist-info/RECORD
+13 files, 27614 bytes uncompressed, 8643 bytes compressed:  68.7%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: pp_project_pkg/version.py
 Comment: 
 
 Filename: pp_project_pkg/wrangling.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306201419.data/scripts/get_tables.py
+Filename: pp_project_pkg-1.0.202306231241.data/scripts/get_tables.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306201419.data/scripts/pp_project_run.py
+Filename: pp_project_pkg-1.0.202306231241.data/scripts/pp_project_run.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306201419.dist-info/METADATA
+Filename: pp_project_pkg-1.0.202306231241.dist-info/METADATA
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306201419.dist-info/WHEEL
+Filename: pp_project_pkg-1.0.202306231241.dist-info/WHEEL
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306201419.dist-info/top_level.txt
+Filename: pp_project_pkg-1.0.202306231241.dist-info/top_level.txt
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306201419.dist-info/RECORD
+Filename: pp_project_pkg-1.0.202306231241.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pp_project_pkg/linear_train.py

```diff
@@ -140,8 +140,31 @@
     # Explore results
     plt.scatter(y_test, y_pred)
     plt.plot([y_test.min(), y_test.max()], [y_pred.min(), y_pred.max()], '--r')
     plt.xlabel('Actual')
     plt.ylabel('Predicted')
     plt.show()
 
-    
+    
+def outliers(data,threshold_val=2.0):
+    """
+    Detect outliers in the file
+    
+    Args:
+        data: pd.DataFrame
+        threshold_val: float
+    Returns:
+        pd.DataFrame
+    """
+    
+    avg_events = data['events'].mean()
+    
+    # Calculate the range of events
+    range_events = data['events'].max() - data['events'].min()
+
+    # Define a threshold value for outliers
+    threshold = threshold_val * range_events
+
+    # Identify the outliers based on the threshold value
+    outliers = data[data['events'] > avg_events + threshold]
+
+    return outliers
```

## pp_project_pkg/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('06')
-VERSION_DAY = int('20')
-VERSION_HOUR = int('14')
-VERSION_MINUTE = int('19')
+VERSION_DAY = int('23')
+VERSION_HOUR = int('12')
+VERSION_MINUTE = int('41')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202306201419
-version_date = '2023/06/20 14:19'
+PATCH_VERSION = 202306231241
+version_date = '2023/06/23 12:41'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `pp_project_pkg-1.0.202306201419.data/scripts/pp_project_run.py` & `pp_project_pkg-1.0.202306231241.data/scripts/pp_project_run.py`

 * *Files identical despite different names*


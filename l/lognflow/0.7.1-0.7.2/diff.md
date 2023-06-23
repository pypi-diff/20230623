# Comparing `tmp/lognflow-0.7.1.tar.gz` & `tmp/lognflow-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lognflow-0.7.1.tar", last modified: Mon May 22 04:55:54 2023, max compression
+gzip compressed data, was "lognflow-0.7.2.tar", last modified: Thu May 25 02:20:05 2023, max compression
```

## Comparing `lognflow-0.7.1.tar` & `lognflow-0.7.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 04:55:54.878346 lognflow-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-22 04:55:41.000000 lognflow-0.7.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-22 04:55:41.000000 lognflow-0.7.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-22 04:55:41.000000 lognflow-0.7.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-22 04:55:41.000000 lognflow-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-22 04:55:41.000000 lognflow-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-05-22 04:55:54.878346 lognflow-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-22 04:55:41.000000 lognflow-0.7.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 04:55:54.874346 lognflow-0.7.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-22 04:55:41.000000 lognflow-0.7.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-22 04:55:41.000000 lognflow-0.7.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-22 04:55:41.000000 lognflow-0.7.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-22 04:55:41.000000 lognflow-0.7.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-22 04:55:41.000000 lognflow-0.7.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-22 04:55:41.000000 lognflow-0.7.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-22 04:55:41.000000 lognflow-0.7.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-22 04:55:41.000000 lognflow-0.7.1/docs/lognflow.rst
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-22 04:55:41.000000 lognflow-0.7.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-22 04:55:41.000000 lognflow-0.7.1/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-22 04:55:41.000000 lognflow-0.7.1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 04:55:54.874346 lognflow-0.7.1/lognflow/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-22 04:55:41.000000 lognflow-0.7.1/lognflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    65386 2023-05-22 04:55:41.000000 lognflow-0.7.1/lognflow/lognflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    11869 2023-05-22 04:55:41.000000 lognflow-0.7.1/lognflow/logviewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-05-22 04:55:41.000000 lognflow-0.7.1/lognflow/printprogress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 04:55:54.878346 lognflow-0.7.1/lognflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-05-22 04:55:54.000000 lognflow-0.7.1/lognflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-22 04:55:54.000000 lognflow-0.7.1/lognflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 04:55:54.000000 lognflow-0.7.1/lognflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 04:55:54.000000 lognflow-0.7.1/lognflow.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-22 04:55:54.000000 lognflow-0.7.1/lognflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-22 04:55:54.000000 lognflow-0.7.1/lognflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-22 04:55:54.878346 lognflow-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-22 04:55:41.000000 lognflow-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 04:55:54.878346 lognflow-0.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-22 04:55:41.000000 lognflow-0.7.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9634 2023-05-22 04:55:42.000000 lognflow-0.7.1/tests/test_lognflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-22 04:55:42.000000 lognflow-0.7.1/tests/test_logviewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-22 04:55:42.000000 lognflow-0.7.1/tests/test_printprogress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:20:05.383602 lognflow-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-25 02:19:51.000000 lognflow-0.7.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-25 02:19:51.000000 lognflow-0.7.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-05-25 02:19:51.000000 lognflow-0.7.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-25 02:19:51.000000 lognflow-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-25 02:19:51.000000 lognflow-0.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-05-25 02:20:05.383602 lognflow-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-25 02:19:51.000000 lognflow-0.7.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:20:05.383602 lognflow-0.7.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-25 02:19:51.000000 lognflow-0.7.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-25 02:19:51.000000 lognflow-0.7.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-25 02:19:51.000000 lognflow-0.7.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-25 02:19:51.000000 lognflow-0.7.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-25 02:19:51.000000 lognflow-0.7.2/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-25 02:19:51.000000 lognflow-0.7.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-25 02:19:51.000000 lognflow-0.7.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-25 02:19:51.000000 lognflow-0.7.2/docs/lognflow.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-25 02:19:51.000000 lognflow-0.7.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-25 02:19:51.000000 lognflow-0.7.2/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-25 02:19:51.000000 lognflow-0.7.2/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:20:05.383602 lognflow-0.7.2/lognflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-25 02:19:51.000000 lognflow-0.7.2/lognflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65386 2023-05-25 02:19:51.000000 lognflow-0.7.2/lognflow/lognflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13651 2023-05-25 02:19:51.000000 lognflow-0.7.2/lognflow/logviewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-05-25 02:19:51.000000 lognflow-0.7.2/lognflow/printprogress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:20:05.383602 lognflow-0.7.2/lognflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-05-25 02:20:05.000000 lognflow-0.7.2/lognflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-25 02:20:05.000000 lognflow-0.7.2/lognflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 02:20:05.000000 lognflow-0.7.2/lognflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 02:20:05.000000 lognflow-0.7.2/lognflow.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-25 02:20:05.000000 lognflow-0.7.2/lognflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 02:20:05.000000 lognflow-0.7.2/lognflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-25 02:20:05.383602 lognflow-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-25 02:19:51.000000 lognflow-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 02:20:05.383602 lognflow-0.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-25 02:19:51.000000 lognflow-0.7.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9634 2023-05-25 02:19:51.000000 lognflow-0.7.2/tests/test_lognflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-05-25 02:19:51.000000 lognflow-0.7.2/tests/test_logviewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-25 02:19:51.000000 lognflow-0.7.2/tests/test_printprogress.py
```

### Comparing `lognflow-0.7.1/CONTRIBUTING.rst` & `lognflow-0.7.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.1/HISTORY.rst` & `lognflow-0.7.2/HISTORY.rst`

 * *Files 14% similar despite different names*

```diff
@@ -84,8 +84,14 @@
 ------------------
 * logviewer returns data by log_sigle if the full name is mentioned.
 
 0.7.1 (2023-05-22)
 ------------------
 * printprogress supports lognflow.
 * bugs fixed in lognflow.
-* For now I guess lognflow and logviewer could be separate.
+* For now I guess lognflow and logviewer could be separate.
+
+0.7.2 (2023-05-25)
+------------------
+* bug fixed in logviewer
+* text_to_object added to logviewer to read dict or list logged via log_single
+* test pass for logviewer including the test for text_to_object
```

### Comparing `lognflow-0.7.1/LICENSE` & `lognflow-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.1/PKG-INFO` & `lognflow-0.7.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lognflow
-Version: 0.7.1
+Version: 0.7.2
 Summary: Log and Flow tracking made easy with Python
 Home-page: https://github.com/arsadri/lognflow
 Author: Alireza Sadri
 Author-email: arsadri@gmail.com
 License: GNU General Public License v3
 Keywords: lognflow
 Classifier: Development Status :: 3 - Alpha
@@ -177,7 +177,13 @@
 * logviewer returns data by log_sigle if the full name is mentioned.
 
 0.7.1 (2023-05-22)
 ------------------
 * printprogress supports lognflow.
 * bugs fixed in lognflow.
 * For now I guess lognflow and logviewer could be separate.
+
+0.7.2 (2023-05-25)
+------------------
+* bug fixed in logviewer
+* text_to_object added to logviewer to read dict or list logged via log_single
+* test pass for logviewer including the test for text_to_object
```

### Comparing `lognflow-0.7.1/README.rst` & `lognflow-0.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.1/docs/Makefile` & `lognflow-0.7.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.1/docs/conf.py` & `lognflow-0.7.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.1/docs/installation.rst` & `lognflow-0.7.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.1/docs/make.bat` & `lognflow-0.7.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.1/lognflow/lognflow.py` & `lognflow-0.7.2/lognflow/lognflow.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.1/lognflow/logviewer.py` & `lognflow-0.7.2/lognflow/logviewer.py`

 * *Files 10% similar despite different names*

```diff
@@ -218,14 +218,20 @@
             else:
                 var_fname = var_dir.name
                 var_dir = var_dir.parent
                 patt = f'{var_fname}*.{suffix}'
                 while('**' in patt):
                     patt = patt.replace('**', '*')
                 flist = list(var_dir.glob(patt))
+        else:
+            var_dir = flist[0].parent
+            assert var_dir.is_dir(),\
+                f'The directory {var_dir} for the '\
+                + 'provided list cannot be accessed.'
+            
         if flist:
             flist.sort()
             n_files = len(flist)
             if((not return_data) & return_flist):
                 return(flist)
             
             ######### asked for data ########
@@ -235,28 +241,28 @@
                     read_func = np.load
                 except:
                     pass
             if(read_func is None):
                 try:
                     from matplotlib.pyplot import imread
                     fdata = imread(flist[0])
-                    read_func = plt.imread
+                    read_func = imread
                 except:
                     pass
             if(read_func is not None):
                 assert callable(read_func), \
                     f'given read_func: {read_func} is not callable.'
                 fdata = read_func(flist[0])
                 dataset = np.zeros((n_files, ) + fdata.shape, 
                                    dtype=fdata.dtype)
-                for fcnt, fpath in enumerate(flist):
-                    dataset[fcnt] = read_func(fpath)
                 if(verbose):
                     self.logger(f'logviewer: Reading dataset from {var_dir}'
                                 f', the shape would be: {dataset.shape}')
+                for fcnt, fpath in enumerate(flist):
+                    dataset[fcnt] = read_func(fpath)
                 if(return_flist):
                     return(dataset, flist)
                 else:
                     return(dataset)
             else:
                 if(verbose):
                     self.logger(f'File {flist[0].name} cannot be opened by '\
@@ -301,7 +307,50 @@
         return(flist_A_new, flist_B_new)
     
     def __repr__(self):
         return f'{self.log_dir}'
 
     def __bool__(self):
         return self.log_dir.is_dir()
+
+def str2type(_element):
+    if _element[0] == '\'':
+        return _element[1:-1]
+    else:
+        try:
+            return int(_element)
+        except ValueError:
+            try:
+                return float(_element)
+            except ValueError:
+                pass
+    return _element
+
+def text_to_object(txt):
+    """ Read a list or dict that was sent to write to text e.g. via log_single:
+    As you may have tried, it is possible to send a Pythonic list to a text file
+    the list will be typed there with [ and ] and ' and ' for strings with ', '
+    in between. In this function we will merely return the actual content
+    of the original list.
+    Now if the type the element of the list was string, it would put ' and ' in
+    the text file. But if it is a number, no kind of punctuation or sign is 
+    used. by write(). We support int or float. Otherwise the written text
+    will be returned as string with any other wierd things attached to it.
+    
+    """
+    if(txt[0] == '['):
+        txt = txt.strip('[').strip(']')
+        txt = txt.split(', ')
+        obj_out = txt
+        for cnt, _element in enumerate(txt):
+            obj_out[cnt] = str2type(_element)
+    elif(txt[0] == '{'):
+        txt = txt.strip('{').strip('}')
+        txt = txt.split(', ')
+        obj_out = dict()
+        for cnt, _element in enumerate(txt):
+            _element_key = str2type(_element.split(': ')[0])
+            _element_value = str2type(_element.split(': ')[1])
+            obj_out[_element_key] = _element_value
+    else:
+        obj_out = txt
+    return obj_out
```

### Comparing `lognflow-0.7.1/lognflow/printprogress.py` & `lognflow-0.7.2/lognflow/printprogress.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.1/lognflow.egg-info/PKG-INFO` & `lognflow-0.7.2/lognflow.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lognflow
-Version: 0.7.1
+Version: 0.7.2
 Summary: Log and Flow tracking made easy with Python
 Home-page: https://github.com/arsadri/lognflow
 Author: Alireza Sadri
 Author-email: arsadri@gmail.com
 License: GNU General Public License v3
 Keywords: lognflow
 Classifier: Development Status :: 3 - Alpha
@@ -177,7 +177,13 @@
 * logviewer returns data by log_sigle if the full name is mentioned.
 
 0.7.1 (2023-05-22)
 ------------------
 * printprogress supports lognflow.
 * bugs fixed in lognflow.
 * For now I guess lognflow and logviewer could be separate.
+
+0.7.2 (2023-05-25)
+------------------
+* bug fixed in logviewer
+* text_to_object added to logviewer to read dict or list logged via log_single
+* test pass for logviewer including the test for text_to_object
```

### Comparing `lognflow-0.7.1/lognflow.egg-info/SOURCES.txt` & `lognflow-0.7.2/lognflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.1/setup.py` & `lognflow-0.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """The setup script for lognflow."""
 
 from setuptools import setup, find_packages
 
 __author__ = 'Alireza Sadri'
 __email__ = 'arsadri@gmail.com'
-__version__ = '0.7.1'
+__version__ = '0.7.2'
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
```

### Comparing `lognflow-0.7.1/tests/test_lognflow.py` & `lognflow-0.7.2/tests/test_lognflow.py`

 * *Files identical despite different names*

### Comparing `lognflow-0.7.1/tests/test_logviewer.py` & `lognflow-0.7.2/tests/test_logviewer.py`

 * *Files 23% similar despite different names*

```diff
@@ -75,16 +75,18 @@
 
     flist_A_AB, flist_B_AB = logged.get_common_files('A/', 'B/')
     logger(flist_A_AB)
     logger(flist_B_AB)
     
     if(flist_A_AB):
         
-        dataset_A = logged.get_stack_of_files(flist = flist_A_AB, return_data = True, return_flist = False)
-        dataset_B = logged.get_stack_of_files(flist = flist_B_AB, return_data = True, return_flist = False)
+        dataset_A = logged.get_stack_of_files('A/',
+            flist = flist_A_AB, return_data = True, return_flist = False)
+        dataset_B = logged.get_stack_of_files('B/',
+            flist = flist_B_AB, return_data = True, return_flist = False)
         
         logger.log_canvas('data_samples', [dataset_A, dataset_B], dpi = 300)
         _ = logger._loggers_dict['main_log'].log_size
         logger('Size of the log file in bytes is: ' \
                + f'{_}')
 
 def test_replace_time_with_index():
@@ -108,12 +110,38 @@
         'test_param', return_data=True, return_flist=True)
     
     logger(flist)
     
     logger(data_in)
     logger(data_out)
 
+def test_text_to_object():
+    from lognflow.logviewer import text_to_object
+    
+    logger = lognflow(temp_dir, time_tag = False)
+    test_list = ['asdf', 1243, "dd"]
+    logger.log_single('test_list', test_list, save_as = 'txt')
+    
+    test_dict = {"one": "asdf", 'two': 1243, 'thre': "dd"}
+    logger.log_single('test_dict', test_dict, save_as = 'txt')
+    
+    logged = logviewer(logger.log_dir)
+    flist = logged.get_stack_of_files('*')
+    print(flist)
+    for file_name_input in flist:
+        print('='*60)
+        print(f'file name: {file_name_input}')
+        with open(file_name_input, 'r') as opened_txt:
+            txt = opened_txt.read()
+        print('text read from the file:')
+        print(txt)
+        print('- '*30)
+        ext_obj = text_to_object(txt)
+        print(f'Extracted object is of type {type(ext_obj)}:')
+        print(ext_obj)
+
 if __name__ == '__main__':
     temp_dir = select_directory()
     test_get_images_as_stack()
     test_replace_time_with_index()
-    test_logviewer()
+    test_logviewer()
+    test_text_to_object()
```

### Comparing `lognflow-0.7.1/tests/test_printprogress.py` & `lognflow-0.7.2/tests/test_printprogress.py`

 * *Files identical despite different names*


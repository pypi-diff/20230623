# Comparing `tmp/urturn-0.1.3.tar.gz` & `tmp/urturn-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "urturn-0.1.3.tar", last modified: Mon May 22 20:07:09 2023, max compression
+gzip compressed data, was "urturn-0.1.4.tar", last modified: Fri Jun 23 18:14:41 2023, max compression
```

## Comparing `urturn-0.1.3.tar` & `urturn-0.1.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:07:09.224119 urturn-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-22 20:06:57.000000 urturn-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-22 20:07:09.224119 urturn-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-22 20:06:57.000000 urturn-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 20:07:09.224119 urturn-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-22 20:06:57.000000 urturn-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:07:09.220119 urturn-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-05-22 20:06:57.000000 urturn-0.1.3/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-05-22 20:06:57.000000 urturn-0.1.3/tests/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-22 20:06:57.000000 urturn-0.1.3/tests/test_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-22 20:06:57.000000 urturn-0.1.3/tests/test_webapp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:07:09.220119 urturn-0.1.3/urturn/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-22 20:07:09.000000 urturn-0.1.3/urturn/REQUIREMENTS
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-22 20:07:09.000000 urturn-0.1.3/urturn/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 20:06:57.000000 urturn-0.1.3/urturn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-05-22 20:06:57.000000 urturn-0.1.3/urturn/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-05-22 20:06:57.000000 urturn-0.1.3/urturn/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:07:09.224119 urturn-0.1.3/urturn/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-05-22 20:06:57.000000 urturn-0.1.3/urturn/templates/adapted.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-22 20:06:57.000000 urturn-0.1.3/urturn/templates/details.css
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-22 20:06:57.000000 urturn-0.1.3/urturn/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-22 20:06:57.000000 urturn-0.1.3/urturn/templates/job_config.html
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-22 20:06:57.000000 urturn-0.1.3/urturn/trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-05-22 20:06:57.000000 urturn-0.1.3/urturn/webapp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 20:07:09.220119 urturn-0.1.3/urturn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-22 20:07:09.000000 urturn-0.1.3/urturn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-22 20:07:09.000000 urturn-0.1.3/urturn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 20:07:09.000000 urturn-0.1.3/urturn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-22 20:07:09.000000 urturn-0.1.3/urturn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-22 20:07:09.000000 urturn-0.1.3/urturn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:14:41.891628 urturn-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-23 18:14:30.000000 urturn-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-23 18:14:41.891628 urturn-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-23 18:14:30.000000 urturn-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 18:14:41.891628 urturn-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-23 18:14:30.000000 urturn-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:14:41.887628 urturn-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-06-23 18:14:30.000000 urturn-0.1.4/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-06-23 18:14:30.000000 urturn-0.1.4/tests/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-23 18:14:30.000000 urturn-0.1.4/tests/test_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-23 18:14:30.000000 urturn-0.1.4/tests/test_webapp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:14:41.887628 urturn-0.1.4/urturn/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-23 18:14:41.000000 urturn-0.1.4/urturn/REQUIREMENTS
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-23 18:14:41.000000 urturn-0.1.4/urturn/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 18:14:30.000000 urturn-0.1.4/urturn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-06-23 18:14:30.000000 urturn-0.1.4/urturn/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-06-23 18:14:30.000000 urturn-0.1.4/urturn/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:14:41.891628 urturn-0.1.4/urturn/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-06-23 18:14:30.000000 urturn-0.1.4/urturn/templates/adapted.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-23 18:14:30.000000 urturn-0.1.4/urturn/templates/details.css
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-23 18:14:30.000000 urturn-0.1.4/urturn/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-23 18:14:30.000000 urturn-0.1.4/urturn/templates/job_config.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-06-23 18:14:30.000000 urturn-0.1.4/urturn/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-06-23 18:14:30.000000 urturn-0.1.4/urturn/webapp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:14:41.891628 urturn-0.1.4/urturn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-23 18:14:41.000000 urturn-0.1.4/urturn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-23 18:14:41.000000 urturn-0.1.4/urturn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 18:14:41.000000 urturn-0.1.4/urturn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-23 18:14:41.000000 urturn-0.1.4/urturn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 18:14:41.000000 urturn-0.1.4/urturn.egg-info/top_level.txt
```

### Comparing `urturn-0.1.3/LICENSE` & `urturn-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `urturn-0.1.3/setup.py` & `urturn-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `urturn-0.1.3/tests/test_job.py` & `urturn-0.1.4/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `urturn-0.1.3/tests/test_scheduler.py` & `urturn-0.1.4/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `urturn-0.1.3/tests/test_trigger.py` & `urturn-0.1.4/tests/test_trigger.py`

 * *Files identical despite different names*

### Comparing `urturn-0.1.3/tests/test_webapp.py` & `urturn-0.1.4/tests/test_webapp.py`

 * *Files identical despite different names*

### Comparing `urturn-0.1.3/urturn/job.py` & `urturn-0.1.4/urturn/job.py`

 * *Files identical despite different names*

### Comparing `urturn-0.1.3/urturn/scheduler.py` & `urturn-0.1.4/urturn/scheduler.py`

 * *Files identical despite different names*

### Comparing `urturn-0.1.3/urturn/templates/adapted.min.css` & `urturn-0.1.4/urturn/templates/adapted.min.css`

 * *Files identical despite different names*

### Comparing `urturn-0.1.3/urturn/templates/details.css` & `urturn-0.1.4/urturn/templates/details.css`

 * *Files identical despite different names*

### Comparing `urturn-0.1.3/urturn/templates/index.html` & `urturn-0.1.4/urturn/templates/index.html`

 * *Files identical despite different names*

### Comparing `urturn-0.1.3/urturn/templates/job_config.html` & `urturn-0.1.4/urturn/templates/job_config.html`

 * *Files identical despite different names*

### Comparing `urturn-0.1.3/urturn/trigger.py` & `urturn-0.1.4/urturn/trigger.py`

 * *Files identical despite different names*

### Comparing `urturn-0.1.3/urturn/webapp.py` & `urturn-0.1.4/urturn/webapp.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,11 +85,10 @@
 
         Args:
             debug (bool, optional): Run the web application in debug mode. Defaults to False.
         """
 
         # Start the scheduler in a separate thread
         scheduler_thread = Thread(target=self.scheduler.start)
-        scheduler_thread.daemon = True
         scheduler_thread.start()
 
         self.app.run(host=host, port=port, debug=debug, use_reloader=False)
```


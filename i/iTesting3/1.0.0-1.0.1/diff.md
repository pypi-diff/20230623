# Comparing `tmp/iTesting3-1.0.0.tar.gz` & `tmp/iTesting3-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iTesting3-1.0.0.tar", last modified: Fri Jun 23 18:18:38 2023, max compression
+gzip compressed data, was "iTesting3-1.0.1.tar", last modified: Fri Jun 23 18:21:50 2023, max compression
```

## Comparing `iTesting3-1.0.0.tar` & `iTesting3-1.0.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 18:18:37.995382 iTesting3-1.0.0/
--rw-rw-rw-   0        0        0      882 2023-06-23 18:18:37.995382 iTesting3-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      445 2023-06-23 12:46:05.000000 iTesting3-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 18:18:37.965417 iTesting3-1.0.0/common/
--rw-rw-rw-   0        0        0        0 2023-06-23 12:46:05.000000 iTesting3-1.0.0/common/__init__.py
--rw-rw-rw-   0        0        0      256 2023-06-23 12:46:05.000000 iTesting3-1.0.0/common/customize_error.py
--rw-rw-rw-   0        0        0      448 2023-06-23 12:46:05.000000 iTesting3-1.0.0/common/data_provider.py
--rw-rw-rw-   0        0        0    37242 2023-06-23 12:46:05.000000 iTesting3-1.0.0/common/html_reporter.py
--rw-rw-rw-   0        0        0     2720 2023-06-23 12:46:05.000000 iTesting3-1.0.0/common/my_logger.py
--rw-rw-rw-   0        0        0     4301 2023-06-23 12:46:05.000000 iTesting3-1.0.0/common/test_case_finder.py
--rw-rw-rw-   0        0        0      757 2023-06-23 12:46:05.000000 iTesting3-1.0.0/common/test_decorator.py
--rw-rw-rw-   0        0        0     1678 2023-06-23 12:46:05.000000 iTesting3-1.0.0/common/test_filter.py
--rw-rw-rw-   0        0        0     3356 2023-06-23 12:46:05.000000 iTesting3-1.0.0/common/user_options.py
-drwxrwxrwx   0        0        0        0 2023-06-23 18:18:37.975381 iTesting3-1.0.0/configs/
--rw-rw-rw-   0        0        0        0 2023-06-23 12:46:05.000000 iTesting3-1.0.0/configs/__init__.py
--rw-rw-rw-   0        0        0      259 2023-06-23 12:46:05.000000 iTesting3-1.0.0/configs/global_config.py
-drwxrwxrwx   0        0        0        0 2023-06-23 18:18:37.985383 iTesting3-1.0.0/iTesting3.egg-info/
--rw-rw-rw-   0        0        0      882 2023-06-23 18:18:37.000000 iTesting3-1.0.0/iTesting3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      552 2023-06-23 18:18:37.000000 iTesting3-1.0.0/iTesting3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 18:18:37.000000 iTesting3-1.0.0/iTesting3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-06-23 18:18:37.000000 iTesting3-1.0.0/iTesting3.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-06-23 18:18:37.000000 iTesting3-1.0.0/iTesting3.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       18 2023-06-23 18:18:37.000000 iTesting3-1.0.0/iTesting3.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-06-23 18:18:37.000000 iTesting3-1.0.0/iTesting3.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 18:18:37.995382 iTesting3-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1245 2023-06-23 18:17:29.000000 iTesting3-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-23 18:18:37.995382 iTesting3-1.0.0/utilities/
--rw-rw-rw-   0        0        0        0 2023-06-23 12:46:05.000000 iTesting3-1.0.0/utilities/__init__.py
--rw-rw-rw-   0        0        0      276 2023-06-23 12:46:05.000000 iTesting3-1.0.0/utilities/yaml_helper.py
+drwxrwxrwx   0        0        0        0 2023-06-23 18:21:50.302128 iTesting3-1.0.1/
+-rw-rw-rw-   0        0        0      882 2023-06-23 18:21:50.292085 iTesting3-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      445 2023-06-23 12:46:05.000000 iTesting3-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 18:21:50.221818 iTesting3-1.0.1/common/
+-rw-rw-rw-   0        0        0        0 2023-06-23 12:46:05.000000 iTesting3-1.0.1/common/__init__.py
+-rw-rw-rw-   0        0        0      256 2023-06-23 12:46:05.000000 iTesting3-1.0.1/common/customize_error.py
+-rw-rw-rw-   0        0        0      448 2023-06-23 12:46:05.000000 iTesting3-1.0.1/common/data_provider.py
+-rw-rw-rw-   0        0        0    37242 2023-06-23 12:46:05.000000 iTesting3-1.0.1/common/html_reporter.py
+-rw-rw-rw-   0        0        0     2720 2023-06-23 12:46:05.000000 iTesting3-1.0.1/common/my_logger.py
+-rw-rw-rw-   0        0        0     4301 2023-06-23 12:46:05.000000 iTesting3-1.0.1/common/test_case_finder.py
+-rw-rw-rw-   0        0        0      757 2023-06-23 12:46:05.000000 iTesting3-1.0.1/common/test_decorator.py
+-rw-rw-rw-   0        0        0     1678 2023-06-23 12:46:05.000000 iTesting3-1.0.1/common/test_filter.py
+-rw-rw-rw-   0        0        0     3356 2023-06-23 12:46:05.000000 iTesting3-1.0.1/common/user_options.py
+drwxrwxrwx   0        0        0        0 2023-06-23 18:21:50.231823 iTesting3-1.0.1/configs/
+-rw-rw-rw-   0        0        0        0 2023-06-23 12:46:05.000000 iTesting3-1.0.1/configs/__init__.py
+-rw-rw-rw-   0        0        0      259 2023-06-23 12:46:05.000000 iTesting3-1.0.1/configs/global_config.py
+drwxrwxrwx   0        0        0        0 2023-06-23 18:21:50.251855 iTesting3-1.0.1/iTesting3.egg-info/
+-rw-rw-rw-   0        0        0      882 2023-06-23 18:21:47.000000 iTesting3-1.0.1/iTesting3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      552 2023-06-23 18:21:48.000000 iTesting3-1.0.1/iTesting3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 18:21:47.000000 iTesting3-1.0.1/iTesting3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-06-23 18:21:48.000000 iTesting3-1.0.1/iTesting3.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-23 18:18:37.000000 iTesting3-1.0.1/iTesting3.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       18 2023-06-23 18:21:48.000000 iTesting3-1.0.1/iTesting3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-06-23 18:21:48.000000 iTesting3-1.0.1/iTesting3.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 18:21:50.302128 iTesting3-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1245 2023-06-23 18:21:22.000000 iTesting3-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 18:21:50.261865 iTesting3-1.0.1/utilities/
+-rw-rw-rw-   0        0        0        0 2023-06-23 12:46:05.000000 iTesting3-1.0.1/utilities/__init__.py
+-rw-rw-rw-   0        0        0      276 2023-06-23 12:46:05.000000 iTesting3-1.0.1/utilities/yaml_helper.py
```

### Comparing `iTesting3-1.0.0/PKG-INFO` & `iTesting3-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iTesting3
-Version: 1.0.0
+Version: 1.0.1
 Summary: iTesting is a common test framework support for both UI and API test with run in parallel ability.
 Home-page: https://www.testertalk.com
 Author: Kevin.cai.HPJ
 Author-email: love.i@outlook.com
 License: GPL
 
 此代码库为本人新书 **<从0到1搭建自动化测试框架：原理、实现与工程实践>** 的配套练习框架。本书基于Python编写，学习完本书，您能够完全自主开发自动化测试框架.
```

### Comparing `iTesting3-1.0.0/common/html_reporter.py` & `iTesting3-1.0.1/common/html_reporter.py`

 * *Files identical despite different names*

### Comparing `iTesting3-1.0.0/common/my_logger.py` & `iTesting3-1.0.1/common/my_logger.py`

 * *Files identical despite different names*

### Comparing `iTesting3-1.0.0/common/test_case_finder.py` & `iTesting3-1.0.1/common/test_case_finder.py`

 * *Files identical despite different names*

### Comparing `iTesting3-1.0.0/common/test_decorator.py` & `iTesting3-1.0.1/common/test_decorator.py`

 * *Files identical despite different names*

### Comparing `iTesting3-1.0.0/common/test_filter.py` & `iTesting3-1.0.1/common/test_filter.py`

 * *Files identical despite different names*

### Comparing `iTesting3-1.0.0/common/user_options.py` & `iTesting3-1.0.1/common/user_options.py`

 * *Files identical despite different names*

### Comparing `iTesting3-1.0.0/iTesting3.egg-info/PKG-INFO` & `iTesting3-1.0.1/iTesting3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iTesting3
-Version: 1.0.0
+Version: 1.0.1
 Summary: iTesting is a common test framework support for both UI and API test with run in parallel ability.
 Home-page: https://www.testertalk.com
 Author: Kevin.cai.HPJ
 Author-email: love.i@outlook.com
 License: GPL
 
 此代码库为本人新书 **<从0到1搭建自动化测试框架：原理、实现与工程实践>** 的配套练习框架。本书基于Python编写，学习完本书，您能够完全自主开发自动化测试框架.
```

### Comparing `iTesting3-1.0.0/iTesting3.egg-info/SOURCES.txt` & `iTesting3-1.0.1/iTesting3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iTesting3-1.0.0/setup.py` & `iTesting3-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='iTesting3',
-    version='1.0.0',
+    version='1.0.1',
     description='iTesting is a common test framework support for both UI and API test with run in parallel ability.',
     long_description='''此代码库为本人新书 **<从0到1搭建自动化测试框架：原理、实现与工程实践>** 的配套练习框架。本书基于Python编写，学习完本书，您能够完全自主开发自动化测试框架.\n
 更多关于自动化测试框架的内容，请 **关注我的微信公众号iTesting** ，跟万人测试团一起成长.\n
 另，对JavaScript及前端自动化测试感兴趣的同学，也可购买我的另一本书<前端自动化测试框架 -- Cypress从入门到精通>.
                                                                         --Kevin Cai（2022.01）
 ''',
     author='Kevin.cai.HPJ',
```


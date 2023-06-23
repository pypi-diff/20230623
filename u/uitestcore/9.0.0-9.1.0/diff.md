# Comparing `tmp/uitestcore-9.0.0.tar.gz` & `tmp/uitestcore-9.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uitestcore-9.0.0.tar", last modified: Wed Jul 20 11:47:01 2022, max compression
+gzip compressed data, was "uitestcore-9.1.0.tar", last modified: Fri Jul 22 16:30:32 2022, max compression
```

## Comparing `uitestcore-9.0.0.tar` & `uitestcore-9.1.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-20 11:47:01.537765 uitestcore-9.0.0/
--rw-r--r--   0 vsts      (1001) docker     (121)     1050 2022-07-20 11:46:32.000000 uitestcore-9.0.0/LICENSE.md
--rw-r--r--   0 vsts      (1001) docker     (121)     4232 2022-07-20 11:47:01.537765 uitestcore-9.0.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     3837 2022-07-20 11:46:32.000000 uitestcore-9.0.0/README.md
--rw-r--r--   0 vsts      (1001) docker     (121)       38 2022-07-20 11:47:01.537765 uitestcore-9.0.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (121)      895 2022-07-20 11:46:32.000000 uitestcore-9.0.0/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-20 11:47:01.533765 uitestcore-9.0.0/uitestcore/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-07-20 11:46:32.000000 uitestcore-9.0.0/uitestcore/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)      408 2022-07-20 11:46:32.000000 uitestcore-9.0.0/uitestcore/custom_assertion.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1349 2022-07-20 11:46:32.000000 uitestcore-9.0.0/uitestcore/custom_expected_conditions.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2596 2022-07-20 11:46:32.000000 uitestcore-9.0.0/uitestcore/finder.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7743 2022-07-20 11:46:32.000000 uitestcore-9.0.0/uitestcore/interactor.py
--rw-r--r--   0 vsts      (1001) docker     (121)    16420 2022-07-20 11:46:32.000000 uitestcore-9.0.0/uitestcore/interrogator.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1150 2022-07-20 11:46:32.000000 uitestcore-9.0.0/uitestcore/page.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1328 2022-07-20 11:46:32.000000 uitestcore-9.0.0/uitestcore/page_element.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-20 11:47:01.537765 uitestcore-9.0.0/uitestcore/utilities/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-07-20 11:46:32.000000 uitestcore-9.0.0/uitestcore/utilities/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8971 2022-07-20 11:46:32.000000 uitestcore-9.0.0/uitestcore/utilities/attachments_api.py
--rw-r--r--   0 vsts      (1001) docker     (121)    10243 2022-07-20 11:46:32.000000 uitestcore-9.0.0/uitestcore/utilities/browser_handler.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1072 2022-07-20 11:46:32.000000 uitestcore-9.0.0/uitestcore/utilities/config_handler.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1561 2022-07-20 11:46:32.000000 uitestcore-9.0.0/uitestcore/utilities/datetime_handler.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2896 2022-07-20 11:46:32.000000 uitestcore-9.0.0/uitestcore/utilities/logger_handler.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1606 2022-07-20 11:46:32.000000 uitestcore-9.0.0/uitestcore/utilities/string_util.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4148 2022-07-20 11:46:32.000000 uitestcore-9.0.0/uitestcore/waiter.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-20 11:47:01.533765 uitestcore-9.0.0/uitestcore.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (121)     4232 2022-07-20 11:47:01.000000 uitestcore-9.0.0/uitestcore.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)      701 2022-07-20 11:47:01.000000 uitestcore-9.0.0/uitestcore.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-07-20 11:47:01.000000 uitestcore-9.0.0/uitestcore.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (121)      147 2022-07-20 11:47:01.000000 uitestcore-9.0.0/uitestcore.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       11 2022-07-20 11:47:01.000000 uitestcore-9.0.0/uitestcore.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-22 16:30:32.927549 uitestcore-9.1.0/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1050 2022-07-22 16:29:55.000000 uitestcore-9.1.0/LICENSE.md
+-rw-r--r--   0 vsts      (1001) docker     (121)     4232 2022-07-22 16:30:32.927549 uitestcore-9.1.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)     3837 2022-07-22 16:29:55.000000 uitestcore-9.1.0/README.md
+-rw-r--r--   0 vsts      (1001) docker     (121)       38 2022-07-22 16:30:32.927549 uitestcore-9.1.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (121)      895 2022-07-22 16:29:55.000000 uitestcore-9.1.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-22 16:30:32.927549 uitestcore-9.1.0/uitestcore/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-07-22 16:29:55.000000 uitestcore-9.1.0/uitestcore/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      408 2022-07-22 16:29:55.000000 uitestcore-9.1.0/uitestcore/custom_assertion.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1349 2022-07-22 16:29:55.000000 uitestcore-9.1.0/uitestcore/custom_expected_conditions.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2596 2022-07-22 16:29:55.000000 uitestcore-9.1.0/uitestcore/finder.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7743 2022-07-22 16:29:55.000000 uitestcore-9.1.0/uitestcore/interactor.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    16420 2022-07-22 16:29:55.000000 uitestcore-9.1.0/uitestcore/interrogator.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1150 2022-07-22 16:29:55.000000 uitestcore-9.1.0/uitestcore/page.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1328 2022-07-22 16:29:55.000000 uitestcore-9.1.0/uitestcore/page_element.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-22 16:30:32.927549 uitestcore-9.1.0/uitestcore/utilities/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-07-22 16:29:55.000000 uitestcore-9.1.0/uitestcore/utilities/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     8971 2022-07-22 16:29:55.000000 uitestcore-9.1.0/uitestcore/utilities/attachments_api.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    10039 2022-07-22 16:29:55.000000 uitestcore-9.1.0/uitestcore/utilities/browser_handler.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1072 2022-07-22 16:29:55.000000 uitestcore-9.1.0/uitestcore/utilities/config_handler.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1561 2022-07-22 16:29:55.000000 uitestcore-9.1.0/uitestcore/utilities/datetime_handler.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2896 2022-07-22 16:29:55.000000 uitestcore-9.1.0/uitestcore/utilities/logger_handler.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1606 2022-07-22 16:29:55.000000 uitestcore-9.1.0/uitestcore/utilities/string_util.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4148 2022-07-22 16:29:55.000000 uitestcore-9.1.0/uitestcore/waiter.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-22 16:30:32.927549 uitestcore-9.1.0/uitestcore.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (121)     4232 2022-07-22 16:30:32.000000 uitestcore-9.1.0/uitestcore.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)      701 2022-07-22 16:30:32.000000 uitestcore-9.1.0/uitestcore.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-07-22 16:30:32.000000 uitestcore-9.1.0/uitestcore.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)      147 2022-07-22 16:30:32.000000 uitestcore-9.1.0/uitestcore.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)       11 2022-07-22 16:30:32.000000 uitestcore-9.1.0/uitestcore.egg-info/top_level.txt
```

### Comparing `uitestcore-9.0.0/LICENSE.md` & `uitestcore-9.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `uitestcore-9.0.0/PKG-INFO` & `uitestcore-9.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uitestcore
-Version: 9.0.0
+Version: 9.1.0
 Summary: Package providing common functionality for UI automation test packs
 Home-page: UNKNOWN
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `uitestcore-9.0.0/README.md` & `uitestcore-9.1.0/README.md`

 * *Files identical despite different names*

### Comparing `uitestcore-9.0.0/setup.py` & `uitestcore-9.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 setup(
     name="uitestcore",
-    version="9.0.0",
+    version="9.1.0",
     description="Package providing common functionality for UI automation test packs",
     long_description=readme,
     long_description_content_type="text/markdown",
     license="MIT",
     homepage="https://github.com/nhsuk/ui-test-core/",
     packages=["uitestcore", "uitestcore.utilities"],
     install_requires=[
```

### Comparing `uitestcore-9.0.0/uitestcore/custom_expected_conditions.py` & `uitestcore-9.1.0/uitestcore/custom_expected_conditions.py`

 * *Files identical despite different names*

### Comparing `uitestcore-9.0.0/uitestcore/finder.py` & `uitestcore-9.1.0/uitestcore/finder.py`

 * *Files identical despite different names*

### Comparing `uitestcore-9.0.0/uitestcore/interactor.py` & `uitestcore-9.1.0/uitestcore/interactor.py`

 * *Files identical despite different names*

### Comparing `uitestcore-9.0.0/uitestcore/interrogator.py` & `uitestcore-9.1.0/uitestcore/interrogator.py`

 * *Files identical despite different names*

### Comparing `uitestcore-9.0.0/uitestcore/page.py` & `uitestcore-9.1.0/uitestcore/page.py`

 * *Files identical despite different names*

### Comparing `uitestcore-9.0.0/uitestcore/page_element.py` & `uitestcore-9.1.0/uitestcore/page_element.py`

 * *Files identical despite different names*

### Comparing `uitestcore-9.0.0/uitestcore/utilities/attachments_api.py` & `uitestcore-9.1.0/uitestcore/utilities/attachments_api.py`

 * *Files identical despite different names*

### Comparing `uitestcore-9.0.0/uitestcore/utilities/browser_handler.py` & `uitestcore-9.1.0/uitestcore/utilities/browser_handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -158,81 +158,83 @@
 
 
 def open_chrome(context):
     """
     Open the Chrome browser
     :param context: the test context instance
     """
+    chrome_options = webdriver.ChromeOptions()
+
     if platform.system() == 'Windows':
         chromedriver_path = ChromeService(executable_path=r"./browser_executables/chromedriver.exe")
-        context.browser = webdriver.Chrome(service=chromedriver_path)
-
     elif platform.system() == 'Darwin':
         chromedriver_path = ChromeService(executable_path=r"./browser_executables/chromedriver")
-        context.browser = webdriver.Chrome(service=chromedriver_path)
-
     else:
-        chrome_options = webdriver.ChromeOptions()
+        chromedriver_path = ChromeService()
         chrome_options.add_argument("--no-sandbox")
         chrome_options.add_argument("--window-size=1420,1080")
         chrome_options.add_argument("--headless")
         chrome_options.add_argument("--disable-gpu")
 
-        # No need to specify the executable as we're using one installed via pip in Dockerfile
-        context.browser = webdriver.Chrome(options=chrome_options)
+    # Add config browser options to chrome options
+    for option in context.browser_options or []:
+        chrome_options.add_argument(option)
+
+    context.browser = webdriver.Chrome(options=chrome_options, service=chromedriver_path)
 
     BrowserHandler.set_browser_size(context)
 
 
 def open_edge(context):
     """
     Open the Edge browser
     :param context: the test context instance
     """
+    edge_options = webdriver.EdgeOptions()
+
     if platform.system() == 'Windows':
         edgedriver_path = EdgeService(executable_path=r"./browser_executables/msedgedriver.exe")
-        context.browser = webdriver.Edge(service=edgedriver_path)
-
     elif platform.system() == 'Darwin':
         edgedriver_path = EdgeService(executable_path=r"./browser_executables/msedgedriver")
-        context.browser = webdriver.Edge(service=edgedriver_path)
-
     else:
-        edge_options = webdriver.EdgeOptions()
+        edgedriver_path = EdgeService()
         edge_options.add_argument("--no-sandbox")
         edge_options.add_argument("--window-size=1420,1080")
         edge_options.add_argument("--headless")
         edge_options.add_argument("--disable-gpu")
 
-        # No need to specify the executable as we're using one installed via pip in Dockerfile
-        context.browser = webdriver.Edge(options=edge_options)
+    # Add config browser options to edge options
+    for option in context.browser_options or []:
+        edge_options.add_argument(option)
+
+    context.browser = webdriver.Edge(options=edge_options, service=edgedriver_path)
 
     BrowserHandler.set_browser_size(context)
 
 
 def open_firefox(context):
     """
     Open the Firefox browser
     :param context: the test context instance
     """
+    firefox_options = webdriver.FirefoxOptions()
+
     if platform.system() == 'Windows':
         geckodriver_path = FirefoxService(executable_path=r"./browser_executables/geckodriver.exe")
-        context.browser = webdriver.Firefox(service=geckodriver_path)
-
     elif platform.system() == 'Darwin':
         geckodriver_path = FirefoxService(executable_path=r"./browser_executables/geckodriver")
-        context.browser = webdriver.Firefox(service=geckodriver_path)
-
     else:
-        firefox_options = webdriver.FirefoxOptions()
+        geckodriver_path = FirefoxService()
         firefox_options.add_argument("--headless")
 
-        # The Firefox driver (geckodriver) must be located in the "firefox" folder when running in Docker
-        geckodriver_path = FirefoxService(executable_path=r"firefox/geckodriver")
-        context.browser = webdriver.Firefox(service=geckodriver_path, options=firefox_options)
+    # Add config browser options to firefox options
+    for option in context.browser_options or []:
+        firefox_options.add_argument(option)
+
+    context.browser = webdriver.Firefox(options=firefox_options, service=geckodriver_path)
 
     BrowserHandler.set_browser_size(context)
 
 
 def start_browserstack(context):
     """
     Start Browserstack with the required options
```

### Comparing `uitestcore-9.0.0/uitestcore/utilities/config_handler.py` & `uitestcore-9.1.0/uitestcore/utilities/config_handler.py`

 * *Files identical despite different names*

### Comparing `uitestcore-9.0.0/uitestcore/utilities/datetime_handler.py` & `uitestcore-9.1.0/uitestcore/utilities/datetime_handler.py`

 * *Files identical despite different names*

### Comparing `uitestcore-9.0.0/uitestcore/utilities/logger_handler.py` & `uitestcore-9.1.0/uitestcore/utilities/logger_handler.py`

 * *Files identical despite different names*

### Comparing `uitestcore-9.0.0/uitestcore/utilities/string_util.py` & `uitestcore-9.1.0/uitestcore/utilities/string_util.py`

 * *Files identical despite different names*

### Comparing `uitestcore-9.0.0/uitestcore/waiter.py` & `uitestcore-9.1.0/uitestcore/waiter.py`

 * *Files identical despite different names*

### Comparing `uitestcore-9.0.0/uitestcore.egg-info/PKG-INFO` & `uitestcore-9.1.0/uitestcore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uitestcore
-Version: 9.0.0
+Version: 9.1.0
 Summary: Package providing common functionality for UI automation test packs
 Home-page: UNKNOWN
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `uitestcore-9.0.0/uitestcore.egg-info/SOURCES.txt` & `uitestcore-9.1.0/uitestcore.egg-info/SOURCES.txt`

 * *Files identical despite different names*


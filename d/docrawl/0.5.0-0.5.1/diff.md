# Comparing `tmp/docrawl-0.5.0.tar.gz` & `tmp/docrawl-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docrawl-0.5.0.tar", last modified: Fri Jun 23 12:56:04 2023, max compression
+gzip compressed data, was "docrawl-0.5.1.tar", last modified: Fri Jun 23 17:12:01 2023, max compression
```

## Comparing `docrawl-0.5.0.tar` & `docrawl-0.5.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 12:56:04.110759 docrawl-0.5.0/
--rw-rw-rw-   0        0        0     1090 2021-08-16 12:38:07.000000 docrawl-0.5.0/LICENSE
--rw-rw-rw-   0        0        0      568 2023-06-23 12:56:04.110759 docrawl-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0       86 2021-08-16 12:38:07.000000 docrawl-0.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-23 12:56:04.103777 docrawl-0.5.0/docrawl/
--rw-rw-rw-   0        0        0        0 2021-08-16 12:40:29.000000 docrawl-0.5.0/docrawl/__init__.py
--rw-rw-rw-   0        0        0    44673 2023-06-23 12:54:49.000000 docrawl-0.5.0/docrawl/docrawl_core.py
--rw-rw-rw-   0        0        0     6505 2023-06-23 12:54:49.000000 docrawl-0.5.0/docrawl/docrawl_launcher.py
--rw-rw-rw-   0        0        0     1108 2023-02-25 18:40:39.000000 docrawl-0.5.0/docrawl/docrawl_logger.py
--rw-rw-rw-   0        0        0     2674 2023-06-23 12:54:49.000000 docrawl-0.5.0/docrawl/elements.py
-drwxrwxrwx   0        0        0        0 2023-06-23 12:56:04.109761 docrawl-0.5.0/docrawl.egg-info/
--rw-rw-rw-   0        0        0      568 2023-06-23 12:56:03.000000 docrawl-0.5.0/docrawl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-06-23 12:56:04.000000 docrawl-0.5.0/docrawl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 12:56:03.000000 docrawl-0.5.0/docrawl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-06-23 12:56:03.000000 docrawl-0.5.0/docrawl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-23 12:56:03.000000 docrawl-0.5.0/docrawl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 12:56:04.110759 docrawl-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0      834 2023-06-23 12:56:00.000000 docrawl-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 17:12:01.819239 docrawl-0.5.1/
+-rw-rw-rw-   0        0        0     1090 2021-08-16 12:38:07.000000 docrawl-0.5.1/LICENSE
+-rw-rw-rw-   0        0        0      568 2023-06-23 17:12:01.817244 docrawl-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2021-08-16 12:38:07.000000 docrawl-0.5.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 17:12:01.786326 docrawl-0.5.1/docrawl/
+-rw-rw-rw-   0        0        0        0 2021-08-16 12:40:29.000000 docrawl-0.5.1/docrawl/__init__.py
+-rw-rw-rw-   0        0        0    44925 2023-06-23 17:11:30.000000 docrawl-0.5.1/docrawl/docrawl_core.py
+-rw-rw-rw-   0        0        0     6753 2023-06-23 17:11:30.000000 docrawl-0.5.1/docrawl/docrawl_launcher.py
+-rw-rw-rw-   0        0        0     1108 2023-02-25 18:40:39.000000 docrawl-0.5.1/docrawl/docrawl_logger.py
+-rw-rw-rw-   0        0        0     2674 2023-06-23 12:54:49.000000 docrawl-0.5.1/docrawl/elements.py
+drwxrwxrwx   0        0        0        0 2023-06-23 17:12:01.816246 docrawl-0.5.1/docrawl.egg-info/
+-rw-rw-rw-   0        0        0      568 2023-06-23 17:12:00.000000 docrawl-0.5.1/docrawl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-06-23 17:12:01.000000 docrawl-0.5.1/docrawl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 17:12:00.000000 docrawl-0.5.1/docrawl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-06-23 17:12:01.000000 docrawl-0.5.1/docrawl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-23 17:12:01.000000 docrawl-0.5.1/docrawl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 17:12:01.819239 docrawl-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      834 2023-06-23 17:11:41.000000 docrawl-0.5.1/setup.py
```

### Comparing `docrawl-0.5.0/LICENSE` & `docrawl-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `docrawl-0.5.0/PKG-INFO` & `docrawl-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docrawl
-Version: 0.5.0
+Version: 0.5.1
 Summary: Do automated crawling of pages using scrapy
 Home-page: https://github.com/DovaX/docrawl
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `docrawl-0.5.0/docrawl/docrawl_core.py` & `docrawl-0.5.1/docrawl/docrawl_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # import sys #PATH initialization of modules
 # try:
 #    sys.path.append("C:\\Users\\EUROCOM\\Documents\\Git\\DovaX")
 # except:
 #    pass
 from docrawl.docrawl_logger import docrawl_logger
-from docrawl.elements import *
+from docrawl.elements import Element, ElementType, classify_element_by_xpath, PREDEFINED_TAGS
 from collections import UserDict
 import datetime
 import scrapy
 import requests
 import time
 import pickle
 import os
@@ -37,18 +37,18 @@
 from webdriver_manager.chrome import ChromeDriverManager
 
 from scrapy.selector import Selector
 from keepvariable.keepvariable_core import VarSafe, kept_variables, save_variables, load_variable_safe, KeepVariableDummyRedisServer
 
 from typing import Optional
 
-redis: Optional[KeepVariableDummyRedisServer] = None
+kv_redis: Optional[KeepVariableDummyRedisServer] = None
 
-redis_key_webpage_elements = 'test_user:test_project:test_pipeline:scraping:elements'
-redis_key_screenshot = 'test_user:test_project:test_pipeline:scraping:screenshot'
+kv_redis_key_webpage_elements = 'elements'
+kv_redis_key_screenshot = 'screenshot'
 
 
 def click_class(browser, class_input, index=0, tag="div", wait1=1):
     name_input = browser.find_elements_by_xpath('//' + tag + '[@class="' + class_input + '"]')
     name_input[index].click()
     time.sleep(wait1)
     return (name_input)
@@ -94,15 +94,15 @@
         # Dictionary with 1 key: data
         string = browser.execute_cdp_cmd('Page.captureScreenshot', screenshot_config)['data']  # Taking screenshot
         # with open(filename, "w+") as fh:
         #     fh.write(string)
     else:
         string = ""
 
-    redis.set(key=redis_key_screenshot, value=string)
+    kv_redis.set(key=kv_redis_key_screenshot, value=string)
     docrawl_logger.warning('SCRENSHOT CREATED')
 
 
 
 def take_png_screenshot(browser, page, inp):
     """
     Takes screenshot of current page and saves it.
@@ -163,15 +163,15 @@
     incl_buttons = inp['incl_buttons']
     by_xpath = inp['by_xpath']
     cookies_xpath = inp['cookies_xpath']        # dev param only
     context_xpath = inp['context_xpath']
     output_folder = inp['output_folder']
 
     # First removed old data
-    redis.set(key=redis_key_webpage_elements, value=[])
+    kv_redis.set(key=kv_redis_key_webpage_elements, value=[])
 
     # Dictionary with elements (XPaths, data)
     final_elements = {}
 
     # Page source for parser
     innerHTML = browser.execute_script("return document.body.innerHTML")
     tree = lxml.html.fromstring(innerHTML)
@@ -504,34 +504,31 @@
         final_elements.update({element_name:
                                    {'selector': selector,
                                     'data': data,
                                     'xpath': xpath}})
 
     new_elements_all = []
 
-    def find_elements(tags, element_type: ElementType, custom_tag=False):
+    def find_elements(element_type: ElementType, custom_tags: list = None):
         """
         Finds elements on page using Selenium Selector and HTML Parser
-            :param tags: list of tags
             :param element_type: type of element (table, bullet, text, headline, link, ...)
-            :param custom_tag: if provided tag is custom (not predefined)
+            :param custom_tags: list of custom tags
         """
 
+        tags = PREDEFINED_TAGS[element_type] if not custom_tags else custom_tags
         elements = []
         elements_tree = []
 
         # If tag is not predefined -> there is no need to add prefix
-        if not custom_tag:
-            prefix = '//'
-        else:
-            prefix = ''
+        prefix = '' if custom_tags else '//'
 
         for tag in tags:
             elements.extend(browser.find_elements(By.XPATH, f'{prefix}{tag}'))
-            if custom_tag:
+            if custom_tags:
                 tag = tag.replace('/body/', '/div/')  # Otherwise, elements_tree will be empty
             elements_tree.extend(tree.xpath(f'{prefix}{tag}'))
 
         if elements:
             added_xpaths = []       # For deduplication of elements
             for i, element in enumerate(elements):
                 elem_name = f'{element_type}_{i}'
@@ -564,76 +561,76 @@
         xpath[2] = 'body'  # For some reason getpath() generates <div> instead of <body>
         xpath = '/'.join(xpath)
 
         return xpath
 
     ##### TABLES SECTION #####
     if incl_tables:
-        find_elements(TABLE_TAGS, element_type=ElementType.TABLE)
+        find_elements(element_type=ElementType.TABLE)
 
     ##### BULLET SECTION #####
     if incl_bullets:
-        find_elements(BULLET_TAGS, element_type=ElementType.BULLET)
+        find_elements(element_type=ElementType.BULLET)
 
     ##### TEXTS SECTION #####
     if incl_texts:
-        find_elements(TEXT_TAGS, element_type=ElementType.TEXT)
+        find_elements(element_type=ElementType.TEXT)
 
     ##### HEADLINES SECTION #####
     if incl_headlines:
-        find_elements(HEADLINE_TAGS, element_type=ElementType.HEADLINE)
+        find_elements(element_type=ElementType.HEADLINE)
 
     ##### LINKS SECTION #####
     if incl_links:
-        find_elements(LINK_TAGS, element_type=ElementType.LINK)
+        find_elements(element_type=ElementType.LINK)
 
     ##### IMAGES SECTION #####
     if incl_images:
-        find_elements(IMAGE_TAGS, element_type=ElementType.IMAGE)
+        find_elements(element_type=ElementType.IMAGE)
 
     ##### BUTTONS SECTION #####
     if incl_buttons:
-        find_elements(BUTTON_TAGS, element_type=ElementType.BUTTON)
+        find_elements(element_type=ElementType.BUTTON)
 
     ##### CUSTOM XPATH SECTION #####
     if by_xpath:
         # Temporary workaround due to weird behaviour of lists in kpv
         if ';' in by_xpath:
             list_of_xpaths = by_xpath.split(';')[:-1]
         else:
             list_of_xpaths = [by_xpath]
 
         for i, elem in enumerate(list_of_xpaths):
             # With text() at the end will not work
             xpath = elem.removesuffix('/text()').rstrip('/')
 
-            custom_tag = [xpath]
+            custom_tags = [xpath]
             element_type = classify_element_by_xpath(xpath)
 
-            find_elements(custom_tag, element_type, custom_tag=True)
+            find_elements(element_type=element_type, custom_tags=custom_tags)
 
     if context_xpath:
         try:
-            find_elements([context_xpath], ElementType.CONTEXT, custom_tag=True)
+            find_elements(element_type=ElementType.CONTEXT, custom_tags=[context_xpath])
         except Exception as e:
             docrawl_logger.error(f'Error while retrieving context elements: {e}')
 
     if cookies_xpath:
-        find_elements([cookies_xpath], ElementType.COOKIES, custom_tag=True)
+        find_elements(element_type=ElementType.COOKIES, custom_tags=[cookies_xpath])
 
     ##### SAVING COORDINATES OF ELEMENTS #####
 
     # names = list(final_elements.keys())
     # selectors = [x['selector'] for x in final_elements.values()]
     # xpaths = [x['xpath'] for x in final_elements.values()]
     # data = [x['data'] for x in final_elements.values()]
     #
     # save_coordinates_of_elements(selectors, names, xpaths, data)
 
-    redis.set(key=redis_key_webpage_elements, value=new_elements_all)
+    kv_redis.set(key=kv_redis_key_webpage_elements, value=new_elements_all)
     docrawl_logger.info(f'Scan Web Page function duration {timedelta_format(datetime.datetime.now(), time_start_f)}')
 
 
 def wait_until_element_is_located(browser, page, inp):
     """
     Waits until certain element is located on page and then clicks on it.
         :param browser: Selenium driver, browser instance
@@ -914,15 +911,15 @@
     else:
         df = pd.DataFrame(result)
 
     # Remove empty rows
     df.dropna(axis=0, how='all', inplace=True)
     df.to_excel(short_filename + '.xlsx')
 
-    redis.set(key='test_user:test_project:test_pipeline:scraping:extracted_table', value=df)
+    kv_redis.set(key='extracted_table', value=df)
 
 
 class BrowserMetaData(UserDict):
     """
     Stores browser metadata such as driver, proxy, request and function info.
 
     Ensures synchronisation with .kpv file.
@@ -996,16 +993,24 @@
 
     def __init__(self, *a, **kw):
         # can be replaced for debugging with browser = webdriver.FireFox()
         # self.browser = webdriver.PhantomJS(executable_path=PHANTOMJS_PATH, service_args=['--ignore-ssl-errors=true'])
         #super().__init__(*a, **kw)
         self.meta_data = BrowserMetaData()
 
-        global redis
-        redis = kw['redis']
+        # TODO: get rid of global variables
+        global kv_redis
+        global kv_redis_key_webpage_elements
+        global kv_redis_key_screenshot
+
+        kv_redis = kw['kv_redis']
+        kv_redis_keys = kw['kv_redis_keys']
+
+        kv_redis_key_webpage_elements = kv_redis_keys.get('elements', kv_redis_key_webpage_elements)
+        kv_redis_key_screenshot = kv_redis_keys.get('screenshot', kv_redis_key_screenshot)
 
         self.browser = self._initialise_browser()
 
         browser_info = {
             'driver': self.driver_type,
             'headless': self.headless,
             'browser_pid': self.browser_pid
```

### Comparing `docrawl-0.5.0/docrawl/docrawl_launcher.py` & `docrawl-0.5.1/docrawl/docrawl_launcher.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import docrawl.docrawl_core as docrawl_core
 from scrapy.crawler import CrawlerRunner
 from crochet import setup
 import keepvariable.keepvariable_core as kv
 import time
+from typing import Optional
 from docrawl.docrawl_logger import docrawl_logger
 
 
 def load_website(url):
     if "http" not in url:
         url = "http://" + url
 
@@ -211,19 +212,21 @@
 
     spider_functions = {"name": function, "input": function_input, "done": False}
     spider_functions = kv.VarSafe(spider_functions, "function", "function")
     kv.save_variables(kv.kept_variables, "browser_meta_data.kpv")
 
 
 
-def run_spider(number, in_browser=True, driver='Firefox', redis=None):
+def run_spider(number, in_browser=True, driver='Firefox', kv_redis=None, kv_redis_keys=Optional[dict]):
     """
     Starts crawler.
         :param in_browser: bool, show browser GUI (-headless option).
         :param driver: string, driver instance to use (Firefox/Geckodriver, Chrome)
+        :param kv_redis: instance of KeepVariableRedis, used to store scraped data
+        :param kv_redis_keys: dictionary with redis keys (naming)
 
         Note: param in_browser is reverse to -headless option, meaning:
             - in_browser=True -> no -headless in driver options
             - in_browser=False -> add -headless to driver options
     """
 
     headless = not in_browser
@@ -233,8 +236,8 @@
     browser = {'headless': headless, 'driver': driver}
     browser = kv.VarSafe(browser, "browser", "browser")
 
     kv.save_variables(kv.kept_variables, "browser_meta_data.kpv")
 
     time.sleep(1)
 
-    crawler.crawl(docrawl_core.DocrawlSpider, redis=redis)
+    crawler.crawl(docrawl_core.DocrawlSpider, kv_redis=kv_redis, kv_redis_keys=kv_redis_keys)
```

### Comparing `docrawl-0.5.0/docrawl/docrawl_logger.py` & `docrawl-0.5.1/docrawl/docrawl_logger.py`

 * *Files identical despite different names*

### Comparing `docrawl-0.5.0/docrawl/elements.py` & `docrawl-0.5.1/docrawl/elements.py`

 * *Files identical despite different names*

### Comparing `docrawl-0.5.0/docrawl.egg-info/PKG-INFO` & `docrawl-0.5.1/docrawl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docrawl
-Version: 0.5.0
+Version: 0.5.1
 Summary: Do automated crawling of pages using scrapy
 Home-page: https://github.com/DovaX/docrawl
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `docrawl-0.5.0/setup.py` & `docrawl-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='docrawl',
-    version='0.5.0',
+    version='0.5.1',
     author='DovaX',
     author_email='dovax.ai@gmail.com',
     description='Do automated crawling of pages using scrapy',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/DovaX/docrawl',
     packages=setuptools.find_packages(),
```


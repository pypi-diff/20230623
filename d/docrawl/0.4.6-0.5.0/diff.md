# Comparing `tmp/docrawl-0.4.6.tar.gz` & `tmp/docrawl-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docrawl-0.4.6.tar", last modified: Wed May 31 01:00:27 2023, max compression
+gzip compressed data, was "docrawl-0.5.0.tar", last modified: Fri Jun 23 12:56:04 2023, max compression
```

## Comparing `docrawl-0.4.6.tar` & `docrawl-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 01:00:27.214808 docrawl-0.4.6/
--rw-rw-rw-   0        0        0     1090 2021-08-16 12:38:07.000000 docrawl-0.4.6/LICENSE
--rw-rw-rw-   0        0        0      568 2023-05-31 01:00:27.213811 docrawl-0.4.6/PKG-INFO
--rw-rw-rw-   0        0        0       86 2021-08-16 12:38:07.000000 docrawl-0.4.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-31 01:00:27.195859 docrawl-0.4.6/docrawl/
--rw-rw-rw-   0        0        0        0 2021-08-16 12:40:29.000000 docrawl-0.4.6/docrawl/__init__.py
--rw-rw-rw-   0        0        0    41350 2023-05-31 00:59:50.000000 docrawl-0.4.6/docrawl/docrawl_core.py
--rw-rw-rw-   0        0        0     6416 2023-05-31 00:59:50.000000 docrawl-0.4.6/docrawl/docrawl_launcher.py
--rw-rw-rw-   0        0        0     1108 2023-02-25 18:40:39.000000 docrawl-0.4.6/docrawl/docrawl_logger.py
-drwxrwxrwx   0        0        0        0 2023-05-31 01:00:27.213811 docrawl-0.4.6/docrawl.egg-info/
--rw-rw-rw-   0        0        0      568 2023-05-31 01:00:26.000000 docrawl-0.4.6/docrawl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-05-31 01:00:27.000000 docrawl-0.4.6/docrawl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 01:00:26.000000 docrawl-0.4.6/docrawl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-05-31 01:00:26.000000 docrawl-0.4.6/docrawl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-31 01:00:26.000000 docrawl-0.4.6/docrawl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 01:00:27.215806 docrawl-0.4.6/setup.cfg
--rw-rw-rw-   0        0        0      834 2023-05-31 01:00:23.000000 docrawl-0.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 12:56:04.110759 docrawl-0.5.0/
+-rw-rw-rw-   0        0        0     1090 2021-08-16 12:38:07.000000 docrawl-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0      568 2023-06-23 12:56:04.110759 docrawl-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2021-08-16 12:38:07.000000 docrawl-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 12:56:04.103777 docrawl-0.5.0/docrawl/
+-rw-rw-rw-   0        0        0        0 2021-08-16 12:40:29.000000 docrawl-0.5.0/docrawl/__init__.py
+-rw-rw-rw-   0        0        0    44673 2023-06-23 12:54:49.000000 docrawl-0.5.0/docrawl/docrawl_core.py
+-rw-rw-rw-   0        0        0     6505 2023-06-23 12:54:49.000000 docrawl-0.5.0/docrawl/docrawl_launcher.py
+-rw-rw-rw-   0        0        0     1108 2023-02-25 18:40:39.000000 docrawl-0.5.0/docrawl/docrawl_logger.py
+-rw-rw-rw-   0        0        0     2674 2023-06-23 12:54:49.000000 docrawl-0.5.0/docrawl/elements.py
+drwxrwxrwx   0        0        0        0 2023-06-23 12:56:04.109761 docrawl-0.5.0/docrawl.egg-info/
+-rw-rw-rw-   0        0        0      568 2023-06-23 12:56:03.000000 docrawl-0.5.0/docrawl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-06-23 12:56:04.000000 docrawl-0.5.0/docrawl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 12:56:03.000000 docrawl-0.5.0/docrawl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-06-23 12:56:03.000000 docrawl-0.5.0/docrawl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-23 12:56:03.000000 docrawl-0.5.0/docrawl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 12:56:04.110759 docrawl-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      834 2023-06-23 12:56:00.000000 docrawl-0.5.0/setup.py
```

### Comparing `docrawl-0.4.6/LICENSE` & `docrawl-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `docrawl-0.4.6/PKG-INFO` & `docrawl-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docrawl
-Version: 0.4.6
+Version: 0.5.0
 Summary: Do automated crawling of pages using scrapy
 Home-page: https://github.com/DovaX/docrawl
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `docrawl-0.4.6/docrawl/docrawl_core.py` & `docrawl-0.5.0/docrawl/docrawl_core.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # import sys #PATH initialization of modules
 # try:
 #    sys.path.append("C:\\Users\\EUROCOM\\Documents\\Git\\DovaX")
 # except:
 #    pass
 from docrawl.docrawl_logger import docrawl_logger
+from docrawl.elements import *
 from collections import UserDict
 import datetime
 import scrapy
 import requests
 import time
 import pickle
 import os
-import shutil
 import re
 import psutil
 import lxml.html
 import pandas as pd
 
 # Due to the problems with selenium wire on linux systems
 try:
@@ -27,21 +27,28 @@
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.proxy import Proxy, ProxyType
 from selenium.webdriver.common.desired_capabilities import DesiredCapabilities
 from selenium.webdriver import FirefoxOptions, ChromeOptions
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.firefox.service import Service
+from selenium.webdriver.remote.webdriver import WebElement
 
 from webdriver_manager.firefox import GeckoDriverManager
 from webdriver_manager.chrome import ChromeDriverManager
 
-
 from scrapy.selector import Selector
-from keepvariable.keepvariable_core import VarSafe, kept_variables, save_variables, load_variable_safe
+from keepvariable.keepvariable_core import VarSafe, kept_variables, save_variables, load_variable_safe, KeepVariableDummyRedisServer
+
+from typing import Optional
+
+redis: Optional[KeepVariableDummyRedisServer] = None
+
+redis_key_webpage_elements = 'test_user:test_project:test_pipeline:scraping:elements'
+redis_key_screenshot = 'test_user:test_project:test_pipeline:scraping:screenshot'
 
 
 def click_class(browser, class_input, index=0, tag="div", wait1=1):
     name_input = browser.find_elements_by_xpath('//' + tag + '[@class="' + class_input + '"]')
     name_input[index].click()
     time.sleep(wait1)
     return (name_input)
@@ -50,26 +57,29 @@
 def take_screenshot(browser, page, inp):
     """
     Takes screenshot of current page and saves it.
         :param browser: Selenium driver, browser instance
         :param inp, list, inputs from launcher (filename)
     """
 
-    filename = inp['filename']
+    #filename = inp['filename']
 
     if type(browser) == webdriver.Firefox:
 
         try:
+            docrawl_logger.warning('START SCREENSHOT CREATED')
             root_element = browser.find_element(By.XPATH, '/html')
             string = browser.get_full_page_screenshot_as_base64()
             browser.execute_script("return arguments[0].scrollIntoView(true);", root_element)
 
-            with open(filename, "w+") as fh:
-                fh.write(string)
+            # with open(filename, "w+") as fh:
+            #     fh.write(string)
+            #     docrawl_logger.warning('SCRENSHOT CREATED')
         except Exception as e:
+            string = ""
             docrawl_logger.error(f'Error while taking page screenshot: {e}')
 
     elif type(browser) == webdriver.Chrome:
         # Get params needed for fullpage screenshot
         page_rect = browser.execute_cdp_cmd('Page.getLayoutMetrics', {})
 
         # Set the width and height of the viewport to screenshot, same as the site's content size
@@ -79,16 +89,23 @@
                                       'height': page_rect['cssContentSize']['height'],
                                       'x': 0,
                                       'y': 0,
                                       'scale': 1},
                              }
         # Dictionary with 1 key: data
         string = browser.execute_cdp_cmd('Page.captureScreenshot', screenshot_config)['data']  # Taking screenshot
-        with open(filename, "w+") as fh:
-            fh.write(string)
+        # with open(filename, "w+") as fh:
+        #     fh.write(string)
+    else:
+        string = ""
+
+    redis.set(key=redis_key_screenshot, value=string)
+    docrawl_logger.warning('SCRENSHOT CREATED')
+
+
 
 def take_png_screenshot(browser, page, inp):
     """
     Takes screenshot of current page and saves it.
         :param browser: Selenium driver, browser instance
         :param inp, list, inputs from launcher (filename)
     """
@@ -103,45 +120,21 @@
     except Exception as e:
         print('Error while taking page screenshot!', e)
     '''
     if type(browser) == webdriver.Firefox:
 
         try:
             root_element = browser.find_element(By.XPATH, '/html')
-            #string = browser.get_full_page_screenshot_as_file(filename)
-            #driver.find_element_by_tag_name('body').screenshot('web_screenshot4.png')
-    
-            screenshot=browser.get_full_page_screenshot_as_file(filename)
-            print(screenshot)
+
+            screenshot = browser.get_full_page_screenshot_as_file(filename)
             browser.execute_script("return arguments[0].scrollIntoView(true);", root_element)
 
-            #with open(filename, "w+") as fh:
-            #    fh.write(string)
+            docrawl_logger.info(f'Png screenshot created')
         except Exception as e:
-            print('Error while taking page screenshot!', e)
-
-    # elif type(browser) == webdriver.Chrome:
-    #     # Get params needed for fullpage screenshot
-    #     page_rect = browser.execute_cdp_cmd('Page.getLayoutMetrics', {})
-
-    #     # Set the width and height of the viewport to screenshot, same as the site's content size
-    #     screenshot_config = {'captureBeyondViewport': True,
-    #                          'fromSurface': True,
-    #                          'clip': {'width': page_rect['cssContentSize']['width'],
-    #                                   'height': page_rect['cssContentSize']['height'],
-    #                                   'x': 0,
-    #                                   'y': 0,
-    #                                   'scale': 1},
-    #                          }
-    #     # Dictionary with 1 key: data
-    #     string = browser.execute_cdp_cmd('Page.captureScreenshot', screenshot_config)['data']  # Taking screenshot
-    #     with open(filename, "w+") as fh:
-    #         fh.write(string)
-
-
+            docrawl_logger.error(f'Error while taking page png screenshot: {e}')
 
 
 def extract_page_source(browser, page, inp):
     """
     Extracts the source of currently scraped page.
         :param page: Selenium Selector, page to export source from
         :param inp: list, inputs from launcher (incl_tables, incl_bullets, output_dir)
@@ -169,51 +162,16 @@
     incl_images = inp['incl_images']
     incl_buttons = inp['incl_buttons']
     by_xpath = inp['by_xpath']
     cookies_xpath = inp['cookies_xpath']        # dev param only
     context_xpath = inp['context_xpath']
     output_folder = inp['output_folder']
 
-    # Predefined tags by type
-    TABLE_TAG = ['table']
-    BULLET_TAGS = ['ul', 'ol']
-    TEXT_TAGS = ['p', 'strong', 'em', 'div[normalize-space(text())]', 'span[normalize-space(text())]']
-    HEADLINE_TAGS = ['h1', 'h2', 'h3', 'h4', 'h5', 'h6']
-    IMAGE_TAGS = ['img']
-    BUTTON_TAGS = ['button', 'a[@role="button"]', 'a[contains(@class, "button")]',
-                   'a[contains(@id, "button")]', 'a[@type="button"]', 'a[contains(@class, "btn")]']
-
-    # <a> tags, excluding links in menu, links as images, mailto links and links with scripts
-    LINK_TAGS = ["""
-                    a[@href
-                    and not(contains(@id, "Menu"))  
-                    and not(contains(@id, "menu"))  
-                    and not(contains(@class, "Menu"))  
-                    and not(contains(@class, "menu"))   
-                    and not(descendant::img) 
-                    and not(descendant::svg)  
-                    and not(contains(@href, "javascript"))  
-                    and not(contains(@href, "mailto"))]
-                    """]
-
-    # All predefined tags
-    PREDEFINED_TAGS = {'table': TABLE_TAG,
-                       'bullet': BULLET_TAGS,
-                       'text': TEXT_TAGS,
-                       'headline': HEADLINE_TAGS,
-                       'image': IMAGE_TAGS,
-                       'button': BUTTON_TAGS,
-                       'link': LINK_TAGS + ['a']}  # + ['a'] is to identify link tags when using custom XPath
-
-    try:
-        shutil.rmtree(output_folder)
-    except:
-        pass
-    finally:
-        os.mkdir(output_folder)
+    # First removed old data
+    redis.set(key=redis_key_webpage_elements, value=[])
 
     # Dictionary with elements (XPaths, data)
     final_elements = {}
 
     # Page source for parser
     innerHTML = browser.execute_script("return document.body.innerHTML")
     tree = lxml.html.fromstring(innerHTML)
@@ -277,25 +235,139 @@
             elems_pos.append({'rect': selector.rect,
                               'name': name,
                               'xpath': xpath,
                               'data': data})
 
             existing_xpaths.append(xpath)
 
-        
-
-        elements_positions = {"elements_positions":elems_pos}
-        filename="elements_positions.kpv"
-        with open(filename,"w+", encoding="utf8",errors='ignore') as file: #TODO: improve KPV to enable multiple keep variable files -> it collided with browser_metadata_kpv,
+        elements_positions = {"elements_positions": elems_pos}
+        filename = "elements_positions.kpv"
+        with open(filename, "w+", encoding="utf8",
+                  errors='ignore') as file:  # TODO: improve KPV to enable multiple keep variable files -> it collided with browser_metadata_kpv,
             file.write(str(elements_positions))
-            
-        #elements_positions = VarSafe(elements_positions, 'elements_positions', 'elements_positions')
-        #save_variables(kept_variables, 'elements_positions.kpv')
 
-    def serialize_and_append_data(element_name, selector, xpath):
+        # elements_positions = VarSafe(elements_positions, 'elements_positions', 'elements_positions')
+        # save_variables(kept_variables, 'elements_positions.kpv')
+
+    def extract_element_data(element: WebElement, xpath: str, element_type: ElementType):
+        if element_type in [ElementType.LINK, ElementType.BUTTON]:
+            xpath_new = xpath + '//text()'
+            text = ''.join(page.xpath(xpath_new).extract()).strip()
+        elif element_type == ElementType.IMAGE:
+            xpath_new = xpath + '//text()'
+            text = page.xpath(xpath_new).extract()
+
+            # if data:
+            #     # Handle images with relative path. E.g. images/logo.png
+            #     if not any([data.startswith(x) for x in ['http', 'www']]):
+            #         data = url_pattern.match(browser.current_url).group(1) + data.replace('./', '')
+            #
+            #     with open(path + '.pickle', 'wb') as pickle_file:
+            #         pickle.dump(data, pickle_file)
+        elif element_type == ElementType.BULLET:
+            text = process_bullet(xpath)
+            #xpath_new = xpath + '//li//text()'
+        elif element_type == ElementType.TABLE:
+            table_2 = page.xpath(xpath)[0]
+
+            result = []  # data
+            titles = []  # columns' names
+            tr_tags = table_2.xpath('.//tr')  # <tr> = table row
+            th_tags = table_2.xpath('.//th')  # <th> = table header (non-essential, so if any)
+
+            for th_tag in th_tags:
+                titles.append(''.join(th_tag.xpath('.//text()').extract()).replace('\n', '').replace('\t', ''))
+
+            for tr_tag in tr_tags:
+                td_tags = tr_tag.xpath('.//td')  # <td> = table data
+
+                row = []
+
+                '''
+                    # Sometimes between td tags there more than 1 tag with text, so that would
+                    # be proceeded as separate values despite of fact it should be in one cell.
+                    # That's why the further loop is needed. The result of it is a list of strings,
+                    # that should be in one cell later in dataframe.
+
+                    # Example: 
+
+                    <td>
+                        <a>Text 1</a>
+                        <a>Text 2</a>
+                    </td>
+
+                    # Without loop it would be two strings ("Text 1", "Text 2") and thus they 
+                    # will be in 2 differrent columns. With loop the result would be ["Text 1", "Text 2"] 
+                    # and after join method - "Text 1 Text 2" in just one cell (column).
+               '''
+
+                for td_tag in td_tags:
+                    data = td_tag.xpath('.//text()').getall()
+
+                    '''
+                        Some table cells include \n or unicode symbols,
+                        so that creates unneccesary "empty" columns and thus
+                        the number of columns doesn't meet the real one
+                    '''
+
+                    data = [string_cleaner(x) for x in data]  # Cleaning the text
+
+                    # data = list(filter(None, data))  # Deleting empty strings
+
+                    row.append('\n'.join(data))  # Making one string value from list
+
+                result.append(row)
+
+                if not titles:  # If table doesn't have <th> tags -> use first row as titles
+                    titles = row  # TODO: IF USER SELECTS THE TABLE, ASK HIM, WHETHER HE WANTS TO HAVE 1 ROW AS TITLES
+
+            try:
+                # If number of columns' names (titles) is the same as number of columns
+                df = pd.DataFrame(result, columns=titles)
+            except Exception:
+                df = pd.DataFrame(result)
+
+            df = df.iloc[1:, :]  # Removing empty row at the beginning of dataframe
+
+            df.dropna(axis=0, how='all', inplace=True)
+
+            text = df
+
+            # # If dataframe is not empty
+            # if not df.dropna().empty and len(df.columns) > 1 and len(df) > 1:
+            #     # Serialize DataFrame
+            #
+            #     with open(path + '.pickle', 'wb') as pickle_file:
+            #         pickle.dump(df, pickle_file)
+        else:
+            xpath += '//text()'
+
+            # Try to extract text from element
+            try:
+                text = ''.join(page.xpath(xpath).extract()).strip()
+            # Extract element otherwise
+            except:
+                xpath = xpath.removesuffix('//text()')
+                text = ''.join(page.xpath(xpath).extract()).strip()
+
+        # attributes = element.get_property('attributes')
+        attributes = browser.execute_script(
+            'var items = {}; for (index = 0; index < arguments[0].attributes.length; ++index) { items[arguments[0].attributes[index].name] = arguments[0].attributes[index].value }; return items;',
+            element)
+
+        # docrawl_logger.warning(attributes)
+        element_data = {
+            'tag_name': re.split('//|/', xpath)[-1].split('[')[0],
+            'text': text,
+            'attributes': attributes
+        }
+
+        return element_data
+
+    def serialize_and_append_data(element_name, selector: WebElement, xpath):
         """
         Serializes data behind the element and updates dictionary with final elements
             :param element_name: variable name to save
             :param selector: Selenium Selector
             :param xpath: XPath of element
         """
 
@@ -423,25 +495,28 @@
             data = None
         else:
             try:
                 data = pickle_file.name
             except Exception as e:
                 data = None
                 docrawl_logger.error(f'Error while retrieving file with data: {e}')
-        
+
+
         final_elements.update({element_name:
                                    {'selector': selector,
                                     'data': data,
                                     'xpath': xpath}})
 
-    def find_elements(tags, element_name, custom_tag=False):
+    new_elements_all = []
+
+    def find_elements(tags, element_type: ElementType, custom_tag=False):
         """
         Finds elements on page using Selenium Selector and HTML Parser
             :param tags: list of tags
-            :param element_name: type of element (table, bullet, text, headline, link, ...)
+            :param element_type: type of element (table, bullet, text, headline, link, ...)
             :param custom_tag: if provided tag is custom (not predefined)
         """
 
         elements = []
         elements_tree = []
 
         # If tag is not predefined -> there is no need to add prefix
@@ -453,27 +528,34 @@
         for tag in tags:
             elements.extend(browser.find_elements(By.XPATH, f'{prefix}{tag}'))
             if custom_tag:
                 tag = tag.replace('/body/', '/div/')  # Otherwise, elements_tree will be empty
             elements_tree.extend(tree.xpath(f'{prefix}{tag}'))
 
         if elements:
+            added_xpaths = []       # For deduplication of elements
             for i, element in enumerate(elements):
-                # Skip tables with no rows
+                elem_name = f'{element_type}_{i}'
 
-                if element_name == 'table' and len(element.find_elements(By.XPATH, './/tr')) < 2:
+                # Skip tables with no rows
+                if element_type == ElementType.TABLE and len(element.find_elements(By.XPATH, './/tr')) < 2:
                     continue
 
                 try:
                     xpath = find_element_xpath(elements_tree, i)
-                    serialize_and_append_data(f'{element_name}_{i}', element, xpath)
 
-                except Exception as e:
-                    docrawl_logger.error(f'Error while extracting data for element {element_name}: {e}')
+                    if xpath not in added_xpaths:
+                        element_data = extract_element_data(element=element, xpath=xpath, element_type=element_type)
+                        element_c = Element(name=elem_name, type=element_type, rect=element.rect, xpath=xpath, data=element_data)
+                        new_elements_all.append(element_c.dict())
+                        added_xpaths.append(xpath)
+                    #serialize_and_append_data(f'{element_name}_{i}', element, xpath)
 
+                except Exception as e:
+                    docrawl_logger.error(f'Error while extracting data for element {elem_name}: {e}')
 
     def find_element_xpath(tree, i):
         """
         Finds the XPath of element using HTML parser.
             :param tree: list of elements
             :param i: element's number
         """
@@ -482,87 +564,76 @@
         xpath[2] = 'body'  # For some reason getpath() generates <div> instead of <body>
         xpath = '/'.join(xpath)
 
         return xpath
 
     ##### TABLES SECTION #####
     if incl_tables:
-        find_elements(TABLE_TAG, 'table')
+        find_elements(TABLE_TAGS, element_type=ElementType.TABLE)
 
     ##### BULLET SECTION #####
     if incl_bullets:
-        find_elements(BULLET_TAGS, 'bullet')
+        find_elements(BULLET_TAGS, element_type=ElementType.BULLET)
 
     ##### TEXTS SECTION #####
     if incl_texts:
-        find_elements(TEXT_TAGS, 'text')
+        find_elements(TEXT_TAGS, element_type=ElementType.TEXT)
 
     ##### HEADLINES SECTION #####
     if incl_headlines:
-        find_elements(HEADLINE_TAGS, 'headline')
+        find_elements(HEADLINE_TAGS, element_type=ElementType.HEADLINE)
 
     ##### LINKS SECTION #####
     if incl_links:
-        find_elements(LINK_TAGS, 'link')
+        find_elements(LINK_TAGS, element_type=ElementType.LINK)
 
     ##### IMAGES SECTION #####
     if incl_images:
-        find_elements(IMAGE_TAGS, 'image')
+        find_elements(IMAGE_TAGS, element_type=ElementType.IMAGE)
 
     ##### BUTTONS SECTION #####
     if incl_buttons:
-        find_elements(BUTTON_TAGS, 'button')
+        find_elements(BUTTON_TAGS, element_type=ElementType.BUTTON)
 
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
 
             custom_tag = [xpath]
-            custom_tag_splitted = re.split('//|/', xpath)  # Split XPath in parts
-            last_element_in_xpath = custom_tag_splitted[-1]  # Last element in XPath
-
-            # Default element's name
-            element_name = 'element'
-
-            # Try to find last element in XPath in predefined tags to identify element name
-            for element_type, predefined_tags in PREDEFINED_TAGS.items():
-                if any([last_element_in_xpath.startswith(x) for x in predefined_tags]):
-                    element_name = element_type
-                    break
+            element_type = classify_element_by_xpath(xpath)
 
-            element_name = f'{element_name}_{i}'
-
-            find_elements(custom_tag, element_name, custom_tag=True)
+            find_elements(custom_tag, element_type, custom_tag=True)
 
     if context_xpath:
         try:
-            find_elements([context_xpath], 'context', custom_tag=True)
+            find_elements([context_xpath], ElementType.CONTEXT, custom_tag=True)
         except Exception as e:
             docrawl_logger.error(f'Error while retrieving context elements: {e}')
 
     if cookies_xpath:
-        find_elements([cookies_xpath], 'cookies', custom_tag=True)
+        find_elements([cookies_xpath], ElementType.COOKIES, custom_tag=True)
 
     ##### SAVING COORDINATES OF ELEMENTS #####
 
-    names = list(final_elements.keys())
-    selectors = [x['selector'] for x in final_elements.values()]
-    xpaths = [x['xpath'] for x in final_elements.values()]
-    data = [x['data'] for x in final_elements.values()]
-
-    save_coordinates_of_elements(selectors, names, xpaths, data)
+    # names = list(final_elements.keys())
+    # selectors = [x['selector'] for x in final_elements.values()]
+    # xpaths = [x['xpath'] for x in final_elements.values()]
+    # data = [x['data'] for x in final_elements.values()]
+    #
+    # save_coordinates_of_elements(selectors, names, xpaths, data)
 
+    redis.set(key=redis_key_webpage_elements, value=new_elements_all)
     docrawl_logger.info(f'Scan Web Page function duration {timedelta_format(datetime.datetime.now(), time_start_f)}')
 
 
 def wait_until_element_is_located(browser, page, inp):
     """
     Waits until certain element is located on page and then clicks on it.
         :param browser: Selenium driver, browser instance
@@ -843,16 +914,15 @@
     else:
         df = pd.DataFrame(result)
 
     # Remove empty rows
     df.dropna(axis=0, how='all', inplace=True)
     df.to_excel(short_filename + '.xlsx')
 
-    with open(filename, 'wb') as pickle_file:
-        pickle.dump(df, pickle_file)
+    redis.set(key='test_user:test_project:test_pipeline:scraping:extracted_table', value=df)
 
 
 class BrowserMetaData(UserDict):
     """
     Stores browser metadata such as driver, proxy, request and function info.
 
     Ensures synchronisation with .kpv file.
@@ -926,14 +996,17 @@
 
     def __init__(self, *a, **kw):
         # can be replaced for debugging with browser = webdriver.FireFox()
         # self.browser = webdriver.PhantomJS(executable_path=PHANTOMJS_PATH, service_args=['--ignore-ssl-errors=true'])
         #super().__init__(*a, **kw)
         self.meta_data = BrowserMetaData()
 
+        global redis
+        redis = kw['redis']
+
         self.browser = self._initialise_browser()
 
         browser_info = {
             'driver': self.driver_type,
             'headless': self.headless,
             'browser_pid': self.browser_pid
         }
```

### Comparing `docrawl-0.4.6/docrawl/docrawl_launcher.py` & `docrawl-0.5.0/docrawl/docrawl_launcher.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,26 +9,30 @@
 def load_website(url):
     if "http" not in url:
         url = "http://" + url
 
     spider_requests = {"url": url, "loaded": False}
 
     spider_requests = kv.VarSafe(spider_requests, "request", "request")
+    docrawl_logger.info(f"SPIDER_REQUESTS: {spider_requests}")
     kv.save_variables(kv.kept_variables, "browser_meta_data.kpv")
 
+    # docrawl_core.spider_requests={"url":url,"loaded":False}
 
-def take_screenshot(filename):
+
+def take_screenshot():
     """
     Launches take_screenshot from core.
-        :param filename: string, output filename (where to save the screenshot)
     """
 
-    inp = {
-        'filename': filename
-    }
+    # inp = {
+    #     'filename': filename
+    # }
+
+    inp = None
 
     run_function('take_screenshot', inp)
 
 
 def take_png_screenshot(filename):
     """
     Launches take_screenshot from core.
@@ -207,15 +211,15 @@
 
     spider_functions = {"name": function, "input": function_input, "done": False}
     spider_functions = kv.VarSafe(spider_functions, "function", "function")
     kv.save_variables(kv.kept_variables, "browser_meta_data.kpv")
 
 
 
-def run_spider(number, in_browser=True, driver='Firefox'):
+def run_spider(number, in_browser=True, driver='Firefox', redis=None):
     """
     Starts crawler.
         :param in_browser: bool, show browser GUI (-headless option).
         :param driver: string, driver instance to use (Firefox/Geckodriver, Chrome)
 
         Note: param in_browser is reverse to -headless option, meaning:
             - in_browser=True -> no -headless in driver options
@@ -229,8 +233,8 @@
     browser = {'headless': headless, 'driver': driver}
     browser = kv.VarSafe(browser, "browser", "browser")
 
     kv.save_variables(kv.kept_variables, "browser_meta_data.kpv")
 
     time.sleep(1)
 
-    crawler.crawl(docrawl_core.DocrawlSpider)
+    crawler.crawl(docrawl_core.DocrawlSpider, redis=redis)
```

### Comparing `docrawl-0.4.6/docrawl/docrawl_logger.py` & `docrawl-0.5.0/docrawl/docrawl_logger.py`

 * *Files identical despite different names*

### Comparing `docrawl-0.4.6/docrawl.egg-info/PKG-INFO` & `docrawl-0.5.0/docrawl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docrawl
-Version: 0.4.6
+Version: 0.5.0
 Summary: Do automated crawling of pages using scrapy
 Home-page: https://github.com/DovaX/docrawl
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `docrawl-0.4.6/setup.py` & `docrawl-0.5.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='docrawl',
-    version='0.4.6',
+    version='0.5.0',
     author='DovaX',
     author_email='dovax.ai@gmail.com',
     description='Do automated crawling of pages using scrapy',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/DovaX/docrawl',
     packages=setuptools.find_packages(),
```


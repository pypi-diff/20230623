# Comparing `tmp/miuc-0.1.4.tar.gz` & `tmp/miuc-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miuc-0.1.4.tar", max compression
+gzip compressed data, was "miuc-0.1.5.tar", max compression
```

## Comparing `miuc-0.1.4.tar` & `miuc-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2022-12-05 18:27:07.136320 miuc-0.1.4/LICENSE
--rw-r--r--   0        0        0       45 2023-06-22 13:40:27.802869 miuc-0.1.4/miuc/__init__.py
--rw-r--r--   0        0        0      925 2023-06-23 16:36:52.557100 miuc-0.1.4/miuc/main.py
--rw-r--r--   0        0        0    23066 2023-06-23 15:00:31.533250 miuc-0.1.4/miuc/site_processor.py
--rw-r--r--   0        0        0     1891 2023-06-23 14:30:39.349344 miuc-0.1.4/miuc/web_parser.py
--rw-r--r--   0        0        0      508 2023-06-23 16:42:17.904686 miuc-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      752 2023-06-23 16:23:33.629091 miuc-0.1.4/README.md
--rw-r--r--   0        0        0     1543 1970-01-01 00:00:00.000000 miuc-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2022-12-05 18:27:07.136320 miuc-0.1.5/LICENSE
+-rw-r--r--   0        0        0       45 2023-06-22 13:40:27.802869 miuc-0.1.5/miuc/__init__.py
+-rw-r--r--   0        0        0      925 2023-06-23 16:36:52.557100 miuc-0.1.5/miuc/main.py
+-rw-r--r--   0        0        0    23066 2023-06-23 15:00:31.533250 miuc-0.1.5/miuc/site_processor.py
+-rw-r--r--   0        0        0     1888 2023-06-23 17:43:34.626260 miuc-0.1.5/miuc/web_parser.py
+-rw-r--r--   0        0        0      508 2023-06-23 17:44:03.181976 miuc-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1334 2023-06-23 17:31:22.612187 miuc-0.1.5/README.md
+-rw-r--r--   0        0        0     2125 1970-01-01 00:00:00.000000 miuc-0.1.5/PKG-INFO
```

### Comparing `miuc-0.1.4/LICENSE` & `miuc-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `miuc-0.1.4/miuc/main.py` & `miuc-0.1.5/miuc/main.py`

 * *Files identical despite different names*

### Comparing `miuc-0.1.4/miuc/site_processor.py` & `miuc-0.1.5/miuc/site_processor.py`

 * *Files identical despite different names*

### Comparing `miuc-0.1.4/miuc/web_parser.py` & `miuc-0.1.5/miuc/web_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,15 +49,15 @@
                 return SPECIFIC_SITES[specific_page_url](max_time_limit)(url)
 
         response = requests.get(url, timeout=max_time_limit)
         if response.status_code != 200:
             # 404 or other unusual error
             return guess_name_by_url(url)
 
-        return parse_html(response.text)
+        return guess_name_by_url(url)
     except Exception as e:
         
         return guess_name_by_url(url)
 
 def parse_html(html: str) -> str:
     """
     parse html and return the title
```

### Comparing `miuc-0.1.4/PKG-INFO` & `miuc-0.1.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miuc
-Version: 0.1.4
+Version: 0.1.5
 Summary: Markdown Intelligence Url Complete
 Home-page: https://github.com/luzhixing12345/miuc
 License: MIT
 Author: luzhixing12345
 Author-email: luzhixing12345@163.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -19,40 +19,46 @@
 Project-URL: Repository, https://github.com/luzhixing12345/miuc
 Description-Content-Type: text/markdown
 
 # miuc
 
 Markdown Intelligence Url Complete
 
+Paste URL by <kbd>ctrl</kbd> + <kbd>v</kbd>, miuc will complete the title for you
+
 ## Features
 
+![action](https://raw.githubusercontent.com/learner-lu/picbed/master/action.gif)
+
 ## Download
 
 Search `miuc` in Vscode extension market or manually download the extension from [miuc-vscode-extension-market](https://marketplace.visualstudio.com/items?itemName=kamilu.miuc)
 
-If you prefer to use in command line, you could download miuc from PYPI
+Vscode Extension miuc depends on python program miuc, it asks you to download miuc by pip for the first time, you could also download by yourself
 
 ```bash
 pip install miuc
-``` 
+```
+
+**Actually, miuc is not mature**, if you meet any bug please report @ [miuc issues](https://github.com/luzhixing12345/miuc/issues)
 
 ## Usage
 
-use `miuc <url>` and return the markdown format url with title
+in Vscode, press <kbd>ctrl</kbd> + <kbd>v</kbd> to paste as usual, miuc will complete the title if URL in your clipboard
+
+in command line, use `miuc <url>` and return the markdown format url with title, you may need this one if you prefer vim/neovim and so on
 
 ```bash
 $ miuc <url>
 # [article-title](url)
 
 $ miuc https://github.com/luzhixing12345/miuc
 # [miuc](https://github.com/luzhixing12345/miuc)
 ```
 
-see more information from [miuc document]()
-
-## Extension Settings
+see more information from [miuc document](https://luzhixing12345.github.io/miuc/)
 
 ## Rerference
   
 - [brandmark](https://brandmark.io/)
 - [autopep8](https://github.com/microsoft/vscode-autopep8)
```


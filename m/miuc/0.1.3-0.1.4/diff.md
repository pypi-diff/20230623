# Comparing `tmp/miuc-0.1.3.tar.gz` & `tmp/miuc-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miuc-0.1.3.tar", max compression
+gzip compressed data, was "miuc-0.1.4.tar", max compression
```

## Comparing `miuc-0.1.3.tar` & `miuc-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0       45 2023-06-22 13:40:27.802869 miuc-0.1.3/miuc/__init__.py
--rw-r--r--   0        0        0      884 2023-06-23 14:30:20.634701 miuc-0.1.3/miuc/main.py
--rw-r--r--   0        0        0    22964 2023-06-23 14:31:04.618328 miuc-0.1.3/miuc/site_processor.py
--rw-r--r--   0        0        0     1891 2023-06-23 14:30:39.349344 miuc-0.1.3/miuc/web_parser.py
--rw-r--r--   0        0        0      508 2023-06-23 14:31:40.926632 miuc-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      967 2023-06-22 14:51:24.993605 miuc-0.1.3/README.md
--rw-r--r--   0        0        0     1758 1970-01-01 00:00:00.000000 miuc-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2022-12-05 18:27:07.136320 miuc-0.1.4/LICENSE
+-rw-r--r--   0        0        0       45 2023-06-22 13:40:27.802869 miuc-0.1.4/miuc/__init__.py
+-rw-r--r--   0        0        0      925 2023-06-23 16:36:52.557100 miuc-0.1.4/miuc/main.py
+-rw-r--r--   0        0        0    23066 2023-06-23 15:00:31.533250 miuc-0.1.4/miuc/site_processor.py
+-rw-r--r--   0        0        0     1891 2023-06-23 14:30:39.349344 miuc-0.1.4/miuc/web_parser.py
+-rw-r--r--   0        0        0      508 2023-06-23 16:42:17.904686 miuc-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      752 2023-06-23 16:23:33.629091 miuc-0.1.4/README.md
+-rw-r--r--   0        0        0     1543 1970-01-01 00:00:00.000000 miuc-0.1.4/PKG-INFO
```

### Comparing `miuc-0.1.3/miuc/main.py` & `miuc-0.1.4/miuc/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 *@date: 2023-06-20
 *@email: luzhixing12345@163.com
 *@Github: luzhixing12345
 """
 
 import argparse
 from .web_parser import parse_url
-from .site_processor import Error, guess_name_by_url
+import io
+import sys
 
 
 def main():
     
     parser = argparse.ArgumentParser("Markdown Intelligence Url Complete")
     parser.add_argument("-s", "--site", action="store_true", help="add site info")
     parser.add_argument("-t", "--max-time-limit", type=int, default=5, help="max time limit")
@@ -21,13 +22,14 @@
     args = parser.parse_args()
 
     if not args.url:
         print("miuc <url>")
         exit(1)
 
     markdown_url = parse_url(args.url, max_time_limit=args.max_time_limit)
+    sys.stdout = io.TextIOWrapper(sys.stdout.buffer, encoding='utf-8')
     print(markdown_url)
     
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `miuc-0.1.3/miuc/site_processor.py` & `miuc-0.1.4/miuc/site_processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,16 +14,21 @@
 
 
 def guess_name_by_url(url):
     """
     when could not access the website or get the html, guess the name by url
     """
     url_title = re.sub(r"^https?://", "", url)
+    urls = url_title.split(".")
+    if urls[0] == 'www':
+        urls = urls[1:-1]
+    else:
+        urls = urls[:-1]
     # remove top domains
-    url_title = ".".join(url_title.split(".")[:-1])
+    url_title = ".".join(urls)
     return f"[{url_title}]({url})"
 
 
 class Error(Exception):
     def __init__(self, url: str, class_name: str, message: str = None) -> None:  # pragma: no cover
         super().__init__()
         self.url = url
```

### Comparing `miuc-0.1.3/miuc/web_parser.py` & `miuc-0.1.4/miuc/web_parser.py`

 * *Files identical despite different names*

### Comparing `miuc-0.1.3/README.md` & `miuc-0.1.4/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 Markdown Intelligence Url Complete
 
 ## Features
 
 ## Download
 
-Search `miuc` in Vscode extension market or manually download the extension from [miuc-vscode-extension-market]()
+Search `miuc` in Vscode extension market or manually download the extension from [miuc-vscode-extension-market](https://marketplace.visualstudio.com/items?itemName=kamilu.miuc)
 
 If you prefer to use in command line, you could download miuc from PYPI
 
 ```bash
 pip install miuc
 ``` 
 
@@ -22,22 +22,15 @@
 $ miuc <url>
 # [article-title](url)
 
 $ miuc https://github.com/luzhixing12345/miuc
 # [miuc](https://github.com/luzhixing12345/miuc)
 ```
 
-If you prefer to display the site like `Github` or `Stackoverflow`, add argument `-s`
-
-```bash
-$ miuc -s https://github.com/luzhixing12345/miuc
-# [Github miuc](https://github.com/luzhixing12345/miuc)
-```
-
-To customize the title like `[Github - miuc](...)` `[Github:miuc](...)`, see more information from [miuc document]()
+see more information from [miuc document]()
 
 ## Extension Settings
 
 ## Rerference
   
 - [brandmark](https://brandmark.io/)
 - [autopep8](https://github.com/microsoft/vscode-autopep8)
```

### Comparing `miuc-0.1.3/PKG-INFO` & `miuc-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miuc
-Version: 0.1.3
+Version: 0.1.4
 Summary: Markdown Intelligence Url Complete
 Home-page: https://github.com/luzhixing12345/miuc
 License: MIT
 Author: luzhixing12345
 Author-email: luzhixing12345@163.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -23,15 +23,15 @@
 
 Markdown Intelligence Url Complete
 
 ## Features
 
 ## Download
 
-Search `miuc` in Vscode extension market or manually download the extension from [miuc-vscode-extension-market]()
+Search `miuc` in Vscode extension market or manually download the extension from [miuc-vscode-extension-market](https://marketplace.visualstudio.com/items?itemName=kamilu.miuc)
 
 If you prefer to use in command line, you could download miuc from PYPI
 
 ```bash
 pip install miuc
 ``` 
 
@@ -43,22 +43,15 @@
 $ miuc <url>
 # [article-title](url)
 
 $ miuc https://github.com/luzhixing12345/miuc
 # [miuc](https://github.com/luzhixing12345/miuc)
 ```
 
-If you prefer to display the site like `Github` or `Stackoverflow`, add argument `-s`
-
-```bash
-$ miuc -s https://github.com/luzhixing12345/miuc
-# [Github miuc](https://github.com/luzhixing12345/miuc)
-```
-
-To customize the title like `[Github - miuc](...)` `[Github:miuc](...)`, see more information from [miuc document]()
+see more information from [miuc document]()
 
 ## Extension Settings
 
 ## Rerference
   
 - [brandmark](https://brandmark.io/)
 - [autopep8](https://github.com/microsoft/vscode-autopep8)
```


# Comparing `tmp/miuc-0.1.1.tar.gz` & `tmp/miuc-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miuc-0.1.1.tar", max compression
+gzip compressed data, was "miuc-0.1.2.tar", max compression
```

## Comparing `miuc-0.1.1.tar` & `miuc-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       69 2023-06-21 10:51:23.812835 miuc-0.1.1/miuc/__init__.py
--rw-r--r--   0        0        0      689 2023-06-21 10:52:37.677332 miuc-0.1.1/miuc/main.py
--rw-r--r--   0        0        0    14634 2023-06-21 08:52:59.396590 miuc-0.1.1/miuc/pages_processor.py
--rw-r--r--   0        0        0     1556 2023-06-21 10:50:33.824387 miuc-0.1.1/miuc/web_parser.py
--rw-r--r--   0        0        0      508 2023-06-21 11:03:19.051036 miuc-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      906 2023-06-21 06:46:27.503404 miuc-0.1.1/README.md
--rw-r--r--   0        0        0     1697 1970-01-01 00:00:00.000000 miuc-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       45 2023-06-22 13:40:27.802869 miuc-0.1.2/miuc/__init__.py
+-rw-r--r--   0        0        0     1100 2023-06-23 02:46:41.841374 miuc-0.1.2/miuc/main.py
+-rw-r--r--   0        0        0    21040 2023-06-23 03:40:04.984934 miuc-0.1.2/miuc/site_processor.py
+-rw-r--r--   0        0        0     1797 2023-06-23 03:22:17.729965 miuc-0.1.2/miuc/web_parser.py
+-rw-r--r--   0        0        0      508 2023-06-23 05:05:06.610721 miuc-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      967 2023-06-22 14:51:24.993605 miuc-0.1.2/README.md
+-rw-r--r--   0        0        0     1758 1970-01-01 00:00:00.000000 miuc-0.1.2/PKG-INFO
```

### Comparing `miuc-0.1.1/miuc/main.py` & `miuc-0.1.2/miuc/main.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,38 @@
-'''
+"""
 *Copyright (c) 2023 All rights reserved
 *@description: main project
 *@author: Zhixing Lu
 *@date: 2023-06-20
 *@email: luzhixing12345@163.com
 *@Github: luzhixing12345
-'''
+"""
 
 import argparse
 from .web_parser import parse_url
+from .site_processor import Error, guess_name_by_url
+
 
 def main():
-    
     parser = argparse.ArgumentParser("Markdown Intelligence Url Complete")
-    parser.add_argument('-s', '--site', action='store_true', help='add site info')
+    parser.add_argument("-s", "--site", action="store_true", help="add site info")
+    parser.add_argument("-t", "--max-time-limit", type=int, default=0.05, help="max time limit")
     parser.add_argument("url", type=str, help="website url")
     args = parser.parse_args()
 
     if not args.url:
-        print('miuc <url>')
+        print("miuc <url>")
         exit(1)
 
-    markdown_url = parse_url(args.url)
+    try:
+        markdown_url = parse_url(args.url, max_time_limit=args.t)
+    except Exception as e:
+        if type(e) == Error:
+            # cause exception in control
+            markdown_url = guess_name_by_url(args.url)
+        else:
+            markdown_url = f'[unknown]({args.url})'
     print(markdown_url)
 
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `miuc-0.1.1/miuc/pages_processor.py` & `miuc-0.1.2/miuc/site_processor.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,77 +5,92 @@
 *@date: 2023-06-20
 *@email: luzhixing12345@163.com
 *@Github: luzhixing12345
 """
 
 import re
 import requests
+import urllib
+import json
+
+
+def guess_name_by_url(url):
+    """
+    when could not access the website or get the html, guess the name by url
+    """
+    url_title = re.sub(r"^https?://", "", url)
+    # remove top domains
+    url_title = ".".join(url_title.split(".")[:-1])
+    return f"[{url_title}]({url})"
 
 
 class Error(Exception):
     def __init__(self, url: str, class_name: str, message: str = None) -> None:  # pragma: no cover
         super().__init__()
         self.url = url
         self.class_name = class_name
         self.message = message
 
 
 class Processor:
-    def __init__(self, formatting_title: str) -> None:
+    def __init__(self, max_time_limit: int = 5) -> None:
         self.class_name = self.__class__.__name__
-        self.formatting_title = formatting_title
         self.url = None
-        self.max_title_length = 50
+        self.max_time_limit = max_time_limit
+        self.headers = {
+            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36",
+            "Accept-Encoding": "gzip",
+            "Connection": "keep-alive",
+            "Content-Type": "text/html;charset=utf-8",
+        }
 
     def __call__(self, url: str):
         self.url: str = url
         self.parse()
         title = self.format()
-        assert (
-            len(title) < self.max_title_length + 10
-        ), f"title too long > {self.max_title_length}, use abbreviation\ntitle = [{title}]"
         return f"[{title}]({self.url})"
 
     def parse(self) -> str:  # pragma: no cover
         """
         override this function for a specific site processor
 
         parse the url
         """
         raise NotImplementedError(self.class_name + "should override parse function")
 
-    def format(self):  # pragma: no cover
+    def format(self) -> str:  # pragma: no cover
         """
         override this function for a specific site processor
 
         return title
         """
-        return "[unknown]"
+        raise NotImplementedError(self.class_name + "should override parse function")
 
     def error(self, msg: str = None):  # pragma: no cover
         """
         call this function if mismatch
         """
         raise Error(self.url, self.class_name, message=msg)
 
     def get_html(self):
         """
         call this function if could not parse only by url
         """
-        response = requests.get(self.url)
+        response = requests.get(self.url, headers=self.headers, timeout=self.max_time_limit)
         if response.status_code != 200:
+            print("?")
             self.error(f"connect {self.url} failed: status code [{response.status_code}]")
         return response.text
 
 
 class GithubProcessor(Processor):
     # https://github.com/microsoft/vscode
 
-    def __init__(self, formatting_title: str) -> None:
-        super().__init__(formatting_title)
+    def __init__(self, max_time_limit: int = 5) -> None:
+        super().__init__(max_time_limit)
 
         self.site = "Github"
         self.user_name = None
         self.repo_name = None
         self.branch_name = None
         self.file_name = None
         self.tab_name = None
@@ -120,29 +135,70 @@
         self.error()  # pragma: no cover
 
     def format(self):
         if self.repo_name is None and self.user_name is None:
             return f"[{self.site}]({self.url})"
 
         if self.repo_name:
-            name = self.repo_name
+            title = self.repo_name
             if self.file_name:
-                name += f" {self.file_name}"
+                title += f" {self.file_name}"
         else:
-            name = self.user_name
+            title = self.user_name
             if self.tab_name:
-                name += f" {self.tab_name}"
+                title += f" {self.tab_name}"
+
+        return title
+
+
+class GithubioProcessor(Processor):
+    """
+    most likely one's blog or github page document site
+    """
+
+    def __init__(self, max_time_limit: int = 5) -> None:
+        super().__init__(max_time_limit)
+        self.user_name = None
+        self.repo_name = None
+        self.routine = None
+
+        self.urls_re = [
+            re.compile(r"^https://(?P<user>.*?)\.github\.io/?$"),  # blog / resume
+            re.compile(r"^https://(?P<user>.*?)\.github.io/(?P<repo>.*?)/?$"),  # github repo
+            re.compile(r"^https://(?P<user>.*?)\.github.io/(?P<repo>.*?)/(?P<routine>.*?)/?$"),
+        ]
+
+    def parse(self) -> str:
+        for url_re in self.urls_re:
+            res = url_re.match(self.url)
+            if res:
+                if "user" in res.groupdict():
+                    self.user_name = res.group("user")
+                if "repo" in res.groupdict():
+                    self.repo_name = res.group("repo")
+                if "routine" in res.groupdict():
+                    origin_routine = res.group("routine").split("/")[-1]
+                    self.routine = urllib.parse.unquote(origin_routine)
+                return
+        self.error("unknown url")
 
-        title = self.formatting_title.replace("<site>", self.site).replace("<title>", name)
+    def format(self):
+        if self.repo_name is None:
+            title = f"{self.user_name}'s blog"
+        else:
+            if self.routine is None:
+                title = f"{self.repo_name} document"
+            else:
+                title = self.routine
         return title
 
 
 class StackoverflowProcessor(Processor):
-    def __init__(self, formatting_title: str) -> None:
-        super().__init__(formatting_title)
+    def __init__(self, max_time_limit: int = 5) -> None:
+        super().__init__(max_time_limit)
         self.site = "stackoverflow"
 
         self.type_name = None
         self.id = None
         self.tag_name = None
         self.user_name = None
 
@@ -187,48 +243,91 @@
                 elif self.type_name == "a":
                     # answer
                     # https://stackoverflow.com/a/601989/17869889
                     html = self.get_html()
                     pattern = re.compile(r'<a .*class="question-hyperlink">(.*?)</a>')
                     self.question_name = pattern.search(html).group(1)
                     self.is_answer = True
-                elif self.type_name == 'users':
+                elif self.type_name == "users":
                     # https://stackoverflow.com/users/5740428/jan-schultke
                     self.user_name = res.group("question")
                 else:
-                    self.error('unknown type') # pragma: no cover
+                    self.error("unknown type")  # pragma: no cover
                 return
 
     def format(self):
         title = ""
         if self.question_name:
-            if len(self.question_name) >= self.max_title_length:
-                title = f"{self.site}"
-                if self.is_answer:
-                    title += " [answer]"
-                else:
-                    title += " [question]"
+            title = self.question_name
+            if self.is_answer:
+                title += " [answer]"
             else:
-                title = self.question_name
-                if self.is_answer:
-                    title += " [answer]"
+                title += " [question]"
         elif self.tag_name:
             title = f"{self.tag_name} tag"
         elif self.user_name:
-            title = f'{self.user_name}'
+            title = f"{self.user_name}"
         else:
             # pure https://stackoverflow.com/
             title = self.site
 
         return title
 
 
+class YoutubeProcessor(Processor):
+    def __init__(self, max_time_limit: int = 5) -> None:
+        super().__init__(max_time_limit)
+        self.site = "youtube"
+        self.user_name = None
+        self.video_name = None
+        self.urls_re = [
+            re.compile(r"^https://www\.youtube\.com/?$"),
+            re.compile(r"^https://www\.youtube\.com/\@(?P<user>.*?)/?$"),
+            re.compile(r"^https://www\.youtube\.com/\@(?P<user>.*?)/.*$"),
+            re.compile(r"^https://www\.youtube\.com/watch\?v=(?P<id>.*?)/?$"),
+            re.compile(r"^https://youtu\.be/(?P<id>.*?)/?"),
+        ]
+
+        # https://www.youtube.com/watch?v=ErV-2tlf9Ls
+
+    def _get_youtube_title(self):
+        # could not directly get youtube video title, instead use the following method
+        # https://stackoverflow.com/a/52664178/17869889
+
+        params = {"format": "json", "url": self.url}
+        url = f"https://www.youtube.com/oembed?{urllib.parse.urlencode(params)}"
+        response = requests.get(url, timeout=self.max_time_limit)
+        data = json.loads(response.text)
+        return data["title"]
+
+    def parse(self) -> str:
+        for url_re in self.urls_re:
+            res = url_re.match(self.url)
+            if res:
+                if "user" in res.groupdict():
+                    self.user_name = res.group("user")
+                if "id" in res.groupdict():
+                    self.video_name = self._get_youtube_title()
+
+    def format(self):
+        if self.user_name is None and self.video_name is None:
+            # pure youtube
+            title = self.site
+        else:
+            if self.video_name is not None:
+                title = self.video_name
+            if self.user_name is not None:
+                title = self.user_name
+
+        return title
+
+
 class ZhihuProcessor(Processor):
-    def __init__(self, formatting_title: str) -> None:
-        super().__init__(formatting_title)
+    def __init__(self, max_time_limit: int = 5) -> None:
+        super().__init__(max_time_limit)
         self.site = "Zhihu"
         self.type_name = None
         self.title = None
 
         self.urls_re = [
             re.compile(r"^https://www\.zhihu\.com/?$"),
             re.compile(r"^https://www\.zhihu\.com/question/\d+/(?P<type>.*?)/(?P<id>.*?)/?$"),
@@ -308,70 +407,133 @@
         self.error()  # pragma: no cover
 
     def format(self):
         return self.title
 
 
 class BilibiliProcessor(Processor):
-
-    def __init__(self, formatting_title: str) -> None:
-        super().__init__(formatting_title)
+    def __init__(self, max_time_limit: int = 5) -> None:
+        super().__init__(max_time_limit)
         self.site = "bilibli"
         self.type_name = None
         self.user_name = None
         self.id = None
         self.name = None
 
         self.urls_re = [
-            re.compile(r'^https://www\.bilibili\.com/?$'),
-            re.compile(r'^https://www\.bilibili\.com/(?P<type>.*?)/(?P<id>.*?)\?.*$'),
-            re.compile(r'^https://www\.bilibili\.com/(?P<type>.*?)/(?P<id>.*)$'),
+            re.compile(r"^https://www\.bilibili\.com/?$"),
+            re.compile(r"^https://www\.bilibili\.com/(?P<type>.*?)/(?P<id>.*?)\?.*$"),
+            re.compile(r"^https://www\.bilibili\.com/(?P<type>.*?)/(?P<id>.*)$"),
         ]
 
         # https://www.bilibili.com/video/BV1ah4y1X73M
         # https://www.bilibili.com/opus/806593844580712449?spm_id_from=333.999.0.0
         # https://www.bilibili.com/read/cv23285665?spm_id_from=333.999.0.0
 
     def parse(self) -> str:
-        
         for url_re in self.urls_re:
             res = url_re.match(self.url)
 
             if res:
-                
                 if "type" not in res.groupdict():
                     # pure bilibili
                     return
                 self.type_name = res.group("type")
                 self.id = res.group("id")
                 # bilibili url often following with "spm_id_from=333.999.0.0 ..."
                 # clean the url
-                self.url = f'https://www.bilibili.com/{self.type_name}/{self.id}'
-                
+                self.url = f"https://www.bilibili.com/{self.type_name}/{self.id}"
+
                 html = self.get_html()
 
-                if self.type_name == 'video':
-                    pattern = re.compile(r'<h1 .*>(.*?)</h1>')
+                if self.type_name == "video":
+                    pattern = re.compile(r"<h1 .*>(.*?)</h1>")
                     self.name = pattern.search(html).group(1)
-                elif self.type_name == 'opus':
+                elif self.type_name == "opus":
                     pass
-                elif self.type_name == 'read':
+                elif self.type_name == "read":
                     pattern = re.compile(r'<title data-vue-meta="true">(.*?)</title>')
-                    self.name = pattern.search(html).group(1).replace(' - 哔哩哔哩','')
+                    self.name = pattern.search(html).group(1).replace(" - 哔哩哔哩", "")
                 return
 
     def format(self):
-
         if self.type_name is None:
             # pure bilibili
             title = self.site
         else:
-            if self.type_name == 'video':
+            if self.type_name == "video":
                 title = self.name
-            elif self.type_name == 'opus':
-                title = f'B站动态'
-            elif self.type_name == 'read':
-                title = f'{self.name} 专栏'
+            elif self.type_name == "opus":
+                title = f"B站动态"
+            elif self.type_name == "read":
+                title = f"{self.name} 专栏"
             else:
-                self.error("unknown type") # pragma: no cover
+                self.error("unknown type")  # pragma: no cover
+
+        return title
+
+
+class CSDNProcessor(Processor):
+    def __init__(self, max_time_limit: int = 5) -> None:
+        super().__init__(max_time_limit)
+        self.site = "csdn"
+        self.user_id = None
+        self.user_name = None
+        self.article_id = None
+        self.article_name = None
+
+        self.urls_re = [
+            re.compile(r"^https://blog\.csdn\.net/?$"),
+            re.compile(r"^https://blog\.csdn\.net/(?P<user_id>.*?)/(?P<category>.*?)\.html$"),
+            re.compile(r"^https://blog\.csdn\.net/(?P<user_id>.*?)\?type=.*$"),
+            re.compile(
+                r"^https://blog\.csdn\.net/(?P<user_id>.*?)/article/details/(?P<article_id>.*?)\?.*$"
+            ),
+            re.compile(
+                r"^https://blog\.csdn\.net/(?P<user_id>.*?)/article/details/(?P<article_id>.*?)$"
+            ),
+            re.compile(r"^http://t\.csdn\.cn/(?P<short_id>.*?)$"),
+        ]
+
+    def parse(self) -> str:
+        for url_re in self.urls_re:
+            res = url_re.match(self.url)
+            if res:
+                if "user_id" not in res.groupdict() and "short_id" not in res.groupdict():
+                    return
+
+                html = self.get_html()
+                # with open("a.txt",'w',encoding='utf-8') as f:
+                #     f.write(html)
+
+                if "article_id" in res.groupdict():
+                    self.user_id = res.group("user_id")
+                    self.article_id = res.group("article_id")
+                    # clean the url
+                    self.url = (
+                        f"https://blog.csdn.net/{self.user_id}/article/details/{self.article_id}"
+                    )
+                    pattern = re.compile(r'<meta name="keywords" content="(.*?)">')
+                    self.article_name = pattern.search(html).group(1)
+                elif "category" in res.groupdict():
+                    pattern = re.compile(r'<h3 class="column_title oneline" title=.*>(.*?)</h3>')
+                    self.article_name = pattern.search(html).group(1)
+                elif "short_id" in res.groupdict():
+                    # for short url
+
+                    pattern = re.compile(r'<meta name="keywords" content="(.*?)">')
+                    self.article_name = pattern.search(html).group(1)
+                else:
+                    # for user home page
+                    pattern = re.compile(r'data-nickname="(.*?)"')
+                    self.user_name = pattern.search(html).group(1)
+                return
 
-        return title
+    def format(self) -> str:
+        if self.user_name is None and self.article_name is None:
+            title = self.site
+        else:
+            if self.article_name:
+                title = self.article_name
+            else:
+                title = self.user_name
+        return title
```

### Comparing `miuc-0.1.1/README.md` & `miuc-0.1.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -34,9 +34,10 @@
 ```
 
 To customize the title like `[Github - miuc](...)` `[Github:miuc](...)`, see more information from [miuc document]()
 
 ## Extension Settings
 
 ## Rerference
-
+  
 - [brandmark](https://brandmark.io/)
+- [autopep8](https://github.com/microsoft/vscode-autopep8)
```

### Comparing `miuc-0.1.1/PKG-INFO` & `miuc-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miuc
-Version: 0.1.1
+Version: 0.1.2
 Summary: Markdown Intelligence Url Complete
 Home-page: https://github.com/luzhixing12345/miuc
 License: MIT
 Author: luzhixing12345
 Author-email: luzhixing12345@163.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -55,10 +55,11 @@
 ```
 
 To customize the title like `[Github - miuc](...)` `[Github:miuc](...)`, see more information from [miuc document]()
 
 ## Extension Settings
 
 ## Rerference
-
+  
 - [brandmark](https://brandmark.io/)
+- [autopep8](https://github.com/microsoft/vscode-autopep8)
```


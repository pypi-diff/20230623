# Comparing `tmp/jmcomic-2.0.5.tar.gz` & `tmp/jmcomic-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jmcomic-2.0.5.tar", last modified: Tue Jun 20 07:54:42 2023, max compression
+gzip compressed data, was "jmcomic-2.0.6.tar", last modified: Fri Jun 23 06:32:58 2023, max compression
```

## Comparing `jmcomic-2.0.5.tar` & `jmcomic-2.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:54:42.889842 jmcomic-2.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-20 07:54:30.000000 jmcomic-2.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-20 07:54:42.889842 jmcomic-2.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-20 07:54:30.000000 jmcomic-2.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 07:54:42.889842 jmcomic-2.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-20 07:54:30.000000 jmcomic-2.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:54:42.889842 jmcomic-2.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:54:42.889842 jmcomic-2.0.5/src/jmcomic/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-20 07:54:30.000000 jmcomic-2.0.5/src/jmcomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-06-20 07:54:30.000000 jmcomic-2.0.5/src/jmcomic/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10552 2023-06-20 07:54:30.000000 jmcomic-2.0.5/src/jmcomic/jm_client_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-06-20 07:54:30.000000 jmcomic-2.0.5/src/jmcomic/jm_client_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-06-20 07:54:30.000000 jmcomic-2.0.5/src/jmcomic/jm_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9152 2023-06-20 07:54:30.000000 jmcomic-2.0.5/src/jmcomic/jm_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-06-20 07:54:30.000000 jmcomic-2.0.5/src/jmcomic/jm_option.py
--rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-06-20 07:54:30.000000 jmcomic-2.0.5/src/jmcomic/jm_toolkit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:54:42.889842 jmcomic-2.0.5/src/jmcomic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-20 07:54:42.000000 jmcomic-2.0.5/src/jmcomic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-20 07:54:42.000000 jmcomic-2.0.5/src/jmcomic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 07:54:42.000000 jmcomic-2.0.5/src/jmcomic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-20 07:54:42.000000 jmcomic-2.0.5/src/jmcomic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 07:54:42.000000 jmcomic-2.0.5/src/jmcomic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:32:58.581547 jmcomic-2.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-23 06:32:49.000000 jmcomic-2.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-23 06:32:58.581547 jmcomic-2.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-23 06:32:49.000000 jmcomic-2.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 06:32:58.581547 jmcomic-2.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-23 06:32:49.000000 jmcomic-2.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:32:58.577546 jmcomic-2.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:32:58.581547 jmcomic-2.0.6/src/jmcomic/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-23 06:32:49.000000 jmcomic-2.0.6/src/jmcomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-06-23 06:32:49.000000 jmcomic-2.0.6/src/jmcomic/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-06-23 06:32:49.000000 jmcomic-2.0.6/src/jmcomic/jm_client_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-06-23 06:32:49.000000 jmcomic-2.0.6/src/jmcomic/jm_client_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-06-23 06:32:49.000000 jmcomic-2.0.6/src/jmcomic/jm_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9152 2023-06-23 06:32:49.000000 jmcomic-2.0.6/src/jmcomic/jm_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-06-23 06:32:49.000000 jmcomic-2.0.6/src/jmcomic/jm_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11284 2023-06-23 06:32:49.000000 jmcomic-2.0.6/src/jmcomic/jm_toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:32:58.581547 jmcomic-2.0.6/src/jmcomic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-23 06:32:58.000000 jmcomic-2.0.6/src/jmcomic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-23 06:32:58.000000 jmcomic-2.0.6/src/jmcomic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 06:32:58.000000 jmcomic-2.0.6/src/jmcomic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 06:32:58.000000 jmcomic-2.0.6/src/jmcomic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-23 06:32:58.000000 jmcomic-2.0.6/src/jmcomic.egg-info/top_level.txt
```

### Comparing `jmcomic-2.0.5/LICENSE` & `jmcomic-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.5/PKG-INFO` & `jmcomic-2.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcomic
-Version: 2.0.5
+Version: 2.0.6
 Summary: Python API For JMComic (禁漫天堂)
 Home-page: https://github.com/hect0x7/JMComic-Crawler-Python
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `jmcomic-2.0.5/README.md` & `jmcomic-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.5/setup.py` & `jmcomic-2.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.5/src/jmcomic/api.py` & `jmcomic-2.0.6/src/jmcomic/api.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.5/src/jmcomic/jm_client_impl.py` & `jmcomic-2.0.6/src/jmcomic/jm_client_impl.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,17 +91,26 @@
                 cache_dict=cache_dict,
                 cache_hit_msg=cache_hit_msg,
                 cache_miss_msg=cache_miss_msg,
             )(func)
 
             setattr(self, func_name, wrap_func)
 
-        wrap_func_cache('get_photo_detail', 'album_cache_dict')
-        wrap_func_cache('get_album_detail', 'photo_cache_dict')
-        wrap_func_cache('search_album', 'search_album_cache_dict')
+        for func in {
+            'get_photo_detail',
+            'get_album_detail',
+            'search_album',
+        }:
+            wrap_func_cache(func, func + '.cache.dict')
+
+    def get_jmcomic_url(self, postman=None):
+        return JmModuleConfig.get_jmcomic_url(postman or self.get_root_postman())
+
+    def get_jmcomic_domain_all(self, postman=None):
+        return JmModuleConfig.get_jmcomic_domain_all(postman or self.get_root_postman())
 
 
 # 基于网页实现的JmClient
 class JmHtmlClient(AbstractJmClient):
 
     def get_album_detail(self, album_id) -> JmAlbumDetail:
         # 参数校验
```

### Comparing `jmcomic-2.0.5/src/jmcomic/jm_client_interface.py` & `jmcomic-2.0.6/src/jmcomic/jm_client_interface.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.5/src/jmcomic/jm_config.py` & `jmcomic-2.0.6/src/jmcomic/jm_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,29 @@
 def default_jm_debug(topic: str, msg: str):
     from common import format_ts
     print(f'{format_ts()}:【{topic}】{msg}')
 
 
+def default_postman_constructor(session, **kwargs):
+    from common import Postmans
+
+    kwargs.setdefault('impersonate', 'chrome110')
+    kwargs.setdefault('headers', JmModuleConfig.headers())
+
+    if session is True:
+        return Postmans.new_session(**kwargs)
+
+    return Postmans.new_postman(**kwargs)
+
+
 class JmModuleConfig:
     # 网站相关
     PROT = "https://"
     DOMAIN = None
-    JM_REDIRECT_URL = f'{PROT}jm365.xyz/3YeBdF'  # 永久網域，怕走失的小伙伴收藏起来
+    JM_REDIRECT_URL = f'{PROT}jm365.work/3YeBdF'  # 永久網域，怕走失的小伙伴收藏起来
     JM_PUB_URL = f'{PROT}jmcomic2.bet'
     JM_CDN_IMAGE_URL_TEMPLATE = PROT + 'cdn-msp.{domain}/media/photos/{photo_id}/{index:05}{suffix}'  # index 从1开始
     JM_IMAGE_SUFFIX = ['.jpg', '.webp', '.png', '.gif']
 
     # 访问JM可能会遇到的异常网页
     JM_ERROR_RESPONSE_TEXT = {
         "Could not connect to mysql! Please check your database settings!": "禁漫服务器内部报错",
@@ -36,14 +48,15 @@
     default_author = 'default-author'
     default_photo_title = 'default-photo-title'
     default_photo_id = 'default-photo-id'
 
     # debug
     enable_jm_debug = True
     debug_executor = default_jm_debug
+    postman_constructor = default_postman_constructor
 
     @classmethod
     def domain(cls, postman=None):
         """
         由于禁漫的域名经常变化，调用此方法可以获取一个当前可用的最新的域名 domain，
         并且设置把 domain 设置为禁漫模块的默认域名。
         这样一来，配置文件也不用配置域名了，一切都在运行时动态获取。
@@ -81,37 +94,37 @@
             cls.debug_executor(topic, msg)
 
     @classmethod
     def disable_jm_debug(cls):
         cls.enable_jm_debug = False
 
     @classmethod
+    def new_postman(cls, session=False, **kwargs):
+        return cls.postman_constructor(session, **kwargs)
+
+    @classmethod
     def get_jmcomic_url(cls, postman=None):
         """
         访问禁漫的永久网域，从而得到一个可用的禁漫网址
         @return: https://jm-comic2.cc
         """
-        if postman is None:
-            from common import Postmans
-            postman = Postmans.new_session()
+        postman = postman or cls.new_postman(session=True)
 
         resp = postman.get(cls.JM_REDIRECT_URL)
         url = resp.url
         cls.jm_debug('获取禁漫地址', f'[{cls.JM_REDIRECT_URL}] → [{url}]')
         return url
 
     @classmethod
     def get_jmcomic_domain_all(cls, postman=None):
         """
         访问禁漫发布页，得到所有禁漫的域名
         @return：['18comic.vip', ..., 'jm365.xyz/ZNPJam'], 最后一个是【APP軟件下載】
         """
-        if postman is None:
-            from common import Postmans
-            postman = Postmans.get_impl_clazz('cffi').create()
+        postman = postman or cls.new_postman(session=True)
 
         resp = postman.get(cls.JM_PUB_URL)
         if resp.status_code != 200:
             raise AssertionError(resp.text)
 
         from .jm_toolkit import JmcomicText
         return JmcomicText.analyse_jm_pub_html(resp.text)
```

### Comparing `jmcomic-2.0.5/src/jmcomic/jm_entity.py` & `jmcomic-2.0.6/src/jmcomic/jm_entity.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.5/src/jmcomic/jm_option.py` & `jmcomic-2.0.6/src/jmcomic/jm_option.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.5/src/jmcomic/jm_toolkit.py` & `jmcomic-2.0.6/src/jmcomic/jm_toolkit.py`

 * *Files identical despite different names*

### Comparing `jmcomic-2.0.5/src/jmcomic.egg-info/PKG-INFO` & `jmcomic-2.0.6/src/jmcomic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jmcomic
-Version: 2.0.5
+Version: 2.0.6
 Summary: Python API For JMComic (禁漫天堂)
 Home-page: https://github.com/hect0x7/JMComic-Crawler-Python
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```


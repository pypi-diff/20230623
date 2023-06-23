# Comparing `tmp/divinegift-2.9.2.1.tar.gz` & `tmp/divinegift-2.9.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/divinegift-2.9.2.1.tar", last modified: Tue Nov  9 04:36:01 2021, max compression
+gzip compressed data, was "dist/divinegift-2.9.2.2.tar", last modified: Tue Nov  9 04:37:51 2021, max compression
```

## Comparing `divinegift-2.9.2.1.tar` & `divinegift-2.9.2.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 malanris   (501) staff       (20)        0 2021-11-09 04:36:01.810456 divinegift-2.9.2.1/
--rw-r--r--   0 malanris   (501) staff       (20)    21230 2021-11-09 04:36:01.810087 divinegift-2.9.2.1/PKG-INFO
--rw-r--r--   0 malanris   (501) staff       (20)    16101 2021-03-19 03:17:56.000000 divinegift-2.9.2.1/README.md
-drwxr-xr-x   0 malanris   (501) staff       (20)        0 2021-11-09 04:36:01.806441 divinegift-2.9.2.1/divinegift/
--rw-r--r--   0 malanris   (501) staff       (20)      286 2021-11-09 04:35:57.000000 divinegift-2.9.2.1/divinegift/__init__.py
--rw-r--r--   0 malanris   (501) staff       (20)     3437 2021-06-10 02:49:42.000000 divinegift-2.9.2.1/divinegift/aims.py
--rw-r--r--   0 malanris   (501) staff       (20)     3482 2021-11-09 04:30:53.000000 divinegift-2.9.2.1/divinegift/app.py
--rw-r--r--   0 malanris   (501) staff       (20)     2771 2020-04-06 06:18:22.000000 divinegift-2.9.2.1/divinegift/banner.py
--rw-r--r--   0 malanris   (501) staff       (20)     2044 2021-04-07 03:51:17.000000 divinegift-2.9.2.1/divinegift/cipher.py
--rw-r--r--   0 malanris   (501) staff       (20)     6517 2021-11-09 04:35:57.000000 divinegift-2.9.2.1/divinegift/config.py
--rw-r--r--   0 malanris   (501) staff       (20)     8966 2021-11-01 03:13:20.000000 divinegift-2.9.2.1/divinegift/db.py
--rw-r--r--   0 malanris   (501) staff       (20)      391 2021-06-10 02:49:42.000000 divinegift-2.9.2.1/divinegift/errors.py
--rw-r--r--   0 malanris   (501) staff       (20)    22631 2021-08-02 05:59:58.000000 divinegift-2.9.2.1/divinegift/excel.py
--rw-r--r--   0 malanris   (501) staff       (20)     5705 2021-09-15 05:14:48.000000 divinegift-2.9.2.1/divinegift/kafka_client.py
--rw-r--r--   0 malanris   (501) staff       (20)     1261 2021-09-09 09:23:47.000000 divinegift-2.9.2.1/divinegift/kthreads.py
--rw-r--r--   0 malanris   (501) staff       (20)     6370 2021-09-09 09:23:47.000000 divinegift-2.9.2.1/divinegift/logger.py
--rw-r--r--   0 malanris   (501) staff       (20)    12685 2021-10-27 06:06:41.000000 divinegift-2.9.2.1/divinegift/main.py
--rw-r--r--   0 malanris   (501) staff       (20)     7412 2021-09-09 09:44:46.000000 divinegift-2.9.2.1/divinegift/sender.py
--rw-r--r--   0 malanris   (501) staff       (20)     1266 2020-10-08 03:18:04.000000 divinegift-2.9.2.1/divinegift/string_avro.py
--rw-r--r--   0 malanris   (501) staff       (20)     1774 2020-10-08 03:17:30.000000 divinegift-2.9.2.1/divinegift/telegram.py
--rw-r--r--   0 malanris   (501) staff       (20)     7790 2021-08-24 03:54:21.000000 divinegift-2.9.2.1/divinegift/templator.py
--rw-r--r--   0 malanris   (501) staff       (20)     2910 2021-09-09 09:23:47.000000 divinegift-2.9.2.1/divinegift/timer.py
--rw-r--r--   0 malanris   (501) staff       (20)     2668 2021-08-24 03:54:21.000000 divinegift-2.9.2.1/divinegift/translit.py
--rw-r--r--   0 malanris   (501) staff       (20)     1060 2021-09-09 08:22:07.000000 divinegift-2.9.2.1/divinegift/zabbix_agent.py
-drwxr-xr-x   0 malanris   (501) staff       (20)        0 2021-11-09 04:36:01.809397 divinegift-2.9.2.1/divinegift.egg-info/
--rw-r--r--   0 malanris   (501) staff       (20)    21230 2021-11-09 04:36:01.000000 divinegift-2.9.2.1/divinegift.egg-info/PKG-INFO
--rw-r--r--   0 malanris   (501) staff       (20)      655 2021-11-09 04:36:01.000000 divinegift-2.9.2.1/divinegift.egg-info/SOURCES.txt
--rw-r--r--   0 malanris   (501) staff       (20)        1 2021-11-09 04:36:01.000000 divinegift-2.9.2.1/divinegift.egg-info/dependency_links.txt
--rw-r--r--   0 malanris   (501) staff       (20)        1 2021-11-09 04:36:01.000000 divinegift-2.9.2.1/divinegift.egg-info/not-zip-safe
--rw-r--r--   0 malanris   (501) staff       (20)       69 2021-11-09 04:36:01.000000 divinegift-2.9.2.1/divinegift.egg-info/requires.txt
--rw-r--r--   0 malanris   (501) staff       (20)       11 2021-11-09 04:36:01.000000 divinegift-2.9.2.1/divinegift.egg-info/top_level.txt
--rw-r--r--   0 malanris   (501) staff       (20)       38 2021-11-09 04:36:01.810556 divinegift-2.9.2.1/setup.cfg
--rw-r--r--   0 malanris   (501) staff       (20)     1176 2021-11-09 04:30:53.000000 divinegift-2.9.2.1/setup.py
+drwxr-xr-x   0 malanris   (501) staff       (20)        0 2021-11-09 04:37:51.881946 divinegift-2.9.2.2/
+-rw-r--r--   0 malanris   (501) staff       (20)    21230 2021-11-09 04:37:51.881455 divinegift-2.9.2.2/PKG-INFO
+-rw-r--r--   0 malanris   (501) staff       (20)    16101 2021-03-19 03:17:56.000000 divinegift-2.9.2.2/README.md
+drwxr-xr-x   0 malanris   (501) staff       (20)        0 2021-11-09 04:37:51.876201 divinegift-2.9.2.2/divinegift/
+-rw-r--r--   0 malanris   (501) staff       (20)      286 2021-11-09 04:37:48.000000 divinegift-2.9.2.2/divinegift/__init__.py
+-rw-r--r--   0 malanris   (501) staff       (20)     3437 2021-06-10 02:49:42.000000 divinegift-2.9.2.2/divinegift/aims.py
+-rw-r--r--   0 malanris   (501) staff       (20)     3482 2021-11-09 04:30:53.000000 divinegift-2.9.2.2/divinegift/app.py
+-rw-r--r--   0 malanris   (501) staff       (20)     2771 2020-04-06 06:18:22.000000 divinegift-2.9.2.2/divinegift/banner.py
+-rw-r--r--   0 malanris   (501) staff       (20)     2044 2021-04-07 03:51:17.000000 divinegift-2.9.2.2/divinegift/cipher.py
+-rw-r--r--   0 malanris   (501) staff       (20)     6493 2021-11-09 04:37:42.000000 divinegift-2.9.2.2/divinegift/config.py
+-rw-r--r--   0 malanris   (501) staff       (20)     8966 2021-11-01 03:13:20.000000 divinegift-2.9.2.2/divinegift/db.py
+-rw-r--r--   0 malanris   (501) staff       (20)      391 2021-06-10 02:49:42.000000 divinegift-2.9.2.2/divinegift/errors.py
+-rw-r--r--   0 malanris   (501) staff       (20)    22631 2021-08-02 05:59:58.000000 divinegift-2.9.2.2/divinegift/excel.py
+-rw-r--r--   0 malanris   (501) staff       (20)     5705 2021-09-15 05:14:48.000000 divinegift-2.9.2.2/divinegift/kafka_client.py
+-rw-r--r--   0 malanris   (501) staff       (20)     1261 2021-09-09 09:23:47.000000 divinegift-2.9.2.2/divinegift/kthreads.py
+-rw-r--r--   0 malanris   (501) staff       (20)     6370 2021-09-09 09:23:47.000000 divinegift-2.9.2.2/divinegift/logger.py
+-rw-r--r--   0 malanris   (501) staff       (20)    12685 2021-10-27 06:06:41.000000 divinegift-2.9.2.2/divinegift/main.py
+-rw-r--r--   0 malanris   (501) staff       (20)     7412 2021-09-09 09:44:46.000000 divinegift-2.9.2.2/divinegift/sender.py
+-rw-r--r--   0 malanris   (501) staff       (20)     1266 2020-10-08 03:18:04.000000 divinegift-2.9.2.2/divinegift/string_avro.py
+-rw-r--r--   0 malanris   (501) staff       (20)     1774 2020-10-08 03:17:30.000000 divinegift-2.9.2.2/divinegift/telegram.py
+-rw-r--r--   0 malanris   (501) staff       (20)     7790 2021-08-24 03:54:21.000000 divinegift-2.9.2.2/divinegift/templator.py
+-rw-r--r--   0 malanris   (501) staff       (20)     2910 2021-09-09 09:23:47.000000 divinegift-2.9.2.2/divinegift/timer.py
+-rw-r--r--   0 malanris   (501) staff       (20)     2668 2021-08-24 03:54:21.000000 divinegift-2.9.2.2/divinegift/translit.py
+-rw-r--r--   0 malanris   (501) staff       (20)     1060 2021-09-09 08:22:07.000000 divinegift-2.9.2.2/divinegift/zabbix_agent.py
+drwxr-xr-x   0 malanris   (501) staff       (20)        0 2021-11-09 04:37:51.880629 divinegift-2.9.2.2/divinegift.egg-info/
+-rw-r--r--   0 malanris   (501) staff       (20)    21230 2021-11-09 04:37:51.000000 divinegift-2.9.2.2/divinegift.egg-info/PKG-INFO
+-rw-r--r--   0 malanris   (501) staff       (20)      655 2021-11-09 04:37:51.000000 divinegift-2.9.2.2/divinegift.egg-info/SOURCES.txt
+-rw-r--r--   0 malanris   (501) staff       (20)        1 2021-11-09 04:37:51.000000 divinegift-2.9.2.2/divinegift.egg-info/dependency_links.txt
+-rw-r--r--   0 malanris   (501) staff       (20)        1 2021-11-09 04:37:51.000000 divinegift-2.9.2.2/divinegift.egg-info/not-zip-safe
+-rw-r--r--   0 malanris   (501) staff       (20)       69 2021-11-09 04:37:51.000000 divinegift-2.9.2.2/divinegift.egg-info/requires.txt
+-rw-r--r--   0 malanris   (501) staff       (20)       11 2021-11-09 04:37:51.000000 divinegift-2.9.2.2/divinegift.egg-info/top_level.txt
+-rw-r--r--   0 malanris   (501) staff       (20)       38 2021-11-09 04:37:51.882148 divinegift-2.9.2.2/setup.cfg
+-rw-r--r--   0 malanris   (501) staff       (20)     1176 2021-11-09 04:30:53.000000 divinegift-2.9.2.2/setup.py
```

### Comparing `divinegift-2.9.2.1/PKG-INFO` & `divinegift-2.9.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: divinegift
-Version: 2.9.2.1
+Version: 2.9.2.2
 Summary: Ver.2.9.2. EasyDict was removed due it could not use int and none as key.
 Home-page: https://gitlab.com/gng-group/divinegift.git
 Author: Malanris
 Author-email: admin@malanris.ru
 License: MIT
 Description: **The most useful package for you, young s7_it programer :)**
```

### Comparing `divinegift-2.9.2.1/README.md` & `divinegift-2.9.2.2/README.md`

 * *Files identical despite different names*

### Comparing `divinegift-2.9.2.1/divinegift/aims.py` & `divinegift-2.9.2.2/divinegift/aims.py`

 * *Files identical despite different names*

### Comparing `divinegift-2.9.2.1/divinegift/app.py` & `divinegift-2.9.2.2/divinegift/app.py`

 * *Files identical despite different names*

### Comparing `divinegift-2.9.2.1/divinegift/banner.py` & `divinegift-2.9.2.2/divinegift/banner.py`

 * *Files identical despite different names*

### Comparing `divinegift-2.9.2.1/divinegift/cipher.py` & `divinegift-2.9.2.2/divinegift/cipher.py`

 * *Files identical despite different names*

### Comparing `divinegift-2.9.2.1/divinegift/config.py` & `divinegift-2.9.2.2/divinegift/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 from divinegift.errors import EmptyConfigError
 
 
 class Settings:
     parse_settings_cnt = 0
 
     def __init__(self, logger_: logger.Logger = None):
-        self.settings: Optional[dict] = None
-        self.settings_encrypted: Optional[dict] = None
+        self.settings: dict = {}
+        self.settings_encrypted: dict = {}
         self.cipher_key = None
         self.cipher_key_fname = None
         self.passwords_cnt = 0
         self.logger = logger_ if logger_ else logger.Logger()
 
     def get_settings(self, param: str = None, default: Union[str, list, dict, bool] = None):
         if param:
```

### Comparing `divinegift-2.9.2.1/divinegift/db.py` & `divinegift-2.9.2.2/divinegift/db.py`

 * *Files identical despite different names*

### Comparing `divinegift-2.9.2.1/divinegift/excel.py` & `divinegift-2.9.2.2/divinegift/excel.py`

 * *Files identical despite different names*

### Comparing `divinegift-2.9.2.1/divinegift/kafka_client.py` & `divinegift-2.9.2.2/divinegift/kafka_client.py`

 * *Files identical despite different names*

### Comparing `divinegift-2.9.2.1/divinegift/kthreads.py` & `divinegift-2.9.2.2/divinegift/kthreads.py`

 * *Files identical despite different names*

### Comparing `divinegift-2.9.2.1/divinegift/logger.py` & `divinegift-2.9.2.2/divinegift/logger.py`

 * *Files identical despite different names*

### Comparing `divinegift-2.9.2.1/divinegift/main.py` & `divinegift-2.9.2.2/divinegift/main.py`

 * *Files identical despite different names*

### Comparing `divinegift-2.9.2.1/divinegift/sender.py` & `divinegift-2.9.2.2/divinegift/sender.py`

 * *Files identical despite different names*

### Comparing `divinegift-2.9.2.1/divinegift/string_avro.py` & `divinegift-2.9.2.2/divinegift/string_avro.py`

 * *Files identical despite different names*

### Comparing `divinegift-2.9.2.1/divinegift/telegram.py` & `divinegift-2.9.2.2/divinegift/telegram.py`

 * *Files identical despite different names*

### Comparing `divinegift-2.9.2.1/divinegift/templator.py` & `divinegift-2.9.2.2/divinegift/templator.py`

 * *Files identical despite different names*

### Comparing `divinegift-2.9.2.1/divinegift/timer.py` & `divinegift-2.9.2.2/divinegift/timer.py`

 * *Files identical despite different names*

### Comparing `divinegift-2.9.2.1/divinegift/translit.py` & `divinegift-2.9.2.2/divinegift/translit.py`

 * *Files identical despite different names*

### Comparing `divinegift-2.9.2.1/divinegift/zabbix_agent.py` & `divinegift-2.9.2.2/divinegift/zabbix_agent.py`

 * *Files identical despite different names*

### Comparing `divinegift-2.9.2.1/divinegift.egg-info/PKG-INFO` & `divinegift-2.9.2.2/divinegift.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: divinegift
-Version: 2.9.2.1
+Version: 2.9.2.2
 Summary: Ver.2.9.2. EasyDict was removed due it could not use int and none as key.
 Home-page: https://gitlab.com/gng-group/divinegift.git
 Author: Malanris
 Author-email: admin@malanris.ru
 License: MIT
 Description: **The most useful package for you, young s7_it programer :)**
```

### Comparing `divinegift-2.9.2.1/divinegift.egg-info/SOURCES.txt` & `divinegift-2.9.2.2/divinegift.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `divinegift-2.9.2.1/setup.py` & `divinegift-2.9.2.2/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/yeref-0.2.2.tar.gz` & `tmp/yeref-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.2.2.tar", last modified: Wed Jun 21 12:17:20 2023, max compression
+gzip compressed data, was "yeref-0.2.3.tar", last modified: Fri Jun 23 11:56:39 2023, max compression
```

## Comparing `yeref-0.2.2.tar` & `yeref-0.2.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-21 12:17:20.873908 yeref-0.2.2/
--rw-r--r--   0 mark       (501) staff       (20)       84 2023-06-21 12:17:20.874122 yeref-0.2.2/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-21 12:17:20.874973 yeref-0.2.2/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1390 2023-06-21 12:16:57.000000 yeref-0.2.2/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-21 12:17:20.868009 yeref-0.2.2/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.2.2/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   558227 2023-06-21 12:16:57.000000 yeref-0.2.2/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   210940 2023-06-19 18:18:21.000000 yeref-0.2.2/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-21 12:17:20.873318 yeref-0.2.2/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       84 2023-06-21 12:17:20.000000 yeref-0.2.2/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-21 12:17:20.000000 yeref-0.2.2/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-21 12:17:20.000000 yeref-0.2.2/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-21 12:17:20.000000 yeref-0.2.2/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-23 11:56:39.373111 yeref-0.2.3/
+-rw-r--r--   0 mark       (501) staff       (20)       84 2023-06-23 11:56:39.373268 yeref-0.2.3/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-23 11:56:39.374089 yeref-0.2.3/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1390 2023-06-23 11:56:08.000000 yeref-0.2.3/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-23 11:56:39.364274 yeref-0.2.3/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.2.3/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   558227 2023-06-21 12:16:57.000000 yeref-0.2.3/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   210956 2023-06-21 16:51:06.000000 yeref-0.2.3/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-23 11:56:39.372494 yeref-0.2.3/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       84 2023-06-23 11:56:39.000000 yeref-0.2.3/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-23 11:56:39.000000 yeref-0.2.3/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-23 11:56:39.000000 yeref-0.2.3/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-23 11:56:39.000000 yeref-0.2.3/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.2.2/setup.py` & `yeref-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.2.02',
+      version='0.2.03',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
```

### Comparing `yeref-0.2.2/yeref/l_.py` & `yeref-0.2.3/yeref/l_.py`

 * *Files identical despite different names*

### Comparing `yeref-0.2.2/yeref/yeref.py` & `yeref-0.2.3/yeref/yeref.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
 
 markupAdmin = types.ReplyKeyboardMarkup(keyboard=[
     [types.KeyboardButton(text='⬅️ Prev'), types.KeyboardButton(text='↩️ Menu'),
      types.KeyboardButton(text='➡️️ Next')]], resize_keyboard=True, selective=True, row_width=3)
 
 BOT_VARS_ = '{"BOT_PROMO": "#911", "BOT_CHANNEL": 0, "BOT_CHANNELTID": 0, "BOT_GROUP": 0, "BOT_GROUPTID": 0, "BOT_TZ": 0, "BOT_TZ": 0, "BOT_DT": "", "BOT_LZ": "en", "BOT_LC": "en"}'
 BOT_LSTS_ = '{"BOT_ADMINS": []}'
-USER_VARS_ = '{"USER_TEXT": "", "USER_EMAIL": "", "USER_PROMO": "", "USER_PHONE": "", "USER_GEO": "", "USER_UTM": "", "USER_ID": 0, "USER_DT": "", "USER_TZ": 0, "USER_LC": "en", "USER_ISADMIN": 0, "USER_ISPREMIUM": 0, "USER_BALL": 0, "USER_RAND": 0, "USER_QUIZ": 0, "USER_DICE": 0, "USER_PAY": 0, "DATE_TIME": 0}'
+USER_VARS_ = '{"USER_TEXT": "", "USER_PUSH": "", USER_EMAIL": "", "USER_PROMO": "", "USER_PHONE": "", "USER_GEO": "", "USER_UTM": "", "USER_ID": 0, "USER_DT": "", "USER_TZ": 0, "USER_LC": "en", "USER_ISADMIN": 0, "USER_ISPREMIUM": 0, "USER_BALL": 0, "USER_RAND": 0, "USER_QUIZ": 0, "USER_DICE": 0, "USER_PAY": 0, "DATE_TIME": 0}'
 USER_LSTS_ = '{"USER_UTMREF": []}'
 # endregion
 
 
 # region db
 def sqlite_lower(value_):
     return value_.lower() if value_ else None
```


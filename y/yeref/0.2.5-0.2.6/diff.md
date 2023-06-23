# Comparing `tmp/yeref-0.2.5.tar.gz` & `tmp/yeref-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.2.5.tar", last modified: Fri Jun 23 16:32:55 2023, max compression
+gzip compressed data, was "yeref-0.2.6.tar", last modified: Fri Jun 23 16:53:05 2023, max compression
```

## Comparing `yeref-0.2.5.tar` & `yeref-0.2.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-23 16:32:55.440592 yeref-0.2.5/
--rw-r--r--   0 mark       (501) staff       (20)       84 2023-06-23 16:32:55.440921 yeref-0.2.5/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-23 16:32:55.441697 yeref-0.2.5/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1390 2023-06-23 16:32:42.000000 yeref-0.2.5/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-23 16:32:55.434059 yeref-0.2.5/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.2.5/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   558227 2023-06-21 12:16:57.000000 yeref-0.2.5/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   211217 2023-06-23 16:32:42.000000 yeref-0.2.5/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-23 16:32:55.439866 yeref-0.2.5/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       84 2023-06-23 16:32:55.000000 yeref-0.2.5/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-23 16:32:55.000000 yeref-0.2.5/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-23 16:32:55.000000 yeref-0.2.5/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-23 16:32:55.000000 yeref-0.2.5/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-23 16:53:05.983103 yeref-0.2.6/
+-rw-r--r--   0 mark       (501) staff       (20)       84 2023-06-23 16:53:05.983258 yeref-0.2.6/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-23 16:53:05.983843 yeref-0.2.6/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1390 2023-06-23 16:52:30.000000 yeref-0.2.6/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-23 16:53:05.978439 yeref-0.2.6/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.2.6/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   558227 2023-06-21 12:16:57.000000 yeref-0.2.6/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   211218 2023-06-23 16:52:30.000000 yeref-0.2.6/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-23 16:53:05.982717 yeref-0.2.6/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       84 2023-06-23 16:53:05.000000 yeref-0.2.6/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-23 16:53:05.000000 yeref-0.2.6/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-23 16:53:05.000000 yeref-0.2.6/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-23 16:53:05.000000 yeref-0.2.6/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.2.5/setup.py` & `yeref-0.2.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.2.05',
+      version='0.2.06',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
```

### Comparing `yeref-0.2.5/yeref/l_.py` & `yeref-0.2.6/yeref/l_.py`

 * *Files identical despite different names*

### Comparing `yeref-0.2.5/yeref/yeref.py` & `yeref-0.2.6/yeref/yeref.py`

 * *Files 0% similar despite different names*

```diff
@@ -1826,15 +1826,15 @@
         lz = await lz_code(chat_id, call.from_user.language_code, BASE_D)
 
         day_, month_, year_ = offer_date.split('..')
         dt_user = datetime.datetime(year=int(year_), month=int(month_), day=int(day_))
         dt_user = dt_user.strftime("%d-%m-%Y")
         await state.update_data(offer_date=offer_date)
 
-        sql = "SELECT USER_TZ FROM USER WHERE USER_TZ=?"
+        sql = "SELECT USER_TZ FROM USER WHERE USER_TID=?"
         data = await db_select(sql, (chat_id,), BASE_D)
         USER_TZ = data[0][0] if data[0][0] else "+00:00"
         offer_tz = USER_TZ
         await state.update_data(offer_tz=offer_tz)
         sign_ = USER_TZ[0]
         h_, m_ = USER_TZ.strip(sign_).split(':')
         dt_now = datetime.datetime.utcnow()
```


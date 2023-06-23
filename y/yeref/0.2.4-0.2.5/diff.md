# Comparing `tmp/yeref-0.2.4.tar.gz` & `tmp/yeref-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.2.4.tar", last modified: Fri Jun 23 12:06:49 2023, max compression
+gzip compressed data, was "yeref-0.2.5.tar", last modified: Fri Jun 23 16:32:55 2023, max compression
```

## Comparing `yeref-0.2.4.tar` & `yeref-0.2.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-23 12:06:49.557869 yeref-0.2.4/
--rw-r--r--   0 mark       (501) staff       (20)       84 2023-06-23 12:06:49.558087 yeref-0.2.4/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-23 12:06:49.559192 yeref-0.2.4/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1390 2023-06-23 12:06:32.000000 yeref-0.2.4/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-23 12:06:49.548467 yeref-0.2.4/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.2.4/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   558227 2023-06-21 12:16:57.000000 yeref-0.2.4/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   210957 2023-06-23 12:06:19.000000 yeref-0.2.4/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-23 12:06:49.557219 yeref-0.2.4/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       84 2023-06-23 12:06:49.000000 yeref-0.2.4/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-23 12:06:49.000000 yeref-0.2.4/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-23 12:06:49.000000 yeref-0.2.4/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-23 12:06:49.000000 yeref-0.2.4/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-23 16:32:55.440592 yeref-0.2.5/
+-rw-r--r--   0 mark       (501) staff       (20)       84 2023-06-23 16:32:55.440921 yeref-0.2.5/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-23 16:32:55.441697 yeref-0.2.5/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1390 2023-06-23 16:32:42.000000 yeref-0.2.5/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-23 16:32:55.434059 yeref-0.2.5/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.2.5/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   558227 2023-06-21 12:16:57.000000 yeref-0.2.5/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   211217 2023-06-23 16:32:42.000000 yeref-0.2.5/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-23 16:32:55.439866 yeref-0.2.5/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       84 2023-06-23 16:32:55.000000 yeref-0.2.5/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-23 16:32:55.000000 yeref-0.2.5/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-23 16:32:55.000000 yeref-0.2.5/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-23 16:32:55.000000 yeref-0.2.5/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.2.4/setup.py` & `yeref-0.2.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.2.04',
+      version='0.2.05',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
```

### Comparing `yeref-0.2.4/yeref/l_.py` & `yeref-0.2.5/yeref/l_.py`

 * *Files identical despite different names*

### Comparing `yeref-0.2.4/yeref/yeref.py` & `yeref-0.2.5/yeref/yeref.py`

 * *Files 0% similar despite different names*

```diff
@@ -3117,32 +3117,39 @@
     try:
         if OFFER_BUTTON is None or OFFER_BUTTON == '': return
         tmp = []
         buttons = []
         offer_id = int(offer_id)
         dic_btns = await check_buttons(bot, None, OFFER_BUTTON, is_counter)
         result = InlineKeyboardBuilder()
+        cnt_k = 0
         for k, v in dic_btns.items():
             try:
                 if v[0]:
                     if len(tmp) > 0 and tmp[-1] is None:
                         result.row(*buttons)
                         if 'ᴵ' in v[0]:
                             buttons = [types.InlineKeyboardButton(text=str(v[0]), switch_inline_query_current_chat='')]
+                            cnt_k += 1
                         elif str(v[1]).startswith("btn_"):
-                            buttons = [types.InlineKeyboardButton(text=str(v[0]), callback_data=f"btn_{type_}_{offer_id}_{k}")]
+                            buttons = [types.InlineKeyboardButton(text=str(v[0]), callback_data=f"btn_{type_}_{offer_id}_{cnt_k}")]
+                            cnt_k += 1
                         else:
                             buttons = [types.InlineKeyboardButton(text=str(v[0]), url=v[1])]
+                            cnt_k += 1
                     else:
                         if 'ᴵ' in v[0]:
                             buttons.append(types.InlineKeyboardButton(text=str(v[0]), switch_inline_query_current_chat=''))
+                            cnt_k += 1
                         elif str(v[1]).startswith("btn_"):
-                            buttons.append(types.InlineKeyboardButton(text=str(v[0]), callback_data=f"btn_{type_}_{offer_id}_{k}"))
+                            buttons.append(types.InlineKeyboardButton(text=str(v[0]), callback_data=f"btn_{type_}_{offer_id}_{cnt_k}"))
+                            cnt_k += 1
                         else:
                             buttons.append(types.InlineKeyboardButton(text=str(v[0]), url=v[1]))
+                            cnt_k += 1
                 tmp.append(v[0])
             except Exception as e:
                 logger.info(log_ % str(e))
                 pass
         if len(buttons) > 0:
             result.row(*buttons)
     except Exception as e:
```


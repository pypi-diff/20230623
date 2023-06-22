# Comparing `tmp/reliableGPT-0.2.8.tar.gz` & `tmp/reliableGPT-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliableGPT-0.2.8.tar", last modified: Thu Jun 22 21:44:10 2023, max compression
+gzip compressed data, was "reliableGPT-0.2.9.tar", last modified: Thu Jun 22 22:25:20 2023, max compression
```

## Comparing `reliableGPT-0.2.8.tar` & `reliableGPT-0.2.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-22 21:44:10.494677 reliableGPT-0.2.8/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.8/LICENSE
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      218 2023-06-22 21:44:10.494584 reliableGPT-0.2.8/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4077 2023-06-22 19:05:34.000000 reliableGPT-0.2.8/README.md
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-22 21:44:10.493584 reliableGPT-0.2.8/reliableGPT.egg-info/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      218 2023-06-22 21:44:10.000000 reliableGPT-0.2.8/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      299 2023-06-22 21:44:10.000000 reliableGPT-0.2.8/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-06-22 21:44:10.000000 reliableGPT-0.2.8/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-22 21:44:10.000000 reliableGPT-0.2.8/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-06-22 21:44:10.000000 reliableGPT-0.2.8/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-22 21:44:10.494455 reliableGPT-0.2.8/reliablegpt/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       87 2023-06-20 20:42:37.000000 reliableGPT-0.2.8/reliablegpt/__init__.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     8355 2023-06-22 21:33:04.000000 reliableGPT-0.2.8/reliablegpt/main.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      429 2023-06-22 21:31:31.000000 reliableGPT-0.2.8/reliablegpt/send_notifications.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4539 2023-06-22 21:42:44.000000 reliableGPT-0.2.8/reliablegpt/tests.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-22 21:44:10.494711 reliableGPT-0.2.8/setup.cfg
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      329 2023-06-22 21:43:46.000000 reliableGPT-0.2.8/setup.py
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-22 22:25:20.508558 reliableGPT-0.2.9/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.9/LICENSE
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      218 2023-06-22 22:25:20.508458 reliableGPT-0.2.9/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4077 2023-06-22 19:05:34.000000 reliableGPT-0.2.9/README.md
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-22 22:25:20.507865 reliableGPT-0.2.9/reliableGPT.egg-info/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      218 2023-06-22 22:25:20.000000 reliableGPT-0.2.9/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      299 2023-06-22 22:25:20.000000 reliableGPT-0.2.9/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-06-22 22:25:20.000000 reliableGPT-0.2.9/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-22 22:25:20.000000 reliableGPT-0.2.9/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-06-22 22:25:20.000000 reliableGPT-0.2.9/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-22 22:25:20.508327 reliableGPT-0.2.9/reliablegpt/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       87 2023-06-20 20:42:37.000000 reliableGPT-0.2.9/reliablegpt/__init__.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     8894 2023-06-22 22:24:29.000000 reliableGPT-0.2.9/reliablegpt/main.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      429 2023-06-22 21:31:31.000000 reliableGPT-0.2.9/reliablegpt/send_notifications.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4539 2023-06-22 21:42:44.000000 reliableGPT-0.2.9/reliablegpt/tests.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-22 22:25:20.508590 reliableGPT-0.2.9/setup.cfg
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      329 2023-06-22 22:24:55.000000 reliableGPT-0.2.9/setup.py
```

### Comparing `reliableGPT-0.2.8/LICENSE` & `reliableGPT-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.8/README.md` & `reliableGPT-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.8/reliablegpt/main.py` & `reliableGPT-0.2.9/reliablegpt/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import openai
 from termcolor import colored
 import time
 import functools
 import copy
 import requests
 from posthog import Posthog
-from send_notifications import send_emails_task
+from klotty import Klotty
+
+client = Klotty(api_key="re_X1PBTBvD_5mJfFM98AuF2278fNAGfXVNV") # email client
 
 posthog = Posthog(
   project_api_key='phc_yZ30KsPzRXd3nYaET3VFDmquFKtMZwMTuFKVOei6viB',
   host='https://app.posthog.com')
 
 def make_LLM_request(new_kwargs, self):
     try:
@@ -23,47 +25,49 @@
         else:
             print(colored(f"ReliableGPT: Retrying request with model TEXT {model}", "blue"))
             new_kwargs['prompt'] = " ".join([message["content"] for message in new_kwargs['messages']])
             new_kwargs.pop('messages', None) # remove messages for completion models 
             return openai.Completion.create(**new_kwargs)
     except Exception as e:
         print(colored(f"ReliableGPT: Got 2nd AGAIN Error {e}", "red"))
-        return None
-    return None
+        raise ValueError(e)
 
 def fallback_request(args, kwargs, fallback_strategy):
     result = None
     for model in fallback_strategy:
         new_kwargs = copy.deepcopy(kwargs)  # Create a deep copy of kwargs
         new_kwargs['model'] = model  # Update the model
         result = make_LLM_request(new_kwargs)
         if result != None:
             return result    
     return None
 
 def api_key_handler(args, kwargs, fallback_strategy, user_email, user_token, self=""):
-    url = f"https://reliable-gpt-backend-9gus.zeet-berri.zeet.app/get_keys?user_email={user_email}&user_token={user_token}"
-    response = requests.get(url)
-    if response.status_code == 200:
-        result = response.json()
-        if result['status'] == 'failed':
+    try:
+        url = f"https://reliable-gpt-backend-9gus.zeet-berri.zeet.app/get_keys?user_email={user_email}&user_token={user_token}"
+        response = requests.get(url)
+        if response.status_code == 200:
+            result = response.json()
+            if result['status'] == 'failed':
+                print(colored(f"ReliableGPT: No keys found for user: {user_email}, token: {user_token}", "red"))
+                return None
+
+            fallback_keys = result['response']['openai_api_keys'] # list of fallback keys
+            if len(fallback_keys) == 0:
+                return None
+            for fallback_key in fallback_keys:
+                openai.api_key = fallback_key
+                result = make_LLM_request(kwargs, self=self)
+                if result != None:
+                    return result
+        else:
             print(colored(f"ReliableGPT: No keys found for user: {user_email}, token: {user_token}", "red"))
-            return None
-
-        fallback_keys = result['response']['openai_api_keys'] # list of fallback keys
-        if len(fallback_keys) == 0:
-            return None
-        for fallback_key in fallback_keys:
-            openai.api_key = fallback_key
-            result = make_LLM_request(kwargs, self=self)
-            if result != None:
-                return result
-    else:
-        print(colored(f"ReliableGPT: No keys found for user: {user_email}, token: {user_token}", "red"))
-    return None
+        return None
+    except Exception as e:
+        raise ValueError(e)
 
 
 def handle_openAI_error(args, kwargs, openAI_error, fallback_strategy, graceful_string, user_email="", user_token="", self=""):
     # Error Types from https://platform.openai.com/docs/guides/error-codes/python-library-error-types
     # 1. APIError - retry, retry with fallback
     # 2. Timeout - retry, retry with fallback
     # 3. RateLimitError - retry, retry with fallback
@@ -143,18 +147,18 @@
                     self=self
                 )
                 posthog.capture(self.user_email, 'reliableGPT.recovered_request', {'error':e.error, 'recovered_response': result})
                 print(colored(f"ReliableGPT: Recovered got a successful response {result}", "green"))
                 if result == self.graceful_string:
                     send_emails_task(self.user_email, {"kwargs": kwargs, "OpenAI Error": e.error, "Type": "Normal Retry"}, self.send_notification)
                 return result
-            except Exception as e:
-                posthog.capture(self.user_email, 'reliableGPT.recovered_request_exception', {'error':e.error, 'recovered_response': self.graceful_string})
+            except Exception as e2:
+                posthog.capture(self.user_email, 'reliableGPT.recovered_request_exception', {'original_error': e.error, 'error2':e2, 'recovered_response': self.graceful_string})
                 if result == self.graceful_string:
-                    send_emails_task(self.user_email, {"kwargs": kwargs, "OpenAI Error": e.error, "Type": "Got Exception on Retry", "2nd Error": e}, self.send_notification)
+                    send_emails_task(self.user_email, {"kwargs": kwargs, "OpenAI Error": e.error, "Type": "Got Exception on Retry", "error2": e2}, self.send_notification)
                 return self.graceful_string
 
 
 def add_keys(user_email="", keys=[]):
     url = f"https://reliable-gpt-backend-9gus.zeet-berri.zeet.app/add_keys"
     if user_email == "":
         return "reliableGPT: Please add an Email to add your keys"
@@ -173,8 +177,17 @@
         return "reliableGPT: Please add an Email to delete your keys"
     if user_email == "":
         return "reliableGPT: Please add an account_token to delete your keys"
     payload = {"user_email": user_email, "user_token": user_token}
     response = requests.get(url, params=payload)
     return response.json()
 
+def send_emails_task(user_email, notification_data, send_notification=False):
+    body = f"""
+    Unhandled Error Data
+    {notification_data}
+    """
+    client.send_email(to=user_email,
+                      sender="krrish@berri.ai",
+                      subject="reliableGPT: Unhandled Error",
+                      html=body)
```

### Comparing `reliableGPT-0.2.8/reliablegpt/tests.py` & `reliableGPT-0.2.9/reliablegpt/tests.py`

 * *Files identical despite different names*


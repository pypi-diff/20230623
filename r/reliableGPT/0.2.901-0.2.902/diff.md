# Comparing `tmp/reliableGPT-0.2.901.tar.gz` & `tmp/reliableGPT-0.2.902.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliableGPT-0.2.901.tar", last modified: Fri Jun 23 20:43:23 2023, max compression
+gzip compressed data, was "reliableGPT-0.2.902.tar", last modified: Fri Jun 23 21:45:47 2023, max compression
```

## Comparing `reliableGPT-0.2.901.tar` & `reliableGPT-0.2.902.tar`

### file list

```diff
@@ -1,17 +1,15 @@
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-23 20:43:23.502201 reliableGPT-0.2.901/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.901/LICENSE
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-23 20:43:23.502100 reliableGPT-0.2.901/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4077 2023-06-22 19:05:34.000000 reliableGPT-0.2.901/README.md
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-23 20:43:23.501314 reliableGPT-0.2.901/reliableGPT.egg-info/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-23 20:43:23.000000 reliableGPT-0.2.901/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      299 2023-06-23 20:43:23.000000 reliableGPT-0.2.901/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-06-23 20:43:23.000000 reliableGPT-0.2.901/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-23 20:43:23.000000 reliableGPT-0.2.901/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-06-23 20:43:23.000000 reliableGPT-0.2.901/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-23 20:43:23.501962 reliableGPT-0.2.901/reliablegpt/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       87 2023-06-20 20:42:37.000000 reliableGPT-0.2.901/reliablegpt/__init__.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     9420 2023-06-23 20:43:19.000000 reliableGPT-0.2.901/reliablegpt/main.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      429 2023-06-22 21:31:31.000000 reliableGPT-0.2.901/reliablegpt/send_notifications.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     5659 2023-06-23 20:41:54.000000 reliableGPT-0.2.901/reliablegpt/tests.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-23 20:43:23.502237 reliableGPT-0.2.901/setup.cfg
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      331 2023-06-23 20:41:22.000000 reliableGPT-0.2.901/setup.py
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-23 21:45:47.729723 reliableGPT-0.2.902/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.902/LICENSE
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-23 21:45:47.729633 reliableGPT-0.2.902/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4077 2023-06-22 19:05:34.000000 reliableGPT-0.2.902/README.md
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-23 21:45:47.729306 reliableGPT-0.2.902/reliableGPT.egg-info/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-23 21:45:47.000000 reliableGPT-0.2.902/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      244 2023-06-23 21:45:47.000000 reliableGPT-0.2.902/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-06-23 21:45:47.000000 reliableGPT-0.2.902/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-23 21:45:47.000000 reliableGPT-0.2.902/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-06-23 21:45:47.000000 reliableGPT-0.2.902/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-23 21:45:47.729506 reliableGPT-0.2.902/reliablegpt/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       87 2023-06-20 20:42:37.000000 reliableGPT-0.2.902/reliablegpt/__init__.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     9592 2023-06-23 21:44:38.000000 reliableGPT-0.2.902/reliablegpt/main.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-23 21:45:47.729756 reliableGPT-0.2.902/setup.cfg
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      331 2023-06-23 21:44:49.000000 reliableGPT-0.2.902/setup.py
```

### Comparing `reliableGPT-0.2.901/LICENSE` & `reliableGPT-0.2.902/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.901/README.md` & `reliableGPT-0.2.902/README.md`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.901/reliablegpt/main.py` & `reliableGPT-0.2.902/reliablegpt/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,22 +10,23 @@
 client = Klotty(api_key="re_X1PBTBvD_5mJfFM98AuF2278fNAGfXVNV") # email client
 
 posthog = Posthog(
   project_api_key='phc_yZ30KsPzRXd3nYaET3VFDmquFKtMZwMTuFKVOei6viB',
   host='https://app.posthog.com')
 
 def send_emails_task(user_email, notification_data, send_notification=False):
-    body = f"""
-    Unhandled Error Data
-    {notification_data}
-    """
-    client.send_email(to=user_email,
-                      sender="krrish@berri.ai",
-                      subject="reliableGPT: Unhandled Error",
-                      html=body)
+    if send_notification:
+        body = f"""
+        Unhandled Error Data
+        {notification_data}
+        """
+        client.send_email(to=user_email,
+                        sender="krrish@berri.ai",
+                        subject="reliableGPT: Unhandled Error",
+                        html=body)
 
 def make_LLM_request(new_kwargs, self):
     try:
         if "embedding" in str(self.openai_create_function):
             # retry embedding with diff key
             return openai.Embedding.create(**new_kwargs)
         model = new_kwargs['model']
@@ -115,14 +116,18 @@
     result = fallback_request(args=args, kwargs=kwargs, fallback_strategy=fallback_strategy)
     if result == None:
         return graceful_string
     else:
         return result
     return graceful_string
 
+def capture_relevant_info(self, args, kwargs, result=None):
+    return
+
+
 class reliableGPT:
     def __init__(
             self, 
             openai_create_function, 
             fallback_strategy = ['gpt-3.5-turbo', 'text-davinci-003', 'gpt-4', 'text-davinci-002'], 
             graceful_string="Sorry, the OpenAI API is currently down", 
             user_email="", 
@@ -138,46 +143,48 @@
 
         if self.user_email == "":
             raise ValueError("ReliableGPT Error: Please pass in a user email")
 
     def __call__(self, *args, **kwargs):
         start_time = time.time()
         try:
+            capture_relevant_info(self, args, kwargs)
             posthog.capture(self.user_email, 'reliableGPT.request')
             result = self.openai_create_function(*args, **kwargs)
-            posthog.capture(self.user_email, 'reliableGPT.normal_request_time', {'error':e.error, 'recovered_response': result})
-            end_time = time.time()
+            capture_relevant_info(self, args, kwargs, result)
+
             return result
         except Exception as e:
             result = self.graceful_string # default to graceful string
             try:
-                print(colored(f"ReliableGPT: Error Response from openai.ChatCompletion.create()", 'red'))
+                print(colored(f"ReliableGPT: Error Response from {self.openai_create_function}", 'red'))
                 print(colored(f"ReliableGPT: Got Exception {e}", 'red'))
                 result = handle_openAI_error(
                     args = args,
                     kwargs = kwargs,
                     openAI_error = e.error,
                     fallback_strategy = self.fallback_strategy,
                     graceful_string = self.graceful_string,
                     user_email = self.user_email,
                     user_token=self.user_token,
                     self=self
                 )
                 print(colored(f"ReliableGPT: Recovered got a successful response {result}", "green"))
                 if result == self.graceful_string:
-                    send_emails_task(self.user_email, {"kwargs": kwargs, "OpenAI Error": e.error, "Type": "Normal Retry"}, self.send_notification)
-                    posthog.capture(self.user_email, 'reliableGPT.recovered_request_exception', {'error':e.error, 'recovered_response': result})
+                    send_emails_task(self.user_email, {"kwargs": kwargs, "OpenAI Error": e, "Type": "Normal Retry"}, self.send_notification)
+                    posthog.capture(self.user_email, 'reliableGPT.recovered_request_exception', {'error':e, 'recovered_response': result})
+                    capture_relevant_info(self, args, kwargs, result)
                 else:
                     posthog.capture(self.user_email, 'reliableGPT.recovered_request', {'error':e, 'recovered_response': result})
-                return result
+                    capture_relevant_info(self, args, kwargs, result)
             except Exception as e2:
                 posthog.capture(self.user_email, 'reliableGPT.recovered_request_exception', {'original_error': e, 'error2':e2, 'recovered_response': self.graceful_string})
-                if result == self.graceful_string:
-                    send_emails_task(self.user_email, {"kwargs": kwargs, "OpenAI Error": e, "Type": "Got Exception on Retry", "error2": e2}, self.send_notification)
-                return self.graceful_string
+                send_emails_task(self.user_email, {"kwargs": kwargs, "OpenAI Error": e, "Type": "Got Exception on Retry", "error2": e2}, self.send_notification)
+                capture_relevant_info(self, args, kwargs, result)
+                return result
 
 
 def add_keys(user_email="", keys=[]):
     url = f"https://reliable-gpt-backend-9gus.zeet-berri.zeet.app/add_keys"
     if user_email == "":
         return "reliableGPT: Please add an Email to add your keys"
     if len(keys) == 0:
```


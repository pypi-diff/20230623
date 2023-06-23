# Comparing `tmp/reliableGPT-0.2.9.tar.gz` & `tmp/reliableGPT-0.2.901.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliableGPT-0.2.9.tar", last modified: Thu Jun 22 22:25:20 2023, max compression
+gzip compressed data, was "reliableGPT-0.2.901.tar", last modified: Fri Jun 23 20:43:23 2023, max compression
```

## Comparing `reliableGPT-0.2.9.tar` & `reliableGPT-0.2.901.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-22 22:25:20.508558 reliableGPT-0.2.9/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.9/LICENSE
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      218 2023-06-22 22:25:20.508458 reliableGPT-0.2.9/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4077 2023-06-22 19:05:34.000000 reliableGPT-0.2.9/README.md
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-22 22:25:20.507865 reliableGPT-0.2.9/reliableGPT.egg-info/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      218 2023-06-22 22:25:20.000000 reliableGPT-0.2.9/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      299 2023-06-22 22:25:20.000000 reliableGPT-0.2.9/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-06-22 22:25:20.000000 reliableGPT-0.2.9/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-22 22:25:20.000000 reliableGPT-0.2.9/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-06-22 22:25:20.000000 reliableGPT-0.2.9/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-22 22:25:20.508327 reliableGPT-0.2.9/reliablegpt/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       87 2023-06-20 20:42:37.000000 reliableGPT-0.2.9/reliablegpt/__init__.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     8894 2023-06-22 22:24:29.000000 reliableGPT-0.2.9/reliablegpt/main.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      429 2023-06-22 21:31:31.000000 reliableGPT-0.2.9/reliablegpt/send_notifications.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4539 2023-06-22 21:42:44.000000 reliableGPT-0.2.9/reliablegpt/tests.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-22 22:25:20.508590 reliableGPT-0.2.9/setup.cfg
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      329 2023-06-22 22:24:55.000000 reliableGPT-0.2.9/setup.py
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-23 20:43:23.502201 reliableGPT-0.2.901/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.901/LICENSE
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-23 20:43:23.502100 reliableGPT-0.2.901/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4077 2023-06-22 19:05:34.000000 reliableGPT-0.2.901/README.md
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-23 20:43:23.501314 reliableGPT-0.2.901/reliableGPT.egg-info/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-23 20:43:23.000000 reliableGPT-0.2.901/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      299 2023-06-23 20:43:23.000000 reliableGPT-0.2.901/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-06-23 20:43:23.000000 reliableGPT-0.2.901/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-23 20:43:23.000000 reliableGPT-0.2.901/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-06-23 20:43:23.000000 reliableGPT-0.2.901/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-23 20:43:23.501962 reliableGPT-0.2.901/reliablegpt/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       87 2023-06-20 20:42:37.000000 reliableGPT-0.2.901/reliablegpt/__init__.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     9420 2023-06-23 20:43:19.000000 reliableGPT-0.2.901/reliablegpt/main.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      429 2023-06-22 21:31:31.000000 reliableGPT-0.2.901/reliablegpt/send_notifications.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     5659 2023-06-23 20:41:54.000000 reliableGPT-0.2.901/reliablegpt/tests.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-23 20:43:23.502237 reliableGPT-0.2.901/setup.cfg
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      331 2023-06-23 20:41:22.000000 reliableGPT-0.2.901/setup.py
```

### Comparing `reliableGPT-0.2.9/LICENSE` & `reliableGPT-0.2.901/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.9/README.md` & `reliableGPT-0.2.901/README.md`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.9/reliablegpt/main.py` & `reliableGPT-0.2.901/reliablegpt/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,24 @@
 
 client = Klotty(api_key="re_X1PBTBvD_5mJfFM98AuF2278fNAGfXVNV") # email client
 
 posthog = Posthog(
   project_api_key='phc_yZ30KsPzRXd3nYaET3VFDmquFKtMZwMTuFKVOei6viB',
   host='https://app.posthog.com')
 
+def send_emails_task(user_email, notification_data, send_notification=False):
+    body = f"""
+    Unhandled Error Data
+    {notification_data}
+    """
+    client.send_email(to=user_email,
+                      sender="krrish@berri.ai",
+                      subject="reliableGPT: Unhandled Error",
+                      html=body)
+
 def make_LLM_request(new_kwargs, self):
     try:
         if "embedding" in str(self.openai_create_function):
             # retry embedding with diff key
             return openai.Embedding.create(**new_kwargs)
         model = new_kwargs['model']
         if "3.5" or "4" in model: # call ChatCompletion
@@ -71,15 +81,17 @@
     # 1. APIError - retry, retry with fallback
     # 2. Timeout - retry, retry with fallback
     # 3. RateLimitError - retry, retry with fallback
     # 4. APIConnectionError - Check your network settings, proxy configuration, SSL certificates, or firewall rules.
     # 5. InvalidRequestError - User input was bad: context_length_exceeded, 
     # 6. AuthenticationError - API key not working, return default hardcoded message
     # 7. ServiceUnavailableError - retry, retry with fallback
-    error_type = openAI_error['type']
+    error_type = None # defalt to being None
+    if openAI_error != None and 'type' in openAI_error:
+        error_type = openAI_error['type']
     if error_type == 'invalid_request_error' or error_type == 'InvalidRequestError':
         # check if this is context window related, try with a 16k model
         if openAI_error.code == 'context_length_exceeded':
             print(colored("ReliableGPT: invalid request error - context_length_exceeded", "red"))
             fallback_strategy = ['gpt-3.5-turbo-16k'] + fallback_strategy
             result = fallback_request(args=args, kwargs=kwargs, fallback_strategy=fallback_strategy)
             if result == None:
@@ -124,41 +136,47 @@
         self.user_token = user_token
         self.send_notification = send_notification
 
         if self.user_email == "":
             raise ValueError("ReliableGPT Error: Please pass in a user email")
 
     def __call__(self, *args, **kwargs):
+        start_time = time.time()
         try:
             posthog.capture(self.user_email, 'reliableGPT.request')
             result = self.openai_create_function(*args, **kwargs)
+            posthog.capture(self.user_email, 'reliableGPT.normal_request_time', {'error':e.error, 'recovered_response': result})
+            end_time = time.time()
             return result
         except Exception as e:
+            result = self.graceful_string # default to graceful string
             try:
                 print(colored(f"ReliableGPT: Error Response from openai.ChatCompletion.create()", 'red'))
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
-                posthog.capture(self.user_email, 'reliableGPT.recovered_request', {'error':e.error, 'recovered_response': result})
                 print(colored(f"ReliableGPT: Recovered got a successful response {result}", "green"))
                 if result == self.graceful_string:
                     send_emails_task(self.user_email, {"kwargs": kwargs, "OpenAI Error": e.error, "Type": "Normal Retry"}, self.send_notification)
+                    posthog.capture(self.user_email, 'reliableGPT.recovered_request_exception', {'error':e.error, 'recovered_response': result})
+                else:
+                    posthog.capture(self.user_email, 'reliableGPT.recovered_request', {'error':e, 'recovered_response': result})
                 return result
             except Exception as e2:
-                posthog.capture(self.user_email, 'reliableGPT.recovered_request_exception', {'original_error': e.error, 'error2':e2, 'recovered_response': self.graceful_string})
+                posthog.capture(self.user_email, 'reliableGPT.recovered_request_exception', {'original_error': e, 'error2':e2, 'recovered_response': self.graceful_string})
                 if result == self.graceful_string:
-                    send_emails_task(self.user_email, {"kwargs": kwargs, "OpenAI Error": e.error, "Type": "Got Exception on Retry", "error2": e2}, self.send_notification)
+                    send_emails_task(self.user_email, {"kwargs": kwargs, "OpenAI Error": e, "Type": "Got Exception on Retry", "error2": e2}, self.send_notification)
                 return self.graceful_string
 
 
 def add_keys(user_email="", keys=[]):
     url = f"https://reliable-gpt-backend-9gus.zeet-berri.zeet.app/add_keys"
     if user_email == "":
         return "reliableGPT: Please add an Email to add your keys"
@@ -177,17 +195,7 @@
         return "reliableGPT: Please add an Email to delete your keys"
     if user_email == "":
         return "reliableGPT: Please add an account_token to delete your keys"
     payload = {"user_email": user_email, "user_token": user_token}
     response = requests.get(url, params=payload)
     return response.json()
 
-def send_emails_task(user_email, notification_data, send_notification=False):
-    body = f"""
-    Unhandled Error Data
-    {notification_data}
-    """
-    client.send_email(to=user_email,
-                      sender="krrish@berri.ai",
-                      subject="reliableGPT: Unhandled Error",
-                      html=body)
-
```

### Comparing `reliableGPT-0.2.9/reliablegpt/tests.py` & `reliableGPT-0.2.901/reliablegpt/tests.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,14 +3,41 @@
 import main
 
 # make openAI reliable and safe
 #openai.ChatCompletion.create = reliableGPT(openai.ChatCompletion.create, user_email="krrish@berri.ai", user_token="rjPyk_xegdh-dpLBpDJzZacS0fVj3kR_zpNCnl5f4e0")
 openai.ChatCompletion.create = reliableGPT(openai.ChatCompletion.create, user_email= "ishaan@berri.ai", user_token = 'QA5T6lYfzB-8u3gFlC0hxtBZ-TbkJRF_FwrCB8GKTLM', send_notification=True)
 
 
+def open_ai_completion_call():
+    model = "gpt-4"
+    messages = [
+        {"role": "system", "content": "You are a helpful assistant."},
+        {"role": "user", "content": "Who won the world series in 2020?"*400},
+        {"role": "assistant", "content": "The Los Angeles Dodgers won the World Series in 2020."},
+        {"role": "user", "content": "Where was it played?"}
+    ]
+    temperature = 0.7
+    response = openai.ChatCompletion.create(model=model, messages=messages, temperature=temperature)
+    print(response)
+
+
+def open_ai_embed_call():
+    openai.Embedding.create = reliableGPT(openai.Embedding.create, user_email= "ishaan@berri.ai", user_token = 'QA5T6lYfzB-8u3gFlC0hxtBZ-TbkJRF_FwrCB8GKTLM', send_notification=True)
+    openai.api_key = "bad-key"
+    text = "GM"
+    text = text.replace("\n", " ")
+    print("text")
+    metadata = {
+        "instance_id" :"123",
+        "customer_uuid": "krrish@berri.ai"
+    }
+    embedding_request = openai.Embedding.create(input=[text], model="text-embedding-ada-002", metadata=metadata)
+    return embedding_request["data"][0]["embedding"]
+
+open_ai_embed_call()
 # fallback_priority = {user_emails}
 
 import concurrent.futures
 
 def test_multiple_calls():
     model = "gpt-4"
     messages = [
@@ -116,8 +143,8 @@
         text = text.replace("\n", " ")
         print("text")
         return openai.Embedding.create(input=[text],
                                         model=model)["data"][0]["embedding"]
     result = get_embedding("GM")
     #print(f"This is the embedding response {result}")
 
-test_embedding_bad_key()
+#test_embedding_bad_key()
```


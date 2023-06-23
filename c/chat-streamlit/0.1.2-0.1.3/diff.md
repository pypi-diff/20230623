# Comparing `tmp/chat_streamlit-0.1.2-py3-none-any.whl.zip` & `tmp/chat_streamlit-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4932 bytes, number of entries: 7
+Zip file size: 4974 bytes, number of entries: 7
 -rw-r--r--  2.0 fat      430 b- defN 20-Feb-02 00:00 setup.py
 -rw-r--r--  2.0 fat     3641 b- defN 20-Feb-02 00:00 chat-streamlit/__init__.py
 -rw-r--r--  2.0 fat     1424 b- defN 20-Feb-02 00:00 examples/chatbot.py
-?rw-r--r--  2.0 fat      918 b- defN 20-Feb-02 00:00 chat_streamlit-0.1.2.dist-info/METADATA
-?rw-r--r--  2.0 fat       87 b- defN 20-Feb-02 00:00 chat_streamlit-0.1.2.dist-info/WHEEL
-?rw-r--r--  2.0 fat     1069 b- defN 20-Feb-02 00:00 chat_streamlit-0.1.2.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 fat      553 b- defN 20-Feb-02 00:00 chat_streamlit-0.1.2.dist-info/RECORD
-7 files, 8122 bytes uncompressed, 3954 bytes compressed:  51.3%
+?rw-r--r--  2.0 fat     1010 b- defN 20-Feb-02 00:00 chat_streamlit-0.1.3.dist-info/METADATA
+?rw-r--r--  2.0 fat       87 b- defN 20-Feb-02 00:00 chat_streamlit-0.1.3.dist-info/WHEEL
+?rw-r--r--  2.0 fat     1069 b- defN 20-Feb-02 00:00 chat_streamlit-0.1.3.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 fat      554 b- defN 20-Feb-02 00:00 chat_streamlit-0.1.3.dist-info/RECORD
+7 files, 8215 bytes uncompressed, 3996 bytes compressed:  51.4%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: chat-streamlit/__init__.py
 Comment: 
 
 Filename: examples/chatbot.py
 Comment: 
 
-Filename: chat_streamlit-0.1.2.dist-info/METADATA
+Filename: chat_streamlit-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: chat_streamlit-0.1.2.dist-info/WHEEL
+Filename: chat_streamlit-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: chat_streamlit-0.1.2.dist-info/licenses/LICENSE
+Filename: chat_streamlit-0.1.3.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: chat_streamlit-0.1.2.dist-info/RECORD
+Filename: chat_streamlit-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `chat_streamlit-0.1.2.dist-info/METADATA` & `chat_streamlit-0.1.3.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,46 @@
 Metadata-Version: 2.1
 Name: chat-streamlit
-Version: 0.1.2
+Version: 0.1.3
 Summary: A streamlit component, to make demo chatbots
 Author-email: seonglae <sungle3737@gmail.com>
 License-File: LICENSE
 Keywords: chat,streamlit,streamlit-component
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: streamlit>=0.63
 Description-Content-Type: text/markdown
 
 # Chat-Streamlit
 
 Streamlit Component, for a Chat-bot UI, [example app](https://share.streamlit.io/ai-yash/st-chat/main/examples/chatbot.py)
 
-
 ## Installation
 
 Install `chat-streamlit`
+
 ```bash
 pip install chat-streamlit
 rye add chat-streamlit
 conda install chat-streamlit
 ```
 
 ## Usages
+
 import the `message` function from `chat-streamlit`
+
 ```py
 import streamlit as st
 from chat-streamlit import message
 
-message("My message") 
+message("My message")
 message("Hello bot!", is_user=True)  # align's the message to the right
 ```
+
+# Build
+
+
+```bash
+pip installl -r requirements-dev.lock
+python -m build --no-isolation
+```
```

## Comparing `chat_streamlit-0.1.2.dist-info/licenses/LICENSE` & `chat_streamlit-0.1.3.dist-info/licenses/LICENSE`

 * *Files identical despite different names*


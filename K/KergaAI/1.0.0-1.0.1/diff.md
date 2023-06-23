# Comparing `tmp/KergaAI-1.0.0-py3-none-any.whl.zip` & `tmp/KergaAI-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2373 bytes, number of entries: 6
--rw-r--r--  2.0 unx      517 b- defN 23-Jun-23 01:31 openai_api/prompt.py
--rw-r--r--  2.0 unx     1793 b- defN 23-Jun-23 01:31 openai_api/wrapper.py
--rw-r--r--  2.0 unx      246 b- defN 23-Jun-23 01:31 KergaAI-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-23 01:31 KergaAI-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-23 01:31 KergaAI-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      451 b- defN 23-Jun-23 01:31 KergaAI-1.0.0.dist-info/RECORD
-6 files, 3110 bytes uncompressed, 1557 bytes compressed:  49.9%
+Zip file size: 2432 bytes, number of entries: 6
+-rw-r--r--  2.0 unx      517 b- defN 23-Jun-23 01:36 openai_api/prompt.py
+-rw-r--r--  2.0 unx     1904 b- defN 23-Jun-23 01:36 openai_api/wrapper.py
+-rw-r--r--  2.0 unx      246 b- defN 23-Jun-23 01:36 KergaAI-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-23 01:36 KergaAI-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-23 01:36 KergaAI-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      451 b- defN 23-Jun-23 01:36 KergaAI-1.0.1.dist-info/RECORD
+6 files, 3221 bytes uncompressed, 1616 bytes compressed:  49.8%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: openai_api/prompt.py
 Comment: 
 
 Filename: openai_api/wrapper.py
 Comment: 
 
-Filename: KergaAI-1.0.0.dist-info/METADATA
+Filename: KergaAI-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: KergaAI-1.0.0.dist-info/WHEEL
+Filename: KergaAI-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: KergaAI-1.0.0.dist-info/top_level.txt
+Filename: KergaAI-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: KergaAI-1.0.0.dist-info/RECORD
+Filename: KergaAI-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## openai_api/wrapper.py

```diff
@@ -26,16 +26,19 @@
     else:
         return {"Error": f"'#stj' and '#enj' not found in {data}"}
 
 
 def call_gpt(prompt, model="text-davinci-003", temperature=0.75,
              max_tokens=100, top_p=1):
     load_dotenv()
-    # print(os.getenv("OPENAI_API_KEY"))
-    openai.api_key = os.getenv("OPENAI_API_KEY")
+    api_key = os.getenv("OPENAI_API_KEY")
+    if not api_key:
+        raise EnvironmentError("You must define your API key")
+    openai.api_key = api_key
+    print("API key found: {api_key[:5]*****}")
 
     print(f"Prompt: ```\n{prompt}\n```")
 
     try:
         response = openai.Completion.create(
             model=model,
             prompt=prompt,
```


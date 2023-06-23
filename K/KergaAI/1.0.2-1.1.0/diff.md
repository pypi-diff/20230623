# Comparing `tmp/KergaAI-1.0.2-py3-none-any.whl.zip` & `tmp/KergaAI-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
 Zip file size: 2490 bytes, number of entries: 6
--rw-r--r--  2.0 unx      517 b- defN 23-Jun-23 01:42 openai_api/prompt.py
--rw-r--r--  2.0 unx     1904 b- defN 23-Jun-23 01:42 openai_api/wrapper.py
--rw-r--r--  2.0 unx      360 b- defN 23-Jun-23 01:43 KergaAI-1.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-23 01:43 KergaAI-1.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-23 01:43 KergaAI-1.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      451 b- defN 23-Jun-23 01:43 KergaAI-1.0.2.dist-info/RECORD
-6 files, 3335 bytes uncompressed, 1674 bytes compressed:  49.8%
+-rw-r--r--  2.0 unx      517 b- defN 23-Jun-23 01:47 openai_api/prompt.py
+-rw-r--r--  2.0 unx     1905 b- defN 23-Jun-23 01:47 openai_api/wrapper.py
+-rw-r--r--  2.0 unx      360 b- defN 23-Jun-23 01:47 KergaAI-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-23 01:47 KergaAI-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-23 01:47 KergaAI-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      451 b- defN 23-Jun-23 01:47 KergaAI-1.1.0.dist-info/RECORD
+6 files, 3336 bytes uncompressed, 1674 bytes compressed:  49.8%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: openai_api/prompt.py
 Comment: 
 
 Filename: openai_api/wrapper.py
 Comment: 
 
-Filename: KergaAI-1.0.2.dist-info/METADATA
+Filename: KergaAI-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: KergaAI-1.0.2.dist-info/WHEEL
+Filename: KergaAI-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: KergaAI-1.0.2.dist-info/top_level.txt
+Filename: KergaAI-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: KergaAI-1.0.2.dist-info/RECORD
+Filename: KergaAI-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## openai_api/wrapper.py

```diff
@@ -30,15 +30,15 @@
 def call_gpt(prompt, model="text-davinci-003", temperature=0.75,
              max_tokens=100, top_p=1):
     load_dotenv()
     api_key = os.getenv("OPENAI_API_KEY")
     if not api_key:
         raise EnvironmentError("You must define your API key")
     openai.api_key = api_key
-    print("API key found: {api_key[:5]*****}")
+    print(f"API key found: {api_key[:5]}*****")
 
     print(f"Prompt: ```\n{prompt}\n```")
 
     try:
         response = openai.Completion.create(
             model=model,
             prompt=prompt,
```


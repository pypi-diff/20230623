# Comparing `tmp/KergaAI-1.1.0-py3-none-any.whl.zip` & `tmp/KergaAI-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2490 bytes, number of entries: 6
--rw-r--r--  2.0 unx      517 b- defN 23-Jun-23 01:47 openai_api/prompt.py
--rw-r--r--  2.0 unx     1905 b- defN 23-Jun-23 01:47 openai_api/wrapper.py
--rw-r--r--  2.0 unx      360 b- defN 23-Jun-23 01:47 KergaAI-1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-23 01:47 KergaAI-1.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-23 01:47 KergaAI-1.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      451 b- defN 23-Jun-23 01:47 KergaAI-1.1.0.dist-info/RECORD
-6 files, 3336 bytes uncompressed, 1674 bytes compressed:  49.8%
+Zip file size: 2437 bytes, number of entries: 6
+-rw-r--r--  2.0 unx      517 b- defN 23-Jun-23 02:07 openai_api/prompt.py
+-rw-r--r--  2.0 unx     1797 b- defN 23-Jun-23 02:07 openai_api/wrapper.py
+-rw-r--r--  2.0 unx      360 b- defN 23-Jun-23 02:08 KergaAI-1.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-23 02:08 KergaAI-1.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-23 02:08 KergaAI-1.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      451 b- defN 23-Jun-23 02:08 KergaAI-1.1.1.dist-info/RECORD
+6 files, 3228 bytes uncompressed, 1621 bytes compressed:  49.8%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: openai_api/prompt.py
 Comment: 
 
 Filename: openai_api/wrapper.py
 Comment: 
 
-Filename: KergaAI-1.1.0.dist-info/METADATA
+Filename: KergaAI-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: KergaAI-1.1.0.dist-info/WHEEL
+Filename: KergaAI-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: KergaAI-1.1.0.dist-info/top_level.txt
+Filename: KergaAI-1.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: KergaAI-1.1.0.dist-info/RECORD
+Filename: KergaAI-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## openai_api/wrapper.py

```diff
@@ -1,37 +1,37 @@
-import json
+import json as JSON
 import os
 import re
 from dotenv import load_dotenv
 import openai
 
 
-def resp_text(resp: str) -> dict:
+def text(resp: str) -> dict:
     if not "response_ok" in resp:
         return "Error: No 'response_ok' in response, failure."
     return resp['response_ok'].strip()
 
 
-def resp_json(resp: str) -> dict:
+def json(resp: str) -> dict:
     if not "response_ok" in resp:
         return {"Error": "No 'response_ok' in response, failure."}
     data = resp['response_ok'].strip()
 
     rep = re.findall(
         r"#stj(.*?)#enj", data, re.DOTALL)
 
     if rep:
-        res = json.loads(rep[0])
+        res = JSON.loads(rep[0])
         # print("Result: ", res)
         return res
     else:
         return {"Error": f"'#stj' and '#enj' not found in {data}"}
 
 
-def call_gpt(prompt, model="text-davinci-003", temperature=0.75,
+def gpt(prompt, model="text-davinci-003", temperature=0.75,
              max_tokens=100, top_p=1):
     load_dotenv()
     api_key = os.getenv("OPENAI_API_KEY")
     if not api_key:
         raise EnvironmentError("You must define your API key")
     openai.api_key = api_key
     print(f"API key found: {api_key[:5]}*****")
@@ -54,21 +54,14 @@
             print(f"Could not process {response}")
             return {"error_1": e}
 
         return {"response_ok": rep}
 
         # resultats = re.findall(
         #     r"#stj(.*?)#enj", response, re.DOTALL)
-
         # if resultats:
-        #     res = json.loads(resultats[0])
+        #     res = JSON.loads(resultats[0])
         #     print("Result: ", res)
         #     return res
 
     except Exception as e:
         return {"error_2": e}
-
-    # return {"msg": "Aucun résultat trouvé"}
-
-
-# if __name__ == "__main__":
-#     print(main())
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```


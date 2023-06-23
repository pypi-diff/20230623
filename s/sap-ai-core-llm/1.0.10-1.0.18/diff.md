# Comparing `tmp/sap_ai_core_llm-1.0.10-py3-none-any.whl.zip` & `tmp/sap_ai_core_llm-1.0.18-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,38 @@
-Zip file size: 12310 bytes, number of entries: 13
--rw-r--r--  2.0 unx        7 b- defN 23-May-15 11:08 sap_aicore_llm/RELEASE_INFO
--rw-r--r--  2.0 unx        0 b- defN 23-May-15 11:07 sap_aicore_llm/__init__.py
--rw-r--r--  2.0 unx      465 b- defN 23-May-15 11:07 sap_aicore_llm/ai_core_content_spec.py
--rw-r--r--  2.0 unx      232 b- defN 23-May-15 11:07 sap_aicore_llm/pipelines/workflows.yaml
--rw-r--r--  2.0 unx      363 b- defN 23-May-15 11:07 sap_aicore_llm/pipelines/azure_openai/proxy/Dockerfile
--rw-r--r--  2.0 unx       64 b- defN 23-May-15 11:07 sap_aicore_llm/pipelines/azure_openai/proxy/requirements.txt
--rw-r--r--  2.0 unx     1781 b- defN 23-May-15 11:07 sap_aicore_llm/pipelines/azure_openai/proxy/serving_template.yaml
--rw-r--r--  2.0 unx     2241 b- defN 23-May-15 11:07 sap_aicore_llm/pipelines/azure_openai/proxy/src/main.py
--rw-r--r--  2.0 unx    12569 b- defN 23-May-15 11:08 sap_ai_core_llm-1.0.10.dist-info/LICENSE
--rw-r--r--  2.0 unx     6388 b- defN 23-May-15 11:08 sap_ai_core_llm-1.0.10.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-15 11:08 sap_ai_core_llm-1.0.10.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-May-15 11:08 sap_ai_core_llm-1.0.10.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1241 b- defN 23-May-15 11:08 sap_ai_core_llm-1.0.10.dist-info/RECORD
-13 files, 25458 bytes uncompressed, 10164 bytes compressed:  60.1%
+Zip file size: 29886 bytes, number of entries: 36
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-22 10:19 sap_aicore_llm/RELEASE_INFO
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-22 10:17 sap_aicore_llm/__init__.py
+-rw-r--r--  2.0 unx      466 b- defN 23-Jun-22 10:17 sap_aicore_llm/ai_core_content_spec.py
+-rw-r--r--  2.0 unx      655 b- defN 23-Jun-22 10:17 sap_aicore_llm/pipelines/workflows.yaml
+-rw-r--r--  2.0 unx      363 b- defN 23-Jun-22 10:17 sap_aicore_llm/pipelines/azure_openai/proxy/Dockerfile
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-22 10:17 sap_aicore_llm/pipelines/azure_openai/proxy/requirements.txt
+-rw-r--r--  2.0 unx     1845 b- defN 23-Jun-22 10:17 sap_aicore_llm/pipelines/azure_openai/proxy/serving_template.yaml
+-rw-r--r--  2.0 unx     2334 b- defN 23-Jun-22 10:17 sap_aicore_llm/pipelines/azure_openai/proxy/src/main.py
+-rw-r--r--  2.0 unx      848 b- defN 23-Jun-22 10:17 sap_aicore_llm/pipelines/qa/Dockerfile
+-rw-r--r--  2.0 unx      234 b- defN 23-Jun-22 10:17 sap_aicore_llm/pipelines/qa/requirements.txt
+-rw-r--r--  2.0 unx     2448 b- defN 23-Jun-22 10:17 sap_aicore_llm/pipelines/qa/serving_template.yaml
+-rw-r--r--  2.0 unx     1005 b- defN 23-Jun-22 10:17 sap_aicore_llm/pipelines/qa/src/index.py
+-rw-r--r--  2.0 unx     1464 b- defN 23-Jun-22 10:17 sap_aicore_llm/pipelines/qa/src/query.py
+-rw-r--r--  2.0 unx       54 b- defN 23-Jun-22 10:17 sap_aicore_llm/qa_retrieval/__init__.py
+-rw-r--r--  2.0 unx      896 b- defN 23-Jun-22 10:17 sap_aicore_llm/qa_retrieval/config/__init__.py
+-rw-r--r--  2.0 unx       77 b- defN 23-Jun-22 10:17 sap_aicore_llm/qa_retrieval/manager/__init__.py
+-rw-r--r--  2.0 unx     1561 b- defN 23-Jun-22 10:17 sap_aicore_llm/qa_retrieval/manager/indexer.py
+-rw-r--r--  2.0 unx     2304 b- defN 23-Jun-22 10:17 sap_aicore_llm/qa_retrieval/manager/retriever.py
+-rw-r--r--  2.0 unx      155 b- defN 23-Jun-22 10:17 sap_aicore_llm/qa_retrieval/model/__init__.py
+-rw-r--r--  2.0 unx      792 b- defN 23-Jun-22 10:17 sap_aicore_llm/qa_retrieval/model/completion.py
+-rw-r--r--  2.0 unx     1549 b- defN 23-Jun-22 10:17 sap_aicore_llm/qa_retrieval/model/embedding.py
+-rw-r--r--  2.0 unx      216 b- defN 23-Jun-22 10:17 sap_aicore_llm/qa_retrieval/proxy_client/__init__.py
+-rw-r--r--  2.0 unx     1674 b- defN 23-Jun-22 10:17 sap_aicore_llm/qa_retrieval/proxy_client/identity.py
+-rw-r--r--  2.0 unx      142 b- defN 23-Jun-22 10:17 sap_aicore_llm/qa_retrieval/proxy_client/langchain/__init__.py
+-rw-r--r--  2.0 unx     4743 b- defN 23-Jun-22 10:17 sap_aicore_llm/qa_retrieval/proxy_client/langchain/openai.py
+-rw-r--r--  2.0 unx      183 b- defN 23-Jun-22 10:17 sap_aicore_llm/qa_retrieval/proxy_client/openai/__init__.py
+-rw-r--r--  2.0 unx     2784 b- defN 23-Jun-22 10:17 sap_aicore_llm/qa_retrieval/proxy_client/openai/proxy_api_engine_resource.py
+-rw-r--r--  2.0 unx     3848 b- defN 23-Jun-22 10:17 sap_aicore_llm/qa_retrieval/proxy_client/openai/proxy_completion.py
+-rw-r--r--  2.0 unx     2578 b- defN 23-Jun-22 10:17 sap_aicore_llm/qa_retrieval/proxy_client/openai/proxy_embedding.py
+-rw-r--r--  2.0 unx       73 b- defN 23-Jun-22 10:17 sap_aicore_llm/qa_retrieval/storage/__init__.py
+-rw-r--r--  2.0 unx      587 b- defN 23-Jun-22 10:17 sap_aicore_llm/qa_retrieval/storage/vector.py
+-rw-r--r--  2.0 unx    12569 b- defN 23-Jun-22 10:19 sap_ai_core_llm-1.0.18.dist-info/LICENSE
+-rw-r--r--  2.0 unx    18330 b- defN 23-Jun-22 10:19 sap_ai_core_llm-1.0.18.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-22 10:19 sap_ai_core_llm-1.0.18.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Jun-22 10:19 sap_ai_core_llm-1.0.18.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     3699 b- defN 23-Jun-22 10:19 sap_ai_core_llm-1.0.18.dist-info/RECORD
+36 files, 70654 bytes uncompressed, 23670 bytes compressed:  66.5%
```

## zipnote {}

```diff
@@ -18,23 +18,92 @@
 
 Filename: sap_aicore_llm/pipelines/azure_openai/proxy/serving_template.yaml
 Comment: 
 
 Filename: sap_aicore_llm/pipelines/azure_openai/proxy/src/main.py
 Comment: 
 
-Filename: sap_ai_core_llm-1.0.10.dist-info/LICENSE
+Filename: sap_aicore_llm/pipelines/qa/Dockerfile
 Comment: 
 
-Filename: sap_ai_core_llm-1.0.10.dist-info/METADATA
+Filename: sap_aicore_llm/pipelines/qa/requirements.txt
 Comment: 
 
-Filename: sap_ai_core_llm-1.0.10.dist-info/WHEEL
+Filename: sap_aicore_llm/pipelines/qa/serving_template.yaml
 Comment: 
 
-Filename: sap_ai_core_llm-1.0.10.dist-info/top_level.txt
+Filename: sap_aicore_llm/pipelines/qa/src/index.py
 Comment: 
 
-Filename: sap_ai_core_llm-1.0.10.dist-info/RECORD
+Filename: sap_aicore_llm/pipelines/qa/src/query.py
+Comment: 
+
+Filename: sap_aicore_llm/qa_retrieval/__init__.py
+Comment: 
+
+Filename: sap_aicore_llm/qa_retrieval/config/__init__.py
+Comment: 
+
+Filename: sap_aicore_llm/qa_retrieval/manager/__init__.py
+Comment: 
+
+Filename: sap_aicore_llm/qa_retrieval/manager/indexer.py
+Comment: 
+
+Filename: sap_aicore_llm/qa_retrieval/manager/retriever.py
+Comment: 
+
+Filename: sap_aicore_llm/qa_retrieval/model/__init__.py
+Comment: 
+
+Filename: sap_aicore_llm/qa_retrieval/model/completion.py
+Comment: 
+
+Filename: sap_aicore_llm/qa_retrieval/model/embedding.py
+Comment: 
+
+Filename: sap_aicore_llm/qa_retrieval/proxy_client/__init__.py
+Comment: 
+
+Filename: sap_aicore_llm/qa_retrieval/proxy_client/identity.py
+Comment: 
+
+Filename: sap_aicore_llm/qa_retrieval/proxy_client/langchain/__init__.py
+Comment: 
+
+Filename: sap_aicore_llm/qa_retrieval/proxy_client/langchain/openai.py
+Comment: 
+
+Filename: sap_aicore_llm/qa_retrieval/proxy_client/openai/__init__.py
+Comment: 
+
+Filename: sap_aicore_llm/qa_retrieval/proxy_client/openai/proxy_api_engine_resource.py
+Comment: 
+
+Filename: sap_aicore_llm/qa_retrieval/proxy_client/openai/proxy_completion.py
+Comment: 
+
+Filename: sap_aicore_llm/qa_retrieval/proxy_client/openai/proxy_embedding.py
+Comment: 
+
+Filename: sap_aicore_llm/qa_retrieval/storage/__init__.py
+Comment: 
+
+Filename: sap_aicore_llm/qa_retrieval/storage/vector.py
+Comment: 
+
+Filename: sap_ai_core_llm-1.0.18.dist-info/LICENSE
+Comment: 
+
+Filename: sap_ai_core_llm-1.0.18.dist-info/METADATA
+Comment: 
+
+Filename: sap_ai_core_llm-1.0.18.dist-info/WHEEL
+Comment: 
+
+Filename: sap_ai_core_llm-1.0.18.dist-info/top_level.txt
+Comment: 
+
+Filename: sap_ai_core_llm-1.0.18.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sap_aicore_llm/RELEASE_INFO

```diff
@@ -1 +1 @@
-1.0.10
+1.0.18
```

## sap_aicore_llm/ai_core_content_spec.py

```diff
@@ -10,9 +10,9 @@
 
 
 spec = ContentPackage(
     name='sap-ai-core-llm',
     workflows_base_path=workflow_yaml.parent,
     workflows=workflows,
     description='content package for large language models for SAP AI Core',
-    version='1.0.0'
-)
+    version='1.1.0'
+)
```

## sap_aicore_llm/pipelines/workflows.yaml

```diff
@@ -1,6 +1,21 @@
 azure-openai-proxy:
     type: DeploymentYaml
     dockerfile: azure_openai/proxy/Dockerfile
     yaml: azure_openai/proxy/serving_template.yaml
     description: >
         Proxy requests to an Azure OpenAI deployment with SAP AI Core.
+
+qa-indexing:
+    type: ExecutionMetaflow
+    dockerfile: qa/Dockerfile
+    description: >
+        Reads documents from S3, embeds them and stores the result in a vector database.
+    py: qa/src/index.py
+    className: IndexUpsert
+
+qa-serving:
+    type: DeploymentYaml
+    dockerfile: qa/Dockerfile
+    yaml: qa/serving_template.yaml
+    description: >
+        Serve queries with context enrichment from a vector database.
```

## sap_aicore_llm/pipelines/azure_openai/proxy/requirements.txt

```diff
@@ -1,4 +1,4 @@
-requests==2.28.2
-Flask==2.2.2
+requests==2.31.0
+Flask==2.2.5
 gunicorn==20.1.0
 gunicorn[gevent]
```

## sap_aicore_llm/pipelines/azure_openai/proxy/serving_template.yaml

```diff
@@ -9,42 +9,43 @@
   labels:
     ai.sap.com/version: "<SCENARIO-VERSION>"
     scenarios.ai.sap.com/id: "<SCENARIO-ID>"
   name: <SERVING-EXECUTABLE-ID>
 spec:
   inputs:
     parameters:
-      - name: AzureDeploymentURL
+      - name: azureDeploymentUrl
         type: string
   template:
     apiVersion: "serving.kserve.io/v1beta1"
     metadata:
       annotations: |
         autoscaling.knative.dev/metric: concurrency   # condition when to scale
         autoscaling.knative.dev/target: 1
         autoscaling.knative.dev/targetBurstCapacity: 0
       labels: |
         ai.sap.com/resourcePlan: starter # computing power
-    spec: |
+    spec: |-
       predictor:
         imagePullSecrets:
           - name: $imagePullSecret
         minReplicas: 1
-        maxReplicas: 2    # how much to scale
+        maxReplicas: 2  # how much to scale
         containers:
         - name: kserve-container
           image: $image
           ports:
-            - containerPort: 9001    # customizable port
+            - containerPort: 9001  # customizable port
               protocol: TCP
           command: ["/bin/sh", "-c"]
           args:
             - >
-              set -e && echo "Starting" && gunicorn --workers 4 --worker-class gevent --chdir /app/src main:app -b 0.0.0.0:9001 # filename `main` flask variable `app`
-          envFrom:
-            - secretRef:
-                name: azure-openai-key
+              set -e && echo "Starting" && gunicorn --workers 4 --worker-class gevent --chdir /app/src main:app -b 0.0.0.0:9001  # filename `main` flask variable `app`
           env:
-            - name: AzureDeploymentURL # name of the environment variable inside Docker container
-              value: "{{inputs.parameters.AzureDeploymentURL}}" # value to set from local (to workflow) variable
+          - name: AZURE_API_KEY
+            valueFrom:
+              secretKeyRef:
+                name: azure-openai-key
+                key: azureapikey
+          - name: AZURE_DEPLOYMENT_URL  # name of the environment variable inside Docker container
+            value: "{{inputs.parameters.azureDeploymentUrl}}"  # value to set from local (to workflow) variable
         timeout: 30
-
```

## sap_aicore_llm/pipelines/azure_openai/proxy/src/main.py

```diff
@@ -2,77 +2,88 @@
 import requests
 import json
 from flask import Flask
 from flask import request as call_request
 from requests.exceptions import HTTPError
 
 config = {}
-config["AZURE_API_KEY"] = os.getenv("AzureAPIKey")
-config["AZURE_API_URL"] = os.getenv("AzureDeploymentURL")
+config["AZURE_API_KEY"] = os.getenv("AZURE_API_KEY")
+config["AZURE_DEPLOYMENT_URL"] = os.getenv("AZURE_DEPLOYMENT_URL")
 
 # Creates Flask serving engine
 app = Flask(__name__)
 
+
 @app.after_request
 def apply_security_headers(response):
     headers = get_security_headers()
     for key, value in headers.items():
         response.headers[key] = value
     return response
 
+
 def get_security_headers():
     headers = {
         "Content-Type": "application/json",
         "Strict-Transport-Security": "max-age=31536000; includeSubDomains",
         "Content-Security-Policy": "default-src 'self'",
         "X-Content-Security-Policy": "default-src 'self'",
         "X-Content-Type-Options": "nosniff"
     }
     return headers
 
+
 @app.errorhandler(HTTPError)
 def handle_http_exception(e):
     """Return JSON instead of HTML for HTTP errors."""
     # replace the body with JSON
     response = {
         "status_code": e.response.status_code,
         "error": f"{type(e).__name__}: {e.response.text}"
     }
- 
+
     response_data = sanitize_json(json.dumps(response))
     return response_data, e.response.status_code, get_security_headers()
 
 
 @app.errorhandler(Exception)
 def handle_exception(e):
     """Return JSON instead of HTML for errors."""
     response = {
         "status_code": 500,
         "error": f"{type(e).__name__}: {str(e)}"
     }
- 
+
     response_data = sanitize_json(json.dumps(response))
     return response_data, 500, get_security_headers()
 
+
 def sanitize_json(json_string):
-    s = json_string.replace("&", "&amp;") # Must be done first!
+    s = json_string.replace("&", "&amp;")  # Must be done first!
     s = s.replace("<", "&lt;")
     s = s.replace(">", "&gt;")
     return s
 
+
 @app.route("/v1/predict", methods=["POST"])
 def predict():
     global config
 
     payload = json.dumps(call_request.get_json())
 
     headers = {
         "api-key": str(config['AZURE_API_KEY']),
         "Content-Type": "application/json"
     }
 
-    response = requests.post(config["AZURE_API_URL"], headers=headers, data=payload)
+    response = requests.post(
+        config["AZURE_DEPLOYMENT_URL"], headers=headers, data=payload)
 
     response.raise_for_status()
 
     response_data = sanitize_json(json.dumps(response.json()))
-    return response_data, 200, get_security_headers()
+    return response_data, 200, get_security_headers()
+
+
+@app.get("/v1/healthz")
+def health():
+    return "OK", 200
```

## Comparing `sap_ai_core_llm-1.0.10.dist-info/LICENSE` & `sap_ai_core_llm-1.0.18.dist-info/LICENSE`

 * *Files identical despite different names*


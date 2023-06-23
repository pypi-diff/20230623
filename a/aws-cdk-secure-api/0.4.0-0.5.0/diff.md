# Comparing `tmp/aws-cdk-secure-api-0.4.0.tar.gz` & `tmp/aws-cdk-secure-api-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-cdk-secure-api-0.4.0.tar", last modified: Wed Jun 21 19:16:49 2023, max compression
+gzip compressed data, was "aws-cdk-secure-api-0.5.0.tar", last modified: Fri Jun 23 19:20:24 2023, max compression
```

## Comparing `aws-cdk-secure-api-0.4.0.tar` & `aws-cdk-secure-api-0.5.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:16:49.189321 aws-cdk-secure-api-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11894 2023-06-21 19:16:49.189321 aws-cdk-secure-api-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:16:49.185321 aws-cdk-secure-api-0.4.0/aws_cdk_secure_api/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/aws_cdk_secure_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/aws_cdk_secure_api/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21983 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/aws_cdk_secure_api/api_construct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:16:49.185321 aws-cdk-secure-api-0.4.0/aws_cdk_secure_api/aws/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/aws_cdk_secure_api/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/aws_cdk_secure_api/aws/client_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/aws_cdk_secure_api/aws/secrets_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/aws_cdk_secure_api/aws/ssm_parameter_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/aws_cdk_secure_api/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/aws_cdk_secure_api/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:16:49.185321 aws-cdk-secure-api-0.4.0/aws_cdk_secure_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11894 2023-06-21 19:16:48.000000 aws-cdk-secure-api-0.4.0/aws_cdk_secure_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-21 19:16:49.000000 aws-cdk-secure-api-0.4.0/aws_cdk_secure_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:16:48.000000 aws-cdk-secure-api-0.4.0/aws_cdk_secure_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:16:48.000000 aws-cdk-secure-api-0.4.0/aws_cdk_secure_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-21 19:16:48.000000 aws-cdk-secure-api-0.4.0/aws_cdk_secure_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-21 19:16:48.000000 aws-cdk-secure-api-0.4.0/aws_cdk_secure_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:16:49.189321 aws-cdk-secure-api-0.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/docs/aws_cdk_secure_api.aws.rst
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/docs/aws_cdk_secure_api.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     4918 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-21 19:16:49.189321 aws-cdk-secure-api-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:16:49.189321 aws-cdk-secure-api-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:16:49.189321 aws-cdk-secure-api-0.4.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-21 19:16:40.000000 aws-cdk-secure-api-0.4.0/tests/unit/test_aws_cdk_secure_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:20:24.631404 aws-cdk-secure-api-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-06-23 19:20:16.000000 aws-cdk-secure-api-0.5.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-23 19:20:16.000000 aws-cdk-secure-api-0.5.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-23 19:20:16.000000 aws-cdk-secure-api-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-23 19:20:16.000000 aws-cdk-secure-api-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12856 2023-06-23 19:20:24.631404 aws-cdk-secure-api-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-06-23 19:20:16.000000 aws-cdk-secure-api-0.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:20:24.627404 aws-cdk-secure-api-0.5.0/aws_cdk_secure_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-23 19:20:16.000000 aws-cdk-secure-api-0.5.0/aws_cdk_secure_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-23 19:20:16.000000 aws-cdk-secure-api-0.5.0/aws_cdk_secure_api/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23267 2023-06-23 19:20:16.000000 aws-cdk-secure-api-0.5.0/aws_cdk_secure_api/api_construct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:20:24.627404 aws-cdk-secure-api-0.5.0/aws_cdk_secure_api/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-23 19:20:16.000000 aws-cdk-secure-api-0.5.0/aws_cdk_secure_api/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-23 19:20:16.000000 aws-cdk-secure-api-0.5.0/aws_cdk_secure_api/aws/client_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-23 19:20:16.000000 aws-cdk-secure-api-0.5.0/aws_cdk_secure_api/aws/secrets_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-06-23 19:20:16.000000 aws-cdk-secure-api-0.5.0/aws_cdk_secure_api/aws/ssm_parameter_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-23 19:20:16.000000 aws-cdk-secure-api-0.5.0/aws_cdk_secure_api/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-23 19:20:16.000000 aws-cdk-secure-api-0.5.0/aws_cdk_secure_api/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:20:24.627404 aws-cdk-secure-api-0.5.0/aws_cdk_secure_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12856 2023-06-23 19:20:24.000000 aws-cdk-secure-api-0.5.0/aws_cdk_secure_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-23 19:20:24.000000 aws-cdk-secure-api-0.5.0/aws_cdk_secure_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 19:20:24.000000 aws-cdk-secure-api-0.5.0/aws_cdk_secure_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 19:20:24.000000 aws-cdk-secure-api-0.5.0/aws_cdk_secure_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-23 19:20:24.000000 aws-cdk-secure-api-0.5.0/aws_cdk_secure_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-23 19:20:24.000000 aws-cdk-secure-api-0.5.0/aws_cdk_secure_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:20:24.627404 aws-cdk-secure-api-0.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-23 19:20:16.000000 aws-cdk-secure-api-0.5.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-23 19:20:16.000000 aws-cdk-secure-api-0.5.0/docs/aws_cdk_secure_api.aws.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-23 19:20:16.000000 aws-cdk-secure-api-0.5.0/docs/aws_cdk_secure_api.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4918 2023-06-23 19:20:16.000000 aws-cdk-secure-api-0.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-23 19:20:16.000000 aws-cdk-secure-api-0.5.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-23 19:20:16.000000 aws-cdk-secure-api-0.5.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-23 19:20:16.000000 aws-cdk-secure-api-0.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-23 19:20:16.000000 aws-cdk-secure-api-0.5.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-23 19:20:16.000000 aws-cdk-secure-api-0.5.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-23 19:20:16.000000 aws-cdk-secure-api-0.5.0/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-23 19:20:16.000000 aws-cdk-secure-api-0.5.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-23 19:20:16.000000 aws-cdk-secure-api-0.5.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-23 19:20:24.631404 aws-cdk-secure-api-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-23 19:20:16.000000 aws-cdk-secure-api-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:20:24.627404 aws-cdk-secure-api-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 19:20:16.000000 aws-cdk-secure-api-0.5.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 19:20:24.631404 aws-cdk-secure-api-0.5.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-23 19:20:16.000000 aws-cdk-secure-api-0.5.0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-23 19:20:16.000000 aws-cdk-secure-api-0.5.0/tests/unit/test_aws_cdk_secure_api.py
```

### Comparing `aws-cdk-secure-api-0.4.0/CONTRIBUTING.rst` & `aws-cdk-secure-api-0.5.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.4.0/HISTORY.rst` & `aws-cdk-secure-api-0.5.0/HISTORY.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,27 @@
 =======
 History
 =======
 
+0.5.0 (2023-06-23)
+------------------
+
+**Features and Improvements**
+
+* Add option ``use_role`` in ``IAMConfig``, which when enabled will set up
+  an IAM Role (with permissions to invoke the API) to be assumed by the IAM User,
+  instead of directly attaching an IAM Policy to said User.
+
+0.4.0 (2023-06-22)
+------------------
+
+**Features and Improvements**
+
+* Add IAM Authentication via the new ``IAMSecureRestApi`` construct.
+
 0.3.0 (2023-05-17)
 ------------------
 
 **Features and Improvements**
 
 * Add a helper method ``add_resource_and_lambda_methods``, to set up a new
   API resource, a lambda integration, and setup HTTP method(s) on the
```

### Comparing `aws-cdk-secure-api-0.4.0/LICENSE` & `aws-cdk-secure-api-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.4.0/PKG-INFO` & `aws-cdk-secure-api-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk-secure-api
-Version: 0.4.0
+Version: 0.5.0
 Summary: A CDK (v2) Construct Library for Secure REST APIs
 Home-page: https://github.com/rnag/aws-cdk-secure-api
 Author: Ritvik Nag
 Author-email: rv.kvetch@gmail.com
 License: MIT
 Project-URL: Documentation, https://aws-cdk-secure-api.readthedocs.io
 Project-URL: Source, https://github.com/rnag/aws-cdk-secure-api
@@ -67,15 +67,15 @@
               a free service) as needed.
         
             * Local cache for the API key, so that API calls are not needed in future
               CDK deployments.
         
           * `AWS IAM authentication`_
         
-            * An IAM User (and Policy) is created with minimal permissions to call / invoke the API.
+            * An IAM User (and Policy/Role) is created with minimal permissions to call / invoke the API.
         
             * The IAM User Credentials (Access Keys) are stored in AWS Secrets Manager.
         
         * Helper methods for all constructs, such as ``add_resource_and_lambda_methods``, to make it easier to
           integrate a method for an AWS Lambda function for example.
         
         .. _`RestApi`: https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_apigateway.RestApi.html
@@ -154,14 +154,20 @@
             )
         
             # GET /path1
             api.add_resource_and_lambda_methods(get_handler, '/path1', 'GET')
             # PUT /path2, POST /path2
             api.add_resource_and_lambda_methods(put_handler, '/path2', Http.PUT, Http.POST)
         
+        To use an IAM Role instead of attaching a Policy directly to User:
+        
+        .. code:: python3
+        
+            IAMConfig(use_role=True)
+        
         AWS Profile
         -----------
         
         Note that if you normally pass the ``--profile`` to the ``cdk`` tool, for example such as::
         
             cdk deploy --profile my-aws-profile
         
@@ -203,28 +209,48 @@
         
         * ``APIKey`` - The API key for the endpoint, which needs to be specified
           as a value in an HTTP request's ``x-api-key`` header.
         
         * ``APIIAMUserCredentials`` - The URL link (to input in a browser) for the Secret
           stored in AWS Secrets Manager containing the AWS IAM Credentials for invoking the REST API.
         
+        * ``APIIAMRoleARN`` - The ARN of the IAM Role, used in an `AssumeRole`_ API call with the IAM User credentials.
+        
+        .. _`AssumeRole`: https://docs.aws.amazon.com/STS/latest/APIReference/API_AssumeRole.html
+        
         Credits
         -------
         
         This package was created with Cookiecutter_ and the `rnag/cookiecutter-pypackage`_ project template.
         
         .. _AWS IAM authentication: https://repost.aws/knowledge-center/iam-authentication-api-gateway
         .. _Cookiecutter: https://github.com/cookiecutter/cookiecutter
         .. _`rnag/cookiecutter-pypackage`: https://github.com/rnag/cookiecutter-pypackage
         
         
         =======
         History
         =======
         
+        0.5.0 (2023-06-23)
+        ------------------
+        
+        **Features and Improvements**
+        
+        * Add option ``use_role`` in ``IAMConfig``, which when enabled will set up
+          an IAM Role (with permissions to invoke the API) to be assumed by the IAM User,
+          instead of directly attaching an IAM Policy to said User.
+        
+        0.4.0 (2023-06-22)
+        ------------------
+        
+        **Features and Improvements**
+        
+        * Add IAM Authentication via the new ``IAMSecureRestApi`` construct.
+        
         0.3.0 (2023-05-17)
         ------------------
         
         **Features and Improvements**
         
         * Add a helper method ``add_resource_and_lambda_methods``, to set up a new
           API resource, a lambda integration, and setup HTTP method(s) on the
```

### Comparing `aws-cdk-secure-api-0.4.0/README.rst` & `aws-cdk-secure-api-0.5.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -57,15 +57,15 @@
       a free service) as needed.
 
     * Local cache for the API key, so that API calls are not needed in future
       CDK deployments.
 
   * `AWS IAM authentication`_
 
-    * An IAM User (and Policy) is created with minimal permissions to call / invoke the API.
+    * An IAM User (and Policy/Role) is created with minimal permissions to call / invoke the API.
 
     * The IAM User Credentials (Access Keys) are stored in AWS Secrets Manager.
 
 * Helper methods for all constructs, such as ``add_resource_and_lambda_methods``, to make it easier to
   integrate a method for an AWS Lambda function for example.
 
 .. _`RestApi`: https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_apigateway.RestApi.html
@@ -144,14 +144,20 @@
     )
 
     # GET /path1
     api.add_resource_and_lambda_methods(get_handler, '/path1', 'GET')
     # PUT /path2, POST /path2
     api.add_resource_and_lambda_methods(put_handler, '/path2', Http.PUT, Http.POST)
 
+To use an IAM Role instead of attaching a Policy directly to User:
+
+.. code:: python3
+
+    IAMConfig(use_role=True)
+
 AWS Profile
 -----------
 
 Note that if you normally pass the ``--profile`` to the ``cdk`` tool, for example such as::
 
     cdk deploy --profile my-aws-profile
 
@@ -193,14 +199,18 @@
 
 * ``APIKey`` - The API key for the endpoint, which needs to be specified
   as a value in an HTTP request's ``x-api-key`` header.
 
 * ``APIIAMUserCredentials`` - The URL link (to input in a browser) for the Secret
   stored in AWS Secrets Manager containing the AWS IAM Credentials for invoking the REST API.
 
+* ``APIIAMRoleARN`` - The ARN of the IAM Role, used in an `AssumeRole`_ API call with the IAM User credentials.
+
+.. _`AssumeRole`: https://docs.aws.amazon.com/STS/latest/APIReference/API_AssumeRole.html
+
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `rnag/cookiecutter-pypackage`_ project template.
 
 .. _AWS IAM authentication: https://repost.aws/knowledge-center/iam-authentication-api-gateway
 .. _Cookiecutter: https://github.com/cookiecutter/cookiecutter
```

### Comparing `aws-cdk-secure-api-0.4.0/aws_cdk_secure_api/__init__.py` & `aws-cdk-secure-api-0.5.0/aws_cdk_secure_api/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.4.0/aws_cdk_secure_api/api_construct.py` & `aws-cdk-secure-api-0.5.0/aws_cdk_secure_api/api_construct.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """AWS CDK Construct module."""
 from __future__ import annotations
 
 import os
 from urllib.parse import quote as url_encode
 
-from aws_cdk import CfnOutput, CfnResource, RemovalPolicy, SecretValue
+from aws_cdk import CfnOutput, CfnResource, Duration, RemovalPolicy, SecretValue
 
 from aws_cdk.aws_apigateway import (
     AuthorizationType,
     IResource,
     Integration,
     LambdaIntegration,
     RestApi,
     UsagePlanPerApiStage,
 )
-from aws_cdk.aws_iam import AccessKey, Policy, PolicyStatement, User
+from aws_cdk.aws_iam import (AccessKey, ArnPrincipal, CompositePrincipal,
+                             Policy, PolicyStatement, Role, User)
 from aws_cdk.aws_lambda import IFunction
 from aws_cdk.aws_secretsmanager import Secret
 from constructs import Construct
 
 from .aws import SecretsManager, SSM
 from .cache import APIKeyCache
 from .models import Config, Http, IAMConfig
@@ -371,27 +372,46 @@
                     access_key.access_key_id
                 ),
                 'secret-access-key': access_key.secret_access_key,
             },
             removal_policy=RemovalPolicy.DESTROY,
         )
 
+        if config.use_role:
+            role = Role(
+                self,
+                'api-invoke-role',
+                # Role can be assumed by the AWS account, or the newly created user
+                assumed_by=CompositePrincipal(
+                    ArnPrincipal(self.stack.format_arn(service='iam', region='', resource='root')),
+                    ArnPrincipal(user.user_arn),
+                ),
+                description='IAM Role to invoke the API',
+                max_session_duration=Duration.hours(3),
+                role_name=f'{stack_name}@api-invoke-role',
+            )
+            # attach this policy to the role created above
+            policy_kwargs = {'roles': [role]}
+        else:
+            role = None
+            # attach this policy to the user created above
+            policy_kwargs = {'users': [user]}
+
         # create an IAM Policy to invoke the API
         Policy(
             self,
             'api-invoke-policy',
             statements=[
                 # grant permissions to invoke the Rest API
                 PolicyStatement(
                     actions=['execute-api:Invoke'],
                     resources=[self.arn_for_execute_api(stage=stage_name)],
                 )
             ],
-            # attach this policy to the user created above
-            users=[user],
+            **policy_kwargs,
         )
 
         # Create usage plan for the API
         usage_plan_name = f'{stack_name}-usage-plan'
 
         self.add_usage_plan(
             usage_plan_name,
@@ -426,14 +446,25 @@
             output_name,
             value=f'https://{region_name}.console.aws.amazon.com/secretsmanager/secret'
             f'?name={url_encode(secret_name, safe="")}&region={region_name}',
             # Needs to be unique per account + region
             export_name=f'{output_name}-{stack_name}',
         )
 
+        if role:
+            # Output the Role ARN (Used for `sts:AssumeRole` API calls, with the IAM User credentials)
+            output_name = 'API:IAM:Role:ARN'
+            CfnOutput(
+                self.stack,
+                output_name,
+                value=role.role_arn,
+                # Needs to be unique per account + region
+                export_name=f'{output_name}-{stack_name}',
+            )
+
     def add_resource_and_lambda_methods(
         self, handler: IFunction, resource_name: str, *methods: Http | str
     ):
         """
         Adds a new resource -- at the `resource_name` path -- to the API Gateway.
 
         Also adds a lambda function the API Gateway, and associates it with one or
```

### Comparing `aws-cdk-secure-api-0.4.0/aws_cdk_secure_api/aws/client_cache.py` & `aws-cdk-secure-api-0.5.0/aws_cdk_secure_api/aws/client_cache.py`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.4.0/aws_cdk_secure_api/aws/secrets_manager.py` & `aws-cdk-secure-api-0.5.0/aws_cdk_secure_api/aws/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.4.0/aws_cdk_secure_api/aws/ssm_parameter_store.py` & `aws-cdk-secure-api-0.5.0/aws_cdk_secure_api/aws/ssm_parameter_store.py`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.4.0/aws_cdk_secure_api/cache.py` & `aws-cdk-secure-api-0.5.0/aws_cdk_secure_api/cache.py`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.4.0/aws_cdk_secure_api/models.py` & `aws-cdk-secure-api-0.5.0/aws_cdk_secure_api/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -46,14 +46,19 @@
 
 @dataclass
 class IAMConfig(Config):
     # secret name to hold the IAM User Credentials (Access Keys) for
     # invoking the Rest API.
     secret_name: str | None = None
 
+    # set up an IAM Role that can be assumed by the IAM User via
+    # the `sts:AssumeRole` API, instead of attaching an IAM Policy
+    # to the User
+    use_role: bool = False
+
 
 # noinspection PyArgumentList
 class Http(Enum):
     """Enum class to represent an HTTP method."""
     OPTIONS = auto()
     GET = auto()
     HEAD = auto()
```

### Comparing `aws-cdk-secure-api-0.4.0/aws_cdk_secure_api.egg-info/PKG-INFO` & `aws-cdk-secure-api-0.5.0/aws_cdk_secure_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cdk-secure-api
-Version: 0.4.0
+Version: 0.5.0
 Summary: A CDK (v2) Construct Library for Secure REST APIs
 Home-page: https://github.com/rnag/aws-cdk-secure-api
 Author: Ritvik Nag
 Author-email: rv.kvetch@gmail.com
 License: MIT
 Project-URL: Documentation, https://aws-cdk-secure-api.readthedocs.io
 Project-URL: Source, https://github.com/rnag/aws-cdk-secure-api
@@ -67,15 +67,15 @@
               a free service) as needed.
         
             * Local cache for the API key, so that API calls are not needed in future
               CDK deployments.
         
           * `AWS IAM authentication`_
         
-            * An IAM User (and Policy) is created with minimal permissions to call / invoke the API.
+            * An IAM User (and Policy/Role) is created with minimal permissions to call / invoke the API.
         
             * The IAM User Credentials (Access Keys) are stored in AWS Secrets Manager.
         
         * Helper methods for all constructs, such as ``add_resource_and_lambda_methods``, to make it easier to
           integrate a method for an AWS Lambda function for example.
         
         .. _`RestApi`: https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_apigateway.RestApi.html
@@ -154,14 +154,20 @@
             )
         
             # GET /path1
             api.add_resource_and_lambda_methods(get_handler, '/path1', 'GET')
             # PUT /path2, POST /path2
             api.add_resource_and_lambda_methods(put_handler, '/path2', Http.PUT, Http.POST)
         
+        To use an IAM Role instead of attaching a Policy directly to User:
+        
+        .. code:: python3
+        
+            IAMConfig(use_role=True)
+        
         AWS Profile
         -----------
         
         Note that if you normally pass the ``--profile`` to the ``cdk`` tool, for example such as::
         
             cdk deploy --profile my-aws-profile
         
@@ -203,28 +209,48 @@
         
         * ``APIKey`` - The API key for the endpoint, which needs to be specified
           as a value in an HTTP request's ``x-api-key`` header.
         
         * ``APIIAMUserCredentials`` - The URL link (to input in a browser) for the Secret
           stored in AWS Secrets Manager containing the AWS IAM Credentials for invoking the REST API.
         
+        * ``APIIAMRoleARN`` - The ARN of the IAM Role, used in an `AssumeRole`_ API call with the IAM User credentials.
+        
+        .. _`AssumeRole`: https://docs.aws.amazon.com/STS/latest/APIReference/API_AssumeRole.html
+        
         Credits
         -------
         
         This package was created with Cookiecutter_ and the `rnag/cookiecutter-pypackage`_ project template.
         
         .. _AWS IAM authentication: https://repost.aws/knowledge-center/iam-authentication-api-gateway
         .. _Cookiecutter: https://github.com/cookiecutter/cookiecutter
         .. _`rnag/cookiecutter-pypackage`: https://github.com/rnag/cookiecutter-pypackage
         
         
         =======
         History
         =======
         
+        0.5.0 (2023-06-23)
+        ------------------
+        
+        **Features and Improvements**
+        
+        * Add option ``use_role`` in ``IAMConfig``, which when enabled will set up
+          an IAM Role (with permissions to invoke the API) to be assumed by the IAM User,
+          instead of directly attaching an IAM Policy to said User.
+        
+        0.4.0 (2023-06-22)
+        ------------------
+        
+        **Features and Improvements**
+        
+        * Add IAM Authentication via the new ``IAMSecureRestApi`` construct.
+        
         0.3.0 (2023-05-17)
         ------------------
         
         **Features and Improvements**
         
         * Add a helper method ``add_resource_and_lambda_methods``, to set up a new
           API resource, a lambda integration, and setup HTTP method(s) on the
```

### Comparing `aws-cdk-secure-api-0.4.0/aws_cdk_secure_api.egg-info/SOURCES.txt` & `aws-cdk-secure-api-0.5.0/aws_cdk_secure_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.4.0/docs/Makefile` & `aws-cdk-secure-api-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.4.0/docs/aws_cdk_secure_api.aws.rst` & `aws-cdk-secure-api-0.5.0/docs/aws_cdk_secure_api.aws.rst`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.4.0/docs/aws_cdk_secure_api.rst` & `aws-cdk-secure-api-0.5.0/docs/aws_cdk_secure_api.rst`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.4.0/docs/conf.py` & `aws-cdk-secure-api-0.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.4.0/docs/installation.rst` & `aws-cdk-secure-api-0.5.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.4.0/docs/make.bat` & `aws-cdk-secure-api-0.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.4.0/setup.py` & `aws-cdk-secure-api-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `aws-cdk-secure-api-0.4.0/tests/unit/test_aws_cdk_secure_api.py` & `aws-cdk-secure-api-0.5.0/tests/unit/test_aws_cdk_secure_api.py`

 * *Files identical despite different names*


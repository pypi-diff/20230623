# Comparing `tmp/cdk-serverless-clamscan-2.4.99.tar.gz` & `tmp/cdk-serverless-clamscan-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-serverless-clamscan-2.4.99.tar", last modified: Tue Nov 29 00:33:02 2022, max compression
+gzip compressed data, was "cdk-serverless-clamscan-2.5.0.tar", last modified: Thu Jun 22 13:12:12 2023, max compression
```

## Comparing `cdk-serverless-clamscan-2.4.99.tar` & `cdk-serverless-clamscan-2.5.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 00:33:02.507713 cdk-serverless-clamscan-2.4.99/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2022-11-29 00:32:45.000000 cdk-serverless-clamscan-2.4.99/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-11-29 00:32:45.000000 cdk-serverless-clamscan-2.4.99/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       91 2022-11-29 00:32:45.000000 cdk-serverless-clamscan-2.4.99/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2022-11-29 00:33:02.507713 cdk-serverless-clamscan-2.4.99/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6186 2022-11-29 00:32:45.000000 cdk-serverless-clamscan-2.4.99/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2022-11-29 00:32:45.000000 cdk-serverless-clamscan-2.4.99/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-11-29 00:33:02.507713 cdk-serverless-clamscan-2.4.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2022-11-29 00:32:45.000000 cdk-serverless-clamscan-2.4.99/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 00:33:02.503713 cdk-serverless-clamscan-2.4.99/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 00:33:02.503713 cdk-serverless-clamscan-2.4.99/src/cdk_serverless_clamscan/
--rw-r--r--   0 runner    (1001) docker     (123)    32243 2022-11-29 00:32:45.000000 cdk-serverless-clamscan-2.4.99/src/cdk_serverless_clamscan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 00:33:02.503713 cdk-serverless-clamscan-2.4.99/src/cdk_serverless_clamscan/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2022-11-29 00:32:45.000000 cdk-serverless-clamscan-2.4.99/src/cdk_serverless_clamscan/_jsii/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 00:33:02.503713 cdk-serverless-clamscan-2.4.99/src/cdk_serverless_clamscan/_jsii/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2022-11-29 00:32:45.000000 cdk-serverless-clamscan-2.4.99/src/cdk_serverless_clamscan/_jsii/bin/0
--rw-r--r--   0 runner    (1001) docker     (123)   137147 2022-11-29 00:32:45.000000 cdk-serverless-clamscan-2.4.99/src/cdk_serverless_clamscan/_jsii/cdk-serverless-clamscan@2.4.99.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-29 00:32:45.000000 cdk-serverless-clamscan-2.4.99/src/cdk_serverless_clamscan/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-29 00:33:02.503713 cdk-serverless-clamscan-2.4.99/src/cdk_serverless_clamscan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2022-11-29 00:33:01.000000 cdk-serverless-clamscan-2.4.99/src/cdk_serverless_clamscan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      551 2022-11-29 00:33:02.000000 cdk-serverless-clamscan-2.4.99/src/cdk_serverless_clamscan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-29 00:33:01.000000 cdk-serverless-clamscan-2.4.99/src/cdk_serverless_clamscan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2022-11-29 00:33:02.000000 cdk-serverless-clamscan-2.4.99/src/cdk_serverless_clamscan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2022-11-29 00:33:02.000000 cdk-serverless-clamscan-2.4.99/src/cdk_serverless_clamscan.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:12:12.207562 cdk-serverless-clamscan-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-22 13:11:57.000000 cdk-serverless-clamscan-2.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-22 13:11:57.000000 cdk-serverless-clamscan-2.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-22 13:11:57.000000 cdk-serverless-clamscan-2.5.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     7195 2023-06-22 13:12:12.207562 cdk-serverless-clamscan-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-06-22 13:11:57.000000 cdk-serverless-clamscan-2.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-22 13:11:57.000000 cdk-serverless-clamscan-2.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 13:12:12.207562 cdk-serverless-clamscan-2.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-22 13:11:57.000000 cdk-serverless-clamscan-2.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:12:12.203562 cdk-serverless-clamscan-2.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:12:12.203562 cdk-serverless-clamscan-2.5.0/src/cdk_serverless_clamscan/
+-rw-r--r--   0 runner    (1001) docker     (123)    33603 2023-06-22 13:11:57.000000 cdk-serverless-clamscan-2.5.0/src/cdk_serverless_clamscan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:12:12.207562 cdk-serverless-clamscan-2.5.0/src/cdk_serverless_clamscan/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-22 13:11:57.000000 cdk-serverless-clamscan-2.5.0/src/cdk_serverless_clamscan/_jsii/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:12:12.207562 cdk-serverless-clamscan-2.5.0/src/cdk_serverless_clamscan/_jsii/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-22 13:11:57.000000 cdk-serverless-clamscan-2.5.0/src/cdk_serverless_clamscan/_jsii/bin/0
+-rw-r--r--   0 runner    (1001) docker     (123)   137088 2023-06-22 13:11:57.000000 cdk-serverless-clamscan-2.5.0/src/cdk_serverless_clamscan/_jsii/cdk-serverless-clamscan@2.5.0.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 13:11:57.000000 cdk-serverless-clamscan-2.5.0/src/cdk_serverless_clamscan/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:12:12.207562 cdk-serverless-clamscan-2.5.0/src/cdk_serverless_clamscan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7195 2023-06-22 13:12:12.000000 cdk-serverless-clamscan-2.5.0/src/cdk_serverless_clamscan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-22 13:12:12.000000 cdk-serverless-clamscan-2.5.0/src/cdk_serverless_clamscan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 13:12:12.000000 cdk-serverless-clamscan-2.5.0/src/cdk_serverless_clamscan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-22 13:12:12.000000 cdk-serverless-clamscan-2.5.0/src/cdk_serverless_clamscan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-22 13:12:12.000000 cdk-serverless-clamscan-2.5.0/src/cdk_serverless_clamscan.egg-info/top_level.txt
```

### Comparing `cdk-serverless-clamscan-2.4.99/LICENSE` & `cdk-serverless-clamscan-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-serverless-clamscan-2.4.99/PKG-INFO` & `cdk-serverless-clamscan-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdk-serverless-clamscan
-Version: 2.4.99
+Version: 2.5.0
 Summary: Serverless architecture to virus scan objects in Amazon S3.
 Home-page: https://github.com/awslabs/cdk-serverless-clamscan
 Author: Amazon Web Services<donti@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/cdk-serverless-clamscan
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
@@ -202,9 +202,7 @@
 ## Contributing
 
 See [CONTRIBUTING](./CONTRIBUTING.md) for more information.
 
 ## License
 
 This project is licensed under the Apache-2.0 License.
-
-
```

### Comparing `cdk-serverless-clamscan-2.4.99/README.md` & `cdk-serverless-clamscan-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `cdk-serverless-clamscan-2.4.99/setup.py` & `cdk-serverless-clamscan-2.5.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-serverless-clamscan",
-    "version": "2.4.99",
+    "version": "2.5.0",
     "description": "Serverless architecture to virus scan objects in Amazon S3.",
     "license": "Apache-2.0",
     "url": "https://github.com/awslabs/cdk-serverless-clamscan",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services<donti@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,37 +22,38 @@
     },
     "packages": [
         "cdk_serverless_clamscan",
         "cdk_serverless_clamscan._jsii"
     ],
     "package_data": {
         "cdk_serverless_clamscan._jsii": [
-            "cdk-serverless-clamscan@2.4.99.jsii.tgz"
+            "cdk-serverless-clamscan@2.5.0.jsii.tgz"
         ],
         "cdk_serverless_clamscan": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.11.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.71.0, <2.0.0",
+        "jsii>=1.84.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved"
     ],
     "scripts": [
         "src/cdk_serverless_clamscan/_jsii/bin/0"
     ]
```

### Comparing `cdk-serverless-clamscan-2.4.99/src/cdk_serverless_clamscan/__init__.py` & `cdk-serverless-clamscan-2.5.0/src/cdk_serverless_clamscan/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -193,25 +193,25 @@
 import publication
 import typing_extensions
 
 from typeguard import check_type
 
 from ._jsii import *
 
-import aws_cdk.aws_efs
-import aws_cdk.aws_events
-import aws_cdk.aws_iam
-import aws_cdk.aws_lambda
-import aws_cdk.aws_s3
-import aws_cdk.aws_sqs
-import constructs
+import aws_cdk.aws_efs as _aws_cdk_aws_efs_ceddda9d
+import aws_cdk.aws_events as _aws_cdk_aws_events_ceddda9d
+import aws_cdk.aws_iam as _aws_cdk_aws_iam_ceddda9d
+import aws_cdk.aws_lambda as _aws_cdk_aws_lambda_ceddda9d
+import aws_cdk.aws_s3 as _aws_cdk_aws_s3_ceddda9d
+import aws_cdk.aws_sqs as _aws_cdk_aws_sqs_ceddda9d
+import constructs as _constructs_77d1e7e8
 
 
 class ServerlessClamscan(
-    constructs.Construct,
+    _constructs_77d1e7e8.Construct,
     metaclass=jsii.JSIIMeta,
     jsii_type="cdk-serverless-clamscan.ServerlessClamscan",
 ):
     '''An `aws-cdk <https://github.com/aws/aws-cdk>`_ construct that uses `ClamAV® <https://www.clamav.net/>`_. to scan objects in Amazon S3 for viruses. The construct provides a flexible interface for a system to act based on the results of a ClamAV virus scan.
 
     The construct creates a Lambda function with EFS integration to support larger files.
     A VPC with isolated subnets, a S3 Gateway endpoint will also be created.
@@ -240,24 +240,24 @@
     Note: The Virus Definitions bucket policy will likely cause a deletion error if you choose to delete
     the stack associated in the construct. However since the bucket itself gets deleted, you can delete
     the stack again to resolve the error.
     '''
 
     def __init__(
         self,
-        scope: constructs.Construct,
+        scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         accept_responsibility_for_using_imported_bucket: typing.Optional[builtins.bool] = None,
-        buckets: typing.Optional[typing.Sequence[aws_cdk.aws_s3.IBucket]] = None,
-        defs_bucket_access_logs_config: typing.Optional[typing.Union["ServerlessClamscanLoggingProps", typing.Dict[str, typing.Any]]] = None,
+        buckets: typing.Optional[typing.Sequence[_aws_cdk_aws_s3_ceddda9d.IBucket]] = None,
+        defs_bucket_access_logs_config: typing.Optional[typing.Union["ServerlessClamscanLoggingProps", typing.Dict[builtins.str, typing.Any]]] = None,
         efs_encryption: typing.Optional[builtins.bool] = None,
-        efs_performance_mode: typing.Optional[aws_cdk.aws_efs.PerformanceMode] = None,
-        on_error: typing.Optional[aws_cdk.aws_lambda.IDestination] = None,
-        on_result: typing.Optional[aws_cdk.aws_lambda.IDestination] = None,
+        efs_performance_mode: typing.Optional[_aws_cdk_aws_efs_ceddda9d.PerformanceMode] = None,
+        on_error: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.IDestination] = None,
+        on_result: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.IDestination] = None,
         reserved_concurrency: typing.Optional[jsii.Number] = None,
         scan_function_memory_size: typing.Optional[jsii.Number] = None,
     ) -> None:
         '''Creates a ServerlessClamscan construct.
 
         :param scope: The parent creating construct (usually ``this``).
         :param id: The construct's name.
@@ -268,30 +268,15 @@
         :param efs_performance_mode: Set the performance mode of the EFS file system (Default: GENERAL_PURPOSE).
         :param on_error: The Lambda Destination for files that fail to scan and are marked 'ERROR' or stuck 'IN PROGRESS' due to a Lambda timeout (Default: Creates and publishes to a new SQS queue if unspecified).
         :param on_result: The Lambda Destination for files marked 'CLEAN' or 'INFECTED' based on the ClamAV Virus scan or 'N/A' for scans triggered by S3 folder creation events marked (Default: Creates and publishes to a new Event Bridge Bus if unspecified).
         :param reserved_concurrency: Optionally set a reserved concurrency for the virus scanning Lambda.
         :param scan_function_memory_size: Optionally set the memory allocation for the scan function. Note that low memory allocations may cause errors. (Default: 10240).
         '''
         if __debug__:
-            def stub(
-                scope: constructs.Construct,
-                id: builtins.str,
-                *,
-                accept_responsibility_for_using_imported_bucket: typing.Optional[builtins.bool] = None,
-                buckets: typing.Optional[typing.Sequence[aws_cdk.aws_s3.IBucket]] = None,
-                defs_bucket_access_logs_config: typing.Optional[typing.Union[ServerlessClamscanLoggingProps, typing.Dict[str, typing.Any]]] = None,
-                efs_encryption: typing.Optional[builtins.bool] = None,
-                efs_performance_mode: typing.Optional[aws_cdk.aws_efs.PerformanceMode] = None,
-                on_error: typing.Optional[aws_cdk.aws_lambda.IDestination] = None,
-                on_result: typing.Optional[aws_cdk.aws_lambda.IDestination] = None,
-                reserved_concurrency: typing.Optional[jsii.Number] = None,
-                scan_function_memory_size: typing.Optional[jsii.Number] = None,
-            ) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__ed8d91de6d3b1d3b5b25b039320198cf5ad1c0f9205948695f5a09421a986084)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = ServerlessClamscanProps(
             accept_responsibility_for_using_imported_bucket=accept_responsibility_for_using_imported_bucket,
             buckets=buckets,
             defs_bucket_access_logs_config=defs_bucket_access_logs_config,
             efs_encryption=efs_encryption,
@@ -301,102 +286,102 @@
             reserved_concurrency=reserved_concurrency,
             scan_function_memory_size=scan_function_memory_size,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
     @jsii.member(jsii_name="addSourceBucket")
-    def add_source_bucket(self, bucket: aws_cdk.aws_s3.IBucket) -> None:
+    def add_source_bucket(self, bucket: _aws_cdk_aws_s3_ceddda9d.IBucket) -> None:
         '''Sets the specified S3 Bucket as a s3:ObjectCreate* for the ClamAV function.
 
         Grants the ClamAV function permissions to get and tag objects.
         Adds a bucket policy to disallow GetObject operations on files that are tagged 'IN PROGRESS', 'INFECTED', or 'ERROR'.
 
         :param bucket: The bucket to add the scanning bucket policy and s3:ObjectCreate* trigger to.
         '''
         if __debug__:
-            def stub(bucket: aws_cdk.aws_s3.IBucket) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__3e814dc0b4006f620db601182ab2e1605421bf11a1ddd8d6862a3542134d7568)
             check_type(argname="argument bucket", value=bucket, expected_type=type_hints["bucket"])
         return typing.cast(None, jsii.invoke(self, "addSourceBucket", [bucket]))
 
     @jsii.member(jsii_name="getPolicyStatementForBucket")
     def get_policy_statement_for_bucket(
         self,
-        bucket: aws_cdk.aws_s3.IBucket,
-    ) -> aws_cdk.aws_iam.PolicyStatement:
+        bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
+    ) -> _aws_cdk_aws_iam_ceddda9d.PolicyStatement:
         '''Returns the statement that should be added to the bucket policy in order to prevent objects to be accessed when they are not clean or there have been scanning errors: this policy should be added manually if external buckets are passed to addSourceBucket().
 
         :param bucket: The bucket which you need to protect with the policy.
 
         :return: PolicyStatement the policy statement if available
         '''
         if __debug__:
-            def stub(bucket: aws_cdk.aws_s3.IBucket) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__7810beb50932b9b83ee8c63bc62209567de654d2032fafbe7348d1b7415fa413)
             check_type(argname="argument bucket", value=bucket, expected_type=type_hints["bucket"])
-        return typing.cast(aws_cdk.aws_iam.PolicyStatement, jsii.invoke(self, "getPolicyStatementForBucket", [bucket]))
+        return typing.cast(_aws_cdk_aws_iam_ceddda9d.PolicyStatement, jsii.invoke(self, "getPolicyStatementForBucket", [bucket]))
 
     @builtins.property
     @jsii.member(jsii_name="errorDest")
-    def error_dest(self) -> aws_cdk.aws_lambda.IDestination:
+    def error_dest(self) -> _aws_cdk_aws_lambda_ceddda9d.IDestination:
         '''The Lambda Destination for failed on erred scans [ERROR, IN PROGRESS (If error is due to Lambda timeout)].'''
-        return typing.cast(aws_cdk.aws_lambda.IDestination, jsii.get(self, "errorDest"))
+        return typing.cast(_aws_cdk_aws_lambda_ceddda9d.IDestination, jsii.get(self, "errorDest"))
 
     @builtins.property
     @jsii.member(jsii_name="resultDest")
-    def result_dest(self) -> aws_cdk.aws_lambda.IDestination:
+    def result_dest(self) -> _aws_cdk_aws_lambda_ceddda9d.IDestination:
         '''The Lambda Destination for completed ClamAV scans [CLEAN, INFECTED].'''
-        return typing.cast(aws_cdk.aws_lambda.IDestination, jsii.get(self, "resultDest"))
+        return typing.cast(_aws_cdk_aws_lambda_ceddda9d.IDestination, jsii.get(self, "resultDest"))
 
     @builtins.property
     @jsii.member(jsii_name="scanAssumedPrincipal")
-    def scan_assumed_principal(self) -> aws_cdk.aws_iam.ArnPrincipal:
+    def scan_assumed_principal(self) -> _aws_cdk_aws_iam_ceddda9d.ArnPrincipal:
         '''
         :return: ArnPrincipal the ARN of the assumed role principal for the scan function
         '''
-        return typing.cast(aws_cdk.aws_iam.ArnPrincipal, jsii.get(self, "scanAssumedPrincipal"))
+        return typing.cast(_aws_cdk_aws_iam_ceddda9d.ArnPrincipal, jsii.get(self, "scanAssumedPrincipal"))
 
     @builtins.property
     @jsii.member(jsii_name="cleanRule")
-    def clean_rule(self) -> typing.Optional[aws_cdk.aws_events.Rule]:
+    def clean_rule(self) -> typing.Optional[_aws_cdk_aws_events_ceddda9d.Rule]:
         '''Conditional: An Event Bridge Rule for files that are marked 'CLEAN' by ClamAV if a success destination was not specified.'''
-        return typing.cast(typing.Optional[aws_cdk.aws_events.Rule], jsii.get(self, "cleanRule"))
+        return typing.cast(typing.Optional[_aws_cdk_aws_events_ceddda9d.Rule], jsii.get(self, "cleanRule"))
 
     @builtins.property
     @jsii.member(jsii_name="defsAccessLogsBucket")
-    def defs_access_logs_bucket(self) -> typing.Optional[aws_cdk.aws_s3.IBucket]:
+    def defs_access_logs_bucket(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket]:
         '''Conditional: The Bucket for access logs for the virus definitions bucket if logging is enabled (defsBucketAccessLogsConfig).'''
-        return typing.cast(typing.Optional[aws_cdk.aws_s3.IBucket], jsii.get(self, "defsAccessLogsBucket"))
+        return typing.cast(typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket], jsii.get(self, "defsAccessLogsBucket"))
 
     @builtins.property
     @jsii.member(jsii_name="errorDeadLetterQueue")
-    def error_dead_letter_queue(self) -> typing.Optional[aws_cdk.aws_sqs.Queue]:
+    def error_dead_letter_queue(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_sqs_ceddda9d.Queue]:
         '''Conditional: The SQS Dead Letter Queue for the errorQueue if a failure (onError) destination was not specified.'''
-        return typing.cast(typing.Optional[aws_cdk.aws_sqs.Queue], jsii.get(self, "errorDeadLetterQueue"))
+        return typing.cast(typing.Optional[_aws_cdk_aws_sqs_ceddda9d.Queue], jsii.get(self, "errorDeadLetterQueue"))
 
     @builtins.property
     @jsii.member(jsii_name="errorQueue")
-    def error_queue(self) -> typing.Optional[aws_cdk.aws_sqs.Queue]:
+    def error_queue(self) -> typing.Optional[_aws_cdk_aws_sqs_ceddda9d.Queue]:
         '''Conditional: The SQS Queue for erred scans if a failure (onError) destination was not specified.'''
-        return typing.cast(typing.Optional[aws_cdk.aws_sqs.Queue], jsii.get(self, "errorQueue"))
+        return typing.cast(typing.Optional[_aws_cdk_aws_sqs_ceddda9d.Queue], jsii.get(self, "errorQueue"))
 
     @builtins.property
     @jsii.member(jsii_name="infectedRule")
-    def infected_rule(self) -> typing.Optional[aws_cdk.aws_events.Rule]:
+    def infected_rule(self) -> typing.Optional[_aws_cdk_aws_events_ceddda9d.Rule]:
         '''Conditional: An Event Bridge Rule for files that are marked 'INFECTED' by ClamAV if a success destination was not specified.'''
-        return typing.cast(typing.Optional[aws_cdk.aws_events.Rule], jsii.get(self, "infectedRule"))
+        return typing.cast(typing.Optional[_aws_cdk_aws_events_ceddda9d.Rule], jsii.get(self, "infectedRule"))
 
     @builtins.property
     @jsii.member(jsii_name="resultBus")
-    def result_bus(self) -> typing.Optional[aws_cdk.aws_events.EventBus]:
+    def result_bus(self) -> typing.Optional[_aws_cdk_aws_events_ceddda9d.EventBus]:
         '''Conditional: The Event Bridge Bus for completed ClamAV scans if a success (onResult) destination was not specified.'''
-        return typing.cast(typing.Optional[aws_cdk.aws_events.EventBus], jsii.get(self, "resultBus"))
+        return typing.cast(typing.Optional[_aws_cdk_aws_events_ceddda9d.EventBus], jsii.get(self, "resultBus"))
 
     @builtins.property
     @jsii.member(jsii_name="useImportedBuckets")
     def use_imported_buckets(self) -> typing.Optional[builtins.bool]:
         '''Conditional: When true, the user accepted the responsibility for using imported buckets.'''
         return typing.cast(typing.Optional[builtins.bool], jsii.get(self, "useImportedBuckets"))
 
@@ -406,45 +391,39 @@
     jsii_struct_bases=[],
     name_mapping={"logs_bucket": "logsBucket", "logs_prefix": "logsPrefix"},
 )
 class ServerlessClamscanLoggingProps:
     def __init__(
         self,
         *,
-        logs_bucket: typing.Optional[typing.Union[builtins.bool, aws_cdk.aws_s3.IBucket]] = None,
+        logs_bucket: typing.Optional[typing.Union[builtins.bool, _aws_cdk_aws_s3_ceddda9d.IBucket]] = None,
         logs_prefix: typing.Optional[builtins.str] = None,
     ) -> None:
         '''Interface for ServerlessClamscan Virus Definitions S3 Bucket Logging.
 
         :param logs_bucket: Destination bucket for the server access logs (Default: Creates a new S3 Bucket for access logs).
         :param logs_prefix: Optional log file prefix to use for the bucket's access logs, option is ignored if logs_bucket is set to false.
         '''
         if __debug__:
-            def stub(
-                *,
-                logs_bucket: typing.Optional[typing.Union[builtins.bool, aws_cdk.aws_s3.IBucket]] = None,
-                logs_prefix: typing.Optional[builtins.str] = None,
-            ) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__c6710eb9eef2e9b05a93d9fba80fbf988499356d748d843afa0ab4772c40b9a4)
             check_type(argname="argument logs_bucket", value=logs_bucket, expected_type=type_hints["logs_bucket"])
             check_type(argname="argument logs_prefix", value=logs_prefix, expected_type=type_hints["logs_prefix"])
-        self._values: typing.Dict[str, typing.Any] = {}
+        self._values: typing.Dict[builtins.str, typing.Any] = {}
         if logs_bucket is not None:
             self._values["logs_bucket"] = logs_bucket
         if logs_prefix is not None:
             self._values["logs_prefix"] = logs_prefix
 
     @builtins.property
     def logs_bucket(
         self,
-    ) -> typing.Optional[typing.Union[builtins.bool, aws_cdk.aws_s3.IBucket]]:
+    ) -> typing.Optional[typing.Union[builtins.bool, _aws_cdk_aws_s3_ceddda9d.IBucket]]:
         '''Destination bucket for the server access logs (Default: Creates a new S3 Bucket for access logs).'''
         result = self._values.get("logs_bucket")
-        return typing.cast(typing.Optional[typing.Union[builtins.bool, aws_cdk.aws_s3.IBucket]], result)
+        return typing.cast(typing.Optional[typing.Union[builtins.bool, _aws_cdk_aws_s3_ceddda9d.IBucket]], result)
 
     @builtins.property
     def logs_prefix(self) -> typing.Optional[builtins.str]:
         '''Optional log file prefix to use for the bucket's access logs, option is ignored if logs_bucket is set to false.'''
         result = self._values.get("logs_prefix")
         return typing.cast(typing.Optional[builtins.str], result)
 
@@ -476,20 +455,20 @@
     },
 )
 class ServerlessClamscanProps:
     def __init__(
         self,
         *,
         accept_responsibility_for_using_imported_bucket: typing.Optional[builtins.bool] = None,
-        buckets: typing.Optional[typing.Sequence[aws_cdk.aws_s3.IBucket]] = None,
-        defs_bucket_access_logs_config: typing.Optional[typing.Union[ServerlessClamscanLoggingProps, typing.Dict[str, typing.Any]]] = None,
+        buckets: typing.Optional[typing.Sequence[_aws_cdk_aws_s3_ceddda9d.IBucket]] = None,
+        defs_bucket_access_logs_config: typing.Optional[typing.Union[ServerlessClamscanLoggingProps, typing.Dict[builtins.str, typing.Any]]] = None,
         efs_encryption: typing.Optional[builtins.bool] = None,
-        efs_performance_mode: typing.Optional[aws_cdk.aws_efs.PerformanceMode] = None,
-        on_error: typing.Optional[aws_cdk.aws_lambda.IDestination] = None,
-        on_result: typing.Optional[aws_cdk.aws_lambda.IDestination] = None,
+        efs_performance_mode: typing.Optional[_aws_cdk_aws_efs_ceddda9d.PerformanceMode] = None,
+        on_error: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.IDestination] = None,
+        on_result: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.IDestination] = None,
         reserved_concurrency: typing.Optional[jsii.Number] = None,
         scan_function_memory_size: typing.Optional[jsii.Number] = None,
     ) -> None:
         '''Interface for creating a ServerlessClamscan.
 
         :param accept_responsibility_for_using_imported_bucket: Allows the use of imported buckets. When using imported buckets the user is responsible for adding the required policy statement to the bucket policy: ``getPolicyStatementForBucket()`` can be used to retrieve the policy statement required by the solution.
         :param buckets: An optional list of S3 buckets to configure for ClamAV Virus Scanning; buckets can be added later by calling addSourceBucket.
@@ -500,38 +479,25 @@
         :param on_result: The Lambda Destination for files marked 'CLEAN' or 'INFECTED' based on the ClamAV Virus scan or 'N/A' for scans triggered by S3 folder creation events marked (Default: Creates and publishes to a new Event Bridge Bus if unspecified).
         :param reserved_concurrency: Optionally set a reserved concurrency for the virus scanning Lambda.
         :param scan_function_memory_size: Optionally set the memory allocation for the scan function. Note that low memory allocations may cause errors. (Default: 10240).
         '''
         if isinstance(defs_bucket_access_logs_config, dict):
             defs_bucket_access_logs_config = ServerlessClamscanLoggingProps(**defs_bucket_access_logs_config)
         if __debug__:
-            def stub(
-                *,
-                accept_responsibility_for_using_imported_bucket: typing.Optional[builtins.bool] = None,
-                buckets: typing.Optional[typing.Sequence[aws_cdk.aws_s3.IBucket]] = None,
-                defs_bucket_access_logs_config: typing.Optional[typing.Union[ServerlessClamscanLoggingProps, typing.Dict[str, typing.Any]]] = None,
-                efs_encryption: typing.Optional[builtins.bool] = None,
-                efs_performance_mode: typing.Optional[aws_cdk.aws_efs.PerformanceMode] = None,
-                on_error: typing.Optional[aws_cdk.aws_lambda.IDestination] = None,
-                on_result: typing.Optional[aws_cdk.aws_lambda.IDestination] = None,
-                reserved_concurrency: typing.Optional[jsii.Number] = None,
-                scan_function_memory_size: typing.Optional[jsii.Number] = None,
-            ) -> None:
-                ...
-            type_hints = typing.get_type_hints(stub)
+            type_hints = typing.get_type_hints(_typecheckingstub__bcf16e4cfa40d24a942937d7d5ee19975f275f2c96366670b2ec79ce3f1a2213)
             check_type(argname="argument accept_responsibility_for_using_imported_bucket", value=accept_responsibility_for_using_imported_bucket, expected_type=type_hints["accept_responsibility_for_using_imported_bucket"])
             check_type(argname="argument buckets", value=buckets, expected_type=type_hints["buckets"])
             check_type(argname="argument defs_bucket_access_logs_config", value=defs_bucket_access_logs_config, expected_type=type_hints["defs_bucket_access_logs_config"])
             check_type(argname="argument efs_encryption", value=efs_encryption, expected_type=type_hints["efs_encryption"])
             check_type(argname="argument efs_performance_mode", value=efs_performance_mode, expected_type=type_hints["efs_performance_mode"])
             check_type(argname="argument on_error", value=on_error, expected_type=type_hints["on_error"])
             check_type(argname="argument on_result", value=on_result, expected_type=type_hints["on_result"])
             check_type(argname="argument reserved_concurrency", value=reserved_concurrency, expected_type=type_hints["reserved_concurrency"])
             check_type(argname="argument scan_function_memory_size", value=scan_function_memory_size, expected_type=type_hints["scan_function_memory_size"])
-        self._values: typing.Dict[str, typing.Any] = {}
+        self._values: typing.Dict[builtins.str, typing.Any] = {}
         if accept_responsibility_for_using_imported_bucket is not None:
             self._values["accept_responsibility_for_using_imported_bucket"] = accept_responsibility_for_using_imported_bucket
         if buckets is not None:
             self._values["buckets"] = buckets
         if defs_bucket_access_logs_config is not None:
             self._values["defs_bucket_access_logs_config"] = defs_bucket_access_logs_config
         if efs_encryption is not None:
@@ -555,21 +521,21 @@
 
         When using imported buckets the user is responsible for adding the required policy statement to the bucket policy: ``getPolicyStatementForBucket()`` can be used to retrieve the policy statement required by the solution.
         '''
         result = self._values.get("accept_responsibility_for_using_imported_bucket")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    def buckets(self) -> typing.Optional[typing.List[aws_cdk.aws_s3.IBucket]]:
+    def buckets(self) -> typing.Optional[typing.List[_aws_cdk_aws_s3_ceddda9d.IBucket]]:
         '''An optional list of S3 buckets to configure for ClamAV Virus Scanning;
 
         buckets can be added later by calling addSourceBucket.
         '''
         result = self._values.get("buckets")
-        return typing.cast(typing.Optional[typing.List[aws_cdk.aws_s3.IBucket]], result)
+        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_s3_ceddda9d.IBucket]], result)
 
     @builtins.property
     def defs_bucket_access_logs_config(
         self,
     ) -> typing.Optional[ServerlessClamscanLoggingProps]:
         '''Whether or not to enable Access Logging for the Virus Definitions bucket, you can specify an existing bucket and prefix (Default: Creates a new S3 Bucket for access logs).'''
         result = self._values.get("defs_bucket_access_logs_config")
@@ -578,30 +544,32 @@
     @builtins.property
     def efs_encryption(self) -> typing.Optional[builtins.bool]:
         '''Whether or not to enable encryption on EFS filesystem (Default: enabled).'''
         result = self._values.get("efs_encryption")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    def efs_performance_mode(self) -> typing.Optional[aws_cdk.aws_efs.PerformanceMode]:
+    def efs_performance_mode(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_efs_ceddda9d.PerformanceMode]:
         '''Set the performance mode of the EFS file system (Default: GENERAL_PURPOSE).'''
         result = self._values.get("efs_performance_mode")
-        return typing.cast(typing.Optional[aws_cdk.aws_efs.PerformanceMode], result)
+        return typing.cast(typing.Optional[_aws_cdk_aws_efs_ceddda9d.PerformanceMode], result)
 
     @builtins.property
-    def on_error(self) -> typing.Optional[aws_cdk.aws_lambda.IDestination]:
+    def on_error(self) -> typing.Optional[_aws_cdk_aws_lambda_ceddda9d.IDestination]:
         '''The Lambda Destination for files that fail to scan and are marked 'ERROR' or stuck 'IN PROGRESS' due to a Lambda timeout (Default: Creates and publishes to a new SQS queue if unspecified).'''
         result = self._values.get("on_error")
-        return typing.cast(typing.Optional[aws_cdk.aws_lambda.IDestination], result)
+        return typing.cast(typing.Optional[_aws_cdk_aws_lambda_ceddda9d.IDestination], result)
 
     @builtins.property
-    def on_result(self) -> typing.Optional[aws_cdk.aws_lambda.IDestination]:
+    def on_result(self) -> typing.Optional[_aws_cdk_aws_lambda_ceddda9d.IDestination]:
         '''The Lambda Destination for files marked 'CLEAN' or 'INFECTED' based on the ClamAV Virus scan or 'N/A' for scans triggered by S3 folder creation events marked (Default: Creates and publishes to a new Event Bridge Bus if unspecified).'''
         result = self._values.get("on_result")
-        return typing.cast(typing.Optional[aws_cdk.aws_lambda.IDestination], result)
+        return typing.cast(typing.Optional[_aws_cdk_aws_lambda_ceddda9d.IDestination], result)
 
     @builtins.property
     def reserved_concurrency(self) -> typing.Optional[jsii.Number]:
         '''Optionally set a reserved concurrency for the virus scanning Lambda.
 
         :see: https://docs.aws.amazon.com/lambda/latest/operatorguide/reserved-concurrency.html
         '''
@@ -634,7 +602,59 @@
 __all__ = [
     "ServerlessClamscan",
     "ServerlessClamscanLoggingProps",
     "ServerlessClamscanProps",
 ]
 
 publication.publish()
+
+def _typecheckingstub__ed8d91de6d3b1d3b5b25b039320198cf5ad1c0f9205948695f5a09421a986084(
+    scope: _constructs_77d1e7e8.Construct,
+    id: builtins.str,
+    *,
+    accept_responsibility_for_using_imported_bucket: typing.Optional[builtins.bool] = None,
+    buckets: typing.Optional[typing.Sequence[_aws_cdk_aws_s3_ceddda9d.IBucket]] = None,
+    defs_bucket_access_logs_config: typing.Optional[typing.Union[ServerlessClamscanLoggingProps, typing.Dict[builtins.str, typing.Any]]] = None,
+    efs_encryption: typing.Optional[builtins.bool] = None,
+    efs_performance_mode: typing.Optional[_aws_cdk_aws_efs_ceddda9d.PerformanceMode] = None,
+    on_error: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.IDestination] = None,
+    on_result: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.IDestination] = None,
+    reserved_concurrency: typing.Optional[jsii.Number] = None,
+    scan_function_memory_size: typing.Optional[jsii.Number] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__3e814dc0b4006f620db601182ab2e1605421bf11a1ddd8d6862a3542134d7568(
+    bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__7810beb50932b9b83ee8c63bc62209567de654d2032fafbe7348d1b7415fa413(
+    bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__c6710eb9eef2e9b05a93d9fba80fbf988499356d748d843afa0ab4772c40b9a4(
+    *,
+    logs_bucket: typing.Optional[typing.Union[builtins.bool, _aws_cdk_aws_s3_ceddda9d.IBucket]] = None,
+    logs_prefix: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__bcf16e4cfa40d24a942937d7d5ee19975f275f2c96366670b2ec79ce3f1a2213(
+    *,
+    accept_responsibility_for_using_imported_bucket: typing.Optional[builtins.bool] = None,
+    buckets: typing.Optional[typing.Sequence[_aws_cdk_aws_s3_ceddda9d.IBucket]] = None,
+    defs_bucket_access_logs_config: typing.Optional[typing.Union[ServerlessClamscanLoggingProps, typing.Dict[builtins.str, typing.Any]]] = None,
+    efs_encryption: typing.Optional[builtins.bool] = None,
+    efs_performance_mode: typing.Optional[_aws_cdk_aws_efs_ceddda9d.PerformanceMode] = None,
+    on_error: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.IDestination] = None,
+    on_result: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.IDestination] = None,
+    reserved_concurrency: typing.Optional[jsii.Number] = None,
+    scan_function_memory_size: typing.Optional[jsii.Number] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
```

### Comparing `cdk-serverless-clamscan-2.4.99/src/cdk_serverless_clamscan.egg-info/PKG-INFO` & `cdk-serverless-clamscan-2.5.0/src/cdk_serverless_clamscan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdk-serverless-clamscan
-Version: 2.4.99
+Version: 2.5.0
 Summary: Serverless architecture to virus scan objects in Amazon S3.
 Home-page: https://github.com/awslabs/cdk-serverless-clamscan
 Author: Amazon Web Services<donti@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/cdk-serverless-clamscan
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
@@ -202,9 +202,7 @@
 ## Contributing
 
 See [CONTRIBUTING](./CONTRIBUTING.md) for more information.
 
 ## License
 
 This project is licensed under the Apache-2.0 License.
-
-
```

### Comparing `cdk-serverless-clamscan-2.4.99/src/cdk_serverless_clamscan.egg-info/SOURCES.txt` & `cdk-serverless-clamscan-2.5.0/src/cdk_serverless_clamscan.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 src/cdk_serverless_clamscan/py.typed
 src/cdk_serverless_clamscan.egg-info/PKG-INFO
 src/cdk_serverless_clamscan.egg-info/SOURCES.txt
 src/cdk_serverless_clamscan.egg-info/dependency_links.txt
 src/cdk_serverless_clamscan.egg-info/requires.txt
 src/cdk_serverless_clamscan.egg-info/top_level.txt
 src/cdk_serverless_clamscan/_jsii/__init__.py
-src/cdk_serverless_clamscan/_jsii/cdk-serverless-clamscan@2.4.99.jsii.tgz
+src/cdk_serverless_clamscan/_jsii/cdk-serverless-clamscan@2.5.0.jsii.tgz
 src/cdk_serverless_clamscan/_jsii/bin/0
```


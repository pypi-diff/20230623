# Comparing `tmp/fb-python-sdk-1.1.3.tar.gz` & `tmp/fb-python-sdk-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fb-python-sdk-1.1.3.tar", last modified: Wed Jun 21 12:11:13 2023, max compression
+gzip compressed data, was "fb-python-sdk-1.1.4.tar", last modified: Fri Jun 23 00:07:43 2023, max compression
```

## Comparing `fb-python-sdk-1.1.3.tar` & `fb-python-sdk-1.1.4.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-21 12:11:13.679507 fb-python-sdk-1.1.3/
--rw-r--r--   0 mac        (501) staff       (20)     1064 2022-11-07 09:43:18.000000 fb-python-sdk-1.1.3/LICENSE
--rw-r--r--   0 mac        (501) staff       (20)       71 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.3/MANIFEST.in
--rw-r--r--   0 mac        (501) staff       (20)    10444 2023-06-21 12:11:13.678982 fb-python-sdk-1.1.3/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     9372 2023-05-15 14:37:00.000000 fb-python-sdk-1.1.3/README.md
--rw-r--r--   0 mac        (501) staff       (20)      128 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.3/dev-requirements.txt
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-21 12:11:13.662927 fb-python-sdk-1.1.3/fb_python_sdk.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)    10444 2023-06-21 12:11:13.000000 fb-python-sdk-1.1.3/fb_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     1210 2023-06-21 12:11:13.000000 fb-python-sdk-1.1.3/fb_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-06-21 12:11:13.000000 fb-python-sdk-1.1.3/fb_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)      218 2023-06-21 12:11:13.000000 fb-python-sdk-1.1.3/fb_python_sdk.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       34 2023-06-21 12:11:13.000000 fb-python-sdk-1.1.3/fb_python_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-21 12:11:13.670471 fb-python-sdk-1.1.3/fbclient/
--rw-r--r--   0 mac        (501) staff       (20)     2249 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.3/fbclient/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     1058 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.3/fbclient/category.py
--rw-r--r--   0 mac        (501) staff       (20)    17863 2023-05-15 14:41:03.000000 fb-python-sdk-1.1.3/fbclient/client.py
--rw-r--r--   0 mac        (501) staff       (20)    10775 2023-04-16 09:36:36.000000 fb-python-sdk-1.1.3/fbclient/common_types.py
--rw-r--r--   0 mac        (501) staff       (20)     8913 2023-04-16 01:04:02.000000 fb-python-sdk-1.1.3/fbclient/config.py
--rw-r--r--   0 mac        (501) staff       (20)     3342 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.3/fbclient/data_storage.py
--rw-r--r--   0 mac        (501) staff       (20)    12389 2023-01-20 17:20:21.000000 fb-python-sdk-1.1.3/fbclient/evaluator.py
--rw-r--r--   0 mac        (501) staff       (20)     9022 2023-05-15 14:41:03.000000 fb-python-sdk-1.1.3/fbclient/event_processor.py
--rw-r--r--   0 mac        (501) staff       (20)     4597 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.3/fbclient/event_types.py
--rw-r--r--   0 mac        (501) staff       (20)     3176 2023-06-21 11:37:24.000000 fb-python-sdk-1.1.3/fbclient/flag_change_notification.py
--rw-r--r--   0 mac        (501) staff       (20)    10087 2023-06-21 12:02:10.000000 fb-python-sdk-1.1.3/fbclient/interfaces.py
--rw-r--r--   0 mac        (501) staff       (20)     1595 2023-06-21 10:36:01.000000 fb-python-sdk-1.1.3/fbclient/notice_broadcaster.py
--rw-r--r--   0 mac        (501) staff       (20)     3688 2023-01-20 17:20:21.000000 fb-python-sdk-1.1.3/fbclient/status.py
--rw-r--r--   0 mac        (501) staff       (20)     3160 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.3/fbclient/status_types.py
--rw-r--r--   0 mac        (501) staff       (20)    10647 2023-06-21 12:02:22.000000 fb-python-sdk-1.1.3/fbclient/streaming.py
--rw-r--r--   0 mac        (501) staff       (20)      629 2023-04-17 09:37:42.000000 fb-python-sdk-1.1.3/fbclient/update_processor.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-21 12:11:13.673530 fb-python-sdk-1.1.3/fbclient/utils/
--rw-r--r--   0 mac        (501) staff       (20)     4339 2023-01-20 17:20:21.000000 fb-python-sdk-1.1.3/fbclient/utils/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     1950 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.3/fbclient/utils/exponential_backoff_jitter_strategy.py
--rw-r--r--   0 mac        (501) staff       (20)     5502 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.3/fbclient/utils/http_client.py
--rw-r--r--   0 mac        (501) staff       (20)     1320 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.3/fbclient/utils/repeatable_task.py
--rw-r--r--   0 mac        (501) staff       (20)     1158 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.3/fbclient/utils/rwlock.py
--rw-r--r--   0 mac        (501) staff       (20)      864 2023-01-20 17:20:21.000000 fb-python-sdk-1.1.3/fbclient/utils/variation_splitting_algorithm.py
--rw-r--r--   0 mac        (501) staff       (20)       18 2023-06-21 12:09:03.000000 fb-python-sdk-1.1.3/fbclient/version.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-21 12:11:13.675238 fb-python-sdk-1.1.3/intergration_tests/
--rw-r--r--   0 mac        (501) staff       (20)        0 2022-12-05 10:02:17.000000 fb-python-sdk-1.1.3/intergration_tests/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      942 2023-05-15 05:29:46.000000 fb-python-sdk-1.1.3/intergration_tests/readme.py
--rw-r--r--   0 mac        (501) staff       (20)     1398 2023-05-15 14:42:32.000000 fb-python-sdk-1.1.3/intergration_tests/run_in_start_no_wait.py
--rw-------   0 mac        (501) staff       (20)     1437 2023-06-21 12:05:39.000000 fb-python-sdk-1.1.3/intergration_tests/run_in_start_wait.py
--rw-r--r--   0 mac        (501) staff       (20)       84 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.3/pyproject.toml
--rw-r--r--   0 mac        (501) staff       (20)       81 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.3/requirements.txt
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-06-21 12:11:13.679608 fb-python-sdk-1.1.3/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)     1851 2023-04-17 09:37:42.000000 fb-python-sdk-1.1.3/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-21 12:11:13.678363 fb-python-sdk-1.1.3/tests/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-04-07 15:01:21.000000 fb-python-sdk-1.1.3/tests/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     3785 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.3/tests/test_data_storage.py
--rw-r--r--   0 mac        (501) staff       (20)     4435 2023-01-20 17:20:21.000000 fb-python-sdk-1.1.3/tests/test_data_update_status_provider.py
--rw-r--r--   0 mac        (501) staff       (20)     4675 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.3/tests/test_evaluator.py
--rw-r--r--   0 mac        (501) staff       (20)     4475 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.3/tests/test_event_processor.py
--rw-r--r--   0 mac        (501) staff       (20)    10823 2023-04-17 09:37:42.000000 fb-python-sdk-1.1.3/tests/test_fbclient.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-23 00:07:43.762469 fb-python-sdk-1.1.4/
+-rw-r--r--   0 mac        (501) staff       (20)     1064 2022-11-07 09:43:18.000000 fb-python-sdk-1.1.4/LICENSE
+-rw-r--r--   0 mac        (501) staff       (20)       71 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.4/MANIFEST.in
+-rw-r--r--   0 mac        (501) staff       (20)    12546 2023-06-23 00:07:43.762018 fb-python-sdk-1.1.4/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)    11474 2023-06-23 00:04:27.000000 fb-python-sdk-1.1.4/README.md
+-rw-r--r--   0 mac        (501) staff       (20)      128 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.4/dev-requirements.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-23 00:07:43.745746 fb-python-sdk-1.1.4/fb_python_sdk.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)    12546 2023-06-23 00:07:43.000000 fb-python-sdk-1.1.4/fb_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     1249 2023-06-23 00:07:43.000000 fb-python-sdk-1.1.4/fb_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-06-23 00:07:43.000000 fb-python-sdk-1.1.4/fb_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)      218 2023-06-23 00:07:43.000000 fb-python-sdk-1.1.4/fb_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       34 2023-06-23 00:07:43.000000 fb-python-sdk-1.1.4/fb_python_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-23 00:07:43.754281 fb-python-sdk-1.1.4/fbclient/
+-rw-r--r--   0 mac        (501) staff       (20)     2249 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.4/fbclient/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     1058 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.4/fbclient/category.py
+-rw-r--r--   0 mac        (501) staff       (20)    18476 2023-06-23 00:04:27.000000 fb-python-sdk-1.1.4/fbclient/client.py
+-rw-r--r--   0 mac        (501) staff       (20)    10775 2023-04-16 09:36:36.000000 fb-python-sdk-1.1.4/fbclient/common_types.py
+-rw-r--r--   0 mac        (501) staff       (20)     8913 2023-04-16 01:04:02.000000 fb-python-sdk-1.1.4/fbclient/config.py
+-rw-r--r--   0 mac        (501) staff       (20)     3342 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.4/fbclient/data_storage.py
+-rw-r--r--   0 mac        (501) staff       (20)    12387 2023-06-23 00:04:27.000000 fb-python-sdk-1.1.4/fbclient/evaluator.py
+-rw-r--r--   0 mac        (501) staff       (20)     9022 2023-05-15 14:41:03.000000 fb-python-sdk-1.1.4/fbclient/event_processor.py
+-rw-r--r--   0 mac        (501) staff       (20)     4597 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.4/fbclient/event_types.py
+-rw-r--r--   0 mac        (501) staff       (20)     8579 2023-06-23 00:04:27.000000 fb-python-sdk-1.1.4/fbclient/flag_change_notification.py
+-rw-r--r--   0 mac        (501) staff       (20)     9861 2023-06-23 00:04:27.000000 fb-python-sdk-1.1.4/fbclient/interfaces.py
+-rw-r--r--   0 mac        (501) staff       (20)     2126 2023-06-23 00:04:27.000000 fb-python-sdk-1.1.4/fbclient/notice_broadcaster.py
+-rw-r--r--   0 mac        (501) staff       (20)     3794 2023-06-23 00:04:27.000000 fb-python-sdk-1.1.4/fbclient/status.py
+-rw-r--r--   0 mac        (501) staff       (20)     3160 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.4/fbclient/status_types.py
+-rw-r--r--   0 mac        (501) staff       (20)    12866 2023-06-23 00:04:27.000000 fb-python-sdk-1.1.4/fbclient/streaming.py
+-rw-r--r--   0 mac        (501) staff       (20)      629 2023-04-17 09:37:42.000000 fb-python-sdk-1.1.4/fbclient/update_processor.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-23 00:07:43.757039 fb-python-sdk-1.1.4/fbclient/utils/
+-rw-r--r--   0 mac        (501) staff       (20)     4339 2023-01-20 17:20:21.000000 fb-python-sdk-1.1.4/fbclient/utils/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     1950 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.4/fbclient/utils/exponential_backoff_jitter_strategy.py
+-rw-r--r--   0 mac        (501) staff       (20)     5502 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.4/fbclient/utils/http_client.py
+-rw-r--r--   0 mac        (501) staff       (20)     1320 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.4/fbclient/utils/repeatable_task.py
+-rw-r--r--   0 mac        (501) staff       (20)     1158 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.4/fbclient/utils/rwlock.py
+-rw-r--r--   0 mac        (501) staff       (20)      864 2023-01-20 17:20:21.000000 fb-python-sdk-1.1.4/fbclient/utils/variation_splitting_algorithm.py
+-rw-r--r--   0 mac        (501) staff       (20)       18 2023-06-23 00:04:27.000000 fb-python-sdk-1.1.4/fbclient/version.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-23 00:07:43.758493 fb-python-sdk-1.1.4/intergration_tests/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2022-12-05 10:02:17.000000 fb-python-sdk-1.1.4/intergration_tests/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)      942 2023-05-15 05:29:46.000000 fb-python-sdk-1.1.4/intergration_tests/readme.py
+-rw-r--r--   0 mac        (501) staff       (20)     1398 2023-05-15 14:42:32.000000 fb-python-sdk-1.1.4/intergration_tests/run_in_start_no_wait.py
+-rw-------   0 mac        (501) staff       (20)     1898 2023-06-22 22:09:31.000000 fb-python-sdk-1.1.4/intergration_tests/run_in_start_wait.py
+-rw-r--r--   0 mac        (501) staff       (20)       84 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.4/pyproject.toml
+-rw-r--r--   0 mac        (501) staff       (20)       81 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.4/requirements.txt
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-06-23 00:07:43.762573 fb-python-sdk-1.1.4/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)     1851 2023-04-17 09:37:42.000000 fb-python-sdk-1.1.4/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-23 00:07:43.761510 fb-python-sdk-1.1.4/tests/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-04-07 15:01:21.000000 fb-python-sdk-1.1.4/tests/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     3785 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.4/tests/test_data_storage.py
+-rw-r--r--   0 mac        (501) staff       (20)     4435 2023-01-20 17:20:21.000000 fb-python-sdk-1.1.4/tests/test_data_update_status_provider.py
+-rw-r--r--   0 mac        (501) staff       (20)     4675 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.4/tests/test_evaluator.py
+-rw-r--r--   0 mac        (501) staff       (20)     4475 2022-12-08 07:25:31.000000 fb-python-sdk-1.1.4/tests/test_event_processor.py
+-rw-r--r--   0 mac        (501) staff       (20)    10800 2023-06-23 00:04:27.000000 fb-python-sdk-1.1.4/tests/test_fbclient.py
+-rw-r--r--   0 mac        (501) staff       (20)     3423 2023-06-23 00:04:27.000000 fb-python-sdk-1.1.4/tests/test_flag_change_notification.py
```

### Comparing `fb-python-sdk-1.1.3/LICENSE` & `fb-python-sdk-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.3/PKG-INFO` & `fb-python-sdk-1.1.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fb-python-sdk
-Version: 1.1.3
+Version: 1.1.4
 Summary: A Python SDK for FeatBit plateform
 Home-page: https://github.com/featbit/featbit-python-sdk
 Author: Dian SUN
 Author-email: featbit.master@gmail.com
 Project-URL: Code, https://github.com/featbit/featbit-python-sdk
 Project-URL: Issue tracker, https://github.com/featbit/featbit/issues
 Classifier: Development Status :: 5 - Production/Stable
@@ -46,14 +46,23 @@
 ### Installation
 install the sdk in using pip, this version of the SDK is compatible with Python 3.6 through 3.11.
 
 ```shell
 pip install fb-python-sdk
 ```
 
+### Prerequisite
+
+Before using the SDK, you need to obtain the environment secret and SDK URLs. 
+
+Follow the documentation below to retrieve these values
+
+- [How to get the environment secret](https://docs.featbit.co/docs/sdk/faq#how-to-get-the-environment-secret)
+- [How to get the SDK URLs](https://docs.featbit.co/docs/sdk/faq#how-to-get-the-sdk-urls)
+  
 ### Quick Start
 
 > Note that the _**env_secret**_, _**streaming_url**_ and _**event_url**_ are required to initialize the SDK.
 
 The following code demonstrates basic usage of the SDK.
 
 ```python
@@ -162,14 +171,48 @@
     user = {'key': user_key, 'name': user_name}
     all_flag_values = client.get_all_latest_flag_variations(user)
     detail = all_flag_values.get(flag_key, default=None)
 ```
 
 > Note that if evaluation called before Go SDK client initialized, you set the wrong flag key/user for the evaluation or the related feature flag is not found, SDK will return the default value you set. The `fbclient.common_types.EvalDetail` will explain the details of the latest evaluation including error raison.
 
+### Flag Tracking
+
+`fbclient.client.FBClient.flag_tracker` registers a listener to be notified of feature flag changes in general.
+
+Note that a flag value change listener is bound to a specific user and flag key.
+
+The flag value change listener will be notified whenever the SDK receives any change to any feature flag's configuration,
+or to a user segment that is referenced by a feature flag. To register a flag value change listener, use `add_flag_value_may_changed_listener` or `add_flag_value_changed_listener`
+
+When you track a flag change using `add_flag_value_may_changed_listener`, this does not necessarily mean the flag's value has changed for any particular flag, only that some part of the flag configuration was changed so that it *_MAY_* return a different value than it previously returned for some user.
+
+If you want to track a flag whose value *_MUST_* be changed, `add_flag_value_changed_listener` will register a listener that will be notified if and only if the flag value changes.
+
+Change notices only work if the SDK is actually connecting to FeatBit feature flag center.
+If the SDK is in offline mode, then it cannot know when there is a change, because flags are read on an as-needed basis.
+
+```python
+if client.initialize:
+    #  flag value may be changed
+    client.flag_tracker.add_flag_value_may_changed_listener(flag_key, user, callback_fn)
+    #  flag value must be changed
+    client.flag_tracker.add_flag_value_changed_listener(flag_key, user, callback_fn)
+
+```
+`flag_key`: the key of the feature flag to track
+
+`user`: the user to evaluate the flag value
+
+`callback_fn`: the function to be called for the flag value change
+* the first argument is the flag key
+* the second argument is the latest flag value
+
+
+
 ### Offline Mode
 
 In some situations, you might want to stop making remote calls to FeatBit. Here is how:
 
 ```python
 config = Config(env_secret, event_url, streaming_url, offline=True)
 ```
```

### Comparing `fb-python-sdk-1.1.3/README.md` & `fb-python-sdk-1.1.4/fb_python_sdk.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+Metadata-Version: 2.1
+Name: fb-python-sdk
+Version: 1.1.4
+Summary: A Python SDK for FeatBit plateform
+Home-page: https://github.com/featbit/featbit-python-sdk
+Author: Dian SUN
+Author-email: featbit.master@gmail.com
+Project-URL: Code, https://github.com/featbit/featbit-python-sdk
+Project-URL: Issue tracker, https://github.com/featbit/featbit/issues
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.6, <=3.11
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # FeatBit Server-Side SDK for Python
 
 ## Introduction
 
 This is the Python Server-Side SDK for the 100% open-source feature flags management platform [FeatBit](https://github.com/featbit/featbit).
 
 The FeatBit Server-Side SDK for Python is designed primarily for use in multi-user systems such as web servers and applications.
@@ -20,14 +46,23 @@
 ### Installation
 install the sdk in using pip, this version of the SDK is compatible with Python 3.6 through 3.11.
 
 ```shell
 pip install fb-python-sdk
 ```
 
+### Prerequisite
+
+Before using the SDK, you need to obtain the environment secret and SDK URLs. 
+
+Follow the documentation below to retrieve these values
+
+- [How to get the environment secret](https://docs.featbit.co/docs/sdk/faq#how-to-get-the-environment-secret)
+- [How to get the SDK URLs](https://docs.featbit.co/docs/sdk/faq#how-to-get-the-sdk-urls)
+  
 ### Quick Start
 
 > Note that the _**env_secret**_, _**streaming_url**_ and _**event_url**_ are required to initialize the SDK.
 
 The following code demonstrates basic usage of the SDK.
 
 ```python
@@ -136,14 +171,48 @@
     user = {'key': user_key, 'name': user_name}
     all_flag_values = client.get_all_latest_flag_variations(user)
     detail = all_flag_values.get(flag_key, default=None)
 ```
 
 > Note that if evaluation called before Go SDK client initialized, you set the wrong flag key/user for the evaluation or the related feature flag is not found, SDK will return the default value you set. The `fbclient.common_types.EvalDetail` will explain the details of the latest evaluation including error raison.
 
+### Flag Tracking
+
+`fbclient.client.FBClient.flag_tracker` registers a listener to be notified of feature flag changes in general.
+
+Note that a flag value change listener is bound to a specific user and flag key.
+
+The flag value change listener will be notified whenever the SDK receives any change to any feature flag's configuration,
+or to a user segment that is referenced by a feature flag. To register a flag value change listener, use `add_flag_value_may_changed_listener` or `add_flag_value_changed_listener`
+
+When you track a flag change using `add_flag_value_may_changed_listener`, this does not necessarily mean the flag's value has changed for any particular flag, only that some part of the flag configuration was changed so that it *_MAY_* return a different value than it previously returned for some user.
+
+If you want to track a flag whose value *_MUST_* be changed, `add_flag_value_changed_listener` will register a listener that will be notified if and only if the flag value changes.
+
+Change notices only work if the SDK is actually connecting to FeatBit feature flag center.
+If the SDK is in offline mode, then it cannot know when there is a change, because flags are read on an as-needed basis.
+
+```python
+if client.initialize:
+    #  flag value may be changed
+    client.flag_tracker.add_flag_value_may_changed_listener(flag_key, user, callback_fn)
+    #  flag value must be changed
+    client.flag_tracker.add_flag_value_changed_listener(flag_key, user, callback_fn)
+
+```
+`flag_key`: the key of the feature flag to track
+
+`user`: the user to evaluate the flag value
+
+`callback_fn`: the function to be called for the flag value change
+* the first argument is the flag key
+* the second argument is the latest flag value
+
+
+
 ### Offline Mode
 
 In some situations, you might want to stop making remote calls to FeatBit. Here is how:
 
 ```python
 config = Config(env_secret, event_url, streaming_url, offline=True)
 ```
```

### Comparing `fb-python-sdk-1.1.3/fb_python_sdk.egg-info/PKG-INFO` & `fb-python-sdk-1.1.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,7 @@
-Metadata-Version: 2.1
-Name: fb-python-sdk
-Version: 1.1.3
-Summary: A Python SDK for FeatBit plateform
-Home-page: https://github.com/featbit/featbit-python-sdk
-Author: Dian SUN
-Author-email: featbit.master@gmail.com
-Project-URL: Code, https://github.com/featbit/featbit-python-sdk
-Project-URL: Issue tracker, https://github.com/featbit/featbit/issues
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6, <=3.11
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # FeatBit Server-Side SDK for Python
 
 ## Introduction
 
 This is the Python Server-Side SDK for the 100% open-source feature flags management platform [FeatBit](https://github.com/featbit/featbit).
 
 The FeatBit Server-Side SDK for Python is designed primarily for use in multi-user systems such as web servers and applications.
@@ -46,14 +20,23 @@
 ### Installation
 install the sdk in using pip, this version of the SDK is compatible with Python 3.6 through 3.11.
 
 ```shell
 pip install fb-python-sdk
 ```
 
+### Prerequisite
+
+Before using the SDK, you need to obtain the environment secret and SDK URLs. 
+
+Follow the documentation below to retrieve these values
+
+- [How to get the environment secret](https://docs.featbit.co/docs/sdk/faq#how-to-get-the-environment-secret)
+- [How to get the SDK URLs](https://docs.featbit.co/docs/sdk/faq#how-to-get-the-sdk-urls)
+  
 ### Quick Start
 
 > Note that the _**env_secret**_, _**streaming_url**_ and _**event_url**_ are required to initialize the SDK.
 
 The following code demonstrates basic usage of the SDK.
 
 ```python
@@ -162,14 +145,48 @@
     user = {'key': user_key, 'name': user_name}
     all_flag_values = client.get_all_latest_flag_variations(user)
     detail = all_flag_values.get(flag_key, default=None)
 ```
 
 > Note that if evaluation called before Go SDK client initialized, you set the wrong flag key/user for the evaluation or the related feature flag is not found, SDK will return the default value you set. The `fbclient.common_types.EvalDetail` will explain the details of the latest evaluation including error raison.
 
+### Flag Tracking
+
+`fbclient.client.FBClient.flag_tracker` registers a listener to be notified of feature flag changes in general.
+
+Note that a flag value change listener is bound to a specific user and flag key.
+
+The flag value change listener will be notified whenever the SDK receives any change to any feature flag's configuration,
+or to a user segment that is referenced by a feature flag. To register a flag value change listener, use `add_flag_value_may_changed_listener` or `add_flag_value_changed_listener`
+
+When you track a flag change using `add_flag_value_may_changed_listener`, this does not necessarily mean the flag's value has changed for any particular flag, only that some part of the flag configuration was changed so that it *_MAY_* return a different value than it previously returned for some user.
+
+If you want to track a flag whose value *_MUST_* be changed, `add_flag_value_changed_listener` will register a listener that will be notified if and only if the flag value changes.
+
+Change notices only work if the SDK is actually connecting to FeatBit feature flag center.
+If the SDK is in offline mode, then it cannot know when there is a change, because flags are read on an as-needed basis.
+
+```python
+if client.initialize:
+    #  flag value may be changed
+    client.flag_tracker.add_flag_value_may_changed_listener(flag_key, user, callback_fn)
+    #  flag value must be changed
+    client.flag_tracker.add_flag_value_changed_listener(flag_key, user, callback_fn)
+
+```
+`flag_key`: the key of the feature flag to track
+
+`user`: the user to evaluate the flag value
+
+`callback_fn`: the function to be called for the flag value change
+* the first argument is the flag key
+* the second argument is the latest flag value
+
+
+
 ### Offline Mode
 
 In some situations, you might want to stop making remote calls to FeatBit. Here is how:
 
 ```python
 config = Config(env_secret, event_url, streaming_url, offline=True)
 ```
```

### Comparing `fb-python-sdk-1.1.3/fb_python_sdk.egg-info/SOURCES.txt` & `fb-python-sdk-1.1.4/fb_python_sdk.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -38,8 +38,9 @@
 intergration_tests/run_in_start_no_wait.py
 intergration_tests/run_in_start_wait.py
 tests/__init__.py
 tests/test_data_storage.py
 tests/test_data_update_status_provider.py
 tests/test_evaluator.py
 tests/test_event_processor.py
-tests/test_fbclient.py
+tests/test_fbclient.py
+tests/test_flag_change_notification.py
```

### Comparing `fb-python-sdk-1.1.3/fbclient/__init__.py` & `fb-python-sdk-1.1.4/fbclient/__init__.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.3/fbclient/category.py` & `fb-python-sdk-1.1.4/fbclient/category.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.3/fbclient/client.py` & `fb-python-sdk-1.1.4/fbclient/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 from fbclient.config import Config
 from fbclient.data_storage import NullDataStorage
 from fbclient.evaluator import (REASON_CLIENT_NOT_READY, REASON_ERROR,
                                 REASON_FLAG_NOT_FOUND,
                                 REASON_USER_NOT_SPECIFIED, Evaluator)
 from fbclient.event_processor import DefaultEventProcessor, NullEventProcessor
 from fbclient.event_types import FlagEvent, Metric, MetricEvent, UserEvent
+from fbclient.flag_change_notification import FlagTracker
 from fbclient.interfaces import DataUpdateStatusProvider
+from fbclient.notice_broadcaster import NoticeBroadcater
 from fbclient.status import DataUpdateStatusProviderImpl
 from fbclient.streaming import Streaming, _data_to_dict
 from fbclient.update_processor import NullUpdateProcessor
 from fbclient.utils import (cast_variation_by_flag_type, check_uwsgi, log,
                             simple_type_inference, valide_all_data)
 from fbclient.utils.http_client import DefaultSender
 
@@ -67,29 +69,31 @@
 
         self._config = config
         if self._config.is_offline:
             log.info("FB Python SDK: SDK is in offline mode")
         else:
             self._config.validate()
 
+        self._broadcaster = NoticeBroadcater()
+        self._flag_tracker = FlagTracker(self._broadcaster, self.variation)
+
         # init components
         # event processor
         self._event_processor = self._build_event_processor(config)
         self._event_handler = lambda event: self._event_processor.send_event(event)
         # data storage
         self._data_storage = config.data_storage
         # evaluator
         self._evaluator = Evaluator(lambda key: self._data_storage.get(FEATURE_FLAGS, key),
                                     lambda key: self._data_storage.get(SEGMENTS, key))
         # data updator and status provider
         self._update_status_provider = DataUpdateStatusProviderImpl(config.data_storage)
         # update processor
         update_processor_ready = threading.Event()
-        self._update_processor = self._build_update_processor(config, self._update_status_provider,
-                                                              update_processor_ready)
+        self._update_processor = self._build_update_processor(config, self._broadcaster, self._update_status_provider, update_processor_ready)
         self._update_processor.start()
 
         if start_wait > 0:
             if not isinstance(self._update_processor, NullUpdateProcessor):
                 log.info("FB Python SDK: Waiting for Client initialization in %s seconds" % str(start_wait))
 
             update_processor_ready.wait(start_wait)
@@ -107,24 +111,24 @@
 
         if config.is_offline:
             log.debug("Offline mode, SDK disable event processing")
             return NullEventProcessor(config, DefaultSender('insight', config, max_size=10))
 
         return DefaultEventProcessor(config, DefaultSender('insight', config, max_size=10))
 
-    def _build_update_processor(self, config: Config, update_status_provider, update_processor_event):
+    def _build_update_processor(self, config: Config, broadcaster: NoticeBroadcater, update_status_provider, update_processor_event):
         if config.update_processor_imp:
             log.debug("Using user-specified update processor: %s" % str(config.update_processor_imp))
             return config.update_processor_imp(config, update_status_provider, update_processor_event)
 
         if config.is_offline:
             log.debug("Offline mode, SDK disable streaming data updating")
             return NullUpdateProcessor(config, update_status_provider, update_processor_event)
 
-        return Streaming(config, update_status_provider, update_processor_event)
+        return Streaming(config, broadcaster, update_status_provider, update_processor_event)
 
     @property
     def initialize(self) -> bool:
         """Returns true if the client has successfully connected to feature flag center.
 
         If this returns false, it means that the client has not yet successfully connected to  feature flag center.
         It might still be in the process of starting up, or it might be attempting to reconnect after an
@@ -132,23 +136,33 @@
         """
         return self._update_processor.initialized
 
     @property
     def update_status_provider(self) -> DataUpdateStatusProvider:
         return self._update_status_provider
 
+    @property
+    def flag_tracker(self) -> FlagTracker:
+        """
+        Returns an object for tracking changes in feature flag configurations.
+        The :class:`FlagTracker` contains methods for requesting notifications about feature flag changes using
+        an event listener model.
+        """
+        return self._flag_tracker
+
     def stop(self):
         """Releases all threads and network connections used by SDK.
 
         Do not attempt to use the client after calling this method.
         """
         log.info("FB Python SDK: Python SDK client is closing...")
         self._data_storage.stop()
         self._update_processor.stop()
         self._event_processor.stop()
+        self._broadcaster.stop()
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, exc_traceback):
         self.stop()
```

### Comparing `fb-python-sdk-1.1.3/fbclient/common_types.py` & `fb-python-sdk-1.1.4/fbclient/common_types.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.3/fbclient/config.py` & `fb-python-sdk-1.1.4/fbclient/config.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.3/fbclient/data_storage.py` & `fb-python-sdk-1.1.4/fbclient/data_storage.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.3/fbclient/evaluator.py` & `fb-python-sdk-1.1.4/fbclient/evaluator.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
                                                   user,
                                                   REASON_FALLTHROUGH,
                                                   flag['key'],
                                                   flag['name'])
 
     def _match_any_rule(self, user: FBUser, rule: dict) -> bool:
         # conditions cannot be empty
-        return all(self._process_condition(user, condiction) for condiction in rule['conditions'])
+        return all(self._process_condition(user, condition) for condition in rule['conditions'])
 
     def _process_condition(self, user: FBUser, condition: dict) -> bool:
         op = condition['op']
         # segment hasn't any operation
         op = condition['property'] if not op else op
         if __THAN_CLAUSE__ in str(op):
             return self._than(user, condition)
```

### Comparing `fb-python-sdk-1.1.3/fbclient/event_processor.py` & `fb-python-sdk-1.1.4/fbclient/event_processor.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.3/fbclient/event_types.py` & `fb-python-sdk-1.1.4/fbclient/event_types.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.3/fbclient/interfaces.py` & `fb-python-sdk-1.1.4/fbclient/interfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,34 +265,17 @@
         Shuts down the connection to feature flag center
         """
         pass
 
 
 class Notice(ABC):
     """
-    This is not an insight event to be sent to FeatBit Flag Center; it is a notification to the SDK.
+    This is not an insight event to be sent to FeatBit Flag Center; it is a notice to notify the SDK that something has happened,
+    such as flag values updated
     """
     @property
     @abstractmethod
     def notice_type(self) -> str:
         """
         Returns the type of this notice
         """
         pass
-
-
-class Notifier(ABC):
-
-    @abstractmethod
-    def handle(self, notice: Notice):
-        """
-        Handles the notice
-        """
-        pass
-
-    @property
-    @abstractmethod
-    def name(self) -> str:
-        """
-        Returns the name of this notifier
-        """
-        pass
```

### Comparing `fb-python-sdk-1.1.3/fbclient/status.py` & `fb-python-sdk-1.1.4/fbclient/status.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,17 @@
             return False
         return True
 
     def __handle_exception(self, error: Exception, error_type: str, message: str):
         log.exception('FB Python SDK: Data Storage error: %s, UpdateProcessor will attempt to receive the data' % str(error))
         self.update_state(State.interrupted_state(error_type, message))
 
+    def get_all(self, kind: Category) -> Mapping[str, dict]:
+        return self.__storage.get_all(kind)
+
     @property
     def initialized(self) -> bool:
         return self.__storage.initialized
 
     @property
     def latest_version(self) -> int:
         return self.__storage.latest_version
```

### Comparing `fb-python-sdk-1.1.3/fbclient/status_types.py` & `fb-python-sdk-1.1.4/fbclient/status_types.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.3/fbclient/streaming.py` & `fb-python-sdk-1.1.4/fbclient/streaming.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,18 @@
 from typing import Optional, Tuple
 
 import websocket
 from websocket._exceptions import WebSocketException
 
 from fbclient.category import FEATURE_FLAGS, SEGMENTS
 from fbclient.config import Config
-from fbclient.interfaces import DataUpdateStatusProvider, UpdateProcessor
+from fbclient.flag_change_notification import FlagChangedNotice
+from fbclient.interfaces import UpdateProcessor
+from fbclient.notice_broadcaster import NoticeBroadcater
+from fbclient.status import DataUpdateStatusProviderImpl
 from fbclient.status_types import (DATA_INVALID_ERROR, NETWORK_ERROR,
                                    REQUEST_INVALID_ERROR, RUNTIME_ERROR,
                                    SYSTEM_QUIT, UNKNOWN_CLOSE_CODE,
                                    UNKNOWN_ERROR, WEBSOCKET_ERROR, State)
 from fbclient.utils import (build_headers, build_token,
                             from_str_datetime_to_millis, log, valide_all_data)
 from fbclient.utils.exponential_backoff_jitter_strategy import \
@@ -47,18 +50,20 @@
     all_data[FEATURE_FLAGS] = flags
     all_data[SEGMENTS] = segments
     for flag in data['featureFlags']:
         flag['timestamp'] = from_str_datetime_to_millis(flag['updatedAt'])
         flag['variationMap'] = dict((var['id'], var['value']) for var in flag['variations'])
         flag['_id'] = flag['id']
         flag['id'] = flag['key']
+        flag['cat'] = FEATURE_FLAGS
         flags[flag['id']] = {'id': flag['id'], 'timestamp': flag['timestamp'], 'isArchived': True} if flag['isArchived'] else flag
         version = max(version, flag['timestamp'])
     for segment in data['segments']:
         segment['timestamp'] = from_str_datetime_to_millis(segment['updatedAt'])
+        segment['cat'] = SEGMENTS
         segments[segment['id']] = {'id': segment['id'], 'timestamp': segment['timestamp'], 'isArchived': True} if segment['isArchived'] else segment
         version = max(version, segment['timestamp'])
     return version, all_data
 
 
 def _handle_ws_error(error: BaseException) -> Tuple[bool, bool, State]:
     if isinstance(error, WebSocketException):
@@ -71,17 +76,18 @@
     # an unexpected error occurs when the custom action is called, close ws connection to jump ws client forever loop
     return True, True, State.interrupted_state(RUNTIME_ERROR, str(error))
 
 
 class Streaming(Thread, UpdateProcessor):
     __ping_interval = 10.0
 
-    def __init__(self, config: Config, dataUpdateStatusProvider: DataUpdateStatusProvider, ready: Event):
+    def __init__(self, config: Config, broadcaster: NoticeBroadcater, dataUpdateStatusProvider: DataUpdateStatusProviderImpl, ready: Event):
         super().__init__(daemon=True)
         self.__config = config
+        self.__broadcaster = broadcaster
         self.__storage = dataUpdateStatusProvider
         self.__ready = ready
         self.__running = True
         self.__strategy = BackoffAndJitterStrategy(config.streaming_first_retry_delay)
         self.__wsapp = None
         self.__self_closed = _SelfClosed()
         self.__closed_by_error = False
@@ -184,27 +190,62 @@
         version = self.__storage.latest_version if self.__storage.latest_version > 0 else 0
         data_sync_msg = {'messageType': 'data-sync', 'data': {'timestamp': version}}
         json_str = json.dumps(data_sync_msg)
         wsapp.send(json_str)
 
     def _on_process_data(self, data):
 
+        def get_feature_flag_keys_from_segment(flags, segment_id):
+            flag_keys = []
+            for flag in flags.values():
+                for rule in flag['rules']:  # type: ignore
+                    for condition in rule['conditions']:  # type: ignore
+                        op = condition['op']  # type: ignore
+                        if not op:
+                            try:
+                                segment_ids = json.loads(condition['value'])  # type: ignore
+                                if segment_id in segment_ids:  # type: ignore
+                                    flag_keys.append(flag['id'])  # type: ignore
+                            except:
+                                pass
+            return set(flag_keys)
+
+        def broacasting():
+            flags = self.__storage.get_all(FEATURE_FLAGS)
+            for items in all_data.values() :
+                for item in sorted(items.values(), key=lambda x: x['timestamp']):
+                    if item['cat'] == FEATURE_FLAGS:
+                        # listen flag changes
+                        if item['id'] not in broacasting_ingnored_flag_keys:
+                            broacasting_ingnored_flag_keys.append(item['id'])
+                            self.__broadcaster.broadcast(FlagChangedNotice(item['id']))
+                    elif item['cat'] == SEGMENTS:
+                        # listen segment changes
+                        flag_keys = get_feature_flag_keys_from_segment(flags, item['id'])
+                        for flag_key in flag_keys:
+                            if flag_key not in broacasting_ingnored_flag_keys:
+                                broacasting_ingnored_flag_keys.append(flag_key)
+                                self.__broadcaster.broadcast(FlagChangedNotice(flag_key))
+
         log.debug('Streaming WebSocket is processing data')
         version, all_data = _data_to_dict(data)
         op_ok = False
         if 'patch' == data['eventType']:
             op_ok = all(self.__storage.upsert(cat, item['id'], item, item['timestamp'])
                         for cat, items in all_data.items() for item in sorted(items.values(), key=lambda x: x['timestamp']))
         else:
             op_ok = self.__storage.init(all_data, version)
         if op_ok:
             if not self.__ready.is_set():
                 # set ready when the initialization is complete.
                 self.__ready.set()
             self.__storage.update_state(State.ok_state())
+            # broadcast the flag change notices
+            broacasting_ingnored_flag_keys = []
+            broacasting()
             log.debug("processing data is well done")
         return op_ok
 
     def _on_message(self, wsapp: websocket.WebSocketApp, msg):
         log.trace('Streaming WebSocket data: %s' % msg)  # type: ignore
         try:
             all_data = json.loads(msg)
```

### Comparing `fb-python-sdk-1.1.3/fbclient/update_processor.py` & `fb-python-sdk-1.1.4/fbclient/update_processor.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.3/fbclient/utils/__init__.py` & `fb-python-sdk-1.1.4/fbclient/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.3/fbclient/utils/exponential_backoff_jitter_strategy.py` & `fb-python-sdk-1.1.4/fbclient/utils/exponential_backoff_jitter_strategy.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.3/fbclient/utils/http_client.py` & `fb-python-sdk-1.1.4/fbclient/utils/http_client.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.3/fbclient/utils/repeatable_task.py` & `fb-python-sdk-1.1.4/fbclient/utils/repeatable_task.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.3/fbclient/utils/rwlock.py` & `fb-python-sdk-1.1.4/fbclient/utils/rwlock.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.3/fbclient/utils/variation_splitting_algorithm.py` & `fb-python-sdk-1.1.4/fbclient/utils/variation_splitting_algorithm.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.3/intergration_tests/readme.py` & `fb-python-sdk-1.1.4/intergration_tests/readme.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.3/intergration_tests/run_in_start_no_wait.py` & `fb-python-sdk-1.1.4/intergration_tests/run_in_start_no_wait.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.3/intergration_tests/run_in_start_wait.py` & `fb-python-sdk-1.1.4/intergration_tests/run_in_start_wait.py`

 * *Files 27% similar despite different names*

```diff
@@ -14,23 +14,33 @@
 
 config = Config(env_secret, event_url='http://localhost:5100', streaming_url='ws://localhost:5100')
 
 set_config(config)
 
 client = get()
 
+previous_flag_changed_keys = []
+
 if client.initialize:
-    client.identify({'key': 'test-python-sdk-user', 'name': 'test-python-sdk-user'})
+    # client.identify({'key': 'test-python-sdk-user', 'name': 'test-python-sdk-user'})
+    def fn(flag_key, new_flag_value):
+        return log.info("%s value is %s" % (flag_key, new_flag_value))
     while True:
         line = input('input user key and flag key seperated by / \n')
         if 'exit' == line.strip():
             break
         try:
             user_key, flag_key, *_ = tuple(line.split('/'))
             user = {'key': user_key, 'name': user_key, 'country': 'cn'}
+            flag_changed_key = f'{user_key}_{flag_key}'
+            if flag_changed_key not in previous_flag_changed_keys:
+                client \
+                    .flag_tracker \
+                    .add_flag_value_changed_listener(flag_key, user, fn)
+                previous_flag_changed_keys.append(flag_key)
             fb_user = FBUser.from_dict(user)
             log.info('FB Python SDK Test: user= %s' % fb_user.to_json_str())
             t1 = time()
             log.info('FB Python SDK Test: variation= %s' % client.variation_detail(flag_key, user).to_json_str())
             t2 = time()
             log.info('FB Python SDK Test: execution time= %f' % (t2 - t1))
         except:
```

### Comparing `fb-python-sdk-1.1.3/setup.py` & `fb-python-sdk-1.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.3/tests/test_data_storage.py` & `fb-python-sdk-1.1.4/tests/test_data_storage.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.3/tests/test_data_update_status_provider.py` & `fb-python-sdk-1.1.4/tests/test_data_update_status_provider.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.3/tests/test_evaluator.py` & `fb-python-sdk-1.1.4/tests/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.3/tests/test_event_processor.py` & `fb-python-sdk-1.1.4/tests/test_event_processor.py`

 * *Files identical despite different names*

### Comparing `fb-python-sdk-1.1.3/tests/test_fbclient.py` & `fb-python-sdk-1.1.4/tests/test_fbclient.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import base64
 from datetime import datetime
 from pathlib import Path
-from time import sleep
 from unittest.mock import patch
 
 import pytest
 
 from fbclient.client import FBClient
 from fbclient.config import Config
 from fbclient.data_storage import InMemoryDataStorage
```


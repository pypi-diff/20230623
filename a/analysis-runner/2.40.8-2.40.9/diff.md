# Comparing `tmp/analysis-runner-2.40.8.tar.gz` & `tmp/analysis-runner-2.40.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "analysis-runner-2.40.8.tar", last modified: Tue Apr 18 08:15:49 2023, max compression
+gzip compressed data, was "analysis-runner-2.40.9.tar", last modified: Fri Jun 23 06:40:32 2023, max compression
```

## Comparing `analysis-runner-2.40.8.tar` & `analysis-runner-2.40.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:15:49.834061 analysis-runner-2.40.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-18 08:15:47.000000 analysis-runner-2.40.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-04-18 08:15:49.834061 analysis-runner-2.40.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-04-18 08:15:47.000000 analysis-runner-2.40.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:15:49.834061 analysis-runner-2.40.8/analysis_runner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:15:47.000000 analysis-runner-2.40.8/analysis_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-18 08:15:47.000000 analysis-runner-2.40.8/analysis_runner/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2125 2023-04-18 08:15:47.000000 analysis-runner-2.40.8/analysis_runner/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-04-18 08:15:47.000000 analysis-runner-2.40.8/analysis_runner/cli_analysisrunner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-04-18 08:15:47.000000 analysis-runner-2.40.8/analysis_runner/cli_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12498 2023-04-18 08:15:47.000000 analysis-runner-2.40.8/analysis_runner/cli_cromwell.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-18 08:15:47.000000 analysis-runner-2.40.8/analysis_runner/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    23811 2023-04-18 08:15:47.000000 analysis-runner-2.40.8/analysis_runner/cromwell.py
--rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-04-18 08:15:47.000000 analysis-runner-2.40.8/analysis_runner/cromwell_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11735 2023-04-18 08:15:47.000000 analysis-runner-2.40.8/analysis_runner/dataproc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-04-18 08:15:47.000000 analysis-runner-2.40.8/analysis_runner/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-04-18 08:15:47.000000 analysis-runner-2.40.8/analysis_runner/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:15:49.834061 analysis-runner-2.40.8/analysis_runner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-04-18 08:15:49.000000 analysis-runner-2.40.8/analysis_runner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-18 08:15:49.000000 analysis-runner-2.40.8/analysis_runner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:15:49.000000 analysis-runner-2.40.8/analysis_runner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-18 08:15:49.000000 analysis-runner-2.40.8/analysis_runner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:15:49.000000 analysis-runner-2.40.8/analysis_runner.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-18 08:15:49.000000 analysis-runner-2.40.8/analysis_runner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-18 08:15:49.000000 analysis-runner-2.40.8/analysis_runner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-18 08:15:47.000000 analysis-runner-2.40.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 08:15:49.834061 analysis-runner-2.40.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-18 08:15:47.000000 analysis-runner-2.40.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:15:49.834061 analysis-runner-2.40.8/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-04-18 08:15:47.000000 analysis-runner-2.40.8/test/test_analysis_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:40:32.625113 analysis-runner-2.40.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-23 06:40:29.000000 analysis-runner-2.40.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-06-23 06:40:32.625113 analysis-runner-2.40.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-06-23 06:40:29.000000 analysis-runner-2.40.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:40:32.625113 analysis-runner-2.40.9/analysis_runner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 06:40:29.000000 analysis-runner-2.40.9/analysis_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-23 06:40:29.000000 analysis-runner-2.40.9/analysis_runner/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2125 2023-06-23 06:40:29.000000 analysis-runner-2.40.9/analysis_runner/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-06-23 06:40:29.000000 analysis-runner-2.40.9/analysis_runner/cli_analysisrunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-06-23 06:40:29.000000 analysis-runner-2.40.9/analysis_runner/cli_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12498 2023-06-23 06:40:29.000000 analysis-runner-2.40.9/analysis_runner/cli_cromwell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-23 06:40:29.000000 analysis-runner-2.40.9/analysis_runner/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24334 2023-06-23 06:40:29.000000 analysis-runner-2.40.9/analysis_runner/cromwell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-06-23 06:40:29.000000 analysis-runner-2.40.9/analysis_runner/cromwell_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11735 2023-06-23 06:40:29.000000 analysis-runner-2.40.9/analysis_runner/dataproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-06-23 06:40:29.000000 analysis-runner-2.40.9/analysis_runner/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-06-23 06:40:29.000000 analysis-runner-2.40.9/analysis_runner/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:40:32.625113 analysis-runner-2.40.9/analysis_runner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-06-23 06:40:32.000000 analysis-runner-2.40.9/analysis_runner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-23 06:40:32.000000 analysis-runner-2.40.9/analysis_runner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 06:40:32.000000 analysis-runner-2.40.9/analysis_runner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-23 06:40:32.000000 analysis-runner-2.40.9/analysis_runner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 06:40:32.000000 analysis-runner-2.40.9/analysis_runner.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-23 06:40:32.000000 analysis-runner-2.40.9/analysis_runner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-23 06:40:32.000000 analysis-runner-2.40.9/analysis_runner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-23 06:40:29.000000 analysis-runner-2.40.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 06:40:32.625113 analysis-runner-2.40.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-23 06:40:29.000000 analysis-runner-2.40.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:40:32.625113 analysis-runner-2.40.9/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-06-23 06:40:29.000000 analysis-runner-2.40.9/test/test_analysis_runner.py
```

### Comparing `analysis-runner-2.40.8/LICENSE` & `analysis-runner-2.40.9/LICENSE`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.40.8/PKG-INFO` & `analysis-runner-2.40.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: analysis-runner
-Version: 2.40.8
+Version: 2.40.9
 Summary: Analysis runner to help make analysis results reproducible
 Home-page: https://github.com/populationgenomics/analysis-runner
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `analysis-runner-2.40.8/README.md` & `analysis-runner-2.40.9/README.md`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.40.8/analysis_runner/cli.py` & `analysis-runner-2.40.9/analysis_runner/cli.py`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.40.8/analysis_runner/cli_analysisrunner.py` & `analysis-runner-2.40.9/analysis_runner/cli_analysisrunner.py`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.40.8/analysis_runner/cli_config.py` & `analysis-runner-2.40.9/analysis_runner/cli_config.py`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.40.8/analysis_runner/cli_cromwell.py` & `analysis-runner-2.40.9/analysis_runner/cli_cromwell.py`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.40.8/analysis_runner/constants.py` & `analysis-runner-2.40.9/analysis_runner/constants.py`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.40.8/analysis_runner/cromwell.py` & `analysis-runner-2.40.9/analysis_runner/cromwell.py`

 * *Files 5% similar despite different names*

```diff
@@ -316,20 +316,20 @@
     import subprocess
     import requests
     import time
     import math
     import json
     from datetime import datetime
     from cloudpathlib.anypath import to_anypath
-    from analysis_runner.cli_cromwell import _check_cromwell_status
     from analysis_runner.util import logger
     from analysis_runner.constants import (
         CROMWELL_AUDIENCE,
         GCLOUD_ACTIVATE_AUTH,
     )
+    from analysis_runner.cromwell_model import WorkflowMetadataModel
 
     # pylint: enable=redefined-outer-name,reimported,import-outside-toplevel
 
     class CromwellError(Exception):
         """Cromwell status error"""
 
     # Also re-defining this function that uses subprocess, for the same reason.
@@ -337,16 +337,15 @@
         """Get oath token for cromwell, specific to audience"""
         token_command = [
             'gcloud',
             'auth',
             'print-identity-token',
             f'--audiences={CROMWELL_AUDIENCE}',
         ]
-        token = subprocess.check_output(token_command).decode().strip()
-        return token
+        return subprocess.check_output(token_command).decode().strip()
 
     def _get_wait_interval(
         start, max_poll_interval, exponential_decrease_seconds
     ) -> int:
         """
         Get wait time between 5s and {max_poll_interval},
         curved between 0s and {exponential_decrease_seconds}.
@@ -360,29 +359,30 @@
         workflow_id = f.read().strip()
     logger.info(f'Received workflow ID: {workflow_id}')
 
     failed_statuses = {'failed', 'aborted'}
     terminal_statuses = {'succeeded'} | failed_statuses
     status_reported = False
     subprocess.check_output(GCLOUD_ACTIVATE_AUTH, shell=True)
-    url = f'https://cromwell.populationgenomics.org.au/api/workflows/v1/{workflow_id}/status'
+    cromwell_workflow_root = f'{CROMWELL_URL}/api/workflows/v1/{workflow_id}'
+    metadata_url = f'{cromwell_workflow_root}/metadata'
+    outputs_url = f'{cromwell_workflow_root}/outputs'
+    status_url = f'{cromwell_workflow_root}/status'
     _remaining_exceptions = max_sequential_exception_count
     start = datetime.now()
 
     while True:
         if _remaining_exceptions <= 0:
             raise CromwellError('Unreachable')
         wait_time = _get_wait_interval(
             start, max_poll_interval, exponential_decrease_seconds
         )
         try:
-            token = _get_cromwell_oauth_token()
-            r = requests.get(
-                url, headers={'Authorization': f'Bearer {token}'}, timeout=60
-            )
+            auth_header = {'Authorization': f'Bearer {_get_cromwell_oauth_token()}'}
+            r = requests.get(status_url, headers=auth_header, timeout=60)
             if not r.ok:
                 _remaining_exceptions -= 1
                 logger.warning(
                     f'Received "not okay" (status={r.status_code}) from cromwell '
                     f'(waiting={wait_time}): {r.text}'
                 )
                 time.sleep(wait_time)
@@ -391,29 +391,26 @@
 
             # if workflow has concluded print logging to hail batch log
             if status.lower() in terminal_statuses and not status_reported:
                 logger.info('Cromwell workflow has concluded - fetching log')
                 # don't report multiple times if we fail fetching output
                 # also don't fail the whole run if we can't fetch metadata
                 status_reported = True
-                _check_cromwell_status(workflow_id, json_output=None)
+                response = requests.get(metadata_url, headers=auth_header, timeout=60)
+                if response.ok:
+                    meta_json = response.json()
+                    print(WorkflowMetadataModel.parse(meta_json).display())
+                else:
+                    print('Failed to collect run Metadata')
 
             if status.lower() == 'succeeded':
                 logger.info(f'Cromwell workflow moved to succeeded state')
                 _remaining_exceptions = max_sequential_exception_count
                 # process outputs here
-                outputs_url = (
-                    f'https://cromwell.populationgenomics.org.au/api/workflows'
-                    f'/v1/{workflow_id}/outputs'
-                )
-                r_outputs = requests.get(
-                    outputs_url,
-                    headers={'Authorization': f'Bearer {token}'},
-                    timeout=60,
-                )
+                r_outputs = requests.get(outputs_url, headers=auth_header, timeout=60)
                 if not r_outputs.ok:
                     logger.warning(
                         'Received error when fetching cromwell outputs, '
                         f'will retry in {wait_time} seconds'
                     )
                     time.sleep(wait_time)
                     continue
@@ -464,14 +461,21 @@
         - a single value, or
         - a list of values
 
     If the starts with "gs://", we'll copy it as a resource file,
     otherwise write the value into a file which will be a batch resource.
 
     :param driver_image: If specified, must contain python3 (w/ requests), gcloud, jq
+    :param b: Batch object
+    :param job_prefix: Prefix for the job name
+    :param workflow_id_file: File containing the workflow ID
+    :param outputs_to_collect: Dict of output name -> CromwellOutputType
+    :param max_poll_interval: Maximum time to wait between polls
+    :param exponential_decrease_seconds: Exponential decrease in wait time
+    :param max_sequential_exception_count: Maximum number of exceptions before giving up
     """
 
     _driver_image = driver_image or os.getenv('DRIVER_IMAGE')
 
     watch_job = b.new_job(job_prefix + '_watch')
     watch_job.cpu(0.25)
```

### Comparing `analysis-runner-2.40.8/analysis_runner/cromwell_model.py` & `analysis-runner-2.40.9/analysis_runner/cromwell_model.py`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.40.8/analysis_runner/dataproc.py` & `analysis-runner-2.40.9/analysis_runner/dataproc.py`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.40.8/analysis_runner/git.py` & `analysis-runner-2.40.9/analysis_runner/git.py`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.40.8/analysis_runner/util.py` & `analysis-runner-2.40.9/analysis_runner/util.py`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.40.8/analysis_runner.egg-info/PKG-INFO` & `analysis-runner-2.40.9/analysis_runner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: analysis-runner
-Version: 2.40.8
+Version: 2.40.9
 Summary: Analysis runner to help make analysis results reproducible
 Home-page: https://github.com/populationgenomics/analysis-runner
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `analysis-runner-2.40.8/analysis_runner.egg-info/SOURCES.txt` & `analysis-runner-2.40.9/analysis_runner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `analysis-runner-2.40.8/setup.py` & `analysis-runner-2.40.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     with open(filename, encoding='utf-8') as f:
         return f.read()
 
 
 setuptools.setup(
     name=PKG,
     # This tag is automatically updated by bump2version
-    version='2.40.8',
+    version='2.40.9',
     description='Analysis runner to help make analysis results reproducible',
     long_description=read_file('README.md'),
     long_description_content_type='text/markdown',
     url=f'https://github.com/populationgenomics/{PKG}',
     license='MIT',
     packages=['analysis_runner'],
     include_package_data=True,
```

### Comparing `analysis-runner-2.40.8/test/test_analysis_runner.py` & `analysis-runner-2.40.9/test/test_analysis_runner.py`

 * *Files identical despite different names*


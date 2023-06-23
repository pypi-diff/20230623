# Comparing `tmp/ws_cleanup_tool-23.6.1.5-py3-none-any.whl.zip` & `tmp/ws_cleanup_tool-23.6.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 14662 bytes, number of entries: 9
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-16 17:53 mend_sca_cleanup_tool/__init__.py
--rw-r--r--  2.0 unx      102 b- defN 23-Jun-16 17:53 mend_sca_cleanup_tool/_version.py
--rw-r--r--  2.0 unx    21762 b- defN 23-Jun-16 17:53 mend_sca_cleanup_tool/sca_cleanup_tool.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jun-16 17:53 ws_cleanup_tool-23.6.1.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     9170 b- defN 23-Jun-16 17:53 ws_cleanup_tool-23.6.1.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-16 17:53 ws_cleanup_tool-23.6.1.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       81 b- defN 23-Jun-16 17:53 ws_cleanup_tool-23.6.1.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       22 b- defN 23-Jun-16 17:53 ws_cleanup_tool-23.6.1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      823 b- defN 23-Jun-16 17:53 ws_cleanup_tool-23.6.1.5.dist-info/RECORD
-9 files, 43409 bytes uncompressed, 13212 bytes compressed:  69.6%
+Zip file size: 14743 bytes, number of entries: 9
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-23 18:01 mend_sca_cleanup_tool/__init__.py
+-rw-r--r--  2.0 unx      100 b- defN 23-Jun-23 18:01 mend_sca_cleanup_tool/_version.py
+-rw-r--r--  2.0 unx    22109 b- defN 23-Jun-23 18:01 mend_sca_cleanup_tool/sca_cleanup_tool.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jun-23 18:01 ws_cleanup_tool-23.6.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     9281 b- defN 23-Jun-23 18:01 ws_cleanup_tool-23.6.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-23 18:01 ws_cleanup_tool-23.6.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       81 b- defN 23-Jun-23 18:01 ws_cleanup_tool-23.6.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-23 18:01 ws_cleanup_tool-23.6.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      811 b- defN 23-Jun-23 18:01 ws_cleanup_tool-23.6.2.dist-info/RECORD
+9 files, 43853 bytes uncompressed, 13317 bytes compressed:  69.6%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: mend_sca_cleanup_tool/_version.py
 Comment: 
 
 Filename: mend_sca_cleanup_tool/sca_cleanup_tool.py
 Comment: 
 
-Filename: ws_cleanup_tool-23.6.1.5.dist-info/LICENSE
+Filename: ws_cleanup_tool-23.6.2.dist-info/LICENSE
 Comment: 
 
-Filename: ws_cleanup_tool-23.6.1.5.dist-info/METADATA
+Filename: ws_cleanup_tool-23.6.2.dist-info/METADATA
 Comment: 
 
-Filename: ws_cleanup_tool-23.6.1.5.dist-info/WHEEL
+Filename: ws_cleanup_tool-23.6.2.dist-info/WHEEL
 Comment: 
 
-Filename: ws_cleanup_tool-23.6.1.5.dist-info/entry_points.txt
+Filename: ws_cleanup_tool-23.6.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: ws_cleanup_tool-23.6.1.5.dist-info/top_level.txt
+Filename: ws_cleanup_tool-23.6.2.dist-info/top_level.txt
 Comment: 
 
-Filename: ws_cleanup_tool-23.6.1.5.dist-info/RECORD
+Filename: ws_cleanup_tool-23.6.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mend_sca_cleanup_tool/_version.py

```diff
@@ -1,3 +1,3 @@
-__version__ = "23.6.1.5"
+__version__ = "23.6.2"
 __tool_name__ = "sca_cleanup_tool"
 __description__ = "Mend SCA Cleanup Tool"
```

## mend_sca_cleanup_tool/sca_cleanup_tool.py

```diff
@@ -66,15 +66,19 @@
             print("No projects to clean up were found")
             exit()
         else:
             print(f"Found {total_projects_to_delete} project(s) to delete, generating reports and removing project(s)...")
         for product_token in product_project_dict:
             for project in product_project_dict[product_token]:
                 if not CONFIG.skip_report_generation:
-                    generate_reports(project)
+                    try:
+                        generate_reports(project)
+                    except:
+                        print(f"There was an issue with the report generation, skipping deletion for project: {project['name']}")
+                        continue
                 else:
                     print("skipReportGeneration flag found, skipping report generation")
                 if not CONFIG.skip_project_deletion:
                     delete_scan(product_token, project)
                 else:
                     print("skipProjectDeletion flag found, skipping project deletion")
     else:
@@ -185,15 +189,17 @@
                 data = get_alerts_report(reports_to_generate[report], project_token, "ignored")
             elif report.lower() == REJECTED_BY_POLICY:
                 data = get_alerts_by_type(reports_to_generate[report], project_token, "REJECTED_BY_POLICY_RESOURCE")
                 reportFormat = "json"
             else:
                 data = get_excel_report(reports_to_generate[report], project_token)
 
-            check_response_error(data)
+            generation_failed = check_response_error(data)
+            if generation_failed:
+                raise Exception(f"Failed to generate report: {report}") 
             report = open(output_dir + report + '.' + reportFormat, "wb")
             report.write(data)
             report.close()
     else:
         print("No reports to generate")
```

## Comparing `ws_cleanup_tool-23.6.1.5.dist-info/LICENSE` & `ws_cleanup_tool-23.6.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ws_cleanup_tool-23.6.1.5.dist-info/METADATA` & `ws_cleanup_tool-23.6.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ws-cleanup-tool
-Version: 23.6.1.5
+Version: 23.6.2
 Summary: Mend SCA Cleanup Tool
 Home-page: https://github.com/whitesource-ps/mend-sca-cleanup-tool
 Author: Mend Professional Services
 Author-email: ps@whitesourcesoftware.com
 License: LICENSE.txt
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
@@ -21,14 +21,15 @@
 [![Logo](https://resources.mend.io/mend-sig/logo/mend-dark-logo-horizontal.png)](https://www.mend.io/)
 [![License](https://img.shields.io/badge/License-Apache%202.0-yellowgreen.svg)](https://opensource.org/licenses/Apache-2.0)
 [![Mend projects cleanup](https://github.com/whitesource-ps/ws-cleanup-tool/actions/workflows/ci.yml/badge.svg)](https://github.com/whitesource-ps/ws-cleanup-tool/actions/workflows/ci.yml)
 [![Python 3.6](https://upload.wikimedia.org/wikipedia/commons/thumb/8/8c/Blue_Python_3.6%2B_Shield_Badge.svg/86px-Blue_Python_3.6%2B_Shield_Badge.svg.png)](https://www.python.org/downloads/release/python-360/)
 [![PyPI](https://img.shields.io/pypi/v/ws-cleanup-tool?style=plastic)](https://pypi.org/project/ws-cleanup-tool/)
 
 # Mend Projects Cleanup CLI Tool
+* Current version v23.6.2
 * The self-hosted CLI tool features cleaning up projects and generating reports before deletion in 2 modes:
   * By stating _OperationMode=FilterProjectsByUpdateTime_ and how many days to keep (-r/ DaysToKeep=)
   * By stating _OperationMode=FilterProjectsByLastCreatedCopies_ and how many copies to keep (-r/ DaysToKeep=)
 * The reports are saved in the designated location as follows: _[Output_DIR]/[PRODUCT NAME]/[PROJECT NAME]/[REPORT NAME]_  
   * The default location is the _[WORKING DIRECTORY]/Mend/Reports/[PRODUCT NAME]/[PROJECT NAME]/[REPORT NAME]_
 * To review the outcome before actual deletion use _-y true_ / _DryRun=True_ flag. It will _NOT_ delete any project nor create reports 
 * By default, the tool generates all possible project-level reports. By specifying ((_-t_ / _Reports=_/) it is possible to select specific reports
@@ -48,15 +49,16 @@
 ## Permissions
 * The user used to execute the tool has to have "Organization Administrator" or "Product Administrator" on all the maintained products and "Organization Auditor" permissions. 
 * It is recommended to use a service user.
 
 ## Installation and Execution from PyPi (recommended):
 1. Install by executing: `pip install mend-sca-cleanup-tool`
 2. Configure the appropriate parameters either by using the command line or in `params.config`.
-3. Execute the tool (`mend_sca_cleanup_tool ...`). 
+3. Execute the tool (`mend_sca_cleanup_tool ...`).
+4. In order to update the tool please run `pip install mend-sca-cleanup-tool --upgrade`
 
 ## Installation and Execution from GitHub:
 1. Download and unzip **mend-sca-cleanup-tool.zip** from the most recent tagged release.
 2. Install requirements: `pip install -r requirements.txt`
 3. Configure the appropriate parameters either by using the command line or `params.config`.
 4. Execute: `python sca_cleanup_tool.py <CONFIG_FILE>`
```

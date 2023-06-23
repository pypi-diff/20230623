# Comparing `tmp/saagieapi-2.5.0.tar.gz` & `tmp/saagieapi-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saagieapi-2.5.0.tar", max compression
+gzip compressed data, was "saagieapi-2.6.0.tar", max compression
```

## Comparing `saagieapi-2.5.0.tar` & `saagieapi-2.6.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0    11357 2023-06-02 14:47:33.139649 saagieapi-2.5.0/LICENSE
--rw-r--r--   0        0        0     4555 2023-06-02 14:47:33.139649 saagieapi-2.5.0/README.md
--rw-r--r--   0        0        0     1562 2023-06-02 14:48:02.680101 saagieapi-2.5.0/pyproject.toml
--rw-r--r--   0        0        0      502 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/__init__.py
--rw-r--r--   0        0        0       43 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/apps/__init__.py
--rw-r--r--   0        0        0    33369 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/apps/apps.py
--rw-r--r--   0        0        0     7591 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/apps/gql_queries.py
--rw-r--r--   0        0        0       83 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/docker_credentials/__init__.py
--rw-r--r--   0        0        0     8465 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/docker_credentials/docker_credentials.py
--rw-r--r--   0        0        0     1657 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/docker_credentials/gql_queries.py
--rw-r--r--   0        0        0       53 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/env_vars/__init__.py
--rw-r--r--   0        0        0    27280 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/env_vars/env_vars.py
--rw-r--r--   0        0        0     2671 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/env_vars/gql_queries.py
--rw-r--r--   0        0        0     2414 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/gql_queries.py
--rw-r--r--   0        0        0       49 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/groups/__init__.py
--rw-r--r--   0        0        0    14568 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/groups/groups.py
--rw-r--r--   0        0        0       43 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/jobs/__init__.py
--rw-r--r--   0        0        0     9510 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/jobs/gql_queries.py
--rw-r--r--   0        0        0    36314 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/jobs/jobs.py
--rw-r--r--   0        0        0      141 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/pipelines/__init__.py
--rw-r--r--   0        0        0     7785 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/pipelines/gql_queries.py
--rw-r--r--   0        0        0     2384 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/pipelines/graph_pipeline.py
--rw-r--r--   0        0        0    29262 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/pipelines/pipelines.py
--rw-r--r--   0        0        0       55 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/profiles/__init__.py
--rw-r--r--   0        0        0     4954 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/profiles/profiles.py
--rw-r--r--   0        0        0       55 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/projects/__init__.py
--rw-r--r--   0        0        0     2962 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/projects/gql_queries.py
--rw-r--r--   0        0        0    24404 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/projects/projects.py
--rw-r--r--   0        0        0       67 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/repositories/__init__.py
--rw-r--r--   0        0        0     8443 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/repositories/gql_queries.py
--rw-r--r--   0        0        0    10534 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/repositories/repositories.py
--rw-r--r--   0        0        0    15082 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/saagie_api.py
--rw-r--r--   0        0        0       55 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/storages/__init__.py
--rw-r--r--   0        0        0     1384 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/storages/gql_queries.py
--rw-r--r--   0        0        0     6561 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/storages/storages.py
--rw-r--r--   0        0        0       46 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/users/__init__.py
--rw-r--r--   0        0        0    10891 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/users/users.py
--rw-r--r--   0        0        0        0 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/utils/__init__.py
--rw-r--r--   0        0        0     1725 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/utils/bearer_auth.py
--rw-r--r--   0        0        0     3969 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/utils/folder_functions.py
--rw-r--r--   0        0        0     3113 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/utils/gql_client.py
--rw-r--r--   0        0        0     2336 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/utils/request_client.py
--rw-r--r--   0        0        0       54 2023-06-02 14:47:33.147650 saagieapi-2.5.0/saagieapi/utils/rich_console.py
--rw-r--r--   0        0        0     5504 1970-01-01 00:00:00.000000 saagieapi-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-23 14:20:49.337028 saagieapi-2.6.0/LICENSE
+-rw-r--r--   0        0        0     4555 2023-06-23 14:20:49.337028 saagieapi-2.6.0/README.md
+-rw-r--r--   0        0        0     1562 2023-06-23 14:21:19.237017 saagieapi-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0      583 2023-06-23 14:20:49.345028 saagieapi-2.6.0/saagieapi/__init__.py
+-rw-r--r--   0        0        0       43 2023-06-23 14:20:49.345028 saagieapi-2.6.0/saagieapi/apps/__init__.py
+-rw-r--r--   0        0        0    33369 2023-06-23 14:20:49.345028 saagieapi-2.6.0/saagieapi/apps/apps.py
+-rw-r--r--   0        0        0     7591 2023-06-23 14:20:49.345028 saagieapi-2.6.0/saagieapi/apps/gql_queries.py
+-rw-r--r--   0        0        0       83 2023-06-23 14:20:49.345028 saagieapi-2.6.0/saagieapi/docker_credentials/__init__.py
+-rw-r--r--   0        0        0     8465 2023-06-23 14:20:49.345028 saagieapi-2.6.0/saagieapi/docker_credentials/docker_credentials.py
+-rw-r--r--   0        0        0     1657 2023-06-23 14:20:49.345028 saagieapi-2.6.0/saagieapi/docker_credentials/gql_queries.py
+-rw-r--r--   0        0        0       53 2023-06-23 14:20:49.345028 saagieapi-2.6.0/saagieapi/env_vars/__init__.py
+-rw-r--r--   0        0        0    27280 2023-06-23 14:20:49.345028 saagieapi-2.6.0/saagieapi/env_vars/env_vars.py
+-rw-r--r--   0        0        0     2671 2023-06-23 14:20:49.345028 saagieapi-2.6.0/saagieapi/env_vars/gql_queries.py
+-rw-r--r--   0        0        0     4677 2023-06-23 14:20:49.345028 saagieapi-2.6.0/saagieapi/gql_queries.py
+-rw-r--r--   0        0        0       49 2023-06-23 14:20:49.345028 saagieapi-2.6.0/saagieapi/groups/__init__.py
+-rw-r--r--   0        0        0    14568 2023-06-23 14:20:49.345028 saagieapi-2.6.0/saagieapi/groups/groups.py
+-rw-r--r--   0        0        0       43 2023-06-23 14:20:49.345028 saagieapi-2.6.0/saagieapi/jobs/__init__.py
+-rw-r--r--   0        0        0     9510 2023-06-23 14:20:49.345028 saagieapi-2.6.0/saagieapi/jobs/gql_queries.py
+-rw-r--r--   0        0        0    36314 2023-06-23 14:20:49.345028 saagieapi-2.6.0/saagieapi/jobs/jobs.py
+-rw-r--r--   0        0        0      222 2023-06-23 14:20:49.345028 saagieapi-2.6.0/saagieapi/pipelines/__init__.py
+-rw-r--r--   0        0        0     8853 2023-06-23 14:20:49.345028 saagieapi-2.6.0/saagieapi/pipelines/gql_queries.py
+-rw-r--r--   0        0        0     3572 2023-06-23 14:20:49.345028 saagieapi-2.6.0/saagieapi/pipelines/graph_pipeline.py
+-rw-r--r--   0        0        0    30113 2023-06-23 14:20:49.345028 saagieapi-2.6.0/saagieapi/pipelines/pipelines.py
+-rw-r--r--   0        0        0       55 2023-06-23 14:20:49.345028 saagieapi-2.6.0/saagieapi/profiles/__init__.py
+-rw-r--r--   0        0        0     4954 2023-06-23 14:20:49.345028 saagieapi-2.6.0/saagieapi/profiles/profiles.py
+-rw-r--r--   0        0        0       55 2023-06-23 14:20:49.345028 saagieapi-2.6.0/saagieapi/projects/__init__.py
+-rw-r--r--   0        0        0     2962 2023-06-23 14:20:49.345028 saagieapi-2.6.0/saagieapi/projects/gql_queries.py
+-rw-r--r--   0        0        0    24404 2023-06-23 14:20:49.345028 saagieapi-2.6.0/saagieapi/projects/projects.py
+-rw-r--r--   0        0        0       67 2023-06-23 14:20:49.345028 saagieapi-2.6.0/saagieapi/repositories/__init__.py
+-rw-r--r--   0        0        0     8443 2023-06-23 14:20:49.345028 saagieapi-2.6.0/saagieapi/repositories/gql_queries.py
+-rw-r--r--   0        0        0    10534 2023-06-23 14:20:49.345028 saagieapi-2.6.0/saagieapi/repositories/repositories.py
+-rw-r--r--   0        0        0    19545 2023-06-23 14:20:49.345028 saagieapi-2.6.0/saagieapi/saagie_api.py
+-rw-r--r--   0        0        0       55 2023-06-23 14:20:49.345028 saagieapi-2.6.0/saagieapi/storages/__init__.py
+-rw-r--r--   0        0        0     1384 2023-06-23 14:20:49.345028 saagieapi-2.6.0/saagieapi/storages/gql_queries.py
+-rw-r--r--   0        0        0     6561 2023-06-23 14:20:49.345028 saagieapi-2.6.0/saagieapi/storages/storages.py
+-rw-r--r--   0        0        0       46 2023-06-23 14:20:49.345028 saagieapi-2.6.0/saagieapi/users/__init__.py
+-rw-r--r--   0        0        0    10981 2023-06-23 14:20:49.345028 saagieapi-2.6.0/saagieapi/users/users.py
+-rw-r--r--   0        0        0        0 2023-06-23 14:20:49.345028 saagieapi-2.6.0/saagieapi/utils/__init__.py
+-rw-r--r--   0        0        0     1725 2023-06-23 14:20:49.345028 saagieapi-2.6.0/saagieapi/utils/bearer_auth.py
+-rw-r--r--   0        0        0     3969 2023-06-23 14:20:49.345028 saagieapi-2.6.0/saagieapi/utils/folder_functions.py
+-rw-r--r--   0        0        0     3113 2023-06-23 14:20:49.349028 saagieapi-2.6.0/saagieapi/utils/gql_client.py
+-rw-r--r--   0        0        0     2336 2023-06-23 14:20:49.349028 saagieapi-2.6.0/saagieapi/utils/request_client.py
+-rw-r--r--   0        0        0       54 2023-06-23 14:20:49.349028 saagieapi-2.6.0/saagieapi/utils/rich_console.py
+-rw-r--r--   0        0        0     5504 1970-01-01 00:00:00.000000 saagieapi-2.6.0/PKG-INFO
```

### Comparing `saagieapi-2.5.0/LICENSE` & `saagieapi-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `saagieapi-2.5.0/README.md` & `saagieapi-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `saagieapi-2.5.0/pyproject.toml` & `saagieapi-2.6.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "saagieapi"
-version = "2.5.0"
+version = "2.6.0"
 description = "Python API to interact with Saagie"
 authors = ["Saagie"]
 license = "GLWTPL"
 readme = "README.md"
 repository = "https://github.com/saagie/api-saagie"
 
 [tool.poetry.dependencies]
```

### Comparing `saagieapi-2.5.0/saagieapi/apps/apps.py` & `saagieapi-2.6.0/saagieapi/apps/apps.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.5.0/saagieapi/apps/gql_queries.py` & `saagieapi-2.6.0/saagieapi/apps/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.5.0/saagieapi/docker_credentials/docker_credentials.py` & `saagieapi-2.6.0/saagieapi/docker_credentials/docker_credentials.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.5.0/saagieapi/docker_credentials/gql_queries.py` & `saagieapi-2.6.0/saagieapi/docker_credentials/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.5.0/saagieapi/env_vars/env_vars.py` & `saagieapi-2.6.0/saagieapi/env_vars/env_vars.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.5.0/saagieapi/env_vars/gql_queries.py` & `saagieapi-2.6.0/saagieapi/env_vars/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.5.0/saagieapi/groups/groups.py` & `saagieapi-2.6.0/saagieapi/groups/groups.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.5.0/saagieapi/jobs/gql_queries.py` & `saagieapi-2.6.0/saagieapi/jobs/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.5.0/saagieapi/jobs/jobs.py` & `saagieapi-2.6.0/saagieapi/jobs/jobs.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.5.0/saagieapi/pipelines/gql_queries.py` & `saagieapi-2.6.0/saagieapi/pipelines/gql_queries.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,28 @@
                 endTime
                 runWithExecutionVariables
                 initialExecutionVariables{
                     key
                     value
                     isPassword
                 }
+                jobsInstance{
+                    id
+                    jobId
+                    number
+                    startTime
+                    endTime
+                }
+                conditionsInstance{
+                    id
+                    conditionNodeId
+                    isSuccess
+                    startTime
+                    endTime
+                }
             }
             versions(limit: $versionsLimit, onlyCurrent: $versionsOnlyCurrent) {
                 number
                 releaseNote
                 graph{
                     jobNodes{
                         id
@@ -109,14 +123,28 @@
             endTime
             runWithExecutionVariables
             initialExecutionVariables{
                 key
                 value
                 isPassword
             }
+            jobsInstance{
+                id
+                jobId
+                number
+                startTime
+                endTime
+            }
+            conditionsInstance{
+                id
+                conditionNodeId
+                isSuccess
+                startTime
+                endTime
+            }
         }
         versions(limit: $versionsLimit, onlyCurrent: $versionsOnlyCurrent) {
             number
             releaseNote
             graph{
                 jobNodes{
                     id
@@ -134,14 +162,17 @@
                     id
                     position{
                         x
                         y
                     }
                     nextNodesSuccess
                     nextNodesFailure
+                    condition {
+                        toString
+                    }
                 }
             }
             creationDate
             creator
             isCurrent
             isMajor
         }
@@ -224,14 +255,28 @@
         endTime
         runWithExecutionVariables
         initialExecutionVariables{
             key
             value
             isPassword
         }
+        jobsInstance{
+            id
+            jobId
+            number
+            startTime
+            endTime
+        }
+        conditionsInstance{
+            id
+            conditionNodeId
+            isSuccess
+            startTime
+            endTime
+        }
     }
 }
 """
 
 GQL_CREATE_GRAPH_PIPELINE = """
 mutation createGraphPipelineMutation($name: String!, 
 									 $description: String,
```

### Comparing `saagieapi-2.5.0/saagieapi/pipelines/pipelines.py` & `saagieapi-2.6.0/saagieapi/pipelines/pipelines.py`

 * *Files 2% similar despite different names*

```diff
@@ -711,14 +711,28 @@
                     conditions_found = []
                     for condition_node in version["graph"]["conditionNodes"]:
                         condition_dict = {
                             "id": condition_node["id"],
                             "nextNodesSuccess": condition_node["nextNodesSuccess"],
                             "nextNodesFailure": condition_node["nextNodesFailure"],
                         }
+                        if "ConditionStatus" in condition_node["condition"]["toString"]:
+                            # example : ConditionStatus(value=AtLeastOneSuccess)
+                            condition_dict["condition"] = {
+                                "status": {"value": condition_node["condition"]["toString"].split("=")[1].split(")")[0]}
+                            }
+
+                        if "ConditionExpression" in condition_node["condition"]["toString"]:
+                            # example : ConditionExpression(expression=\"1 + 1 == 2\")
+                            condition_dict["condition"] = {
+                                "custom": {
+                                    "expression": condition_node["condition"]["toString"].split('="')[1].split('")')[0]
+                                }
+                            }
+
                         conditions_found.append(condition_dict)
 
                     if len(jobs_not_found) > 0:
                         result = False
                         not_found = ""
                         for job in jobs_not_found:
                             not_found += job + ", "
```

### Comparing `saagieapi-2.5.0/saagieapi/profiles/profiles.py` & `saagieapi-2.6.0/saagieapi/profiles/profiles.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.5.0/saagieapi/projects/gql_queries.py` & `saagieapi-2.6.0/saagieapi/projects/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.5.0/saagieapi/projects/projects.py` & `saagieapi-2.6.0/saagieapi/projects/projects.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.5.0/saagieapi/repositories/gql_queries.py` & `saagieapi-2.6.0/saagieapi/repositories/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.5.0/saagieapi/repositories/repositories.py` & `saagieapi-2.6.0/saagieapi/repositories/repositories.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.5.0/saagieapi/saagie_api.py` & `saagieapi-2.6.0/saagieapi/saagie_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,15 +5,24 @@
 import pytz
 from croniter import croniter
 from gql import gql
 
 from .apps import Apps
 from .docker_credentials import DockerCredentials
 from .env_vars import EnvVars
-from .gql_queries import GQL_GET_CLUSTER_INFO, GQL_GET_PLATFORM_INFO, GQL_GET_REPOSITORIES_INFO, GQL_GET_RUNTIMES
+from .gql_queries import (
+    GQL_CHECK_CUSTOM_EXPRESSION,
+    GQL_COUNT_CONDITION_LOGS,
+    GQL_GET_CLUSTER_INFO,
+    GQL_GET_CONDITION_LOGS_BY_CONDITION,
+    GQL_GET_CONDITION_LOGS_BY_INSTANCE,
+    GQL_GET_PLATFORM_INFO,
+    GQL_GET_REPOSITORIES_INFO,
+    GQL_GET_RUNTIMES,
+)
 from .groups import Groups
 from .jobs import Jobs
 from .pipelines import Pipelines
 from .profiles import Profiles
 from .projects import Projects
 from .repositories import Repositories
 from .storages import Storages
@@ -427,7 +436,144 @@
         dict
             String of runtime label
 
         """
         runtimes = self.get_runtimes(technology_id)
 
         return [runtime["label"] for runtime in runtimes["technology"]["appContexts"] if runtime["id"] == runtime_id]
+
+    # ##########################################################
+    # ###                    Conditions                     ####
+    # ##########################################################
+
+    def check_condition_expression(self, expression: str, project_id: str, variables: Dict = None) -> Dict:
+        """Test the condition expression
+
+        Parameters
+        ----------
+        expression : str
+            Expression to test
+        project_id : str
+            UUID of the project
+        variables : Dict
+            List of logs files name to see (example : STDERR, STDOUT)
+
+        Returns
+        -------
+        Dict
+            Dict of result of the condition expression
+        """
+
+        params = {
+            "projectId": project_id,
+            "expression": expression,
+            "variables": variables if variables else {"key": "", "value": ""},
+        }
+        return self.client.execute(query=gql(GQL_CHECK_CUSTOM_EXPRESSION), variable_values=params)
+
+    def count_condition_logs(self, condition_instance_id: str, project_id: str, streams: List[str]) -> Dict:
+        """Get number of logs line for an instance of a condition on Environment Variable
+
+        Parameters
+        ----------
+        condition_instance_id : str
+            UUID of the condition instance
+        project_id : str
+            UUID of the project
+        streams : List[str]
+            List of logs files name to see (example : STDERR, STDOUT)
+
+        Returns
+        -------
+        Dic
+            Dict of number of logs lines
+        """
+
+        params = {"conditionInstanceId": condition_instance_id, "projectID": project_id, "streams": streams}
+
+        return self.client.execute(query=gql(GQL_COUNT_CONDITION_LOGS), variable_values=params)
+
+    def get_condition_instance_logs_by_condition(
+        self,
+        condition_id: str,
+        project_id: str,
+        pipeline_instance_id: str,
+        streams: List[str],
+        limit: int = None,
+        skip: int = None,
+    ) -> Dict:
+        """Get logs for a condition on Environment Variable of a pipeline instance
+
+        Parameters
+        ----------
+        condition_id : str
+            UUID of the condition
+        project_id : str
+            UUID of the project
+        pipeline_instance_id ! str
+            UUID of the pipeline instance
+        streams : List[str]
+            List of logs files name to see (example : STDERR, STDOUT)
+        limit : int
+            Number of logs lines to return from the beginning
+        skip : int
+            Number of logs lines to doesn't display from the beginning
+
+        Returns
+        -------
+        dict
+            Dict of logs lines
+        """
+        params = {
+            "conditionNodeID": condition_id,
+            "projectID": project_id,
+            "pipelineInstanceID": pipeline_instance_id,
+            "streams": streams,
+        }
+        if limit:
+            params["limit"] = limit
+
+        if skip:
+            params["skip"] = skip
+
+        return self.client.execute(query=gql(GQL_GET_CONDITION_LOGS_BY_CONDITION), variable_values=params)
+
+    def get_condition_instance_logs_by_instance(
+        self,
+        condition_instance_id: str,
+        project_id: str,
+        streams: List[str],
+        limit: int = None,
+        skip: int = None,
+    ) -> Dict:
+        """Get instance's logs of a condition on Environment Variable
+
+        Parameters
+        ----------
+        condition_instance_id : str
+            UUID of the condition instance
+        project_id : str
+            UUID of the project
+        streams : List[str]
+            List of logs files name to see (example : STDERR, STDOUT)
+        limit : int
+            Number of logs lines to return from the beginning
+        skip : int
+            Number of logs lines to doesn't display from the beginning
+
+        Returns
+        -------
+        dict
+            Dict of logs lines
+        """
+        params = {
+            "conditionInstanceId": condition_instance_id,
+            "projectId": project_id,
+            "streams": streams,
+        }
+        if limit:
+            params["limit"] = limit
+
+        if skip:
+            params["skip"] = skip
+
+        return self.client.execute(query=gql(GQL_GET_CONDITION_LOGS_BY_INSTANCE), variable_values=params)
```

### Comparing `saagieapi-2.5.0/saagieapi/storages/gql_queries.py` & `saagieapi-2.6.0/saagieapi/storages/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.5.0/saagieapi/storages/storages.py` & `saagieapi-2.6.0/saagieapi/storages/storages.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.5.0/saagieapi/users/users.py` & `saagieapi-2.6.0/saagieapi/users/users.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,15 @@
 
         Returns
         -------
         bool
             True if users are exported False otherwise
         """
         users = None
+        verify_ssl = verify_ssl if verify_ssl is not None else self.saagie_api.verify_ssl
         try:
             users = self.list(verify_ssl=verify_ssl)
         except Exception as exception:
             logging.warning("❌ Cannot get the user's information on the platform")
             logging.error("Something went wrong %s", exception)
         if users:
             output_folder = check_folder_path(output_folder)
```

### Comparing `saagieapi-2.5.0/saagieapi/utils/bearer_auth.py` & `saagieapi-2.6.0/saagieapi/utils/bearer_auth.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.5.0/saagieapi/utils/folder_functions.py` & `saagieapi-2.6.0/saagieapi/utils/folder_functions.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.5.0/saagieapi/utils/gql_client.py` & `saagieapi-2.6.0/saagieapi/utils/gql_client.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.5.0/saagieapi/utils/request_client.py` & `saagieapi-2.6.0/saagieapi/utils/request_client.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.5.0/PKG-INFO` & `saagieapi-2.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saagieapi
-Version: 2.5.0
+Version: 2.6.0
 Summary: Python API to interact with Saagie
 Home-page: https://github.com/saagie/api-saagie
 License: GLWTPL
 Author: Saagie
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```


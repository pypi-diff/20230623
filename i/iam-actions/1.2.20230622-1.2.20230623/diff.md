# Comparing `tmp/iam_actions-1.2.20230622.tar.gz` & `tmp/iam_actions-1.2.20230623.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230622.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230623.tar", max compression
```

## Comparing `iam_actions-1.2.20230622.tar` & `iam_actions-1.2.20230623.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-06-22 02:36:55.355579 iam_actions-1.2.20230622/LICENSE
--rw-r--r--   0        0        0     2302 2023-06-22 02:36:55.355579 iam_actions-1.2.20230622/README.md
--rw-r--r--   0        0        0      228 2023-06-22 02:36:55.355579 iam_actions-1.2.20230622/iam_actions/__init__.py
--rw-r--r--   0        0        0  4339454 2023-06-22 02:38:18.882778 iam_actions-1.2.20230622/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-06-22 02:36:55.355579 iam_actions-1.2.20230622/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-06-22 02:36:55.355579 iam_actions-1.2.20230622/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-06-22 02:36:55.355579 iam_actions-1.2.20230622/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-06-22 02:36:55.355579 iam_actions-1.2.20230622/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-06-22 02:36:55.355579 iam_actions-1.2.20230622/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-06-22 02:36:55.355579 iam_actions-1.2.20230622/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-06-22 02:36:55.355579 iam_actions-1.2.20230622/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-06-22 02:36:55.355579 iam_actions-1.2.20230622/iam_actions/generate/services.py
--rw-r--r--   0        0        0   557867 2023-06-22 02:38:18.882778 iam_actions-1.2.20230622/iam_actions/policies.json
--rw-r--r--   0        0        0   196684 2023-06-22 02:38:18.882778 iam_actions-1.2.20230622/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   541083 2023-06-22 02:38:18.882778 iam_actions-1.2.20230622/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-06-22 02:38:19.914865 iam_actions-1.2.20230622/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230622/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230622/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-23 02:53:23.692726 iam_actions-1.2.20230623/LICENSE
+-rw-r--r--   0        0        0     2302 2023-06-23 02:53:23.692726 iam_actions-1.2.20230623/README.md
+-rw-r--r--   0        0        0      228 2023-06-23 02:53:23.692726 iam_actions-1.2.20230623/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4341498 2023-06-23 02:54:44.404923 iam_actions-1.2.20230623/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-06-23 02:53:23.692726 iam_actions-1.2.20230623/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-06-23 02:53:23.692726 iam_actions-1.2.20230623/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-06-23 02:53:23.692726 iam_actions-1.2.20230623/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-06-23 02:53:23.692726 iam_actions-1.2.20230623/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-06-23 02:53:23.692726 iam_actions-1.2.20230623/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-06-23 02:53:23.692726 iam_actions-1.2.20230623/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-06-23 02:53:23.692726 iam_actions-1.2.20230623/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-06-23 02:53:23.692726 iam_actions-1.2.20230623/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   558388 2023-06-23 02:54:44.404923 iam_actions-1.2.20230623/iam_actions/policies.json
+-rw-r--r--   0        0        0   196684 2023-06-23 02:54:44.404923 iam_actions-1.2.20230623/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   541563 2023-06-23 02:54:44.404923 iam_actions-1.2.20230623/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-06-23 02:54:45.396926 iam_actions-1.2.20230623/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230623/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230623/PKG-INFO
```

### Comparing `iam_actions-1.2.20230622/LICENSE` & `iam_actions-1.2.20230623/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230622/README.md` & `iam_actions-1.2.20230623/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230622/iam_actions/actions.json` & `iam_actions-1.2.20230623/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996431751805076%*

 * *Differences: {"'appconfig'": "{'ListTagsForResource': {'resources': {insert: [(5, 'extension'), (6, "*

 * *                "'extensionassociation')]}}}",*

 * * "'backup'": "{'ListTags': {'resources': {insert: [(3, 'legalHold')]}}, 'StartBackupJob': "*

 * *             "{'condition_keys': []}, 'UpdateBackupPlan': {'condition_keys': []}, "*

 * *             "'UpdateFramework': {'condition_keys': []}}",*

 * * "'iam'": "{'GetMFADevice': OrderedDict([('access_level', 'Undocumented'), ('action', "*

 * *          "'GetMFADevice'), ('condition_keys', []), ( […]*

```diff
@@ -3963,15 +3963,17 @@
             "description": "Grants permission to view a list of resource tags for a specified resource",
             "orphan": false,
             "resources": [
                 "application",
                 "configurationprofile",
                 "deployment",
                 "deploymentstrategy",
-                "environment"
+                "environment",
+                "extension",
+                "extensionassociation"
             ]
         },
         "StartConfigurationSession": {
             "access_level": "Write",
             "action": "StartConfigurationSession",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}"
@@ -11377,14 +11379,15 @@
             "condition_keys": [],
             "description": "Grants permission to list tags for a resource",
             "orphan": false,
             "resources": [
                 "backupPlan",
                 "backupVault",
                 "framework",
+                "legalHold",
                 "recoveryPoint",
                 "reportPlan"
             ]
         },
         "PutBackupVaultAccessPolicy": {
             "access_level": "Permissions management",
             "action": "PutBackupVaultAccessPolicy",
@@ -11416,18 +11419,15 @@
             "resources": [
                 "backupVault"
             ]
         },
         "StartBackupJob": {
             "access_level": "Write",
             "action": "StartBackupJob",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys"
-            ],
+            "condition_keys": [],
             "description": "Grants permission to start a new backup job",
             "orphan": false,
             "resources": [
                 "backupVault"
             ]
         },
         "StartCopyJob": {
@@ -11502,31 +11502,25 @@
                 "recoveryPoint",
                 "reportPlan"
             ]
         },
         "UpdateBackupPlan": {
             "access_level": "Write",
             "action": "UpdateBackupPlan",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys"
-            ],
+            "condition_keys": [],
             "description": "Grants permission to update a backup plan",
             "orphan": false,
             "resources": [
                 "backupPlan"
             ]
         },
         "UpdateFramework": {
             "access_level": "Write",
             "action": "UpdateFramework",
-            "condition_keys": [
-                "aws:RequestTag/${TagKey}",
-                "aws:TagKeys"
-            ],
+            "condition_keys": [],
             "description": "Grants permission to update a framework",
             "orphan": false,
             "resources": [
                 "framework"
             ]
         },
         "UpdateGlobalSettings": {
@@ -72562,14 +72556,22 @@
             "access_level": "Undocumented",
             "action": "GetLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "GetMFADevice": {
+            "access_level": "Undocumented",
+            "action": "GetMFADevice",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetOpenIDConnectProvider": {
             "access_level": "Undocumented",
             "action": "GetOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
@@ -84517,14 +84519,22 @@
             "condition_keys": [],
             "description": "Grants permission to query documents and faqs",
             "orphan": false,
             "resources": [
                 "index"
             ]
         },
+        "Retrieve": {
+            "access_level": "Undocumented",
+            "action": "Retrieve",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "StartDataSourceSyncJob": {
             "access_level": "Write",
             "action": "StartDataSourceSyncJob",
             "condition_keys": [],
             "description": "Grants permission to start Data Source sync job",
             "orphan": false,
             "resources": [
@@ -142212,14 +142222,22 @@
             ],
             "description": "Grants permission to create a state machine",
             "orphan": false,
             "resources": [
                 "statemachine"
             ]
         },
+        "CreateStateMachineAlias": {
+            "access_level": "Undocumented",
+            "action": "CreateStateMachineAlias",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteActivity": {
             "access_level": "Write",
             "action": "DeleteActivity",
             "condition_keys": [],
             "description": "Grants permission to delete an activity",
             "orphan": false,
             "resources": [
@@ -142232,14 +142250,30 @@
             "condition_keys": [],
             "description": "Grants permission to delete a state machine",
             "orphan": false,
             "resources": [
                 "statemachine"
             ]
         },
+        "DeleteStateMachineAlias": {
+            "access_level": "Undocumented",
+            "action": "DeleteStateMachineAlias",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteStateMachineVersion": {
+            "access_level": "Undocumented",
+            "action": "DeleteStateMachineVersion",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DescribeActivity": {
             "access_level": "Read",
             "action": "DescribeActivity",
             "condition_keys": [],
             "description": "Grants permission to describe an activity",
             "orphan": false,
             "resources": [
@@ -142273,14 +142307,22 @@
             "condition_keys": [],
             "description": "Grants permission to describe a state machine",
             "orphan": false,
             "resources": [
                 "statemachine"
             ]
         },
+        "DescribeStateMachineAlias": {
+            "access_level": "Undocumented",
+            "action": "DescribeStateMachineAlias",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DescribeStateMachineForExecution": {
             "access_level": "Read",
             "action": "DescribeStateMachineForExecution",
             "condition_keys": [],
             "description": "Grants permission to describe the state machine for an execution",
             "orphan": false,
             "resources": [
@@ -142332,14 +142374,30 @@
             "condition_keys": [],
             "description": "Grants permission to list the map runs of an execution",
             "orphan": false,
             "resources": [
                 "execution"
             ]
         },
+        "ListStateMachineAliases": {
+            "access_level": "Undocumented",
+            "action": "ListStateMachineAliases",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListStateMachineVersions": {
+            "access_level": "Undocumented",
+            "action": "ListStateMachineVersions",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListStateMachines": {
             "access_level": "List",
             "action": "ListStateMachines",
             "condition_keys": [],
             "description": "Grants permission to lists the existing state machines",
             "orphan": false,
             "resources": []
@@ -142351,14 +142409,22 @@
             "description": "Grants permission to list tags for an AWS Step Functions resource",
             "orphan": false,
             "resources": [
                 "activity",
                 "statemachine"
             ]
         },
+        "PublishStateMachineVersion": {
+            "access_level": "Undocumented",
+            "action": "PublishStateMachineVersion",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "SendTaskFailure": {
             "access_level": "Write",
             "action": "SendTaskFailure",
             "condition_keys": [],
             "description": "Grants permission to report that the task identified by the taskToken failed",
             "orphan": false,
             "resources": []
@@ -142454,14 +142520,22 @@
                 "aws:TagKeys"
             ],
             "description": "Grants permission to update a state machine",
             "orphan": false,
             "resources": [
                 "statemachine"
             ]
+        },
+        "UpdateStateMachineAlias": {
+            "access_level": "Undocumented",
+            "action": "UpdateStateMachineAlias",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
         }
     },
     "storagegateway": {
         "ActivateGateway": {
             "access_level": "Write",
             "action": "ActivateGateway",
             "condition_keys": [
```

### Comparing `iam_actions-1.2.20230622/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230623/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230622/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230623/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230622/iam_actions/generate/generate.py` & `iam_actions-1.2.20230623/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230622/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230623/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230622/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230623/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230622/iam_actions/generate/services.py` & `iam_actions-1.2.20230623/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230622/iam_actions/policies.json` & `iam_actions-1.2.20230623/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994243372189386%*

 * *Differences: {"'serviceMap'": "{'AWS Network Manager': {'ARNFormat': "*

 * *                 "'arn:aws:networkmanager::${Account}:${ResourceType}/${ResourceName}'}, 'AWS Step "*

 * *                 "Functions': {'Actions': {insert: [(2, 'CreateStateMachineAlias'), (5, "*

 * *                 "'DeleteStateMachineAlias'), (6, 'DeleteStateMachineVersion'), (11, "*

 * *                 "'DescribeStateMachineAlias'), (18, 'ListStateMachineAliases'), (19, "*

 * *                 "'ListStateMachineVersions'), (22, 'PublishStateMachineVersion'), (33,  […]*

```diff
@@ -687,15 +687,18 @@
                 "StartExportTask",
                 "StartImportTask",
                 "StopContinuousExport",
                 "StopDataCollectionByAgentIds",
                 "UpdateApplication"
             ],
             "HasResource": false,
-            "StringPrefix": "discovery"
+            "StringPrefix": "discovery",
+            "conditionKeys": [
+                "aws:TagKeys"
+            ]
         },
         "AWS Application Migration Service": {
             "ARNFormat": "arn:aws:mgn:${Region}:${Account}:${ResourceType}/${ResourceName}",
             "ARNRegex": "^arn:aws:mgn:.+",
             "Actions": [
                 "ArchiveApplication",
                 "ArchiveWave",
@@ -4756,15 +4759,15 @@
                 "StartSync",
                 "StopSync",
                 "UpdateSyncTarget"
             ],
             "HasResource": true,
             "StringPrefix": "identity-sync"
         },
-        "AWS Identity and Access Management": {
+        "AWS Identity and Access Management (IAM)": {
             "ARNFormat": "arn:aws:iam::${Account}:${ResourceType}/${ResourceName}",
             "ARNRegex": "^arn:aws:iam::.+",
             "Actions": [
                 "AddClientIDToOpenIDConnectProvider",
                 "AddRoleToInstanceProfile",
                 "AddUserToGroup",
                 "AttachGroupPolicy",
@@ -4827,14 +4830,15 @@
                 "GetContextKeysForCustomPolicy",
                 "GetContextKeysForPrincipalPolicy",
                 "GetCredentialReport",
                 "GetGroup",
                 "GetGroupPolicy",
                 "GetInstanceProfile",
                 "GetLoginProfile",
+                "GetMFADevice",
                 "GetOpenIDConnectProvider",
                 "GetOrganizationsAccessReport",
                 "GetPolicy",
                 "GetPolicyVersion",
                 "GetRole",
                 "GetRolePolicy",
                 "GetSAMLProvider",
@@ -4939,18 +4943,22 @@
             "StringPrefix": "iam",
             "conditionKeys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys",
                 "iam:AWSServiceName",
                 "iam:AssociatedResourceArn",
+                "iam:FIDO-FIPS-140-2-certification",
+                "iam:FIDO-FIPS-140-3-certification",
+                "iam:FIDO-certification",
                 "iam:OrganizationsPolicyId",
                 "iam:PassedToService",
                 "iam:PermissionsBoundary",
                 "iam:PolicyARN",
+                "iam:RegisterSecurityKey",
                 "iam:ResourceTag/${TagKey}"
             ]
         },
         "AWS Identity and Access Management Roles Anywhere": {
             "ARNFormat": "arn:aws:rolesanywhere:${Region}:${Account}:${ResourceType}/${ResourceId}",
             "ARNRegex": "^arn:aws:rolesanywhere:.+:.+:.+",
             "Actions": [
@@ -6852,15 +6860,15 @@
             "conditionKeys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys"
             ]
         },
         "AWS Network Manager": {
-            "ARNFormat": "arn:aws:networkmanager::${AccountId}:${ResourceType}/${ResourceName}",
+            "ARNFormat": "arn:aws:networkmanager::${Account}:${ResourceType}/${ResourceName}",
             "ARNRegex": "^arn:aws:networkmanager::.+:.+",
             "Actions": [
                 "AcceptAttachment",
                 "AssociateConnectPeer",
                 "AssociateCustomerGateway",
                 "AssociateLink",
                 "AssociateTransitGatewayConnectPeer",
@@ -8480,45 +8488,54 @@
         },
         "AWS Step Functions": {
             "ARNFormat": "arn:aws:states:${Region}:${Account}:${ResourceType}:${ResourceName}",
             "ARNRegex": "^arn:aws:states:.+",
             "Actions": [
                 "CreateActivity",
                 "CreateStateMachine",
+                "CreateStateMachineAlias",
                 "DeleteActivity",
                 "DeleteStateMachine",
+                "DeleteStateMachineAlias",
+                "DeleteStateMachineVersion",
                 "DescribeActivity",
                 "DescribeExecution",
                 "DescribeMapRun",
                 "DescribeStateMachine",
+                "DescribeStateMachineAlias",
                 "DescribeStateMachineForExecution",
                 "GetActivityTask",
                 "GetExecutionHistory",
                 "ListActivities",
                 "ListExecutions",
                 "ListMapRuns",
+                "ListStateMachineAliases",
+                "ListStateMachineVersions",
                 "ListStateMachines",
                 "ListTagsForResource",
+                "PublishStateMachineVersion",
                 "SendTaskFailure",
                 "SendTaskHeartbeat",
                 "SendTaskSuccess",
                 "StartExecution",
                 "StartSyncExecution",
                 "StopExecution",
                 "TagResource",
                 "UntagResource",
                 "UpdateMapRun",
-                "UpdateStateMachine"
+                "UpdateStateMachine",
+                "UpdateStateMachineAlias"
             ],
             "HasResource": true,
             "StringPrefix": "states",
             "conditionKeys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
-                "aws:TagKeys"
+                "aws:TagKeys",
+                "states:StateMachineQualifier"
             ]
         },
         "AWS Storage Gateway": {
             "ARNFormat": "arn:aws:storagegateway:${Region}:${Account}:${ResourceType}/${ResourceName}",
             "ARNRegex": "^arn:aws:storagegateway:.+",
             "Actions": [
                 "ActivateGateway",
@@ -14822,14 +14839,15 @@
                 "ListGroupsOlderThanOrderingId",
                 "ListIndices",
                 "ListQuerySuggestionsBlockLists",
                 "ListTagsForResource",
                 "ListThesauri",
                 "PutPrincipalMapping",
                 "Query",
+                "Retrieve",
                 "StartDataSourceSyncJob",
                 "StopDataSourceSyncJob",
                 "SubmitFeedback",
                 "TagResource",
                 "UntagResource",
                 "UpdateAccessControlConfiguration",
                 "UpdateDataSource",
```

### Comparing `iam_actions-1.2.20230622/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230623/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230622/iam_actions/services.json` & `iam_actions-1.2.20230623/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999563535005556%*

 * *Differences: {"'discovery'": "{'ConditionKeys': ['aws:TagKeys']}",*

 * * "'iam'": "{'Actions': {insert: [(67, 'GetMFADevice')]}, 'ServiceNames': ['AWS Identity and Access "*

 * *          "Management (IAM)'], 'ConditionKeys': {insert: [(5, "*

 * *          "'iam:FIDO-FIPS-140-2-certification'), (6, 'iam:FIDO-FIPS-140-3-certification'), (7, "*

 * *          "'iam:FIDO-certification'), (12, 'iam:RegisterSecurityKey')]}}",*

 * * "'kendra'": "{'Actions': {insert: [(52, 'Retrieve')]}}",*

 * * "'networkmanager'": "{'ARNFormats': "*

 * *                     "[' […]*

```diff
@@ -5776,15 +5776,17 @@
             "StartDataCollectionByAgentIds",
             "StartExportTask",
             "StartImportTask",
             "StopContinuousExport",
             "StopDataCollectionByAgentIds",
             "UpdateApplication"
         ],
-        "ConditionKeys": [],
+        "ConditionKeys": [
+            "aws:TagKeys"
+        ],
         "HasResource": false,
         "ServiceNames": [
             "AWS Application Discovery Service"
         ]
     },
     "dlm": {
         "ARNFormats": [
@@ -9920,14 +9922,15 @@
             "GetContextKeysForCustomPolicy",
             "GetContextKeysForPrincipalPolicy",
             "GetCredentialReport",
             "GetGroup",
             "GetGroupPolicy",
             "GetInstanceProfile",
             "GetLoginProfile",
+            "GetMFADevice",
             "GetOpenIDConnectProvider",
             "GetOrganizationsAccessReport",
             "GetPolicy",
             "GetPolicyVersion",
             "GetRole",
             "GetRolePolicy",
             "GetSAMLProvider",
@@ -10030,23 +10033,27 @@
         ],
         "ConditionKeys": [
             "aws:RequestTag/${TagKey}",
             "aws:ResourceTag/${TagKey}",
             "aws:TagKeys",
             "iam:AWSServiceName",
             "iam:AssociatedResourceArn",
+            "iam:FIDO-FIPS-140-2-certification",
+            "iam:FIDO-FIPS-140-3-certification",
+            "iam:FIDO-certification",
             "iam:OrganizationsPolicyId",
             "iam:PassedToService",
             "iam:PermissionsBoundary",
             "iam:PolicyARN",
+            "iam:RegisterSecurityKey",
             "iam:ResourceTag/${TagKey}"
         ],
         "HasResource": true,
         "ServiceNames": [
-            "AWS Identity and Access Management"
+            "AWS Identity and Access Management (IAM)"
         ]
     },
     "identity-sync": {
         "ARNFormats": [
             "arn:aws:identity-sync:${Region}:${Account}:${ResourceType}/${ResourcePath}"
         ],
         "ARNRegexes": [
@@ -11690,14 +11697,15 @@
             "ListGroupsOlderThanOrderingId",
             "ListIndices",
             "ListQuerySuggestionsBlockLists",
             "ListTagsForResource",
             "ListThesauri",
             "PutPrincipalMapping",
             "Query",
+            "Retrieve",
             "StartDataSourceSyncJob",
             "StopDataSourceSyncJob",
             "SubmitFeedback",
             "TagResource",
             "UntagResource",
             "UpdateAccessControlConfiguration",
             "UpdateDataSource",
@@ -14257,15 +14265,15 @@
         "HasResource": true,
         "ServiceNames": [
             "AWS Network Firewall"
         ]
     },
     "networkmanager": {
         "ARNFormats": [
-            "arn:aws:networkmanager::${AccountId}:${ResourceType}/${ResourceName}"
+            "arn:aws:networkmanager::${Account}:${ResourceType}/${ResourceName}"
         ],
         "ARNRegexes": [
             "^arn:aws:networkmanager::.+:.+"
         ],
         "Actions": [
             "AcceptAttachment",
             "AssociateConnectPeer",
@@ -19779,43 +19787,52 @@
         ],
         "ARNRegexes": [
             "^arn:aws:states:.+"
         ],
         "Actions": [
             "CreateActivity",
             "CreateStateMachine",
+            "CreateStateMachineAlias",
             "DeleteActivity",
             "DeleteStateMachine",
+            "DeleteStateMachineAlias",
+            "DeleteStateMachineVersion",
             "DescribeActivity",
             "DescribeExecution",
             "DescribeMapRun",
             "DescribeStateMachine",
+            "DescribeStateMachineAlias",
             "DescribeStateMachineForExecution",
             "GetActivityTask",
             "GetExecutionHistory",
             "ListActivities",
             "ListExecutions",
             "ListMapRuns",
+            "ListStateMachineAliases",
+            "ListStateMachineVersions",
             "ListStateMachines",
             "ListTagsForResource",
+            "PublishStateMachineVersion",
             "SendTaskFailure",
             "SendTaskHeartbeat",
             "SendTaskSuccess",
             "StartExecution",
             "StartSyncExecution",
             "StopExecution",
             "TagResource",
             "UntagResource",
             "UpdateMapRun",
-            "UpdateStateMachine"
+            "UpdateStateMachine",
+            "UpdateStateMachineAlias"
         ],
         "ConditionKeys": [
             "aws:RequestTag/${TagKey}",
             "aws:ResourceTag/${TagKey}",
-            "aws:TagKeys"
+            "aws:TagKeys",
+            "states:StateMachineQualifier"
         ],
         "HasResource": true,
         "ServiceNames": [
             "AWS Step Functions"
         ]
     },
     "storagegateway": {
```

### Comparing `iam_actions-1.2.20230622/pyproject.toml` & `iam_actions-1.2.20230623/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230622"
+version = "1.2.20230623"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230622/setup.py` & `iam_actions-1.2.20230623/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230622',
+    'version': '1.2.20230623',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230622/PKG-INFO` & `iam_actions-1.2.20230623/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230622
+Version: 1.2.20230623
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```


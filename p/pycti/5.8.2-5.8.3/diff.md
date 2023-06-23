# Comparing `tmp/pycti-5.8.2.tar.gz` & `tmp/pycti-5.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycti-5.8.2.tar", last modified: Mon Jun 19 19:14:46 2023, max compression
+gzip compressed data, was "pycti-5.8.3.tar", last modified: Fri Jun 23 11:17:04 2023, max compression
```

## Comparing `pycti-5.8.2.tar` & `pycti-5.8.3.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 19:14:46.156202 pycti-5.8.2/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-06-19 19:14:32.000000 pycti-5.8.2/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4087 2023-06-19 19:14:46.156202 pycti-5.8.2/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3177 2023-06-19 19:14:32.000000 pycti-5.8.2/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 19:14:46.144202 pycti-5.8.2/pycti/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3856 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 19:14:46.148202 pycti-5.8.2/pycti/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    28410 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/api/opencti_api_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3565 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/api/opencti_api_connector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6824 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/api/opencti_api_work.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 19:14:46.148202 pycti-5.8.2/pycti/connector/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/connector/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2294 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/connector/opencti_connector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    45416 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/connector/opencti_connector_helper.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 19:14:46.156202 pycti-5.8.2/pycti/entities/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/entities/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18880 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/entities/opencti_attack_pattern.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13376 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/entities/opencti_campaign.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25113 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/entities/opencti_case_incident.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24427 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/entities/opencti_case_rfi.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24435 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/entities/opencti_case_rft.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13858 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/entities/opencti_channel.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14512 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/entities/opencti_course_of_action.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14598 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/entities/opencti_data_component.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14155 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/entities/opencti_data_source.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14003 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/entities/opencti_event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10891 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/entities/opencti_external_reference.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25480 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/entities/opencti_feedback.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22913 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/entities/opencti_grouping.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17564 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/entities/opencti_identity.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14024 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/entities/opencti_incident.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23077 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/entities/opencti_indicator.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15944 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/entities/opencti_infrastructure.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14455 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/entities/opencti_intrusion_set.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7854 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/entities/opencti_kill_chain_phase.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7350 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/entities/opencti_label.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13006 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/entities/opencti_language.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14554 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/entities/opencti_location.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16288 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/entities/opencti_malware.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17551 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/entities/opencti_malware_analysis.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12156 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/entities/opencti_marking_definition.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13948 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/entities/opencti_narrative.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22348 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/entities/opencti_note.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22667 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/entities/opencti_observed_data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20971 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/entities/opencti_opinion.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23782 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/entities/opencti_report.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2399 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/entities/opencti_stix.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    32440 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/entities/opencti_stix_core_object.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    41865 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/entities/opencti_stix_core_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    92142 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/entities/opencti_stix_cyber_observable.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    64861 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/entities/opencti_stix_domain_object.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12081 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/entities/opencti_stix_nested_ref_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16091 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/entities/opencti_stix_object_or_stix_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27612 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/entities/opencti_stix_sighting_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23493 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/entities/opencti_task.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18371 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/entities/opencti_threat_actor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14210 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/entities/opencti_tool.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5870 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/entities/opencti_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17683 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/entities/opencti_vulnerability.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 19:14:46.156202 pycti-5.8.2/pycti/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/utils/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3397 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/utils/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   103481 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/utils/opencti_stix2.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4496 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/utils/opencti_stix2_splitter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14520 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/utils/opencti_stix2_update.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3677 2023-06-19 19:14:32.000000 pycti-5.8.2/pycti/utils/opencti_stix2_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-19 19:14:46.148202 pycti-5.8.2/pycti.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4087 2023-06-19 19:14:46.000000 pycti-5.8.2/pycti.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2324 2023-06-19 19:14:46.000000 pycti-5.8.2/pycti.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-19 19:14:46.000000 pycti-5.8.2/pycti.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      581 2023-06-19 19:14:46.000000 pycti-5.8.2/pycti.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-06-19 19:14:46.000000 pycti-5.8.2/pycti.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2023-06-19 19:14:32.000000 pycti-5.8.2/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1596 2023-06-19 19:14:46.156202 pycti-5.8.2/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 11:17:04.363731 pycti-5.8.3/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-06-23 11:16:52.000000 pycti-5.8.3/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4087 2023-06-23 11:17:04.363731 pycti-5.8.3/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3177 2023-06-23 11:16:52.000000 pycti-5.8.3/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 11:17:04.355731 pycti-5.8.3/pycti/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3856 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 11:17:04.355731 pycti-5.8.3/pycti/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    28410 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/api/opencti_api_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3565 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/api/opencti_api_connector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6825 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/api/opencti_api_work.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 11:17:04.355731 pycti-5.8.3/pycti/connector/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/connector/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2294 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/connector/opencti_connector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    45735 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/connector/opencti_connector_helper.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 11:17:04.363731 pycti-5.8.3/pycti/entities/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18880 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_attack_pattern.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13376 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_campaign.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25113 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_case_incident.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24427 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_case_rfi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24435 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_case_rft.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13858 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_channel.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14512 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_course_of_action.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14598 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_data_component.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14155 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_data_source.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14003 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10891 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_external_reference.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25480 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_feedback.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22913 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_grouping.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17564 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_identity.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14024 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_incident.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23077 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_indicator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15944 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_infrastructure.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14455 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_intrusion_set.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7854 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_kill_chain_phase.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7350 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_label.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13006 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_language.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14554 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_location.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16288 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_malware.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17551 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_malware_analysis.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12156 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_marking_definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13948 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_narrative.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22348 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_note.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22667 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_observed_data.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20971 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_opinion.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23782 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_report.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2399 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_stix.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    32440 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_stix_core_object.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    41865 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_stix_core_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    92142 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_stix_cyber_observable.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    64861 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_stix_domain_object.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12081 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_stix_nested_ref_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16091 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_stix_object_or_stix_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27612 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_stix_sighting_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23493 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_task.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18371 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_threat_actor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14210 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_tool.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5870 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17683 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_vulnerability.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 11:17:04.363731 pycti-5.8.3/pycti/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3397 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/utils/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   103481 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/utils/opencti_stix2.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4496 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/utils/opencti_stix2_splitter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14520 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/utils/opencti_stix2_update.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3677 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/utils/opencti_stix2_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 11:17:04.355731 pycti-5.8.3/pycti.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4087 2023-06-23 11:17:04.000000 pycti-5.8.3/pycti.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2324 2023-06-23 11:17:04.000000 pycti-5.8.3/pycti.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-23 11:17:04.000000 pycti-5.8.3/pycti.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      581 2023-06-23 11:17:04.000000 pycti-5.8.3/pycti.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-06-23 11:17:04.000000 pycti-5.8.3/pycti.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2023-06-23 11:16:52.000000 pycti-5.8.3/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1596 2023-06-23 11:17:04.363731 pycti-5.8.3/setup.cfg
```

### Comparing `pycti-5.8.2/LICENSE` & `pycti-5.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/PKG-INFO` & `pycti-5.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycti
-Version: 5.8.2
+Version: 5.8.3
 Summary: Python API client for OpenCTI.
 Home-page: https://github.com/OpenCTI-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pycti Version: 5.8.2 Summary: Python API client for
+Metadata-Version: 2.1 Name: pycti Version: 5.8.3 Summary: Python API client for
 OpenCTI. Home-page: https://github.com/OpenCTI-Platform/client-python Author:
 Filigran Author-email: contact@filigran.io Maintainer: Filigran License: Apache
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
 Classifier: Natural Language :: French Classifier: Operating System :: OS
```

### Comparing `pycti-5.8.2/README.md` & `pycti-5.8.3/README.md`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/__init__.py` & `pycti-5.8.3/pycti/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-__version__ = "5.8.2"
+__version__ = "5.8.3"
 
 from .api.opencti_api_client import OpenCTIApiClient
 from .api.opencti_api_connector import OpenCTIApiConnector
 from .api.opencti_api_work import OpenCTIApiWork
 from .connector.opencti_connector import ConnectorType, OpenCTIConnector
 from .connector.opencti_connector_helper import (
     OpenCTIConnectorHelper,
```

### Comparing `pycti-5.8.2/pycti/api/opencti_api_client.py` & `pycti-5.8.3/pycti/api/opencti_api_client.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/api/opencti_api_connector.py` & `pycti-5.8.3/pycti/api/opencti_api_connector.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/api/opencti_api_work.py` & `pycti-5.8.3/pycti/api/opencti_api_work.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
                     toReceived (message: $message)
                 }
             }
            """
         self.api.query(query, {"id": work_id, "message": message})
 
     def to_processed(self, work_id: str, message: str, in_error: bool = False):
-        LOGGER.info("Reporting work update_received %s", work_id)
+        LOGGER.info("Reporting work update_processed %s", work_id)
         query = """
             mutation workToProcessed($id: ID!, $message: String, $inError: Boolean) {
                 workEdit(id: $id) {
                     toProcessed (message: $message, inError: $inError)
                 }
             }
            """
```

### Comparing `pycti-5.8.2/pycti/connector/opencti_connector.py` & `pycti-5.8.3/pycti/connector/opencti_connector.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/connector/opencti_connector_helper.py` & `pycti-5.8.3/pycti/connector/opencti_connector_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 
 def get_config_variable(
     env_var: str,
     yaml_path: List,
     config: Dict = {},
     isNumber: Optional[bool] = False,
     default=None,
+    required=False,
 ) -> Union[bool, int, None, str]:
     """[summary]
 
     :param env_var: environment variable name
     :param yaml_path: path to yaml config
     :param config: client config dict, defaults to {}
     :param isNumber: specify if the variable is a number, defaults to False
@@ -70,14 +71,21 @@
     if result in TRUTHY:
         return True
     if result in FALSY:
         return False
     if isNumber:
         return int(result)
 
+    if (
+        required
+        and default is None
+        and (result is None or (isinstance(result, str) and len(result) == 0))
+    ):
+        raise ValueError("The configuration " + env_var + " is required")
+
     if isinstance(result, str) and len(result) == 0:
         return default
 
     return result
 
 
 def is_memory_certificate(certificate):
@@ -1194,14 +1202,17 @@
         :type tlp: str
         :param max_tlp: the highest allowed TLP level
         :type max_tlp: str
         :return: TLP level in allowed TLPs
         :rtype: bool
         """
 
+        if tlp is None or max_tlp is None:
+            return True
+
         allowed_tlps: Dict[str, List[str]] = {
             "TLP:RED": [
                 "TLP:WHITE",
                 "TLP:CLEAR",
                 "TLP:GREEN",
                 "TLP:AMBER",
                 "TLP:AMBER+STRICT",
@@ -1216,15 +1227,15 @@
             ],
             "TLP:AMBER": ["TLP:WHITE", "TLP:CLEAR", "TLP:GREEN", "TLP:AMBER"],
             "TLP:GREEN": ["TLP:WHITE", "TLP:CLEAR", "TLP:GREEN"],
             "TLP:WHITE": ["TLP:WHITE", "TLP:CLEAR"],
             "TLP:CLEAR": ["TLP:WHITE", "TLP:CLEAR"],
         }
 
-        return tlp in allowed_tlps[max_tlp]
+        return tlp.upper() in allowed_tlps[max_tlp.upper()]
 
     @staticmethod
     def get_attribute_in_extension(key, object) -> any:
         if (
             "extensions" in object
             and "extension-definition--ea279b3e-5c71-4632-ac08-831c66a786ba"
             in object["extensions"]
```

### Comparing `pycti-5.8.2/pycti/entities/opencti_attack_pattern.py` & `pycti-5.8.3/pycti/entities/opencti_attack_pattern.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/entities/opencti_campaign.py` & `pycti-5.8.3/pycti/entities/opencti_campaign.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/entities/opencti_case_incident.py` & `pycti-5.8.3/pycti/entities/opencti_case_incident.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/entities/opencti_case_rfi.py` & `pycti-5.8.3/pycti/entities/opencti_case_rfi.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/entities/opencti_case_rft.py` & `pycti-5.8.3/pycti/entities/opencti_case_rft.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/entities/opencti_channel.py` & `pycti-5.8.3/pycti/entities/opencti_channel.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/entities/opencti_course_of_action.py` & `pycti-5.8.3/pycti/entities/opencti_course_of_action.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/entities/opencti_data_component.py` & `pycti-5.8.3/pycti/entities/opencti_data_component.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/entities/opencti_data_source.py` & `pycti-5.8.3/pycti/entities/opencti_data_source.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/entities/opencti_event.py` & `pycti-5.8.3/pycti/entities/opencti_event.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/entities/opencti_external_reference.py` & `pycti-5.8.3/pycti/entities/opencti_external_reference.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/entities/opencti_feedback.py` & `pycti-5.8.3/pycti/entities/opencti_feedback.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/entities/opencti_grouping.py` & `pycti-5.8.3/pycti/entities/opencti_grouping.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/entities/opencti_identity.py` & `pycti-5.8.3/pycti/entities/opencti_identity.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/entities/opencti_incident.py` & `pycti-5.8.3/pycti/entities/opencti_incident.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/entities/opencti_indicator.py` & `pycti-5.8.3/pycti/entities/opencti_indicator.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/entities/opencti_infrastructure.py` & `pycti-5.8.3/pycti/entities/opencti_infrastructure.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/entities/opencti_intrusion_set.py` & `pycti-5.8.3/pycti/entities/opencti_intrusion_set.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/entities/opencti_kill_chain_phase.py` & `pycti-5.8.3/pycti/entities/opencti_kill_chain_phase.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/entities/opencti_label.py` & `pycti-5.8.3/pycti/entities/opencti_label.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/entities/opencti_language.py` & `pycti-5.8.3/pycti/entities/opencti_language.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/entities/opencti_location.py` & `pycti-5.8.3/pycti/entities/opencti_location.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/entities/opencti_malware.py` & `pycti-5.8.3/pycti/entities/opencti_malware.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/entities/opencti_malware_analysis.py` & `pycti-5.8.3/pycti/entities/opencti_malware_analysis.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/entities/opencti_marking_definition.py` & `pycti-5.8.3/pycti/entities/opencti_marking_definition.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/entities/opencti_narrative.py` & `pycti-5.8.3/pycti/entities/opencti_narrative.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/entities/opencti_note.py` & `pycti-5.8.3/pycti/entities/opencti_note.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/entities/opencti_observed_data.py` & `pycti-5.8.3/pycti/entities/opencti_observed_data.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/entities/opencti_opinion.py` & `pycti-5.8.3/pycti/entities/opencti_opinion.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/entities/opencti_report.py` & `pycti-5.8.3/pycti/entities/opencti_report.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/entities/opencti_stix.py` & `pycti-5.8.3/pycti/entities/opencti_stix.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/entities/opencti_stix_core_object.py` & `pycti-5.8.3/pycti/entities/opencti_stix_core_object.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/entities/opencti_stix_core_relationship.py` & `pycti-5.8.3/pycti/entities/opencti_stix_core_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/entities/opencti_stix_cyber_observable.py` & `pycti-5.8.3/pycti/entities/opencti_stix_cyber_observable.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/entities/opencti_stix_domain_object.py` & `pycti-5.8.3/pycti/entities/opencti_stix_domain_object.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/entities/opencti_stix_nested_ref_relationship.py` & `pycti-5.8.3/pycti/entities/opencti_stix_nested_ref_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/entities/opencti_stix_object_or_stix_relationship.py` & `pycti-5.8.3/pycti/entities/opencti_stix_object_or_stix_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/entities/opencti_stix_sighting_relationship.py` & `pycti-5.8.3/pycti/entities/opencti_stix_sighting_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/entities/opencti_task.py` & `pycti-5.8.3/pycti/entities/opencti_task.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/entities/opencti_threat_actor.py` & `pycti-5.8.3/pycti/entities/opencti_threat_actor.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/entities/opencti_tool.py` & `pycti-5.8.3/pycti/entities/opencti_tool.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/entities/opencti_vocabulary.py` & `pycti-5.8.3/pycti/entities/opencti_vocabulary.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/entities/opencti_vulnerability.py` & `pycti-5.8.3/pycti/entities/opencti_vulnerability.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/utils/constants.py` & `pycti-5.8.3/pycti/utils/constants.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/utils/opencti_stix2.py` & `pycti-5.8.3/pycti/utils/opencti_stix2.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/utils/opencti_stix2_splitter.py` & `pycti-5.8.3/pycti/utils/opencti_stix2_splitter.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/utils/opencti_stix2_update.py` & `pycti-5.8.3/pycti/utils/opencti_stix2_update.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti/utils/opencti_stix2_utils.py` & `pycti-5.8.3/pycti/utils/opencti_stix2_utils.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti.egg-info/PKG-INFO` & `pycti-5.8.3/pycti.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycti
-Version: 5.8.2
+Version: 5.8.3
 Summary: Python API client for OpenCTI.
 Home-page: https://github.com/OpenCTI-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pycti Version: 5.8.2 Summary: Python API client for
+Metadata-Version: 2.1 Name: pycti Version: 5.8.3 Summary: Python API client for
 OpenCTI. Home-page: https://github.com/OpenCTI-Platform/client-python Author:
 Filigran Author-email: contact@filigran.io Maintainer: Filigran License: Apache
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
 Classifier: Natural Language :: French Classifier: Operating System :: OS
```

### Comparing `pycti-5.8.2/pycti.egg-info/SOURCES.txt` & `pycti-5.8.3/pycti.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/pycti.egg-info/requires.txt` & `pycti-5.8.3/pycti.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 datefinder~=0.7.3
 pika~=1.3.1
 python_json_logger~=2.0.4
 pyyaml~=6.0
 requests~=2.31.0
-setuptools~=67.8.0
+setuptools~=68.0.0
 filigran-sseclient~=1.0.0
 stix2~=3.0.1
 cachetools~=5.3.0
 
 [:sys_platform == "linux" or sys_platform == "darwin"]
 python-magic~=0.4.27
```

### Comparing `pycti-5.8.2/pyproject.toml` & `pycti-5.8.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pycti-5.8.2/setup.cfg` & `pycti-5.8.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 	datefinder~=0.7.3
 	pika~=1.3.1
 	python-magic~=0.4.27; sys_platform == "linux" or sys_platform == "darwin"
 	python-magic-bin~=0.4.14; sys_platform == "win32"
 	python_json_logger~=2.0.4
 	pyyaml~=6.0
 	requests~=2.31.0
-	setuptools~=67.8.0
+	setuptools~=68.0.0
 	filigran-sseclient~=1.0.0
 	stix2~=3.0.1
 	cachetools~=5.3.0
 
 [options.extras_require]
 dev = 
 	black~=23.3.0
```


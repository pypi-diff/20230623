# Comparing `tmp/lusid-notification-sdk-preview-0.1.748.post6.tar.gz` & `tmp/lusid-notification-sdk-preview-0.1.756.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lusid-notification-sdk-preview-0.1.748.post6.tar", last modified: Wed Jun 21 13:45:56 2023, max compression
+gzip compressed data, was "dist/lusid-notification-sdk-preview-0.1.756.tar", last modified: Fri Jun 23 12:35:51 2023, max compression
```

## Comparing `lusid-notification-sdk-preview-0.1.748.post6.tar` & `lusid-notification-sdk-preview-0.1.756.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:45:56.000000 lusid-notification-sdk-preview-0.1.748.post6/
--rw-r--r--   0 root         (0) root         (0)       53 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      385 2023-06-21 13:45:56.000000 lusid-notification-sdk-preview-0.1.748.post6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7789 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:45:56.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/
--rw-r--r--   0 root         (0) root         (0)     4201 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/__init__.py
--rw-r--r--   0 root         (0) root         (0)       26 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:45:56.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/api/
--rw-r--r--   0 root         (0) root         (0)      442 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6851 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/api/application_metadata_api.py
--rw-r--r--   0 root         (0) root         (0)    13990 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/api/event_types_api.py
--rw-r--r--   0 root         (0) root         (0)     7824 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/api/manual_event_api.py
--rw-r--r--   0 root         (0) root         (0)    52809 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/api/notifications_api.py
--rw-r--r--   0 root         (0) root         (0)    47815 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/api/subscriptions_api.py
--rw-r--r--   0 root         (0) root         (0)    27787 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/api_client.py
--rw-r--r--   0 root         (0) root         (0)    16601 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5101 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:45:56.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/
--rw-r--r--   0 root         (0) root         (0)     2911 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7256 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/access_controlled_action.py
--rw-r--r--   0 root         (0) root         (0)     9019 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7233 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/action_id.py
--rw-r--r--   0 root         (0) root         (0)    10756 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/amazon_sqs_notification_type.py
--rw-r--r--   0 root         (0) root         (0)     9033 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/api_request_notification_type.py
--rw-r--r--   0 root         (0) root         (0)    10781 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/create_notification_request.py
--rw-r--r--   0 root         (0) root         (0)    12415 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/create_subscription.py
--rw-r--r--   0 root         (0) root         (0)    14734 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/email_notification_type.py
--rw-r--r--   0 root         (0) root         (0)    11112 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/event_type_schema.py
--rw-r--r--   0 root         (0) root         (0)     8023 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/id_selector_definition.py
--rw-r--r--   0 root         (0) root         (0)     9512 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/identifier_part_schema.py
--rw-r--r--   0 root         (0) root         (0)     6427 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/link.py
--rw-r--r--   0 root         (0) root         (0)     9541 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/lusid_problem_details.py
--rw-r--r--   0 root         (0) root         (0)    10706 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/lusid_validation_problem_details.py
--rw-r--r--   0 root         (0) root         (0)     5088 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/manual_event.py
--rw-r--r--   0 root         (0) root         (0)     7865 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/manual_event_body.py
--rw-r--r--   0 root         (0) root         (0)     6829 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/manual_event_header.py
--rw-r--r--   0 root         (0) root         (0)     4164 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/manual_event_request.py
--rw-r--r--   0 root         (0) root         (0)     7438 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/matching_pattern.py
--rw-r--r--   0 root         (0) root         (0)    15653 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/notification.py
--rw-r--r--   0 root         (0) root         (0)     5156 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/notification_status.py
--rw-r--r--   0 root         (0) root         (0)    35982 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/notification_type.py
--rw-r--r--   0 root         (0) root         (0)     6100 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/resource_id.py
--rw-r--r--   0 root         (0) root         (0)     7770 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7518 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/resource_list_of_event_type_schema.py
--rw-r--r--   0 root         (0) root         (0)     7434 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/resource_list_of_notification.py
--rw-r--r--   0 root         (0) root         (0)     7434 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/resource_list_of_subscription.py
--rw-r--r--   0 root         (0) root         (0)     7811 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/sms_notification_type.py
--rw-r--r--   0 root         (0) root         (0)    16642 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/subscription.py
--rw-r--r--   0 root         (0) root         (0)     8610 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/update_notification_request.py
--rw-r--r--   0 root         (0) root         (0)    11553 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/update_subscription.py
--rw-r--r--   0 root         (0) root         (0)    15602 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/webhook_notification_type.py
--rw-r--r--   0 root         (0) root         (0)    13562 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:45:56.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/utilities/
--rw-r--r--   0 root         (0) root         (0)       64 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1040 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/utilities/config_keys.json
--rw-r--r--   0 root         (0) root         (0)      295 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/utilities/config_keys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 13:45:56.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification_sdk_preview.egg-info/
--rw-r--r--   0 root         (0) root         (0)      385 2023-06-21 13:45:56.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification_sdk_preview.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2566 2023-06-21 13:45:56.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification_sdk_preview.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 13:45:56.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification_sdk_preview.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      116 2023-06-21 13:45:56.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification_sdk_preview.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-06-21 13:45:56.000000 lusid-notification-sdk-preview-0.1.748.post6/lusid_notification_sdk_preview.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 13:45:56.000000 lusid-notification-sdk-preview-0.1.748.post6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2327 2023-06-21 13:45:25.000000 lusid-notification-sdk-preview-0.1.748.post6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 12:35:51.000000 lusid-notification-sdk-preview-0.1.756/
+-rw-r--r--   0 root         (0) root         (0)       53 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      379 2023-06-23 12:35:51.000000 lusid-notification-sdk-preview-0.1.756/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7826 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 12:35:51.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/
+-rw-r--r--   0 root         (0) root         (0)     4279 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       24 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 12:35:51.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/api/
+-rw-r--r--   0 root         (0) root         (0)      442 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6847 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/api/application_metadata_api.py
+-rw-r--r--   0 root         (0) root         (0)    13984 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/api/event_types_api.py
+-rw-r--r--   0 root         (0) root         (0)     7820 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/api/manual_event_api.py
+-rw-r--r--   0 root         (0) root         (0)    52797 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/api/notifications_api.py
+-rw-r--r--   0 root         (0) root         (0)    47803 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/api/subscriptions_api.py
+-rw-r--r--   0 root         (0) root         (0)    27431 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    16631 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5099 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 12:35:51.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/models/
+-rw-r--r--   0 root         (0) root         (0)     2991 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7254 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/models/access_controlled_action.py
+-rw-r--r--   0 root         (0) root         (0)     9017 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/models/access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7231 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/models/action_id.py
+-rw-r--r--   0 root         (0) root         (0)    11055 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/models/amazon_sqs_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)     9333 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/models/api_request_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)    10779 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/models/create_notification_request.py
+-rw-r--r--   0 root         (0) root         (0)    12413 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/models/create_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    15029 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/models/email_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)     4726 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/models/event_field_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9778 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/models/event_type_schema.py
+-rw-r--r--   0 root         (0) root         (0)     8021 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/models/id_selector_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9510 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/models/identifier_part_schema.py
+-rw-r--r--   0 root         (0) root         (0)     6425 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/models/link.py
+-rw-r--r--   0 root         (0) root         (0)     9539 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/models/lusid_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)    10704 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/models/lusid_validation_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)     5086 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/models/manual_event.py
+-rw-r--r--   0 root         (0) root         (0)     7863 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/models/manual_event_body.py
+-rw-r--r--   0 root         (0) root         (0)     6827 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/models/manual_event_header.py
+-rw-r--r--   0 root         (0) root         (0)     4162 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/models/manual_event_request.py
+-rw-r--r--   0 root         (0) root         (0)     7436 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/models/matching_pattern.py
+-rw-r--r--   0 root         (0) root         (0)    15651 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/models/notification.py
+-rw-r--r--   0 root         (0) root         (0)     5154 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/models/notification_status.py
+-rw-r--r--   0 root         (0) root         (0)    35621 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/models/notification_type.py
+-rw-r--r--   0 root         (0) root         (0)     6098 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/models/resource_id.py
+-rw-r--r--   0 root         (0) root         (0)     7768 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7516 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/models/resource_list_of_event_type_schema.py
+-rw-r--r--   0 root         (0) root         (0)     7432 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/models/resource_list_of_notification.py
+-rw-r--r--   0 root         (0) root         (0)     7432 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/models/resource_list_of_subscription.py
+-rw-r--r--   0 root         (0) root         (0)     8104 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/models/sms_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)    16640 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/models/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     8608 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/models/update_notification_request.py
+-rw-r--r--   0 root         (0) root         (0)    11551 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/models/update_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    15899 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/models/webhook_notification_type.py
+-rw-r--r--   0 root         (0) root         (0)    13560 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 12:35:51.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/utilities/
+-rw-r--r--   0 root         (0) root         (0)       64 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/utilities/config_keys.json
+-rw-r--r--   0 root         (0) root         (0)      295 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification/utilities/config_keys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 12:35:51.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification_sdk_preview.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      379 2023-06-23 12:35:51.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification_sdk_preview.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2618 2023-06-23 12:35:51.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification_sdk_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 12:35:51.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification_sdk_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      116 2023-06-23 12:35:51.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification_sdk_preview.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-06-23 12:35:51.000000 lusid-notification-sdk-preview-0.1.756/lusid_notification_sdk_preview.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 12:35:51.000000 lusid-notification-sdk-preview-0.1.756/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2327 2023-06-23 12:35:12.000000 lusid-notification-sdk-preview-0.1.756/setup.py
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/README.md` & `lusid-notification-sdk-preview-0.1.756/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-notification-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.748-6
-- Package version: 0.1.748-6
+- API version: 0.1.756
+- Package version: 0.1.756
 - Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
@@ -49,28 +49,28 @@
 from __future__ import print_function
 
 import time
 import lusid_notification
 from lusid_notification.rest import ApiException
 from pprint import pprint
 
-# Defining the host is optional and defaults to http://localhost
+# Defining the host is optional and defaults to https://www.lusid.com/notification
 # See configuration.py for a list of all supported configuration parameters.
 configuration = lusid_notification.Configuration(
-    host = "http://localhost"
+    host = "https://www.lusid.com/notification"
 )
 
 # The client must configure the authentication and authorization parameters
 # in accordance with the API server security policy.
 # Examples for each auth method are provided below, use the example that
 # satisfies your auth use case.
 
 # Configure OAuth2 access token for authorization: oauth2
 configuration = lusid_notification.Configuration(
-    host = "http://localhost"
+    host = "https://www.lusid.com/notification"
 )
 configuration.access_token = 'YOUR_ACCESS_TOKEN'
 
 
 # Enter a context with an instance of the API client
 with lusid_notification.ApiClient(configuration) as api_client:
     # Create an instance of the API class
@@ -83,15 +83,15 @@
     except ApiException as e:
         print("Exception when calling ApplicationMetadataApi->list_access_controlled_resources: %s\n" % e)
     
 ```
 
 ## Documentation for API Endpoints
 
-All URIs are relative to *http://localhost*
+All URIs are relative to *https://www.lusid.com/notification*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *ApplicationMetadataApi* | [**list_access_controlled_resources**](docs/ApplicationMetadataApi.md#list_access_controlled_resources) | **GET** /api/metadata/access/resources | [EARLY ACCESS] ListAccessControlledResources: Get resources available for access control
 *EventTypesApi* | [**get_event_type**](docs/EventTypesApi.md#get_event_type) | **GET** /api/eventtypes/{eventType} | [EXPERIMENTAL] GetEventType: Gets the specified event type schema.
 *EventTypesApi* | [**list_event_types**](docs/EventTypesApi.md#list_event_types) | **GET** /api/eventtypes | [EXPERIMENTAL] ListEventTypes: Lists all of the available event types.
 *ManualEventApi* | [**trigger_manual_event**](docs/ManualEventApi.md#trigger_manual_event) | **POST** /api/manualevent | [EXPERIMENTAL] TriggerManualEvent: Trigger a manual event.
@@ -113,14 +113,15 @@
  - [AccessControlledResource](docs/AccessControlledResource.md)
  - [ActionId](docs/ActionId.md)
  - [AmazonSqsNotificationType](docs/AmazonSqsNotificationType.md)
  - [ApiRequestNotificationType](docs/ApiRequestNotificationType.md)
  - [CreateNotificationRequest](docs/CreateNotificationRequest.md)
  - [CreateSubscription](docs/CreateSubscription.md)
  - [EmailNotificationType](docs/EmailNotificationType.md)
+ - [EventFieldDefinition](docs/EventFieldDefinition.md)
  - [EventTypeSchema](docs/EventTypeSchema.md)
  - [IdSelectorDefinition](docs/IdSelectorDefinition.md)
  - [IdentifierPartSchema](docs/IdentifierPartSchema.md)
  - [Link](docs/Link.md)
  - [LusidProblemDetails](docs/LusidProblemDetails.md)
  - [LusidValidationProblemDetails](docs/LusidValidationProblemDetails.md)
  - [ManualEvent](docs/ManualEvent.md)
@@ -139,25 +140,22 @@
  - [SmsNotificationType](docs/SmsNotificationType.md)
  - [Subscription](docs/Subscription.md)
  - [UpdateNotificationRequest](docs/UpdateNotificationRequest.md)
  - [UpdateSubscription](docs/UpdateSubscription.md)
  - [WebhookNotificationType](docs/WebhookNotificationType.md)
 
 
-<a id="documentation-for-authorization"></a>
 ## Documentation For Authorization
 
 
-Authentication schemes defined for the API:
-<a id="oauth2"></a>
-### oauth2
+## oauth2
 
 - **Type**: OAuth
 - **Flow**: implicit
-- **Authorization URL**: https://dummyurl.lusid.com/
+- **Authorization URL**: https://lusid.okta.com/oauth2/default/v1/authorize
 - **Scopes**: N/A
 
 
 ## Author
 
 info@finbourne.com
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/__init__.py` & `lusid-notification-sdk-preview-0.1.756/lusid_notification/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-6
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.1.748-6"
+__version__ = "0.1.756"
 
 # import apis into sdk package
 from lusid_notification.api.application_metadata_api import ApplicationMetadataApi
 from lusid_notification.api.event_types_api import EventTypesApi
 from lusid_notification.api.manual_event_api import ManualEventApi
 from lusid_notification.api.notifications_api import NotificationsApi
 from lusid_notification.api.subscriptions_api import SubscriptionsApi
@@ -37,14 +37,15 @@
 from lusid_notification.models.access_controlled_resource import AccessControlledResource
 from lusid_notification.models.action_id import ActionId
 from lusid_notification.models.amazon_sqs_notification_type import AmazonSqsNotificationType
 from lusid_notification.models.api_request_notification_type import ApiRequestNotificationType
 from lusid_notification.models.create_notification_request import CreateNotificationRequest
 from lusid_notification.models.create_subscription import CreateSubscription
 from lusid_notification.models.email_notification_type import EmailNotificationType
+from lusid_notification.models.event_field_definition import EventFieldDefinition
 from lusid_notification.models.event_type_schema import EventTypeSchema
 from lusid_notification.models.id_selector_definition import IdSelectorDefinition
 from lusid_notification.models.identifier_part_schema import IdentifierPartSchema
 from lusid_notification.models.link import Link
 from lusid_notification.models.lusid_problem_details import LusidProblemDetails
 from lusid_notification.models.lusid_validation_problem_details import LusidValidationProblemDetails
 from lusid_notification.models.manual_event import ManualEvent
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/api/application_metadata_api.py` & `lusid-notification-sdk-preview-0.1.756/lusid_notification/api/application_metadata_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-6
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -141,15 +141,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.748-6'
+        header_params['X-LUSID-SDK-Version'] = '0.1.756'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfAccessControlledResource",
         }
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/api/event_types_api.py` & `lusid-notification-sdk-preview-0.1.756/lusid_notification/api/event_types_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-6
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -160,15 +160,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.748-6'
+        header_params['X-LUSID-SDK-Version'] = '0.1.756'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "EventTypeSchema",
             400: "LusidValidationProblemDetails",
@@ -292,15 +292,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.748-6'
+        header_params['X-LUSID-SDK-Version'] = '0.1.756'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfEventTypeSchema",
             404: "str",
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/api/manual_event_api.py` & `lusid-notification-sdk-preview-0.1.756/lusid_notification/api/manual_event_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-6
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -155,15 +155,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.748-6'
+        header_params['X-LUSID-SDK-Version'] = '0.1.756'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "ManualEvent",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/api/notifications_api.py` & `lusid-notification-sdk-preview-0.1.756/lusid_notification/api/notifications_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-6
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -195,15 +195,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.748-6'
+        header_params['X-LUSID-SDK-Version'] = '0.1.756'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Notification",
             400: "LusidValidationProblemDetails",
@@ -375,15 +375,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.748-6'
+        header_params['X-LUSID-SDK-Version'] = '0.1.756'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
@@ -552,15 +552,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.748-6'
+        header_params['X-LUSID-SDK-Version'] = '0.1.756'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
@@ -722,15 +722,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.748-6'
+        header_params['X-LUSID-SDK-Version'] = '0.1.756'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfNotification",
             400: "LusidValidationProblemDetails",
@@ -925,15 +925,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.748-6'
+        header_params['X-LUSID-SDK-Version'] = '0.1.756'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/api/subscriptions_api.py` & `lusid-notification-sdk-preview-0.1.756/lusid_notification/api/subscriptions_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-6
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -157,15 +157,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.748-6'
+        header_params['X-LUSID-SDK-Version'] = '0.1.756'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Subscription",
             400: "LusidValidationProblemDetails",
@@ -326,15 +326,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.748-6'
+        header_params['X-LUSID-SDK-Version'] = '0.1.756'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
@@ -492,15 +492,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.748-6'
+        header_params['X-LUSID-SDK-Version'] = '0.1.756'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Subscription",
             400: "LusidValidationProblemDetails",
@@ -680,15 +680,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.748-6'
+        header_params['X-LUSID-SDK-Version'] = '0.1.756'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfSubscription",
             400: "LusidValidationProblemDetails",
@@ -863,15 +863,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.748-6'
+        header_params['X-LUSID-SDK-Version'] = '0.1.756'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Subscription",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/api_client.py` & `lusid-notification-sdk-preview-0.1.756/lusid_notification/api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-6
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.1.748-6/python'
+        self.user_agent = 'OpenAPI-Generator/0.1.756/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
@@ -193,27 +193,27 @@
 
         self.last_response = response_data
 
         return_data = response_data
 
         if not _preload_content:
             return return_data
-
+        
         response_type = response_types_map.get(response_data.status, None)
 
         if six.PY3 and response_type not in ["file", "bytes"]:
             match = None
             content_type = response_data.getheader('content-type')
             if content_type is not None:
                 match = re.search(r"charset=([a-zA-Z\-\d]+)[\s\;]?", content_type)
             encoding = match.group(1) if match else "utf-8"
             response_data.data = response_data.data.decode(encoding)
 
         # deserialize response data
-
+        
         if response_type:
             return_data = self.deserialize(response_data, response_type)
         else:
             return_data = None
 
         if _return_http_data_only:
             return (return_data)
@@ -298,16 +298,16 @@
 
         if type(klass) == str:
             if klass.startswith('list['):
                 sub_kls = re.match(r'list\[(.*)\]', klass).group(1)
                 return [self.__deserialize(sub_data, sub_kls)
                         for sub_data in data]
 
-            if klass.startswith('dict['):
-                sub_kls = re.match(r'dict\[([^,]*), (.*)\]', klass).group(2)
+            if klass.startswith('dict('):
+                sub_kls = re.match(r'dict\(([^,]*), (.*)\)', klass).group(2)
                 return {k: self.__deserialize(v, sub_kls)
                         for k, v in six.iteritems(data)}
 
             # convert str to class
             if klass in self.NATIVE_TYPES_MAPPING:
                 klass = self.NATIVE_TYPES_MAPPING[klass]
             else:
@@ -518,72 +518,65 @@
         accepts = [x.lower() for x in accepts]
 
         if 'application/json' in accepts:
             return 'application/json'
         else:
             return ', '.join(accepts)
 
-    def select_header_content_type(self, content_types, method=None, body=None):
+    def select_header_content_type(self, content_types):
         """Returns `Content-Type` based on an array of content_types provided.
 
         :param content_types: List of content-types.
-        :param method: http method (e.g. POST, PATCH).
-        :param body: http body to send.
         :return: Content-Type (e.g. application/json).
         """
         if not content_types:
-            return None
+            return 'application/json'
 
         content_types = [x.lower() for x in content_types]
 
-        if (method == 'PATCH' and
-                'application/json-patch+json' in content_types and
-                isinstance(body, list)):
-            return 'application/json-patch+json'
-
         if 'application/json' in content_types or '*/*' in content_types:
             return 'application/json'
         else:
             return content_types[0]
 
-    def update_params_for_auth(self, headers, queries, auth_settings,
+    def update_params_for_auth(self, headers, querys, auth_settings,
                                request_auth=None):
         """Updates header and query params based on authentication setting.
 
         :param headers: Header parameters dict to be updated.
-        :param queries: Query parameters tuple list to be updated.
+        :param querys: Query parameters tuple list to be updated.
         :param auth_settings: Authentication setting identifiers list.
         :param request_auth: if set, the provided settings will
                              override the token in the configuration.
         """
         if not auth_settings:
             return
 
         if request_auth:
-            self._apply_auth_params(headers, queries, request_auth)
+            self._apply_auth_params(headers, querys, request_auth)
             return
 
         for auth in auth_settings:
             auth_setting = self.configuration.auth_settings().get(auth)
             if auth_setting:
-                self._apply_auth_params(headers, queries, auth_setting)
+                self._apply_auth_params(headers, querys, auth_setting)
 
-    def _apply_auth_params(self, headers, queries, auth_setting):
+    def _apply_auth_params(self, headers, querys, auth_setting):
         """Updates the request parameters based on a single auth_setting
 
         :param headers: Header parameters dict to be updated.
-        :param queries: Query parameters tuple list to be updated.
+        :param querys: Query parameters tuple list to be updated.
         :param auth_setting: auth settings for the endpoint
         """
         if auth_setting['in'] == 'cookie':
             headers['Cookie'] = auth_setting['value']
         elif auth_setting['in'] == 'header':
             headers[auth_setting['key']] = auth_setting['value']
         elif auth_setting['in'] == 'query':
-            queries.append((auth_setting['key'], auth_setting['value']))
+            querys.append((auth_setting['key'], auth_setting['value']))
         else:
             raise ApiValueError(
                 'Authentication token must be in `query` or `header`'
             )
 
     def __deserialize_file(self, response):
         """Deserializes body to file
@@ -688,15 +681,14 @@
                 klass.openapi_types is not None and
                 isinstance(data, (list, dict))):
             for attr, attr_type in six.iteritems(klass.openapi_types):
                 if klass.attribute_map[attr] in data:
                     value = data[klass.attribute_map[attr]]
                     kwargs[attr] = self.__deserialize(value, attr_type)
 
-        kwargs["local_vars_configuration"] = self.configuration
         instance = klass(**kwargs)
 
         if has_discriminator:
             klass_name = instance.get_real_child_model(data)
             if klass_name:
                 instance = self.__deserialize(data, klass_name)
         return instance
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/configuration.py` & `lusid-notification-sdk-preview-0.1.756/lusid_notification/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-6
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -95,15 +95,15 @@
                  server_index=None, server_variables=None,
                  server_operation_index=None, server_operation_variables=None,
                  ssl_ca_cert=None,
                  tcp_keep_alive=False,
                  ):
         """Constructor
         """
-        self._base_path = "http://localhost" if host is None else host
+        self._base_path = "https://www.lusid.com/notification" if host is None else host
         """Default Base url
         """
         self.server_index = 0 if server_index is None and host is None else server_index
         self.server_operation_index = server_operation_index or {}
         """Default server index
         """
         self.server_variables = server_variables or {}
@@ -392,26 +392,26 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.1.748-6\n"\
-               "SDK Package Version: 0.1.748-6".\
+               "Version of the API: 0.1.756\n"\
+               "SDK Package Version: 0.1.756".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
         return [
             {
-                'url': "http://localhost",
+                'url': "https://www.lusid.com/notification",
                 'description': "No description provided",
             }
         ]
 
     def get_host_from_settings(self, index, variables=None, servers=None):
         """Gets host URL based on the index and variables
         :param index: array index of the host settings
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/exceptions.py` & `lusid-notification-sdk-preview-0.1.756/lusid_notification/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-6
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/__init__.py` & `lusid-notification-sdk-preview-0.1.756/lusid_notification/models/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-6
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -19,14 +19,15 @@
 from lusid_notification.models.access_controlled_resource import AccessControlledResource
 from lusid_notification.models.action_id import ActionId
 from lusid_notification.models.amazon_sqs_notification_type import AmazonSqsNotificationType
 from lusid_notification.models.api_request_notification_type import ApiRequestNotificationType
 from lusid_notification.models.create_notification_request import CreateNotificationRequest
 from lusid_notification.models.create_subscription import CreateSubscription
 from lusid_notification.models.email_notification_type import EmailNotificationType
+from lusid_notification.models.event_field_definition import EventFieldDefinition
 from lusid_notification.models.event_type_schema import EventTypeSchema
 from lusid_notification.models.id_selector_definition import IdSelectorDefinition
 from lusid_notification.models.identifier_part_schema import IdentifierPartSchema
 from lusid_notification.models.link import Link
 from lusid_notification.models.lusid_problem_details import LusidProblemDetails
 from lusid_notification.models.lusid_validation_problem_details import LusidValidationProblemDetails
 from lusid_notification.models.manual_event import ManualEvent
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/access_controlled_action.py` & `lusid-notification-sdk-preview-0.1.756/lusid_notification/models/access_controlled_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-6
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/access_controlled_resource.py` & `lusid-notification-sdk-preview-0.1.756/lusid_notification/models/access_controlled_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-6
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/action_id.py` & `lusid-notification-sdk-preview-0.1.756/lusid_notification/models/action_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-6
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/amazon_sqs_notification_type.py` & `lusid-notification-sdk-preview-0.1.756/lusid_notification/models/amazon_sqs_notification_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-6
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -61,15 +61,15 @@
         'body': 'required',
         'queue_url_ref': 'required'
     }
 
     def __init__(self, type=None, api_key_ref=None, api_secret_ref=None, body=None, queue_url_ref=None, local_vars_configuration=None):  # noqa: E501
         """AmazonSqsNotificationType - a model defined in OpenAPI"
         
-        :param type:  (required)
+        :param type:  The type of delivery mechanism for this notification (required)
         :type type: str
         :param api_key_ref:  Reference to API key from Configuration Store (required)
         :type api_key_ref: str
         :param api_secret_ref:  Reference to API secret from Configuration Store (required)
         :type api_secret_ref: str
         :param body:  The body of the Amazon Queue Message (required)
         :type body: str
@@ -94,33 +94,38 @@
         self.body = body
         self.queue_url_ref = queue_url_ref
 
     @property
     def type(self):
         """Gets the type of this AmazonSqsNotificationType.  # noqa: E501
 
+        The type of delivery mechanism for this notification  # noqa: E501
 
         :return: The type of this AmazonSqsNotificationType.  # noqa: E501
         :rtype: str
         """
         return self._type
 
     @type.setter
     def type(self, type):
         """Sets the type of this AmazonSqsNotificationType.
 
+        The type of delivery mechanism for this notification  # noqa: E501
 
         :param type: The type of this AmazonSqsNotificationType.  # noqa: E501
         :type type: str
         """
         if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
             raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                type is not None and len(type) < 1):
-            raise ValueError("Invalid value for `type`, length must be greater than or equal to `1`")  # noqa: E501
+        allowed_values = ["AmazonSqs"]  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and type not in allowed_values:  # noqa: E501
+            raise ValueError(
+                "Invalid value for `type` ({0}), must be one of {1}"  # noqa: E501
+                .format(type, allowed_values)
+            )
 
         self._type = type
 
     @property
     def api_key_ref(self):
         """Gets the api_key_ref of this AmazonSqsNotificationType.  # noqa: E501
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/api_request_notification_type.py` & `lusid-notification-sdk-preview-0.1.756/lusid_notification/models/api_request_notification_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-6
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -58,15 +58,15 @@
         'path_and_query': 'required',
         'content': 'optional'
     }
 
     def __init__(self, type=None, http_method=None, path_and_query=None, content=None, local_vars_configuration=None):  # noqa: E501
         """ApiRequestNotificationType - a model defined in OpenAPI"
         
-        :param type:  (required)
+        :param type:  The type of delivery mechanism for this notification (required)
         :type type: str
         :param http_method:  The HTTP method such as GET, POST, etc. to use on the Api Request (required)
         :type http_method: str
         :param path_and_query:  The url to send the request to. (required)
         :type path_and_query: str
         :param content:  The content of the request
         :type content: object
@@ -87,33 +87,38 @@
         self.path_and_query = path_and_query
         self.content = content
 
     @property
     def type(self):
         """Gets the type of this ApiRequestNotificationType.  # noqa: E501
 
+        The type of delivery mechanism for this notification  # noqa: E501
 
         :return: The type of this ApiRequestNotificationType.  # noqa: E501
         :rtype: str
         """
         return self._type
 
     @type.setter
     def type(self, type):
         """Sets the type of this ApiRequestNotificationType.
 
+        The type of delivery mechanism for this notification  # noqa: E501
 
         :param type: The type of this ApiRequestNotificationType.  # noqa: E501
         :type type: str
         """
         if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
             raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                type is not None and len(type) < 1):
-            raise ValueError("Invalid value for `type`, length must be greater than or equal to `1`")  # noqa: E501
+        allowed_values = ["ApiRequest"]  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and type not in allowed_values:  # noqa: E501
+            raise ValueError(
+                "Invalid value for `type` ({0}), must be one of {1}"  # noqa: E501
+                .format(type, allowed_values)
+            )
 
         self._type = type
 
     @property
     def http_method(self):
         """Gets the http_method of this ApiRequestNotificationType.  # noqa: E501
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/create_notification_request.py` & `lusid-notification-sdk-preview-0.1.756/lusid_notification/models/create_notification_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-6
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/create_subscription.py` & `lusid-notification-sdk-preview-0.1.756/lusid_notification/models/create_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-6
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/email_notification_type.py` & `lusid-notification-sdk-preview-0.1.756/lusid_notification/models/email_notification_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-6
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -67,15 +67,15 @@
         'email_address_cc': 'optional',
         'email_address_bcc': 'optional'
     }
 
     def __init__(self, type=None, subject=None, plain_text_body=None, html_body=None, email_address_to=None, email_address_cc=None, email_address_bcc=None, local_vars_configuration=None):  # noqa: E501
         """EmailNotificationType - a model defined in OpenAPI"
         
-        :param type:  (required)
+        :param type:  The type of delivery mechanism for this notification (required)
         :type type: str
         :param subject:  The subject of the email (required)
         :type subject: str
         :param plain_text_body:  The plain text body of the email (required)
         :type plain_text_body: str
         :param html_body:  The HTML body of the email (if any)
         :type html_body: str
@@ -108,33 +108,38 @@
         self.email_address_cc = email_address_cc
         self.email_address_bcc = email_address_bcc
 
     @property
     def type(self):
         """Gets the type of this EmailNotificationType.  # noqa: E501
 
+        The type of delivery mechanism for this notification  # noqa: E501
 
         :return: The type of this EmailNotificationType.  # noqa: E501
         :rtype: str
         """
         return self._type
 
     @type.setter
     def type(self, type):
         """Sets the type of this EmailNotificationType.
 
+        The type of delivery mechanism for this notification  # noqa: E501
 
         :param type: The type of this EmailNotificationType.  # noqa: E501
         :type type: str
         """
         if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
             raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                type is not None and len(type) < 1):
-            raise ValueError("Invalid value for `type`, length must be greater than or equal to `1`")  # noqa: E501
+        allowed_values = ["Email"]  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and type not in allowed_values:  # noqa: E501
+            raise ValueError(
+                "Invalid value for `type` ({0}), must be one of {1}"  # noqa: E501
+                .format(type, allowed_values)
+            )
 
         self._type = type
 
     @property
     def subject(self):
         """Gets the subject of this EmailNotificationType.  # noqa: E501
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/event_type_schema.py` & `lusid-notification-sdk-preview-0.1.756/lusid_notification/models/event_type_schema.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-6
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -38,90 +38,76 @@
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
         'id': 'str',
         'display_name': 'str',
         'description': 'str',
-        'entity': 'str',
         'application': 'str',
-        'json_schema': 'object',
-        'header_schema': 'object',
-        'body_schema': 'object',
+        'header_schema': 'list[EventFieldDefinition]',
+        'body_schema': 'list[EventFieldDefinition]',
         'href': 'str'
     }
 
     attribute_map = {
         'id': 'id',
         'display_name': 'displayName',
         'description': 'description',
-        'entity': 'entity',
         'application': 'application',
-        'json_schema': 'jsonSchema',
         'header_schema': 'headerSchema',
         'body_schema': 'bodySchema',
         'href': 'href'
     }
 
     required_map = {
         'id': 'optional',
         'display_name': 'optional',
         'description': 'optional',
-        'entity': 'optional',
         'application': 'optional',
-        'json_schema': 'optional',
         'header_schema': 'optional',
         'body_schema': 'optional',
         'href': 'optional'
     }
 
-    def __init__(self, id=None, display_name=None, description=None, entity=None, application=None, json_schema=None, header_schema=None, body_schema=None, href=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, id=None, display_name=None, description=None, application=None, header_schema=None, body_schema=None, href=None, local_vars_configuration=None):  # noqa: E501
         """EventTypeSchema - a model defined in OpenAPI"
         
         :param id:  The identifier of the event type
         :type id: str
         :param display_name:  Identifier name of the event
         :type display_name: str
         :param description:  The summary of the event
         :type description: str
-        :param entity:  The entity against which the event originated
-        :type entity: str
         :param application:  The application associated with the event
         :type application: str
-        :param json_schema:  The schema of the event
-        :type json_schema: object
-        :param header_schema:  Header
-        :type header_schema: object
-        :param body_schema:  Body
-        :type body_schema: object
+        :param header_schema:  The header schema for the event type
+        :type header_schema: list[lusid_notification.EventFieldDefinition]
+        :param body_schema:  The body schema for the event type
+        :type body_schema: list[lusid_notification.EventFieldDefinition]
         :param href:  A URI for retrieving this schema
         :type href: str
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._display_name = None
         self._description = None
-        self._entity = None
         self._application = None
-        self._json_schema = None
         self._header_schema = None
         self._body_schema = None
         self._href = None
         self.discriminator = None
 
         self.id = id
         self.display_name = display_name
         self.description = description
-        self.entity = entity
         self.application = application
-        self.json_schema = json_schema
         self.header_schema = header_schema
         self.body_schema = body_schema
         self.href = href
 
     @property
     def id(self):
         """Gets the id of this EventTypeSchema.  # noqa: E501
@@ -188,37 +174,14 @@
         :param description: The description of this EventTypeSchema.  # noqa: E501
         :type description: str
         """
 
         self._description = description
 
     @property
-    def entity(self):
-        """Gets the entity of this EventTypeSchema.  # noqa: E501
-
-        The entity against which the event originated  # noqa: E501
-
-        :return: The entity of this EventTypeSchema.  # noqa: E501
-        :rtype: str
-        """
-        return self._entity
-
-    @entity.setter
-    def entity(self, entity):
-        """Sets the entity of this EventTypeSchema.
-
-        The entity against which the event originated  # noqa: E501
-
-        :param entity: The entity of this EventTypeSchema.  # noqa: E501
-        :type entity: str
-        """
-
-        self._entity = entity
-
-    @property
     def application(self):
         """Gets the application of this EventTypeSchema.  # noqa: E501
 
         The application associated with the event  # noqa: E501
 
         :return: The application of this EventTypeSchema.  # noqa: E501
         :rtype: str
@@ -234,78 +197,55 @@
         :param application: The application of this EventTypeSchema.  # noqa: E501
         :type application: str
         """
 
         self._application = application
 
     @property
-    def json_schema(self):
-        """Gets the json_schema of this EventTypeSchema.  # noqa: E501
-
-        The schema of the event  # noqa: E501
-
-        :return: The json_schema of this EventTypeSchema.  # noqa: E501
-        :rtype: object
-        """
-        return self._json_schema
-
-    @json_schema.setter
-    def json_schema(self, json_schema):
-        """Sets the json_schema of this EventTypeSchema.
-
-        The schema of the event  # noqa: E501
-
-        :param json_schema: The json_schema of this EventTypeSchema.  # noqa: E501
-        :type json_schema: object
-        """
-
-        self._json_schema = json_schema
-
-    @property
     def header_schema(self):
         """Gets the header_schema of this EventTypeSchema.  # noqa: E501
 
-        Header  # noqa: E501
+        The header schema for the event type  # noqa: E501
 
         :return: The header_schema of this EventTypeSchema.  # noqa: E501
-        :rtype: object
+        :rtype: list[lusid_notification.EventFieldDefinition]
         """
         return self._header_schema
 
     @header_schema.setter
     def header_schema(self, header_schema):
         """Sets the header_schema of this EventTypeSchema.
 
-        Header  # noqa: E501
+        The header schema for the event type  # noqa: E501
 
         :param header_schema: The header_schema of this EventTypeSchema.  # noqa: E501
-        :type header_schema: object
+        :type header_schema: list[lusid_notification.EventFieldDefinition]
         """
 
         self._header_schema = header_schema
 
     @property
     def body_schema(self):
         """Gets the body_schema of this EventTypeSchema.  # noqa: E501
 
-        Body  # noqa: E501
+        The body schema for the event type  # noqa: E501
 
         :return: The body_schema of this EventTypeSchema.  # noqa: E501
-        :rtype: object
+        :rtype: list[lusid_notification.EventFieldDefinition]
         """
         return self._body_schema
 
     @body_schema.setter
     def body_schema(self, body_schema):
         """Sets the body_schema of this EventTypeSchema.
 
-        Body  # noqa: E501
+        The body schema for the event type  # noqa: E501
 
         :param body_schema: The body_schema of this EventTypeSchema.  # noqa: E501
-        :type body_schema: object
+        :type body_schema: list[lusid_notification.EventFieldDefinition]
         """
 
         self._body_schema = body_schema
 
     @property
     def href(self):
         """Gets the href of this EventTypeSchema.  # noqa: E501
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/id_selector_definition.py` & `lusid-notification-sdk-preview-0.1.756/lusid_notification/models/id_selector_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-6
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -35,15 +35,15 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
-        'identifier': 'dict[str, str]',
+        'identifier': 'dict(str, str)',
         'actions': 'list[ActionId]',
         'name': 'str',
         'description': 'str'
     }
 
     attribute_map = {
         'identifier': 'identifier',
@@ -59,15 +59,15 @@
         'description': 'optional'
     }
 
     def __init__(self, identifier=None, actions=None, name=None, description=None, local_vars_configuration=None):  # noqa: E501
         """IdSelectorDefinition - a model defined in OpenAPI"
         
         :param identifier:  (required)
-        :type identifier: dict[str, str]
+        :type identifier: dict(str, str)
         :param actions:  (required)
         :type actions: list[lusid_notification.ActionId]
         :param name: 
         :type name: str
         :param description: 
         :type description: str
 
@@ -89,25 +89,25 @@
 
     @property
     def identifier(self):
         """Gets the identifier of this IdSelectorDefinition.  # noqa: E501
 
 
         :return: The identifier of this IdSelectorDefinition.  # noqa: E501
-        :rtype: dict[str, str]
+        :rtype: dict(str, str)
         """
         return self._identifier
 
     @identifier.setter
     def identifier(self, identifier):
         """Sets the identifier of this IdSelectorDefinition.
 
 
         :param identifier: The identifier of this IdSelectorDefinition.  # noqa: E501
-        :type identifier: dict[str, str]
+        :type identifier: dict(str, str)
         """
         if self.local_vars_configuration.client_side_validation and identifier is None:  # noqa: E501
             raise ValueError("Invalid value for `identifier`, must not be `None`")  # noqa: E501
 
         self._identifier = identifier
 
     @property
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/identifier_part_schema.py` & `lusid-notification-sdk-preview-0.1.756/lusid_notification/models/identifier_part_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-6
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/link.py` & `lusid-notification-sdk-preview-0.1.756/lusid_notification/models/link.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-6
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/lusid_problem_details.py` & `lusid-notification-sdk-preview-0.1.756/lusid_notification/models/lusid_problem_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-6
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -36,15 +36,15 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
         'name': 'str',
-        'error_details': 'list[dict[str, str]]',
+        'error_details': 'list[dict(str, str)]',
         'code': 'int',
         'type': 'str',
         'title': 'str',
         'status': 'int',
         'detail': 'str',
         'instance': 'str'
     }
@@ -73,15 +73,15 @@
 
     def __init__(self, name=None, error_details=None, code=None, type=None, title=None, status=None, detail=None, instance=None, local_vars_configuration=None):  # noqa: E501
         """LusidProblemDetails - a model defined in OpenAPI"
         
         :param name:  (required)
         :type name: str
         :param error_details: 
-        :type error_details: list[dict[str, str]]
+        :type error_details: list[dict(str, str)]
         :param code:  (required)
         :type code: int
         :param type: 
         :type type: str
         :param title: 
         :type title: str
         :param status: 
@@ -143,25 +143,25 @@
 
     @property
     def error_details(self):
         """Gets the error_details of this LusidProblemDetails.  # noqa: E501
 
 
         :return: The error_details of this LusidProblemDetails.  # noqa: E501
-        :rtype: list[dict[str, str]]
+        :rtype: list[dict(str, str)]
         """
         return self._error_details
 
     @error_details.setter
     def error_details(self, error_details):
         """Sets the error_details of this LusidProblemDetails.
 
 
         :param error_details: The error_details of this LusidProblemDetails.  # noqa: E501
-        :type error_details: list[dict[str, str]]
+        :type error_details: list[dict(str, str)]
         """
 
         self._error_details = error_details
 
     @property
     def code(self):
         """Gets the code of this LusidProblemDetails.  # noqa: E501
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/lusid_validation_problem_details.py` & `lusid-notification-sdk-preview-0.1.756/lusid_notification/models/lusid_validation_problem_details.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-6
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -36,17 +36,17 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
       required_map (dict): The key is attribute name
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
         'name': 'str',
-        'error_details': 'list[dict[str, str]]',
+        'error_details': 'list[dict(str, str)]',
         'code': 'int',
-        'errors': 'dict[str, list[str]]',
+        'errors': 'dict(str, list[str])',
         'type': 'str',
         'title': 'str',
         'status': 'int',
         'detail': 'str',
         'instance': 'str'
     }
 
@@ -76,19 +76,19 @@
 
     def __init__(self, name=None, error_details=None, code=None, errors=None, type=None, title=None, status=None, detail=None, instance=None, local_vars_configuration=None):  # noqa: E501
         """LusidValidationProblemDetails - a model defined in OpenAPI"
         
         :param name:  (required)
         :type name: str
         :param error_details: 
-        :type error_details: list[dict[str, str]]
+        :type error_details: list[dict(str, str)]
         :param code:  (required)
         :type code: int
         :param errors: 
-        :type errors: dict[str, list[str]]
+        :type errors: dict(str, list[str])
         :param type: 
         :type type: str
         :param title: 
         :type title: str
         :param status: 
         :type status: int
         :param detail: 
@@ -150,25 +150,25 @@
 
     @property
     def error_details(self):
         """Gets the error_details of this LusidValidationProblemDetails.  # noqa: E501
 
 
         :return: The error_details of this LusidValidationProblemDetails.  # noqa: E501
-        :rtype: list[dict[str, str]]
+        :rtype: list[dict(str, str)]
         """
         return self._error_details
 
     @error_details.setter
     def error_details(self, error_details):
         """Sets the error_details of this LusidValidationProblemDetails.
 
 
         :param error_details: The error_details of this LusidValidationProblemDetails.  # noqa: E501
-        :type error_details: list[dict[str, str]]
+        :type error_details: list[dict(str, str)]
         """
 
         self._error_details = error_details
 
     @property
     def code(self):
         """Gets the code of this LusidValidationProblemDetails.  # noqa: E501
@@ -194,25 +194,25 @@
 
     @property
     def errors(self):
         """Gets the errors of this LusidValidationProblemDetails.  # noqa: E501
 
 
         :return: The errors of this LusidValidationProblemDetails.  # noqa: E501
-        :rtype: dict[str, list[str]]
+        :rtype: dict(str, list[str])
         """
         return self._errors
 
     @errors.setter
     def errors(self, errors):
         """Sets the errors of this LusidValidationProblemDetails.
 
 
         :param errors: The errors of this LusidValidationProblemDetails.  # noqa: E501
-        :type errors: dict[str, list[str]]
+        :type errors: dict(str, list[str])
         """
 
         self._errors = errors
 
     @property
     def type(self):
         """Gets the type of this LusidValidationProblemDetails.  # noqa: E501
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/manual_event.py` & `lusid-notification-sdk-preview-0.1.756/lusid_notification/models/manual_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-6
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/manual_event_body.py` & `lusid-notification-sdk-preview-0.1.756/lusid_notification/models/manual_event_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-6
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/manual_event_header.py` & `lusid-notification-sdk-preview-0.1.756/lusid_notification/models/manual_event_header.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-6
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/manual_event_request.py` & `lusid-notification-sdk-preview-0.1.756/lusid_notification/models/manual_event_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-6
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/matching_pattern.py` & `lusid-notification-sdk-preview-0.1.756/lusid_notification/models/matching_pattern.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-6
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/notification.py` & `lusid-notification-sdk-preview-0.1.756/lusid_notification/models/notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-6
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/notification_status.py` & `lusid-notification-sdk-preview-0.1.756/lusid_notification/models/notification_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-6
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/notification_type.py` & `lusid-notification-sdk-preview-0.1.756/lusid_notification/models/notification_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-6
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -52,15 +52,15 @@
         'html_body': 'str',
         'email_address_to': 'list[str]',
         'email_address_cc': 'list[str]',
         'email_address_bcc': 'list[str]',
         'recipients': 'list[str]',
         'url': 'str',
         'authentication_type': 'str',
-        'authentication_configuration_item_paths': 'dict[str, str]',
+        'authentication_configuration_item_paths': 'dict(str, str)',
         'content_type': 'str'
     }
 
     attribute_map = {
         'type': 'type',
         'api_key_ref': 'apiKeyRef',
         'api_secret_ref': 'apiSecretRef',
@@ -100,17 +100,14 @@
         'recipients': 'required',
         'url': 'required',
         'authentication_type': 'required',
         'authentication_configuration_item_paths': 'optional',
         'content_type': 'required'
     }
 
-    discriminator_value_class_map = {
-    }
-
     def __init__(self, type=None, api_key_ref=None, api_secret_ref=None, body=None, queue_url_ref=None, http_method=None, path_and_query=None, content=None, subject=None, plain_text_body=None, html_body=None, email_address_to=None, email_address_cc=None, email_address_bcc=None, recipients=None, url=None, authentication_type=None, authentication_configuration_item_paths=None, content_type=None, local_vars_configuration=None):  # noqa: E501
         """NotificationType - a model defined in OpenAPI"
         
         :param type:  The type of delivery mechanism for this notification
         :type type: str
         :param api_key_ref:  Reference to API key from Configuration Store (required)
         :type api_key_ref: str
@@ -141,15 +138,15 @@
         :param recipients:  The phone numbers to which the SMS will be sent to (E.164 format) (required)
         :type recipients: list[str]
         :param url:  The URL to send the request to (required)
         :type url: str
         :param authentication_type:  The type of authentication to use on the request (required)
         :type authentication_type: str
         :param authentication_configuration_item_paths:  The paths of the Configuration Store configuration items that contain the authentication configuration. Each  authentication type requires different keys:  - Lusid - None required  - BasicAuth - Requires 'Username' and 'Password'  - BearerToken - Requires 'BearerToken' and optionally 'BearerScheme'                e.g. the following would be valid assuming that the config is present in the configuration store at the  specified paths:                    \"authenticationType\": \"BasicAuth\",      \"authenticationConfigurationItemPaths\": {          \"Username\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminUser\",          \"Password\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminPassword\"      }
-        :type authentication_configuration_item_paths: dict[str, str]
+        :type authentication_configuration_item_paths: dict(str, str)
         :param content_type:  The type of the content e.g. Json (required)
         :type content_type: str
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
@@ -169,15 +166,15 @@
         self._email_address_cc = None
         self._email_address_bcc = None
         self._recipients = None
         self._url = None
         self._authentication_type = None
         self._authentication_configuration_item_paths = None
         self._content_type = None
-        self.discriminator = 'type'
+        self.discriminator = None
 
         self.type = type
         self.api_key_ref = api_key_ref
         self.api_secret_ref = api_secret_ref
         self.body = body
         self.queue_url_ref = queue_url_ref
         self.http_method = http_method
@@ -700,26 +697,26 @@
     @property
     def authentication_configuration_item_paths(self):
         """Gets the authentication_configuration_item_paths of this NotificationType.  # noqa: E501
 
         The paths of the Configuration Store configuration items that contain the authentication configuration. Each  authentication type requires different keys:  - Lusid - None required  - BasicAuth - Requires 'Username' and 'Password'  - BearerToken - Requires 'BearerToken' and optionally 'BearerScheme'                e.g. the following would be valid assuming that the config is present in the configuration store at the  specified paths:                    \"authenticationType\": \"BasicAuth\",      \"authenticationConfigurationItemPaths\": {          \"Username\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminUser\",          \"Password\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminPassword\"      }  # noqa: E501
 
         :return: The authentication_configuration_item_paths of this NotificationType.  # noqa: E501
-        :rtype: dict[str, str]
+        :rtype: dict(str, str)
         """
         return self._authentication_configuration_item_paths
 
     @authentication_configuration_item_paths.setter
     def authentication_configuration_item_paths(self, authentication_configuration_item_paths):
         """Sets the authentication_configuration_item_paths of this NotificationType.
 
         The paths of the Configuration Store configuration items that contain the authentication configuration. Each  authentication type requires different keys:  - Lusid - None required  - BasicAuth - Requires 'Username' and 'Password'  - BearerToken - Requires 'BearerToken' and optionally 'BearerScheme'                e.g. the following would be valid assuming that the config is present in the configuration store at the  specified paths:                    \"authenticationType\": \"BasicAuth\",      \"authenticationConfigurationItemPaths\": {          \"Username\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminUser\",          \"Password\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminPassword\"      }  # noqa: E501
 
         :param authentication_configuration_item_paths: The authentication_configuration_item_paths of this NotificationType.  # noqa: E501
-        :type authentication_configuration_item_paths: dict[str, str]
+        :type authentication_configuration_item_paths: dict(str, str)
         """
 
         self._authentication_configuration_item_paths = authentication_configuration_item_paths
 
     @property
     def content_type(self):
         """Gets the content_type of this NotificationType.  # noqa: E501
@@ -744,20 +741,14 @@
             raise ValueError("Invalid value for `content_type`, must not be `None`")  # noqa: E501
         if (self.local_vars_configuration.client_side_validation and
                 content_type is not None and len(content_type) < 1):
             raise ValueError("Invalid value for `content_type`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._content_type = content_type
 
-    def get_real_child_model(self, data):
-        """Returns the real base class specified by the discriminator"""
-        discriminator_key = self.attribute_map[self.discriminator]
-        discriminator_value = data[discriminator_key]
-        return self.discriminator_value_class_map.get(discriminator_value)
-
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
                 args = getfullargspec(x.to_dict).args
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/resource_id.py` & `lusid-notification-sdk-preview-0.1.756/lusid_notification/models/resource_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-6
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/resource_list_of_access_controlled_resource.py` & `lusid-notification-sdk-preview-0.1.756/lusid_notification/models/resource_list_of_access_controlled_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-6
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/resource_list_of_event_type_schema.py` & `lusid-notification-sdk-preview-0.1.756/lusid_notification/models/resource_list_of_event_type_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-6
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/resource_list_of_notification.py` & `lusid-notification-sdk-preview-0.1.756/lusid_notification/models/resource_list_of_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-6
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/resource_list_of_subscription.py` & `lusid-notification-sdk-preview-0.1.756/lusid_notification/models/resource_list_of_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-6
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/sms_notification_type.py` & `lusid-notification-sdk-preview-0.1.756/lusid_notification/models/sms_notification_type.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-6
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -55,15 +55,15 @@
         'body': 'required',
         'recipients': 'required'
     }
 
     def __init__(self, type=None, body=None, recipients=None, local_vars_configuration=None):  # noqa: E501
         """SmsNotificationType - a model defined in OpenAPI"
         
-        :param type:  (required)
+        :param type:  The type of delivery mechanism for this notification (required)
         :type type: str
         :param body:  The body of the SMS (required)
         :type body: str
         :param recipients:  The phone numbers to which the SMS will be sent to (E.164 format) (required)
         :type recipients: list[str]
 
         """  # noqa: E501
@@ -80,33 +80,38 @@
         self.body = body
         self.recipients = recipients
 
     @property
     def type(self):
         """Gets the type of this SmsNotificationType.  # noqa: E501
 
+        The type of delivery mechanism for this notification  # noqa: E501
 
         :return: The type of this SmsNotificationType.  # noqa: E501
         :rtype: str
         """
         return self._type
 
     @type.setter
     def type(self, type):
         """Sets the type of this SmsNotificationType.
 
+        The type of delivery mechanism for this notification  # noqa: E501
 
         :param type: The type of this SmsNotificationType.  # noqa: E501
         :type type: str
         """
         if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
             raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                type is not None and len(type) < 1):
-            raise ValueError("Invalid value for `type`, length must be greater than or equal to `1`")  # noqa: E501
+        allowed_values = ["Sms"]  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and type not in allowed_values:  # noqa: E501
+            raise ValueError(
+                "Invalid value for `type` ({0}), must be one of {1}"  # noqa: E501
+                .format(type, allowed_values)
+            )
 
         self._type = type
 
     @property
     def body(self):
         """Gets the body of this SmsNotificationType.  # noqa: E501
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/subscription.py` & `lusid-notification-sdk-preview-0.1.756/lusid_notification/models/subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-6
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/update_notification_request.py` & `lusid-notification-sdk-preview-0.1.756/lusid_notification/models/update_notification_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-6
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/update_subscription.py` & `lusid-notification-sdk-preview-0.1.756/lusid_notification/models/update_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-6
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/models/webhook_notification_type.py` & `lusid-notification-sdk-preview-0.1.756/lusid_notification/models/webhook_notification_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-6
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -39,15 +39,15 @@
                            and the value is whether it is 'required' or 'optional'.
     """
     openapi_types = {
         'type': 'str',
         'http_method': 'str',
         'url': 'str',
         'authentication_type': 'str',
-        'authentication_configuration_item_paths': 'dict[str, str]',
+        'authentication_configuration_item_paths': 'dict(str, str)',
         'content_type': 'str',
         'content': 'object'
     }
 
     attribute_map = {
         'type': 'type',
         'http_method': 'httpMethod',
@@ -67,24 +67,24 @@
         'content_type': 'required',
         'content': 'optional'
     }
 
     def __init__(self, type=None, http_method=None, url=None, authentication_type=None, authentication_configuration_item_paths=None, content_type=None, content=None, local_vars_configuration=None):  # noqa: E501
         """WebhookNotificationType - a model defined in OpenAPI"
         
-        :param type:  (required)
+        :param type:  The type of delivery mechanism for this notification (required)
         :type type: str
         :param http_method:  The HTTP method such as GET, POST, etc. to use on the request (required)
         :type http_method: str
         :param url:  The URL to send the request to (required)
         :type url: str
         :param authentication_type:  The type of authentication to use on the request (required)
         :type authentication_type: str
         :param authentication_configuration_item_paths:  The paths of the Configuration Store configuration items that contain the authentication configuration. Each  authentication type requires different keys:  - Lusid - None required  - BasicAuth - Requires 'Username' and 'Password'  - BearerToken - Requires 'BearerToken' and optionally 'BearerScheme'                e.g. the following would be valid assuming that the config is present in the configuration store at the  specified paths:                    \"authenticationType\": \"BasicAuth\",      \"authenticationConfigurationItemPaths\": {          \"Username\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminUser\",          \"Password\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminPassword\"      }
-        :type authentication_configuration_item_paths: dict[str, str]
+        :type authentication_configuration_item_paths: dict(str, str)
         :param content_type:  The type of the content e.g. Json (required)
         :type content_type: str
         :param content:  The content of the request
         :type content: object
 
         """  # noqa: E501
         if local_vars_configuration is None:
@@ -108,33 +108,38 @@
         self.content_type = content_type
         self.content = content
 
     @property
     def type(self):
         """Gets the type of this WebhookNotificationType.  # noqa: E501
 
+        The type of delivery mechanism for this notification  # noqa: E501
 
         :return: The type of this WebhookNotificationType.  # noqa: E501
         :rtype: str
         """
         return self._type
 
     @type.setter
     def type(self, type):
         """Sets the type of this WebhookNotificationType.
 
+        The type of delivery mechanism for this notification  # noqa: E501
 
         :param type: The type of this WebhookNotificationType.  # noqa: E501
         :type type: str
         """
         if self.local_vars_configuration.client_side_validation and type is None:  # noqa: E501
             raise ValueError("Invalid value for `type`, must not be `None`")  # noqa: E501
-        if (self.local_vars_configuration.client_side_validation and
-                type is not None and len(type) < 1):
-            raise ValueError("Invalid value for `type`, length must be greater than or equal to `1`")  # noqa: E501
+        allowed_values = ["Webhook"]  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and type not in allowed_values:  # noqa: E501
+            raise ValueError(
+                "Invalid value for `type` ({0}), must be one of {1}"  # noqa: E501
+                .format(type, allowed_values)
+            )
 
         self._type = type
 
     @property
     def http_method(self):
         """Gets the http_method of this WebhookNotificationType.  # noqa: E501
 
@@ -227,26 +232,26 @@
     @property
     def authentication_configuration_item_paths(self):
         """Gets the authentication_configuration_item_paths of this WebhookNotificationType.  # noqa: E501
 
         The paths of the Configuration Store configuration items that contain the authentication configuration. Each  authentication type requires different keys:  - Lusid - None required  - BasicAuth - Requires 'Username' and 'Password'  - BearerToken - Requires 'BearerToken' and optionally 'BearerScheme'                e.g. the following would be valid assuming that the config is present in the configuration store at the  specified paths:                    \"authenticationType\": \"BasicAuth\",      \"authenticationConfigurationItemPaths\": {          \"Username\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminUser\",          \"Password\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminPassword\"      }  # noqa: E501
 
         :return: The authentication_configuration_item_paths of this WebhookNotificationType.  # noqa: E501
-        :rtype: dict[str, str]
+        :rtype: dict(str, str)
         """
         return self._authentication_configuration_item_paths
 
     @authentication_configuration_item_paths.setter
     def authentication_configuration_item_paths(self, authentication_configuration_item_paths):
         """Sets the authentication_configuration_item_paths of this WebhookNotificationType.
 
         The paths of the Configuration Store configuration items that contain the authentication configuration. Each  authentication type requires different keys:  - Lusid - None required  - BasicAuth - Requires 'Username' and 'Password'  - BearerToken - Requires 'BearerToken' and optionally 'BearerScheme'                e.g. the following would be valid assuming that the config is present in the configuration store at the  specified paths:                    \"authenticationType\": \"BasicAuth\",      \"authenticationConfigurationItemPaths\": {          \"Username\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminUser\",          \"Password\": \"config://personal/myUserId/WebhookConfigurations/ExampleService/AdminPassword\"      }  # noqa: E501
 
         :param authentication_configuration_item_paths: The authentication_configuration_item_paths of this WebhookNotificationType.  # noqa: E501
-        :type authentication_configuration_item_paths: dict[str, str]
+        :type authentication_configuration_item_paths: dict(str, str)
         """
 
         self._authentication_configuration_item_paths = authentication_configuration_item_paths
 
     @property
     def content_type(self):
         """Gets the content_type of this WebhookNotificationType.  # noqa: E501
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/rest.py` & `lusid-notification-sdk-preview-0.1.756/lusid_notification/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748-6
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification/utilities/config_keys.json` & `lusid-notification-sdk-preview-0.1.756/lusid_notification/utilities/config_keys.json`

 * *Files identical despite different names*

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/lusid_notification_sdk_preview.egg-info/SOURCES.txt` & `lusid-notification-sdk-preview-0.1.756/lusid_notification_sdk_preview.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 lusid_notification/models/access_controlled_resource.py
 lusid_notification/models/action_id.py
 lusid_notification/models/amazon_sqs_notification_type.py
 lusid_notification/models/api_request_notification_type.py
 lusid_notification/models/create_notification_request.py
 lusid_notification/models/create_subscription.py
 lusid_notification/models/email_notification_type.py
+lusid_notification/models/event_field_definition.py
 lusid_notification/models/event_type_schema.py
 lusid_notification/models/id_selector_definition.py
 lusid_notification/models/identifier_part_schema.py
 lusid_notification/models/link.py
 lusid_notification/models/lusid_problem_details.py
 lusid_notification/models/lusid_validation_problem_details.py
 lusid_notification/models/manual_event.py
```

### Comparing `lusid-notification-sdk-preview-0.1.748.post6/setup.py` & `lusid-notification-sdk-preview-0.1.756/setup.py`

 * *Files identical despite different names*


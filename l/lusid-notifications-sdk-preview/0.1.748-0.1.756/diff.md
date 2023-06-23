# Comparing `tmp/lusid-notifications-sdk-preview-0.1.748.tar.gz` & `tmp/lusid-notifications-sdk-preview-0.1.756.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lusid-notifications-sdk-preview-0.1.748.tar", last modified: Fri Jun 16 11:26:26 2023, max compression
+gzip compressed data, was "dist/lusid-notifications-sdk-preview-0.1.756.tar", last modified: Fri Jun 23 11:47:54 2023, max compression
```

## Comparing `lusid-notifications-sdk-preview-0.1.748.tar` & `lusid-notifications-sdk-preview-0.1.756.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:26:26.000000 lusid-notifications-sdk-preview-0.1.748/
--rw-r--r--   0 root         (0) root         (0)       54 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      373 2023-06-16 11:26:26.000000 lusid-notifications-sdk-preview-0.1.748/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9590 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:26:26.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/
--rw-r--r--   0 root         (0) root         (0)     4349 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/__init__.py
--rw-r--r--   0 root         (0) root         (0)       24 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:26:26.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/api/
--rw-r--r--   0 root         (0) root         (0)      501 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6851 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/api/application_metadata_api.py
--rw-r--r--   0 root         (0) root         (0)    10524 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/api/deliveries_api.py
--rw-r--r--   0 root         (0) root         (0)    13990 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/api/event_types_api.py
--rw-r--r--   0 root         (0) root         (0)     6975 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/api/events_api.py
--rw-r--r--   0 root         (0) root         (0)   122660 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/api/notifications_api.py
--rw-r--r--   0 root         (0) root         (0)    47811 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/api/subscriptions_api.py
--rw-r--r--   0 root         (0) root         (0)    27436 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/api_client.py
--rw-r--r--   0 root         (0) root         (0)    16635 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5099 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:26:26.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/
--rw-r--r--   0 root         (0) root         (0)     2995 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7264 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/access_controlled_action.py
--rw-r--r--   0 root         (0) root         (0)     9027 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7232 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/action_id.py
--rw-r--r--   0 root         (0) root         (0)     6512 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/attempt.py
--rw-r--r--   0 root         (0) root         (0)     5557 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/attempt_status.py
--rw-r--r--   0 root         (0) root         (0)    11703 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/create_aws_sqs_notification.py
--rw-r--r--   0 root         (0) root         (0)    16290 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/create_email_notification.py
--rw-r--r--   0 root         (0) root         (0)     8814 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/create_sms_notification.py
--rw-r--r--   0 root         (0) root         (0)    12632 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/create_subscription.py
--rw-r--r--   0 root         (0) root         (0)    16161 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/create_webhook_notification.py
--rw-r--r--   0 root         (0) root         (0)    12397 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/delivery.py
--rw-r--r--   0 root         (0) root         (0)     4091 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/event_details.py
--rw-r--r--   0 root         (0) root         (0)    10287 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/event_type_schema.py
--rw-r--r--   0 root         (0) root         (0)     8025 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/id_selector_definition.py
--rw-r--r--   0 root         (0) root         (0)     9514 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/identifier_part_schema.py
--rw-r--r--   0 root         (0) root         (0)     6426 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/link.py
--rw-r--r--   0 root         (0) root         (0)     9540 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/lusid_problem_details.py
--rw-r--r--   0 root         (0) root         (0)    10705 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/lusid_validation_problem_details.py
--rw-r--r--   0 root         (0) root         (0)     7437 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/matching_pattern.py
--rw-r--r--   0 root         (0) root         (0)    18059 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/notification.py
--rw-r--r--   0 root         (0) root         (0)     5155 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/notification_status.py
--rw-r--r--   0 root         (0) root         (0)     6099 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/resource_id.py
--rw-r--r--   0 root         (0) root         (0)     7775 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7327 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/resource_list_of_delivery.py
--rw-r--r--   0 root         (0) root         (0)     7523 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/resource_list_of_event_type_schema.py
--rw-r--r--   0 root         (0) root         (0)     7439 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/resource_list_of_notification.py
--rw-r--r--   0 root         (0) root         (0)     7439 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/resource_list_of_subscription.py
--rw-r--r--   0 root         (0) root         (0)    16992 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/subscription.py
--rw-r--r--   0 root         (0) root         (0)    11703 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/update_aws_sqs_notification.py
--rw-r--r--   0 root         (0) root         (0)    16290 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/update_email_notification.py
--rw-r--r--   0 root         (0) root         (0)     8814 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/update_sms_notification.py
--rw-r--r--   0 root         (0) root         (0)    11767 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/update_subscription.py
--rw-r--r--   0 root         (0) root         (0)    16161 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/update_webhook_notification.py
--rw-r--r--   0 root         (0) root         (0)    13561 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:26:26.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/utilities/
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1042 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/utilities/config_keys.json
--rw-r--r--   0 root         (0) root         (0)      295 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications/utilities/config_keys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 11:26:26.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications_sdk_preview.egg-info/
--rw-r--r--   0 root         (0) root         (0)      373 2023-06-16 11:26:26.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications_sdk_preview.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2692 2023-06-16 11:26:26.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications_sdk_preview.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 11:26:26.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications_sdk_preview.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      116 2023-06-16 11:26:26.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications_sdk_preview.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-06-16 11:26:26.000000 lusid-notifications-sdk-preview-0.1.748/lusid_notifications_sdk_preview.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-16 11:26:26.000000 lusid-notifications-sdk-preview-0.1.748/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2322 2023-06-16 11:25:37.000000 lusid-notifications-sdk-preview-0.1.748/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:47:54.000000 lusid-notifications-sdk-preview-0.1.756/
+-rw-r--r--   0 root         (0) root         (0)       54 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      373 2023-06-23 11:47:54.000000 lusid-notifications-sdk-preview-0.1.756/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9646 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:47:54.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/
+-rw-r--r--   0 root         (0) root         (0)     4432 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       24 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:47:54.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/api/
+-rw-r--r--   0 root         (0) root         (0)      501 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6851 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/api/application_metadata_api.py
+-rw-r--r--   0 root         (0) root         (0)    10524 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/api/deliveries_api.py
+-rw-r--r--   0 root         (0) root         (0)    13990 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/api/event_types_api.py
+-rw-r--r--   0 root         (0) root         (0)     6975 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/api/events_api.py
+-rw-r--r--   0 root         (0) root         (0)   122660 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/api/notifications_api.py
+-rw-r--r--   0 root         (0) root         (0)    47811 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/api/subscriptions_api.py
+-rw-r--r--   0 root         (0) root         (0)    27436 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    16635 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5099 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:47:54.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/
+-rw-r--r--   0 root         (0) root         (0)     3078 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7264 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/access_controlled_action.py
+-rw-r--r--   0 root         (0) root         (0)     9027 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7232 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/action_id.py
+-rw-r--r--   0 root         (0) root         (0)     6512 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/attempt.py
+-rw-r--r--   0 root         (0) root         (0)     5557 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/attempt_status.py
+-rw-r--r--   0 root         (0) root         (0)    11703 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/create_aws_sqs_notification.py
+-rw-r--r--   0 root         (0) root         (0)    16290 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/create_email_notification.py
+-rw-r--r--   0 root         (0) root         (0)     8814 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/create_sms_notification.py
+-rw-r--r--   0 root         (0) root         (0)    12632 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/create_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    16161 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/create_webhook_notification.py
+-rw-r--r--   0 root         (0) root         (0)    12397 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/delivery.py
+-rw-r--r--   0 root         (0) root         (0)     4091 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/event_details.py
+-rw-r--r--   0 root         (0) root         (0)     4727 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/event_field_definition.py
+-rw-r--r--   0 root         (0) root         (0)    10747 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/event_type_schema.py
+-rw-r--r--   0 root         (0) root         (0)     8025 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/id_selector_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9514 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/identifier_part_schema.py
+-rw-r--r--   0 root         (0) root         (0)     6426 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/link.py
+-rw-r--r--   0 root         (0) root         (0)     9540 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/lusid_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)    10705 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/lusid_validation_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)     7437 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/matching_pattern.py
+-rw-r--r--   0 root         (0) root         (0)    18059 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/notification.py
+-rw-r--r--   0 root         (0) root         (0)     5155 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/notification_status.py
+-rw-r--r--   0 root         (0) root         (0)     6099 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/resource_id.py
+-rw-r--r--   0 root         (0) root         (0)     7775 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7327 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/resource_list_of_delivery.py
+-rw-r--r--   0 root         (0) root         (0)     7523 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/resource_list_of_event_type_schema.py
+-rw-r--r--   0 root         (0) root         (0)     7439 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/resource_list_of_notification.py
+-rw-r--r--   0 root         (0) root         (0)     7439 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/resource_list_of_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    16992 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/subscription.py
+-rw-r--r--   0 root         (0) root         (0)    11703 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/update_aws_sqs_notification.py
+-rw-r--r--   0 root         (0) root         (0)    16290 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/update_email_notification.py
+-rw-r--r--   0 root         (0) root         (0)     8814 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/update_sms_notification.py
+-rw-r--r--   0 root         (0) root         (0)    11767 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/update_subscription.py
+-rw-r--r--   0 root         (0) root         (0)    16161 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/update_webhook_notification.py
+-rw-r--r--   0 root         (0) root         (0)    13561 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:47:54.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/utilities/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/utilities/config_keys.json
+-rw-r--r--   0 root         (0) root         (0)      295 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications/utilities/config_keys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:47:54.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications_sdk_preview.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      373 2023-06-23 11:47:54.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications_sdk_preview.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2745 2023-06-23 11:47:54.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications_sdk_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 11:47:54.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications_sdk_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      116 2023-06-23 11:47:54.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications_sdk_preview.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-23 11:47:54.000000 lusid-notifications-sdk-preview-0.1.756/lusid_notifications_sdk_preview.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 11:47:54.000000 lusid-notifications-sdk-preview-0.1.756/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2322 2023-06-23 11:45:07.000000 lusid-notifications-sdk-preview-0.1.756/setup.py
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/README.md` & `lusid-notifications-sdk-preview-0.1.756/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-notifications-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.748
-- Package version: 0.1.748
+- API version: 0.1.756
+- Package version: 0.1.756
 - Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
@@ -124,14 +124,15 @@
  - [CreateAwsSqsNotification](docs/CreateAwsSqsNotification.md)
  - [CreateEmailNotification](docs/CreateEmailNotification.md)
  - [CreateSmsNotification](docs/CreateSmsNotification.md)
  - [CreateSubscription](docs/CreateSubscription.md)
  - [CreateWebhookNotification](docs/CreateWebhookNotification.md)
  - [Delivery](docs/Delivery.md)
  - [EventDetails](docs/EventDetails.md)
+ - [EventFieldDefinition](docs/EventFieldDefinition.md)
  - [EventTypeSchema](docs/EventTypeSchema.md)
  - [IdSelectorDefinition](docs/IdSelectorDefinition.md)
  - [IdentifierPartSchema](docs/IdentifierPartSchema.md)
  - [Link](docs/Link.md)
  - [LusidProblemDetails](docs/LusidProblemDetails.md)
  - [LusidValidationProblemDetails](docs/LusidValidationProblemDetails.md)
  - [MatchingPattern](docs/MatchingPattern.md)
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/__init__.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.1.748"
+__version__ = "0.1.756"
 
 # import apis into sdk package
 from lusid_notifications.api.application_metadata_api import ApplicationMetadataApi
 from lusid_notifications.api.deliveries_api import DeliveriesApi
 from lusid_notifications.api.event_types_api import EventTypesApi
 from lusid_notifications.api.events_api import EventsApi
 from lusid_notifications.api.notifications_api import NotificationsApi
@@ -42,14 +42,15 @@
 from lusid_notifications.models.create_aws_sqs_notification import CreateAwsSqsNotification
 from lusid_notifications.models.create_email_notification import CreateEmailNotification
 from lusid_notifications.models.create_sms_notification import CreateSmsNotification
 from lusid_notifications.models.create_subscription import CreateSubscription
 from lusid_notifications.models.create_webhook_notification import CreateWebhookNotification
 from lusid_notifications.models.delivery import Delivery
 from lusid_notifications.models.event_details import EventDetails
+from lusid_notifications.models.event_field_definition import EventFieldDefinition
 from lusid_notifications.models.event_type_schema import EventTypeSchema
 from lusid_notifications.models.id_selector_definition import IdSelectorDefinition
 from lusid_notifications.models.identifier_part_schema import IdentifierPartSchema
 from lusid_notifications.models.link import Link
 from lusid_notifications.models.lusid_problem_details import LusidProblemDetails
 from lusid_notifications.models.lusid_validation_problem_details import LusidValidationProblemDetails
 from lusid_notifications.models.matching_pattern import MatchingPattern
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/api/application_metadata_api.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/api/application_metadata_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
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
-        header_params['X-LUSID-SDK-Version'] = '0.1.748'
+        header_params['X-LUSID-SDK-Version'] = '0.1.756'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfAccessControlledResource",
         }
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/api/deliveries_api.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/api/deliveries_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -179,15 +179,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.748'
+        header_params['X-LUSID-SDK-Version'] = '0.1.756'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfDelivery",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/api/event_types_api.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/api/event_types_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
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
-        header_params['X-LUSID-SDK-Version'] = '0.1.748'
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
-        header_params['X-LUSID-SDK-Version'] = '0.1.748'
+        header_params['X-LUSID-SDK-Version'] = '0.1.756'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfEventTypeSchema",
             404: "str",
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/api/events_api.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/api/events_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -150,15 +150,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.748'
+        header_params['X-LUSID-SDK-Version'] = '0.1.756'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "EventDetails",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/api/notifications_api.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/api/notifications_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -201,15 +201,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.748'
+        header_params['X-LUSID-SDK-Version'] = '0.1.756'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Notification",
             400: "LusidValidationProblemDetails",
@@ -384,15 +384,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.748'
+        header_params['X-LUSID-SDK-Version'] = '0.1.756'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Notification",
             400: "LusidValidationProblemDetails",
@@ -567,15 +567,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.748'
+        header_params['X-LUSID-SDK-Version'] = '0.1.756'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Notification",
             400: "LusidValidationProblemDetails",
@@ -750,15 +750,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.748'
+        header_params['X-LUSID-SDK-Version'] = '0.1.756'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Notification",
             400: "LusidValidationProblemDetails",
@@ -930,15 +930,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.748'
+        header_params['X-LUSID-SDK-Version'] = '0.1.756'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
@@ -1107,15 +1107,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.748'
+        header_params['X-LUSID-SDK-Version'] = '0.1.756'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
@@ -1277,15 +1277,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.748'
+        header_params['X-LUSID-SDK-Version'] = '0.1.756'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfNotification",
             400: "LusidValidationProblemDetails",
@@ -1480,15 +1480,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.748'
+        header_params['X-LUSID-SDK-Version'] = '0.1.756'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
@@ -1683,15 +1683,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.748'
+        header_params['X-LUSID-SDK-Version'] = '0.1.756'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
@@ -1886,15 +1886,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.748'
+        header_params['X-LUSID-SDK-Version'] = '0.1.756'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
@@ -2089,15 +2089,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.748'
+        header_params['X-LUSID-SDK-Version'] = '0.1.756'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Notification",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/api/subscriptions_api.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/api/subscriptions_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
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
-        header_params['X-LUSID-SDK-Version'] = '0.1.748'
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
-        header_params['X-LUSID-SDK-Version'] = '0.1.748'
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
-        header_params['X-LUSID-SDK-Version'] = '0.1.748'
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
-        header_params['X-LUSID-SDK-Version'] = '0.1.748'
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
-        header_params['X-LUSID-SDK-Version'] = '0.1.748'
+        header_params['X-LUSID-SDK-Version'] = '0.1.756'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Subscription",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/api_client.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
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
-        self.user_agent = 'OpenAPI-Generator/0.1.748/python'
+        self.user_agent = 'OpenAPI-Generator/0.1.756/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/configuration.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -392,16 +392,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.1.748\n"\
-               "SDK Package Version: 0.1.748".\
+               "Version of the API: 0.1.756\n"\
+               "SDK Package Version: 0.1.756".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/exceptions.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/__init__.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -23,14 +23,15 @@
 from lusid_notifications.models.create_aws_sqs_notification import CreateAwsSqsNotification
 from lusid_notifications.models.create_email_notification import CreateEmailNotification
 from lusid_notifications.models.create_sms_notification import CreateSmsNotification
 from lusid_notifications.models.create_subscription import CreateSubscription
 from lusid_notifications.models.create_webhook_notification import CreateWebhookNotification
 from lusid_notifications.models.delivery import Delivery
 from lusid_notifications.models.event_details import EventDetails
+from lusid_notifications.models.event_field_definition import EventFieldDefinition
 from lusid_notifications.models.event_type_schema import EventTypeSchema
 from lusid_notifications.models.id_selector_definition import IdSelectorDefinition
 from lusid_notifications.models.identifier_part_schema import IdentifierPartSchema
 from lusid_notifications.models.link import Link
 from lusid_notifications.models.lusid_problem_details import LusidProblemDetails
 from lusid_notifications.models.lusid_validation_problem_details import LusidValidationProblemDetails
 from lusid_notifications.models.matching_pattern import MatchingPattern
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/access_controlled_action.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/access_controlled_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/access_controlled_resource.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/access_controlled_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/action_id.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/action_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/attempt.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/attempt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/attempt_status.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/attempt_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/create_aws_sqs_notification.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/create_aws_sqs_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/create_email_notification.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/create_email_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/create_sms_notification.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/create_sms_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/create_subscription.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/create_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/create_webhook_notification.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/create_webhook_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/delivery.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/delivery.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/event_details.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/event_details.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/event_type_schema.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/event_type_schema.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
@@ -41,16 +41,16 @@
     openapi_types = {
         'id': 'str',
         'event_name': 'str',
         'description': 'str',
         'entity': 'str',
         'application': 'str',
         'json_schema': 'object',
-        'header_schema': 'object',
-        'body_schema': 'object'
+        'header_schema': 'list[EventFieldDefinition]',
+        'body_schema': 'list[EventFieldDefinition]'
     }
 
     attribute_map = {
         'id': 'id',
         'event_name': 'eventName',
         'description': 'description',
         'entity': 'entity',
@@ -82,18 +82,18 @@
         :type description: str
         :param entity:  The entity against which the event originated
         :type entity: str
         :param application:  The application associated with the event
         :type application: str
         :param json_schema:  The schema of the event
         :type json_schema: object
-        :param header_schema:  Header
-        :type header_schema: object
-        :param body_schema:  Body
-        :type body_schema: object
+        :param header_schema:  The header schema for the event type
+        :type header_schema: list[lusid_notifications.EventFieldDefinition]
+        :param body_schema:  The body schema for the event type
+        :type body_schema: list[lusid_notifications.EventFieldDefinition]
 
         """  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
@@ -253,52 +253,52 @@
 
         self._json_schema = json_schema
 
     @property
     def header_schema(self):
         """Gets the header_schema of this EventTypeSchema.  # noqa: E501
 
-        Header  # noqa: E501
+        The header schema for the event type  # noqa: E501
 
         :return: The header_schema of this EventTypeSchema.  # noqa: E501
-        :rtype: object
+        :rtype: list[lusid_notifications.EventFieldDefinition]
         """
         return self._header_schema
 
     @header_schema.setter
     def header_schema(self, header_schema):
         """Sets the header_schema of this EventTypeSchema.
 
-        Header  # noqa: E501
+        The header schema for the event type  # noqa: E501
 
         :param header_schema: The header_schema of this EventTypeSchema.  # noqa: E501
-        :type header_schema: object
+        :type header_schema: list[lusid_notifications.EventFieldDefinition]
         """
 
         self._header_schema = header_schema
 
     @property
     def body_schema(self):
         """Gets the body_schema of this EventTypeSchema.  # noqa: E501
 
-        Body  # noqa: E501
+        The body schema for the event type  # noqa: E501
 
         :return: The body_schema of this EventTypeSchema.  # noqa: E501
-        :rtype: object
+        :rtype: list[lusid_notifications.EventFieldDefinition]
         """
         return self._body_schema
 
     @body_schema.setter
     def body_schema(self, body_schema):
         """Sets the body_schema of this EventTypeSchema.
 
-        Body  # noqa: E501
+        The body schema for the event type  # noqa: E501
 
         :param body_schema: The body_schema of this EventTypeSchema.  # noqa: E501
-        :type body_schema: object
+        :type body_schema: list[lusid_notifications.EventFieldDefinition]
         """
 
         self._body_schema = body_schema
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/id_selector_definition.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/id_selector_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/identifier_part_schema.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/identifier_part_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/link.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/link.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/lusid_problem_details.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/lusid_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/lusid_validation_problem_details.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/lusid_validation_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/matching_pattern.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/matching_pattern.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/notification.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/notification.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/notification_status.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/notification_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/resource_id.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/resource_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/resource_list_of_access_controlled_resource.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/resource_list_of_access_controlled_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/resource_list_of_delivery.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/resource_list_of_delivery.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/resource_list_of_event_type_schema.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/resource_list_of_event_type_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/resource_list_of_notification.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/resource_list_of_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/resource_list_of_subscription.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/resource_list_of_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/subscription.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/update_aws_sqs_notification.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/update_aws_sqs_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/update_email_notification.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/update_email_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/update_sms_notification.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/update_sms_notification.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/update_subscription.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/update_subscription.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/models/update_webhook_notification.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/models/update_webhook_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/rest.py` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Notifications API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.748
+    The version of the OpenAPI document: 0.1.756
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications/utilities/config_keys.json` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications/utilities/config_keys.json`

 * *Files identical despite different names*

### Comparing `lusid-notifications-sdk-preview-0.1.748/lusid_notifications_sdk_preview.egg-info/SOURCES.txt` & `lusid-notifications-sdk-preview-0.1.756/lusid_notifications_sdk_preview.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 lusid_notifications/models/create_aws_sqs_notification.py
 lusid_notifications/models/create_email_notification.py
 lusid_notifications/models/create_sms_notification.py
 lusid_notifications/models/create_subscription.py
 lusid_notifications/models/create_webhook_notification.py
 lusid_notifications/models/delivery.py
 lusid_notifications/models/event_details.py
+lusid_notifications/models/event_field_definition.py
 lusid_notifications/models/event_type_schema.py
 lusid_notifications/models/id_selector_definition.py
 lusid_notifications/models/identifier_part_schema.py
 lusid_notifications/models/link.py
 lusid_notifications/models/lusid_problem_details.py
 lusid_notifications/models/lusid_validation_problem_details.py
 lusid_notifications/models/matching_pattern.py
```

### Comparing `lusid-notifications-sdk-preview-0.1.748/setup.py` & `lusid-notifications-sdk-preview-0.1.756/setup.py`

 * *Files identical despite different names*


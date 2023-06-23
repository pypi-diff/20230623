# Comparing `tmp/keycloak-admin-aio-1.3.1.tar.gz` & `tmp/keycloak_admin_aio-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keycloak-admin-aio-1.3.1.tar", last modified: Fri Mar 17 19:14:29 2023, max compression
+gzip compressed data, was "keycloak_admin_aio-1.3.3.tar", max compression
```

## Comparing `keycloak-admin-aio-1.3.1.tar` & `keycloak_admin_aio-1.3.3.tar`

### file list

```diff
@@ -1,84 +1,83 @@
--rw-r--r--   0        0        0    11357 2023-03-17 19:14:13.165345 keycloak-admin-aio-1.3.1/LICENSE
--rw-r--r--   0        0        0     2124 2023-03-17 19:14:13.165345 keycloak-admin-aio-1.3.1/README.rst
--rw-r--r--   0        0        0      169 2023-03-17 19:14:13.165345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/__init__.py
--rw-r--r--   0        0        0       22 2023-03-17 19:14:13.165345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/__version__.py
--rw-r--r--   0        0        0      360 2023-03-17 19:14:13.165345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_httpx_args.py
--rw-r--r--   0        0        0     9640 2023-03-17 19:14:13.165345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_keycloak_admin_aio.py
--rw-r--r--   0        0        0     1291 2023-03-17 19:14:13.165345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_lib/utils.py
--rw-r--r--   0        0        0      524 2023-03-17 19:14:13.165345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/__init__.py
--rw-r--r--   0        0        0       38 2023-03-17 19:14:13.165345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/admin_events/__init__.py
--rw-r--r--   0        0        0     1846 2023-03-17 19:14:13.165345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/admin_events/admin_events.py
--rw-r--r--   0        0        0      139 2023-03-17 19:14:13.165345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/attack_detection/__init__.py
--rw-r--r--   0        0        0      384 2023-03-17 19:14:13.165345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/attack_detection/attack_detection.py
--rw-r--r--   0        0        0       36 2023-03-17 19:14:13.165345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/attack_detection/brute_force/__init__.py
--rw-r--r--   0        0        0      337 2023-03-17 19:14:13.165345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/attack_detection/brute_force/brute_force.py
--rw-r--r--   0        0        0       25 2023-03-17 19:14:13.165345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/attack_detection/brute_force/users/__init__.py
--rw-r--r--   0        0        0       48 2023-03-17 19:14:13.165345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/attack_detection/brute_force/users/by_id/__init__.py
--rw-r--r--   0        0        0     1143 2023-03-17 19:14:13.165345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/attack_detection/brute_force/users/by_id/by_id.py
--rw-r--r--   0        0        0      913 2023-03-17 19:14:13.165345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/attack_detection/brute_force/users/users.py
--rw-r--r--   0        0        0      145 2023-03-17 19:14:13.165345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/authentication/__init__.py
--rw-r--r--   0        0        0      476 2023-03-17 19:14:13.165345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/authentication/authentication.py
--rw-r--r--   0        0        0       60 2023-03-17 19:14:13.165345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/authentication/required_actions/__init__.py
--rw-r--r--   0        0        0      947 2023-03-17 19:14:13.165345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/authentication/required_actions/required_actions.py
--rw-r--r--   0        0        0      130 2023-03-17 19:14:13.165345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/client_scopes/__init__.py
--rw-r--r--   0        0        0       36 2023-03-17 19:14:13.165345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/client_scopes/by_id/__init__.py
--rw-r--r--   0        0        0     1913 2023-03-17 19:14:13.165345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/client_scopes/by_id/by_id.py
--rw-r--r--   0        0        0       54 2023-03-17 19:14:13.165345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/client_scopes/by_id/scope_mappings/__init__.py
--rw-r--r--   0        0        0       50 2023-03-17 19:14:13.165345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/client_scopes/by_id/scope_mappings/realm/__init__.py
--rw-r--r--   0        0        0     2212 2023-03-17 19:14:13.165345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/client_scopes/by_id/scope_mappings/realm/realm.py
--rw-r--r--   0        0        0     1172 2023-03-17 19:14:13.165345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/client_scopes/by_id/scope_mappings/scope_mappings.py
--rw-r--r--   0        0        0     1710 2023-03-17 19:14:13.165345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/client_scopes/client_scopes.py
--rw-r--r--   0        0        0      298 2023-03-17 19:14:13.165345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/clients/__init__.py
--rw-r--r--   0        0        0       31 2023-03-17 19:14:13.165345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/clients/by_id/__init__.py
--rw-r--r--   0        0        0     1954 2023-03-17 19:14:13.165345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/clients/by_id/by_id.py
--rw-r--r--   0        0        0       66 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/clients/by_id/default_client_scopes/__init__.py
--rw-r--r--   0        0        0       54 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/clients/by_id/default_client_scopes/by_id/__init__.py
--rw-r--r--   0        0        0     1108 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/clients/by_id/default_client_scopes/by_id/by_id.py
--rw-r--r--   0        0        0     1371 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/clients/by_id/default_client_scopes/default_client_scopes.py
--rw-r--r--   0        0        0       51 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/clients/by_id/user_sessions/__init__.py
--rw-r--r--   0        0        0     1062 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/clients/by_id/user_sessions/user_sessions.py
--rw-r--r--   0        0        0     2190 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/clients/clients.py
--rw-r--r--   0        0        0      110 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/groups/__init__.py
--rw-r--r--   0        0        0       30 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/groups/by_id/__init__.py
--rw-r--r--   0        0        0     1795 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/groups/by_id/by_id.py
--rw-r--r--   0        0        0       41 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/groups/by_id/children/__init__.py
--rw-r--r--   0        0        0      900 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/groups/by_id/children/children.py
--rw-r--r--   0        0        0       39 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/groups/by_id/members/__init__.py
--rw-r--r--   0        0        0     1257 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/groups/by_id/members/members.py
--rw-r--r--   0        0        0     2505 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/groups/groups.py
--rw-r--r--   0        0        0     3175 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/keycloak_resource.py
--rw-r--r--   0        0        0      107 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/roles/__init__.py
--rw-r--r--   0        0        0      117 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/roles/by_id/__init__.py
--rw-r--r--   0        0        0     1673 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/roles/by_id/by_id.py
--rw-r--r--   0        0        0       44 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/roles/by_id/composites/__init__.py
--rw-r--r--   0        0        0     1955 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/roles/by_id/composites/composites.py
--rw-r--r--   0        0        0       33 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/roles/by_name/__init__.py
--rw-r--r--   0        0        0     1683 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/roles/by_name/by_name.py
--rw-r--r--   0        0        0       46 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/roles/by_name/composites/__init__.py
--rw-r--r--   0        0        0     1931 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/roles/by_name/composites/composites.py
--rw-r--r--   0        0        0     2245 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/roles/roles.py
--rw-r--r--   0        0        0       31 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/sessions/__init__.py
--rw-r--r--   0        0        0       32 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/sessions/by_id/__init__.py
--rw-r--r--   0        0        0      652 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/sessions/by_id/by_id.py
--rw-r--r--   0        0        0      409 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/sessions/sessions.py
--rw-r--r--   0        0        0      107 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/users/__init__.py
--rw-r--r--   0        0        0       29 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/users/by_id/__init__.py
--rw-r--r--   0        0        0     2004 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/users/by_id/by_id.py
--rw-r--r--   0        0        0       64 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/users/by_id/execute_actions_email/__init__.py
--rw-r--r--   0        0        0     1097 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/users/by_id/execute_actions_email/execute_actions_email.py
--rw-r--r--   0        0        0       36 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/users/by_id/groups/__init__.py
--rw-r--r--   0        0        0       39 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/users/by_id/groups/by_id/__init__.py
--rw-r--r--   0        0        0      452 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/users/by_id/groups/by_id/by_id.py
--rw-r--r--   0        0        0     2083 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/users/by_id/groups/groups.py
--rw-r--r--   0        0        0       49 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/users/by_id/role_mappings/__init__.py
--rw-r--r--   0        0        0       46 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/users/by_id/role_mappings/realm/__init__.py
--rw-r--r--   0        0        0     2815 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/users/by_id/role_mappings/realm/realm.py
--rw-r--r--   0        0        0     1063 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/users/by_id/role_mappings/role_mappings.py
--rw-r--r--   0        0        0     3693 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/users/users.py
--rw-r--r--   0        0        0        0 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/py.typed
--rw-r--r--   0        0        0     2522 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/types/__init__.py
--rw-r--r--   0        0        0      715 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/types/_data_class.py
--rw-r--r--   0        0        0    10639 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/keycloak_admin_aio/types/types.py
--rw-r--r--   0        0        0     1333 2023-03-17 19:14:13.169345 keycloak-admin-aio-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     4910 2023-03-17 19:14:29.178963 keycloak-admin-aio-1.3.1/setup.py
--rw-r--r--   0        0        0     2620 2023-03-17 19:14:29.179373 keycloak-admin-aio-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-23 16:10:30.450904 keycloak_admin_aio-1.3.3/LICENSE
+-rw-r--r--   0        0        0     2123 2023-06-23 16:10:30.450904 keycloak_admin_aio-1.3.3/README.rst
+-rw-r--r--   0        0        0      169 2023-06-23 16:10:30.450904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-23 16:10:30.450904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/__version__.py
+-rw-r--r--   0        0        0      360 2023-06-23 16:10:30.450904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_httpx_args.py
+-rw-r--r--   0        0        0     9640 2023-06-23 16:10:30.450904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_keycloak_admin_aio.py
+-rw-r--r--   0        0        0     1291 2023-06-23 16:10:30.450904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_lib/utils.py
+-rw-r--r--   0        0        0      524 2023-06-23 16:10:30.450904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/__init__.py
+-rw-r--r--   0        0        0       38 2023-06-23 16:10:30.450904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/admin_events/__init__.py
+-rw-r--r--   0        0        0     1846 2023-06-23 16:10:30.450904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/admin_events/admin_events.py
+-rw-r--r--   0        0        0      139 2023-06-23 16:10:30.450904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/attack_detection/__init__.py
+-rw-r--r--   0        0        0      384 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/attack_detection/attack_detection.py
+-rw-r--r--   0        0        0       36 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/attack_detection/brute_force/__init__.py
+-rw-r--r--   0        0        0      337 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/attack_detection/brute_force/brute_force.py
+-rw-r--r--   0        0        0       25 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/attack_detection/brute_force/users/__init__.py
+-rw-r--r--   0        0        0       48 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/attack_detection/brute_force/users/by_id/__init__.py
+-rw-r--r--   0        0        0     1143 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/attack_detection/brute_force/users/by_id/by_id.py
+-rw-r--r--   0        0        0      913 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/attack_detection/brute_force/users/users.py
+-rw-r--r--   0        0        0      145 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/authentication/__init__.py
+-rw-r--r--   0        0        0      476 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/authentication/authentication.py
+-rw-r--r--   0        0        0       60 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/authentication/required_actions/__init__.py
+-rw-r--r--   0        0        0      947 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/authentication/required_actions/required_actions.py
+-rw-r--r--   0        0        0      130 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/client_scopes/__init__.py
+-rw-r--r--   0        0        0       36 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/client_scopes/by_id/__init__.py
+-rw-r--r--   0        0        0     1913 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/client_scopes/by_id/by_id.py
+-rw-r--r--   0        0        0       54 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/client_scopes/by_id/scope_mappings/__init__.py
+-rw-r--r--   0        0        0       50 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/client_scopes/by_id/scope_mappings/realm/__init__.py
+-rw-r--r--   0        0        0     2212 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/client_scopes/by_id/scope_mappings/realm/realm.py
+-rw-r--r--   0        0        0     1172 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/client_scopes/by_id/scope_mappings/scope_mappings.py
+-rw-r--r--   0        0        0     1710 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/client_scopes/client_scopes.py
+-rw-r--r--   0        0        0      298 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/clients/__init__.py
+-rw-r--r--   0        0        0       31 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/clients/by_id/__init__.py
+-rw-r--r--   0        0        0     1954 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/clients/by_id/by_id.py
+-rw-r--r--   0        0        0       66 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/clients/by_id/default_client_scopes/__init__.py
+-rw-r--r--   0        0        0       54 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/clients/by_id/default_client_scopes/by_id/__init__.py
+-rw-r--r--   0        0        0     1108 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/clients/by_id/default_client_scopes/by_id/by_id.py
+-rw-r--r--   0        0        0     1371 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/clients/by_id/default_client_scopes/default_client_scopes.py
+-rw-r--r--   0        0        0       51 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/clients/by_id/user_sessions/__init__.py
+-rw-r--r--   0        0        0     1062 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/clients/by_id/user_sessions/user_sessions.py
+-rw-r--r--   0        0        0     2190 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/clients/clients.py
+-rw-r--r--   0        0        0      110 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/groups/__init__.py
+-rw-r--r--   0        0        0       30 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/groups/by_id/__init__.py
+-rw-r--r--   0        0        0     1795 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/groups/by_id/by_id.py
+-rw-r--r--   0        0        0       41 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/groups/by_id/children/__init__.py
+-rw-r--r--   0        0        0      900 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/groups/by_id/children/children.py
+-rw-r--r--   0        0        0       39 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/groups/by_id/members/__init__.py
+-rw-r--r--   0        0        0     1257 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/groups/by_id/members/members.py
+-rw-r--r--   0        0        0     2505 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/groups/groups.py
+-rw-r--r--   0        0        0     3175 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/keycloak_resource.py
+-rw-r--r--   0        0        0      107 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/roles/__init__.py
+-rw-r--r--   0        0        0      117 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/roles/by_id/__init__.py
+-rw-r--r--   0        0        0     1673 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/roles/by_id/by_id.py
+-rw-r--r--   0        0        0       44 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/roles/by_id/composites/__init__.py
+-rw-r--r--   0        0        0     1955 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/roles/by_id/composites/composites.py
+-rw-r--r--   0        0        0       33 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/roles/by_name/__init__.py
+-rw-r--r--   0        0        0     1683 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/roles/by_name/by_name.py
+-rw-r--r--   0        0        0       46 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/roles/by_name/composites/__init__.py
+-rw-r--r--   0        0        0     1931 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/roles/by_name/composites/composites.py
+-rw-r--r--   0        0        0     2245 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/roles/roles.py
+-rw-r--r--   0        0        0       31 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/sessions/__init__.py
+-rw-r--r--   0        0        0       32 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/sessions/by_id/__init__.py
+-rw-r--r--   0        0        0      652 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/sessions/by_id/by_id.py
+-rw-r--r--   0        0        0      409 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/sessions/sessions.py
+-rw-r--r--   0        0        0      107 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/users/__init__.py
+-rw-r--r--   0        0        0       29 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/users/by_id/__init__.py
+-rw-r--r--   0        0        0     2004 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/users/by_id/by_id.py
+-rw-r--r--   0        0        0       64 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/users/by_id/execute_actions_email/__init__.py
+-rw-r--r--   0        0        0     1097 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/users/by_id/execute_actions_email/execute_actions_email.py
+-rw-r--r--   0        0        0       36 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/users/by_id/groups/__init__.py
+-rw-r--r--   0        0        0       39 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/users/by_id/groups/by_id/__init__.py
+-rw-r--r--   0        0        0      452 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/users/by_id/groups/by_id/by_id.py
+-rw-r--r--   0        0        0     2083 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/users/by_id/groups/groups.py
+-rw-r--r--   0        0        0       49 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/users/by_id/role_mappings/__init__.py
+-rw-r--r--   0        0        0       46 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/users/by_id/role_mappings/realm/__init__.py
+-rw-r--r--   0        0        0     2815 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/users/by_id/role_mappings/realm/realm.py
+-rw-r--r--   0        0        0     1063 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/users/by_id/role_mappings/role_mappings.py
+-rw-r--r--   0        0        0     3693 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/users/users.py
+-rw-r--r--   0        0        0        0 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/py.typed
+-rw-r--r--   0        0        0     2522 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/types/__init__.py
+-rw-r--r--   0        0        0      715 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/types/_data_class.py
+-rw-r--r--   0        0        0    10639 2023-06-23 16:10:30.454904 keycloak_admin_aio-1.3.3/keycloak_admin_aio/types/types.py
+-rw-r--r--   0        0        0     1344 2023-06-23 16:10:30.458904 keycloak_admin_aio-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0     2782 1970-01-01 00:00:00.000000 keycloak_admin_aio-1.3.3/PKG-INFO
```

### Comparing `keycloak-admin-aio-1.3.1/LICENSE` & `keycloak_admin_aio-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `keycloak-admin-aio-1.3.1/README.rst` & `keycloak_admin_aio-1.3.3/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 The main dependencies are:
 
 - `httpx <https://github.com/encode/httpx/>`_: asynchronous http client
 - `dacite <https://github.com/konradhalas/dacite>`_: parse nested dictionaries into nested dataclasses
 
 Links:
 
-- `Source code <https://github.com/delphai/keycloak-admin-aio>`_
-- `Documentation <https://delphai.github.io/keycloak-admin-aio/>`_
+- `Source code <https://github.com/V-Mann-Nick/keycloak-admin-aio>`_
+- `Documentation <https://v-mann-nick.github.io/keycloak-admin-aio/>`_
 - `Pypi <https://pypi.org/project/keycloak-admin-aio/>`_
 
 How to install?
 ---------------
 
 .. code:: shell
 
@@ -79,8 +79,8 @@
 
 License
 -------
 
 `Apache License, Version 2.0 <https://www.apache.org/licenses/LICENSE-2.0>`_
 
 
-© Copyright 2021, delphai by AtomLeap GmbH
+© Copyright 2023, Nicklas Sedlock
```

### Comparing `keycloak-admin-aio-1.3.1/keycloak_admin_aio/_keycloak_admin_aio.py` & `keycloak_admin_aio-1.3.3/keycloak_admin_aio/_keycloak_admin_aio.py`

 * *Files identical despite different names*

### Comparing `keycloak-admin-aio-1.3.1/keycloak_admin_aio/_lib/utils.py` & `keycloak_admin_aio-1.3.3/keycloak_admin_aio/_lib/utils.py`

 * *Files identical despite different names*

### Comparing `keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/__init__.py` & `keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/admin_events/admin_events.py` & `keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/admin_events/admin_events.py`

 * *Files identical despite different names*

### Comparing `keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/attack_detection/brute_force/users/by_id/by_id.py` & `keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/attack_detection/brute_force/users/by_id/by_id.py`

 * *Files identical despite different names*

### Comparing `keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/attack_detection/brute_force/users/users.py` & `keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/attack_detection/brute_force/users/users.py`

 * *Files identical despite different names*

### Comparing `keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/authentication/required_actions/required_actions.py` & `keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/authentication/required_actions/required_actions.py`

 * *Files identical despite different names*

### Comparing `keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/client_scopes/by_id/by_id.py` & `keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/client_scopes/by_id/by_id.py`

 * *Files identical despite different names*

### Comparing `keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/client_scopes/by_id/scope_mappings/realm/realm.py` & `keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/client_scopes/by_id/scope_mappings/realm/realm.py`

 * *Files identical despite different names*

### Comparing `keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/client_scopes/by_id/scope_mappings/scope_mappings.py` & `keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/client_scopes/by_id/scope_mappings/scope_mappings.py`

 * *Files identical despite different names*

### Comparing `keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/client_scopes/client_scopes.py` & `keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/client_scopes/client_scopes.py`

 * *Files identical despite different names*

### Comparing `keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/clients/by_id/by_id.py` & `keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/clients/by_id/by_id.py`

 * *Files identical despite different names*

### Comparing `keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/clients/by_id/default_client_scopes/by_id/by_id.py` & `keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/clients/by_id/default_client_scopes/by_id/by_id.py`

 * *Files identical despite different names*

### Comparing `keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/clients/by_id/default_client_scopes/default_client_scopes.py` & `keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/clients/by_id/default_client_scopes/default_client_scopes.py`

 * *Files identical despite different names*

### Comparing `keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/clients/by_id/user_sessions/user_sessions.py` & `keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/clients/by_id/user_sessions/user_sessions.py`

 * *Files identical despite different names*

### Comparing `keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/clients/clients.py` & `keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/clients/clients.py`

 * *Files identical despite different names*

### Comparing `keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/groups/by_id/by_id.py` & `keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/groups/by_id/by_id.py`

 * *Files identical despite different names*

### Comparing `keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/groups/by_id/children/children.py` & `keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/groups/by_id/children/children.py`

 * *Files identical despite different names*

### Comparing `keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/groups/by_id/members/members.py` & `keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/groups/by_id/members/members.py`

 * *Files identical despite different names*

### Comparing `keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/groups/groups.py` & `keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/groups/groups.py`

 * *Files identical despite different names*

### Comparing `keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/keycloak_resource.py` & `keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/keycloak_resource.py`

 * *Files identical despite different names*

### Comparing `keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/roles/by_id/by_id.py` & `keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/roles/by_id/by_id.py`

 * *Files identical despite different names*

### Comparing `keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/roles/by_id/composites/composites.py` & `keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/roles/by_id/composites/composites.py`

 * *Files identical despite different names*

### Comparing `keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/roles/by_name/by_name.py` & `keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/roles/by_name/by_name.py`

 * *Files identical despite different names*

### Comparing `keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/roles/by_name/composites/composites.py` & `keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/roles/by_name/composites/composites.py`

 * *Files identical despite different names*

### Comparing `keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/roles/roles.py` & `keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/roles/roles.py`

 * *Files identical despite different names*

### Comparing `keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/sessions/by_id/by_id.py` & `keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/sessions/by_id/by_id.py`

 * *Files identical despite different names*

### Comparing `keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/users/by_id/by_id.py` & `keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/users/by_id/by_id.py`

 * *Files identical despite different names*

### Comparing `keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/users/by_id/execute_actions_email/execute_actions_email.py` & `keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/users/by_id/execute_actions_email/execute_actions_email.py`

 * *Files identical despite different names*

### Comparing `keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/users/by_id/groups/groups.py` & `keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/users/by_id/groups/groups.py`

 * *Files identical despite different names*

### Comparing `keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/users/by_id/role_mappings/realm/realm.py` & `keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/users/by_id/role_mappings/realm/realm.py`

 * *Files identical despite different names*

### Comparing `keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/users/by_id/role_mappings/role_mappings.py` & `keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/users/by_id/role_mappings/role_mappings.py`

 * *Files identical despite different names*

### Comparing `keycloak-admin-aio-1.3.1/keycloak_admin_aio/_resources/users/users.py` & `keycloak_admin_aio-1.3.3/keycloak_admin_aio/_resources/users/users.py`

 * *Files identical despite different names*

### Comparing `keycloak-admin-aio-1.3.1/keycloak_admin_aio/types/__init__.py` & `keycloak_admin_aio-1.3.3/keycloak_admin_aio/types/__init__.py`

 * *Files identical despite different names*

### Comparing `keycloak-admin-aio-1.3.1/keycloak_admin_aio/types/_data_class.py` & `keycloak_admin_aio-1.3.3/keycloak_admin_aio/types/_data_class.py`

 * *Files identical despite different names*

### Comparing `keycloak-admin-aio-1.3.1/keycloak_admin_aio/types/types.py` & `keycloak_admin_aio-1.3.3/keycloak_admin_aio/types/types.py`

 * *Files identical despite different names*

### Comparing `keycloak-admin-aio-1.3.1/pyproject.toml` & `keycloak_admin_aio-1.3.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "keycloak-admin-aio"
-version = "1.3.1"
+version = "1.3.3"
 description = "async keycloak admin api wrapper"
-authors = ["Nicklas Sedlock <nicklas@delphai.com>"]
-homepage = "https://github.com/delphai/keycloak-admin-aio"
+authors = ["Nicklas Sedlock <nicklas.sedlock@posteo.net>"]
+homepage = "https://github.com/V-Mann-Nick/keycloak-admin-aio"
 license = "Apache-2.0"
 readme = "README.rst"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 httpx = "^0.23.3"
 dacite = "^1.6.0"
@@ -24,15 +24,15 @@
 pytest = "^6.2.5"
 pytest-asyncio = "^0.16.0"
 pytest-dependency = "^0.5.1"
 mypy = "^0.910"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.3.1"
+version = "1.3.3"
 version_files = [
     "keycloak_admin_aio/__version__.py",
     "pyproject.toml:version"
 ]
 tag_format = "$version"
 
 [tool.poe.tasks]
```

### Comparing `keycloak-admin-aio-1.3.1/PKG-INFO` & `keycloak_admin_aio-1.3.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: keycloak-admin-aio
-Version: 1.3.1
+Version: 1.3.3
 Summary: async keycloak admin api wrapper
-Home-page: https://github.com/delphai/keycloak-admin-aio
+Home-page: https://github.com/V-Mann-Nick/keycloak-admin-aio
 License: Apache-2.0
 Author: Nicklas Sedlock
-Author-email: nicklas@delphai.com
+Author-email: nicklas.sedlock@posteo.net
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dacite (>=1.6.0,<2.0.0)
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
 Description-Content-Type: text/x-rst
 
 What is keycloak_admin_aio?
 ---------------------------
 
@@ -22,16 +25,16 @@
 The main dependencies are:
 
 - `httpx <https://github.com/encode/httpx/>`_: asynchronous http client
 - `dacite <https://github.com/konradhalas/dacite>`_: parse nested dictionaries into nested dataclasses
 
 Links:
 
-- `Source code <https://github.com/delphai/keycloak-admin-aio>`_
-- `Documentation <https://delphai.github.io/keycloak-admin-aio/>`_
+- `Source code <https://github.com/V-Mann-Nick/keycloak-admin-aio>`_
+- `Documentation <https://v-mann-nick.github.io/keycloak-admin-aio/>`_
 - `Pypi <https://pypi.org/project/keycloak-admin-aio/>`_
 
 How to install?
 ---------------
 
 .. code:: shell
 
@@ -94,9 +97,9 @@
 
 License
 -------
 
 `Apache License, Version 2.0 <https://www.apache.org/licenses/LICENSE-2.0>`_
 
 
-© Copyright 2021, delphai by AtomLeap GmbH
+© Copyright 2023, Nicklas Sedlock
```


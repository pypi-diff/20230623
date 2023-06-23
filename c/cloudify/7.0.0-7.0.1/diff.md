# Comparing `tmp/cloudify-7.0.0.tar.gz` & `tmp/cloudify-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudify-7.0.0.tar", last modified: Tue Apr 25 11:56:05 2023, max compression
+gzip compressed data, was "cloudify-7.0.1.tar", last modified: Fri Jun 23 15:26:41 2023, max compression
```

## Comparing `cloudify-7.0.0.tar` & `cloudify-7.0.1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:56:05.291888 cloudify-7.0.0/
--rw-r--r--   0 root         (0) root         (0)    11325 2023-04-25 11:55:41.000000 cloudify-7.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      189 2023-04-25 11:56:05.291888 cloudify-7.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      591 2023-04-25 11:55:41.000000 cloudify-7.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:56:05.279890 cloudify-7.0.0/cloudify.egg-info/
--rw-r--r--   0 root         (0) root         (0)      189 2023-04-25 11:56:05.000000 cloudify-7.0.0/cloudify.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2162 2023-04-25 11:56:05.000000 cloudify-7.0.0/cloudify.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 11:56:05.000000 cloudify-7.0.0/cloudify.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       47 2023-04-25 11:56:05.000000 cloudify-7.0.0/cloudify.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      222 2023-04-25 11:56:05.000000 cloudify-7.0.0/cloudify.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-25 11:56:05.000000 cloudify-7.0.0/cloudify.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:56:05.283889 cloudify-7.0.0/cloudify_cli/
--rw-r--r--   0 root         (0) root         (0)      641 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:56:05.283889 cloudify-7.0.0/cloudify_cli/async_commands/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/async_commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2275 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/async_commands/audit_log.py
--rw-r--r--   0 root         (0) root         (0)     6759 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/blueprint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:56:05.283889 cloudify-7.0.0/cloudify_cli/cli/
--rw-r--r--   0 root         (0) root         (0)      641 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    78764 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/cli/cfy.py
--rw-r--r--   0 root         (0) root         (0)     1967 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/cli/completion_utils.py
--rw-r--r--   0 root         (0) root         (0)    31831 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/cli/helptexts.py
--rw-r--r--   0 root         (0) root         (0)     6054 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/colorful_event.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:56:05.291888 cloudify-7.0.0/cloudify_cli/commands/
--rw-r--r--   0 root         (0) root         (0)      641 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16037 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/agents.py
--rw-r--r--   0 root         (0) root         (0)    10374 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/apply.py
--rw-r--r--   0 root         (0) root         (0)     5480 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/audit_log.py
--rw-r--r--   0 root         (0) root         (0)    31561 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/blueprints.py
--rw-r--r--   0 root         (0) root         (0)    14297 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/certificates.py
--rw-r--r--   0 root         (0) root         (0)    16691 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/cluster.py
--rw-r--r--   0 root         (0) root         (0)     1359 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/community.py
--rw-r--r--   0 root         (0) root         (0)     2404 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/config.py
--rw-r--r--   0 root         (0) root         (0)    71965 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/deployments.py
--rw-r--r--   0 root         (0) root         (0)    12209 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/events.py
--rw-r--r--   0 root         (0) root         (0)    33757 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/executions.py
--rw-r--r--   0 root         (0) root         (0)     2785 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/groups.py
--rw-r--r--   0 root         (0) root         (0)      383 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/idp.py
--rw-r--r--   0 root         (0) root         (0)     6587 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/init.py
--rw-r--r--   0 root         (0) root         (0)     8223 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/install.py
--rw-r--r--   0 root         (0) root         (0)     3166 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/ldap.py
--rw-r--r--   0 root         (0) root         (0)     4505 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/license.py
--rw-r--r--   0 root         (0) root         (0)     3999 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/log_bundles.py
--rw-r--r--   0 root         (0) root         (0)     5465 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/maintenance_mode.py
--rw-r--r--   0 root         (0) root         (0)    10411 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/node_instances.py
--rw-r--r--   0 root         (0) root         (0)     8827 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/nodes.py
--rw-r--r--   0 root         (0) root         (0)     1909 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/permissions.py
--rw-r--r--   0 root         (0) root         (0)    41310 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/plugins.py
--rw-r--r--   0 root         (0) root         (0)    27830 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/profiles.py
--rw-r--r--   0 root         (0) root         (0)    21581 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/secrets.py
--rw-r--r--   0 root         (0) root         (0)     5512 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/sites.py
--rw-r--r--   0 root         (0) root         (0)    10099 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/snapshots.py
--rw-r--r--   0 root         (0) root         (0)     2419 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/status.py
--rw-r--r--   0 root         (0) root         (0)     2264 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/summary.py
--rw-r--r--   0 root         (0) root         (0)    10822 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/tenants.py
--rw-r--r--   0 root         (0) root         (0)     2866 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/tokens.py
--rw-r--r--   0 root         (0) root         (0)     4148 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/uninstall.py
--rw-r--r--   0 root         (0) root         (0)     6937 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/user_groups.py
--rw-r--r--   0 root         (0) root         (0)     9355 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/users.py
--rw-r--r--   0 root         (0) root         (0)     5644 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/commands/workflows.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:56:05.291888 cloudify-7.0.0/cloudify_cli/config/
--rw-r--r--   0 root         (0) root         (0)      641 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4228 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/config/config.py
--rw-r--r--   0 root         (0) root         (0)     2812 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/constants.py
--rw-r--r--   0 root         (0) root         (0)    22806 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/env.py
--rw-r--r--   0 root         (0) root         (0)     1498 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     9183 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/execution_events_fetcher.py
--rw-r--r--   0 root         (0) root         (0)    13653 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/filters_utils.py
--rw-r--r--   0 root         (0) root         (0)     6006 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/inputs.py
--rw-r--r--   0 root         (0) root         (0)     5989 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/labels_utils.py
--rw-r--r--   0 root         (0) root         (0)     8492 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/local.py
--rw-r--r--   0 root         (0) root         (0)     6868 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/logger.py
--rw-r--r--   0 root         (0) root         (0)    13189 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/main.py
--rw-r--r--   0 root         (0) root         (0)    54445 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/prettytable.py
--rw-r--r--   0 root         (0) root         (0)    10905 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/replace_certificates_config.py
--rw-r--r--   0 root         (0) root         (0)     6697 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/table.py
--rw-r--r--   0 root         (0) root         (0)    16280 2023-04-25 11:55:41.000000 cloudify-7.0.0/cloudify_cli/utils.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 11:56:05.291888 cloudify-7.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1579 2023-04-25 11:55:41.000000 cloudify-7.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:26:41.114862 cloudify-7.0.1/
+-rw-r--r--   0 root         (0) root         (0)    11325 2023-06-23 15:26:18.000000 cloudify-7.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      189 2023-06-23 15:26:41.114862 cloudify-7.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      591 2023-06-23 15:26:18.000000 cloudify-7.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:26:41.106862 cloudify-7.0.1/cloudify.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      189 2023-06-23 15:26:41.000000 cloudify-7.0.1/cloudify.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2162 2023-06-23 15:26:41.000000 cloudify-7.0.1/cloudify.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 15:26:41.000000 cloudify-7.0.1/cloudify.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2023-06-23 15:26:41.000000 cloudify-7.0.1/cloudify.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      222 2023-06-23 15:26:41.000000 cloudify-7.0.1/cloudify.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-23 15:26:41.000000 cloudify-7.0.1/cloudify.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:26:41.106862 cloudify-7.0.1/cloudify_cli/
+-rw-r--r--   0 root         (0) root         (0)      641 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:26:41.106862 cloudify-7.0.1/cloudify_cli/async_commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/async_commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2275 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/async_commands/audit_log.py
+-rw-r--r--   0 root         (0) root         (0)     6759 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/blueprint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:26:41.106862 cloudify-7.0.1/cloudify_cli/cli/
+-rw-r--r--   0 root         (0) root         (0)      641 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    78946 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/cli/cfy.py
+-rw-r--r--   0 root         (0) root         (0)     1967 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/cli/completion_utils.py
+-rw-r--r--   0 root         (0) root         (0)    31948 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/cli/helptexts.py
+-rw-r--r--   0 root         (0) root         (0)     6054 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/colorful_event.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:26:41.110862 cloudify-7.0.1/cloudify_cli/commands/
+-rw-r--r--   0 root         (0) root         (0)      641 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16037 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/commands/agents.py
+-rw-r--r--   0 root         (0) root         (0)    10374 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/commands/apply.py
+-rw-r--r--   0 root         (0) root         (0)     5480 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/commands/audit_log.py
+-rw-r--r--   0 root         (0) root         (0)    31561 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/commands/blueprints.py
+-rw-r--r--   0 root         (0) root         (0)    14297 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/commands/certificates.py
+-rw-r--r--   0 root         (0) root         (0)    16691 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/commands/cluster.py
+-rw-r--r--   0 root         (0) root         (0)     1359 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/commands/community.py
+-rw-r--r--   0 root         (0) root         (0)     2404 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/commands/config.py
+-rw-r--r--   0 root         (0) root         (0)    72161 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/commands/deployments.py
+-rw-r--r--   0 root         (0) root         (0)    12209 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/commands/events.py
+-rw-r--r--   0 root         (0) root         (0)    33757 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/commands/executions.py
+-rw-r--r--   0 root         (0) root         (0)     2785 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/commands/groups.py
+-rw-r--r--   0 root         (0) root         (0)      383 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/commands/idp.py
+-rw-r--r--   0 root         (0) root         (0)     6587 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/commands/init.py
+-rw-r--r--   0 root         (0) root         (0)     8223 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/commands/install.py
+-rw-r--r--   0 root         (0) root         (0)     3166 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/commands/ldap.py
+-rw-r--r--   0 root         (0) root         (0)     4505 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/commands/license.py
+-rw-r--r--   0 root         (0) root         (0)     3984 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/commands/log_bundles.py
+-rw-r--r--   0 root         (0) root         (0)     5465 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/commands/maintenance_mode.py
+-rw-r--r--   0 root         (0) root         (0)    10411 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/commands/node_instances.py
+-rw-r--r--   0 root         (0) root         (0)     8827 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/commands/nodes.py
+-rw-r--r--   0 root         (0) root         (0)     1909 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/commands/permissions.py
+-rw-r--r--   0 root         (0) root         (0)    41310 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/commands/plugins.py
+-rw-r--r--   0 root         (0) root         (0)    27830 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/commands/profiles.py
+-rw-r--r--   0 root         (0) root         (0)    21581 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/commands/secrets.py
+-rw-r--r--   0 root         (0) root         (0)     5512 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/commands/sites.py
+-rw-r--r--   0 root         (0) root         (0)    10099 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/commands/snapshots.py
+-rw-r--r--   0 root         (0) root         (0)     2419 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/commands/status.py
+-rw-r--r--   0 root         (0) root         (0)     2264 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/commands/summary.py
+-rw-r--r--   0 root         (0) root         (0)    10822 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/commands/tenants.py
+-rw-r--r--   0 root         (0) root         (0)     2866 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/commands/tokens.py
+-rw-r--r--   0 root         (0) root         (0)     4293 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/commands/uninstall.py
+-rw-r--r--   0 root         (0) root         (0)     6937 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/commands/user_groups.py
+-rw-r--r--   0 root         (0) root         (0)     9355 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/commands/users.py
+-rw-r--r--   0 root         (0) root         (0)     5644 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/commands/workflows.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:26:41.110862 cloudify-7.0.1/cloudify_cli/config/
+-rw-r--r--   0 root         (0) root         (0)      641 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4228 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/config/config.py
+-rw-r--r--   0 root         (0) root         (0)     2812 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/constants.py
+-rw-r--r--   0 root         (0) root         (0)    22806 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/env.py
+-rw-r--r--   0 root         (0) root         (0)     1498 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     9183 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/execution_events_fetcher.py
+-rw-r--r--   0 root         (0) root         (0)    13653 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/filters_utils.py
+-rw-r--r--   0 root         (0) root         (0)     6006 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/inputs.py
+-rw-r--r--   0 root         (0) root         (0)     5989 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/labels_utils.py
+-rw-r--r--   0 root         (0) root         (0)     8492 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/local.py
+-rw-r--r--   0 root         (0) root         (0)     6868 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/logger.py
+-rw-r--r--   0 root         (0) root         (0)    13189 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/main.py
+-rw-r--r--   0 root         (0) root         (0)    54445 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/prettytable.py
+-rw-r--r--   0 root         (0) root         (0)    10905 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/replace_certificates_config.py
+-rw-r--r--   0 root         (0) root         (0)     6697 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/table.py
+-rw-r--r--   0 root         (0) root         (0)    16280 2023-06-23 15:26:18.000000 cloudify-7.0.1/cloudify_cli/utils.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 15:26:41.114862 cloudify-7.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1579 2023-06-23 15:26:18.000000 cloudify-7.0.1/setup.py
```

### Comparing `cloudify-7.0.0/LICENSE` & `cloudify-7.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/README.md` & `cloudify-7.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify.egg-info/SOURCES.txt` & `cloudify-7.0.1/cloudify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/__init__.py` & `cloudify-7.0.1/cloudify_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/async_commands/audit_log.py` & `cloudify-7.0.1/cloudify_cli/async_commands/audit_log.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/blueprint.py` & `cloudify-7.0.1/cloudify_cli/blueprint.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/cli/__init__.py` & `cloudify-7.0.1/cloudify_cli/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/cli/cfy.py` & `cloudify-7.0.1/cloudify_cli/cli/cfy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1918,14 +1918,20 @@
         self.evaluate_functions = click.option(
             '--evaluate-functions',
             is_flag=True,
             default=False,
             required=False,
             help=helptexts.EVALUATE_FUNCTIONS,
         )
+        self.recursive_delete = click.option(
+            '--recursive',
+            default=False,
+            is_flag=True,
+            help=helptexts.RECURSIVE_DELETE,
+        )
 
     def common_options(self, f):
         """A shorthand for applying commonly used arguments.
 
         To be used for arguments that are going to be applied for all or
         almost all commands.
         """
@@ -1988,14 +1994,15 @@
             is_flag=True,
             help=helptexts.AGENT_ALL_STATES,
         )
 
         # we add separate --node-instance-id, --node-id and --deployment-id
         # arguments, but only expose a agents_filter = {'node_id': ..} dict
         # to the decorated function
+
         def _filters_deco(f):
             @wraps(f)
             def _inner(*args, **kwargs):
                 filters = {}
                 for arg_name, filter_name in [
                         ('node_id', AGENT_FILTER_NODE_IDS),
                         ('node_instance_id', AGENT_FILTER_NODE_INSTANCE_IDS),
```

### Comparing `cloudify-7.0.0/cloudify_cli/cli/completion_utils.py` & `cloudify-7.0.1/cloudify_cli/cli/completion_utils.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/cli/helptexts.py` & `cloudify-7.0.1/cloudify_cli/cli/helptexts.py`

 * *Files 0% similar despite different names*

```diff
@@ -619,7 +619,9 @@
 SECRETS_PROVIDER_CONNECTION_PARAMETERS = """
     Secrets Provider's connection parameters in stringify JSON format
     """
 SECRETS_PROVIDER_OPTIONS = """
     Secrets Provider's options in stringify JSON format
     """
 EVALUATE_FUNCTIONS = "Evaluate functions in returned nodes and node instances"
+RECURSIVE_DELETE = 'Recursively delete all service deployments contained in ' \
+                   'this deployment'
```

### Comparing `cloudify-7.0.0/cloudify_cli/colorful_event.py` & `cloudify-7.0.1/cloudify_cli/colorful_event.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/commands/__init__.py` & `cloudify-7.0.1/cloudify_cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/commands/agents.py` & `cloudify-7.0.1/cloudify_cli/commands/agents.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/commands/apply.py` & `cloudify-7.0.1/cloudify_cli/commands/apply.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/commands/audit_log.py` & `cloudify-7.0.1/cloudify_cli/commands/audit_log.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/commands/blueprints.py` & `cloudify-7.0.1/cloudify_cli/commands/blueprints.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/commands/certificates.py` & `cloudify-7.0.1/cloudify_cli/commands/certificates.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/commands/cluster.py` & `cloudify-7.0.1/cloudify_cli/commands/cluster.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/commands/community.py` & `cloudify-7.0.1/cloudify_cli/commands/community.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/commands/config.py` & `cloudify-7.0.1/cloudify_cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/commands/deployments.py` & `cloudify-7.0.1/cloudify_cli/commands/deployments.py`

 * *Files 1% similar despite different names*

```diff
@@ -694,27 +694,40 @@
 @deployments.command(name='delete',
                      short_help='Delete a deployment [manager only]')
 @cfy.argument('deployment-id')
 @cfy.options.force(help=helptexts.FORCE_DELETE_DEPLOYMENT)
 @cfy.options.common_options
 @cfy.options.with_logs
 @cfy.options.tenant_name(required=False, resource_name_for_help='deployment')
+@cfy.options.recursive_delete
 @cfy.assert_manager_active()
 @cfy.pass_client()
 @cfy.pass_logger
-def manager_delete(deployment_id, force, with_logs, logger, client,
-                   tenant_name):
+def manager_delete(
+    deployment_id,
+    force,
+    with_logs,
+    recursive,
+    logger,
+    client,
+    tenant_name,
+):
     """Delete a deployment from the manager
 
     `DEPLOYMENT_ID` is the id of the deployment to delete.
     """
 
     utils.explicit_tenant_name_message(tenant_name, logger)
     logger.info('Trying to delete deployment %s...', deployment_id)
-    client.deployments.delete(deployment_id, force, with_logs=with_logs)
+    client.deployments.delete(
+        deployment_id,
+        force,
+        with_logs=with_logs,
+        recursive=recursive,
+    )
     try:
         execution = get_deployment_environment_execution(
             client, deployment_id, DELETE_DEP)
         if execution:
             execution_events_fetcher.wait_for_execution(
                 client, execution, logger=logger)
 
@@ -1188,30 +1201,39 @@
     logger.info('Group %s created', deployment_group_name)
 
 
 @groups.command('delete', short_help='Delete a deployment group')
 @click.argument('deployment-group-name')
 @cfy.options.delete_deployments
 @cfy.options.with_logs
+@cfy.options.recursive_delete
 @cfy.options.force(help=helptexts.FORCE_DELETE_DEPLOYMENT)
 @cfy.pass_client()
 @cfy.pass_logger
-def groups_delete(deployment_group_name, delete_deployments, force, with_logs,
-                  client, logger):
+def groups_delete(
+    deployment_group_name,
+    delete_deployments,
+    force,
+    with_logs,
+    recursive,
+    client,
+    logger,
+):
     """Delete a deployment group
 
     This deletes a deployment group, which by default only removes the
     grouping, the deployments in the group are still left intact.
     To delete all deployments, pass `--delete-deployments`.
     """
     client.deployment_groups.delete(
         deployment_group_name,
         delete_deployments=delete_deployments,
         force=force,
         with_logs=with_logs,
+        recursive=recursive,
     )
     logger.info('Group %s deleted', deployment_group_name)
 
 
 @groups.command('update', short_help='Update a deployment group')
 @click.argument('deployment-group-name')
 @cfy.options.inputs
```

### Comparing `cloudify-7.0.0/cloudify_cli/commands/events.py` & `cloudify-7.0.1/cloudify_cli/commands/events.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/commands/executions.py` & `cloudify-7.0.1/cloudify_cli/commands/executions.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/commands/groups.py` & `cloudify-7.0.1/cloudify_cli/commands/groups.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/commands/init.py` & `cloudify-7.0.1/cloudify_cli/commands/init.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/commands/install.py` & `cloudify-7.0.1/cloudify_cli/commands/install.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/commands/ldap.py` & `cloudify-7.0.1/cloudify_cli/commands/ldap.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/commands/license.py` & `cloudify-7.0.1/cloudify_cli/commands/license.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/commands/log_bundles.py` & `cloudify-7.0.1/cloudify_cli/commands/log_bundles.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,18 +46,18 @@
 
 @log_bundles.command(name='delete',
                      short_help='Delete a log bundle [manager only]')
 @cfy.argument('log-bundle-id')
 @cfy.options.common_options
 @cfy.pass_client()
 @cfy.pass_logger
-def delete(log_bundle_id, logger, client, tenant_name):
+def delete(log_bundle_id, logger, client):
     """Delete a log_bundle from the manager
 
-    `LOG_BUNDLE_ID` is the id of the log bundle to download.
+    `LOG_BUNDLE_ID` is the id of the log bundle to delete.
     """
     logger.info('Deleting log_bundle {0}...'.format(log_bundle_id))
     client.log_bundles.delete(log_bundle_id)
     logger.info('Log bundle deleted successfully')
 
 
 @log_bundles.command(name='download',
```

### Comparing `cloudify-7.0.0/cloudify_cli/commands/maintenance_mode.py` & `cloudify-7.0.1/cloudify_cli/commands/maintenance_mode.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/commands/node_instances.py` & `cloudify-7.0.1/cloudify_cli/commands/node_instances.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/commands/nodes.py` & `cloudify-7.0.1/cloudify_cli/commands/nodes.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/commands/permissions.py` & `cloudify-7.0.1/cloudify_cli/commands/permissions.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/commands/plugins.py` & `cloudify-7.0.1/cloudify_cli/commands/plugins.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/commands/profiles.py` & `cloudify-7.0.1/cloudify_cli/commands/profiles.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/commands/secrets.py` & `cloudify-7.0.1/cloudify_cli/commands/secrets.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/commands/sites.py` & `cloudify-7.0.1/cloudify_cli/commands/sites.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/commands/snapshots.py` & `cloudify-7.0.1/cloudify_cli/commands/snapshots.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/commands/status.py` & `cloudify-7.0.1/cloudify_cli/commands/status.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/commands/summary.py` & `cloudify-7.0.1/cloudify_cli/commands/summary.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/commands/tenants.py` & `cloudify-7.0.1/cloudify_cli/commands/tenants.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/commands/tokens.py` & `cloudify-7.0.1/cloudify_cli/commands/tokens.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/commands/uninstall.py` & `cloudify-7.0.1/cloudify_cli/commands/uninstall.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,27 +22,29 @@
 
 
 @cfy.command(name='uninstall',
              short_help='Uninstall an application blueprint [manager only]')
 @cfy.argument('deployment-id')
 @cfy.options.workflow_id('uninstall')
 @cfy.options.force(help=helptexts.FORCE_CONCURRENT_EXECUTION)
+@cfy.options.recursive_delete
 @cfy.options.parameters
 @cfy.options.allow_custom_parameters
 @cfy.options.timeout()
 @cfy.options.include_logs
 @cfy.options.json_output
 @cfy.options.common_options
 @cfy.options.tenant_name(required=False,
                          resource_name_for_help='blueprint and deployment')
 @cfy.pass_context
 def manager(ctx,
             deployment_id,
             workflow_id,
             force,
+            recursive,
             parameters,
             allow_custom_parameters,
             timeout,
             include_logs,
             json_output,
             tenant_name):
     """Uninstall an application via the manager
@@ -53,14 +55,16 @@
     `DEPLOYMENT_ID` is the id of the deployment to uninstall.
     """
     env.assert_manager_active()
 
     # if no workflow was supplied, execute the `uninstall` workflow
     workflow_id = workflow_id or DEFAULT_UNINSTALL_WORKFLOW
 
+    if recursive:
+        parameters['recursive'] = True
     ctx.invoke(
         executions.manager_start,
         workflow_id=workflow_id,
         deployment_id=deployment_id,
         timeout=timeout,
         force=force,
         allow_custom_parameters=allow_custom_parameters,
@@ -75,15 +79,17 @@
     deployment = client.deployments.get(
         deployment_id, _include=['blueprint_id'])
     blueprint_id = deployment.blueprint_id
     ctx.invoke(
         deployments.manager_delete,
         deployment_id=deployment_id,
         force=force,
-        tenant_name=tenant_name)
+        tenant_name=tenant_name,
+        recursive=recursive,
+    )
     ctx.invoke(
         blueprints.delete,
         blueprint_id=blueprint_id,
         force=force,
         tenant_name=tenant_name)
```

### Comparing `cloudify-7.0.0/cloudify_cli/commands/user_groups.py` & `cloudify-7.0.1/cloudify_cli/commands/user_groups.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/commands/users.py` & `cloudify-7.0.1/cloudify_cli/commands/users.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/commands/workflows.py` & `cloudify-7.0.1/cloudify_cli/commands/workflows.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/config/__init__.py` & `cloudify-7.0.1/cloudify_cli/config/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/config/config.py` & `cloudify-7.0.1/cloudify_cli/config/config.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/constants.py` & `cloudify-7.0.1/cloudify_cli/constants.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/env.py` & `cloudify-7.0.1/cloudify_cli/env.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/exceptions.py` & `cloudify-7.0.1/cloudify_cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/execution_events_fetcher.py` & `cloudify-7.0.1/cloudify_cli/execution_events_fetcher.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/filters_utils.py` & `cloudify-7.0.1/cloudify_cli/filters_utils.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/inputs.py` & `cloudify-7.0.1/cloudify_cli/inputs.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/labels_utils.py` & `cloudify-7.0.1/cloudify_cli/labels_utils.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/local.py` & `cloudify-7.0.1/cloudify_cli/local.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/logger.py` & `cloudify-7.0.1/cloudify_cli/logger.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/main.py` & `cloudify-7.0.1/cloudify_cli/main.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/prettytable.py` & `cloudify-7.0.1/cloudify_cli/prettytable.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/replace_certificates_config.py` & `cloudify-7.0.1/cloudify_cli/replace_certificates_config.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/table.py` & `cloudify-7.0.1/cloudify_cli/table.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/cloudify_cli/utils.py` & `cloudify-7.0.1/cloudify_cli/utils.py`

 * *Files identical despite different names*

### Comparing `cloudify-7.0.0/setup.py` & `cloudify-7.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,29 +19,29 @@
 install_requires = [
         'click>8,<9',
         'wagon[venv]>=0.11.2',
         'retrying==1.3.3',
         'colorama==0.4.4',
         'requests>=2.7.0,<3.0.0',
         'click_didyoumean==0.3.0',
-        'cloudify-common[dispatcher]==7.0.0',
+        'cloudify-common[dispatcher]==7.0.1',
         'backports.shutil_get_terminal_size==1.0.0',
         'cryptography>=37,<40',
         'fabric==2.7.1',
 ]
 
 packages = ['cloudify_cli',
             'cloudify_cli.cli',
             'cloudify_cli.commands',
             'cloudify_cli.config',
             'cloudify_cli.async_commands']
 
 setup(
     name='cloudify',
-    version='7.0.0',
+    version='7.0.1',
     author='Cloudify',
     author_email='cosmo-admin@cloudify.co',
     packages=packages,
     license='LICENSE',
     description="Cloudify's Command Line Interface",
     entry_points={
         'console_scripts': [
```


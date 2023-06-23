# Comparing `tmp/cloudify-common-7.0.0.tar.gz` & `tmp/cloudify-common-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudify-common-7.0.0.tar", last modified: Tue Apr 25 11:53:36 2023, max compression
+gzip compressed data, was "cloudify-common-7.0.1.tar", last modified: Fri Jun 23 15:13:39 2023, max compression
```

## Comparing `cloudify-common-7.0.0.tar` & `cloudify-common-7.0.1.tar`

### file list

```diff
@@ -1,183 +1,183 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:53:36.558777 cloudify-common-7.0.0/
--rw-r--r--   0 root         (0) root         (0)    10273 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       39 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      226 2023-04-25 11:53:36.558777 cloudify-common-7.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3034 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:53:36.534777 cloudify-common-7.0.0/cloudify/
--rw-r--r--   0 root         (0) root         (0)     2286 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5056 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/agent_utils.py
--rw-r--r--   0 root         (0) root         (0)    23830 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/amqp_client.py
--rw-r--r--   0 root         (0) root         (0)     4028 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/cluster.py
--rw-r--r--   0 root         (0) root         (0)     1335 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/cluster_status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:53:36.534777 cloudify-common-7.0.0/cloudify/compute/
--rw-r--r--   0 root         (0) root         (0)     4460 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/compute/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1302 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/conflict_handlers.py
--rw-r--r--   0 root         (0) root         (0)     4385 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/constants.py
--rw-r--r--   0 root         (0) root         (0)    47099 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/context.py
--rw-r--r--   0 root         (0) root         (0)     3855 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/cryptography_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:53:36.534777 cloudify-common-7.0.0/cloudify/ctx_wrappers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/ctx_wrappers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8328 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/ctx_wrappers/ctx-py.py
--rw-r--r--   0 root         (0) root         (0)     4271 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/decorators.py
--rw-r--r--   0 root         (0) root         (0)     3394 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/deployment_dependencies.py
--rw-r--r--   0 root         (0) root         (0)    18954 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/dispatch.py
--rw-r--r--   0 root         (0) root         (0)    19018 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/endpoint.py
--rw-r--r--   0 root         (0) root         (0)     3741 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/error_handling.py
--rw-r--r--   0 root         (0) root         (0)     4872 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/event.py
--rw-r--r--   0 root         (0) root         (0)     5918 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    15865 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/logs.py
--rw-r--r--   0 root         (0) root         (0)    18303 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/manager.py
--rw-r--r--   0 root         (0) root         (0)     7829 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/mocks.py
--rw-r--r--   0 root         (0) root         (0)     4914 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/models_states.py
--rw-r--r--   0 root         (0) root         (0)    20337 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/plugin_installer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:53:36.534777 cloudify-common-7.0.0/cloudify/plugins/
--rw-r--r--   0 root         (0) root         (0)      643 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1213 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/plugins/install_utils.py
--rw-r--r--   0 root         (0) root         (0)    53945 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/plugins/lifecycle.py
--rw-r--r--   0 root         (0) root         (0)    56356 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/plugins/workflows.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:53:36.534777 cloudify-common-7.0.0/cloudify/proxy/
--rw-r--r--   0 root         (0) root         (0)      637 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/proxy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3965 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/proxy/client.py
--rw-r--r--   0 root         (0) root         (0)     8157 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/proxy/server.py
--rw-r--r--   0 root         (0) root         (0)     6223 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/rabbitmq_client.py
--rw-r--r--   0 root         (0) root         (0)      832 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/snapshots.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:53:36.534777 cloudify-common-7.0.0/cloudify/snmp/
--rw-r--r--   0 root         (0) root         (0)     5393 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/snmp/CLOUDIFY-MIB.mib
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/snmp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4934 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/snmp/snmp_trap.py
--rw-r--r--   0 root         (0) root         (0)     3054 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/state.py
--rw-r--r--   0 root         (0) root         (0)     2330 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/systemddbus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:53:36.534777 cloudify-common-7.0.0/cloudify/test_utils/
--rw-r--r--   0 root         (0) root         (0)      751 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/test_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      999 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/test_utils/dispatch_helper.py
--rw-r--r--   0 root         (0) root         (0)    11243 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/test_utils/local_workflow_decorator.py
--rw-r--r--   0 root         (0) root         (0)     3892 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/test_utils/mock_rest_client.py
--rw-r--r--   0 root         (0) root         (0)    37803 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:53:36.538777 cloudify-common-7.0.0/cloudify/workflows/
--rw-r--r--   0 root         (0) root         (0)      848 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/workflows/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8618 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/workflows/amqp_dispatcher.py
--rw-r--r--   0 root         (0) root         (0)     5562 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/workflows/events.py
--rw-r--r--   0 root         (0) root         (0)    36444 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/workflows/local.py
--rw-r--r--   0 root         (0) root         (0)    40724 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/workflows/tasks.py
--rw-r--r--   0 root         (0) root         (0)    26098 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/workflows/tasks_graph.py
--rw-r--r--   0 root         (0) root         (0)     2782 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/workflows/workflow_api.py
--rw-r--r--   0 root         (0) root         (0)    80330 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/workflows/workflow_context.py
--rw-r--r--   0 root         (0) root         (0)     1746 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify/zip_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:53:36.538777 cloudify-common-7.0.0/cloudify_async_client/
--rw-r--r--   0 root         (0) root         (0)       69 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_async_client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1258 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_async_client/audit_log.py
--rw-r--r--   0 root         (0) root         (0)     1530 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_async_client/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:53:36.538777 cloudify-common-7.0.0/cloudify_common.egg-info/
--rw-r--r--   0 root         (0) root         (0)      226 2023-04-25 11:53:36.000000 cloudify-common-7.0.0/cloudify_common.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4997 2023-04-25 11:53:36.000000 cloudify-common-7.0.0/cloudify_common.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 11:53:36.000000 cloudify-common-7.0.0/cloudify_common.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2023-04-25 11:53:36.000000 cloudify-common-7.0.0/cloudify_common.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 11:53:36.000000 cloudify-common-7.0.0/cloudify_common.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      242 2023-04-25 11:53:36.000000 cloudify-common-7.0.0/cloudify_common.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       77 2023-04-25 11:53:36.000000 cloudify-common-7.0.0/cloudify_common.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:53:36.550778 cloudify-common-7.0.0/cloudify_rest_client/
--rw-r--r--   0 root         (0) root         (0)      731 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4122 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/_datetime_compat.py
--rw-r--r--   0 root         (0) root         (0)     7494 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/agents.py
--rw-r--r--   0 root         (0) root         (0)     3565 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/audit_log.py
--rw-r--r--   0 root         (0) root         (0)    23374 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/blueprints.py
--rw-r--r--   0 root         (0) root         (0)     3766 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/bytes_stream_utils.py
--rw-r--r--   0 root         (0) root         (0)    22799 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/client.py
--rw-r--r--   0 root         (0) root         (0)     1009 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/cluster.py
--rw-r--r--   0 root         (0) root         (0)     1205 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/community_contacts.py
--rw-r--r--   0 root         (0) root         (0)     1077 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/constants.py
--rw-r--r--   0 root         (0) root         (0)     6367 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/deployment_modifications.py
--rw-r--r--   0 root         (0) root         (0)     8791 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/deployment_updates.py
--rw-r--r--   0 root         (0) root         (0)    34027 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/deployments.py
--rw-r--r--   0 root         (0) root         (0)     1963 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/evaluate.py
--rw-r--r--   0 root         (0) root         (0)     5855 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/events.py
--rw-r--r--   0 root         (0) root         (0)    10493 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    11252 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/execution_schedules.py
--rw-r--r--   0 root         (0) root         (0)    18715 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/executions.py
--rw-r--r--   0 root         (0) root         (0)     4817 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/filters.py
--rw-r--r--   0 root         (0) root         (0)      284 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/idp.py
--rw-r--r--   0 root         (0) root         (0)     9024 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/inter_deployment_dependencies.py
--rw-r--r--   0 root         (0) root         (0)     1852 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/labels.py
--rw-r--r--   0 root         (0) root         (0)     3760 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/ldap.py
--rw-r--r--   0 root         (0) root         (0)     2886 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/license.py
--rw-r--r--   0 root         (0) root         (0)     4568 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/log_bundles.py
--rw-r--r--   0 root         (0) root         (0)     2947 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/maintenance.py
--rw-r--r--   0 root         (0) root         (0)    15074 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/manager.py
--rw-r--r--   0 root         (0) root         (0)    10973 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/node_instances.py
--rw-r--r--   0 root         (0) root         (0)    11333 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/nodes.py
--rw-r--r--   0 root         (0) root         (0)     6699 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/operations.py
--rw-r--r--   0 root         (0) root         (0)     1432 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/permissions.py
--rw-r--r--   0 root         (0) root         (0)    15934 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/plugins.py
--rw-r--r--   0 root         (0) root         (0)     7141 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/plugins_update.py
--rw-r--r--   0 root         (0) root         (0)    11395 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/resources.py
--rw-r--r--   0 root         (0) root         (0)     2800 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/responses.py
--rw-r--r--   0 root         (0) root         (0)     8474 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/secrets.py
--rw-r--r--   0 root         (0) root         (0)     6019 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/secrets_providers.py
--rw-r--r--   0 root         (0) root         (0)     5032 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/sites.py
--rw-r--r--   0 root         (0) root         (0)     8391 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/snapshots.py
--rw-r--r--   0 root         (0) root         (0)     1708 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/summary.py
--rw-r--r--   0 root         (0) root         (0)     6841 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/tenants.py
--rw-r--r--   0 root         (0) root         (0)     2891 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/tokens.py
--rw-r--r--   0 root         (0) root         (0)     3840 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/user_groups.py
--rw-r--r--   0 root         (0) root         (0)     5324 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/users.py
--rw-r--r--   0 root         (0) root         (0)     4076 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/utils.py
--rw-r--r--   0 root         (0) root         (0)     1851 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/cloudify_rest_client/workflows.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:53:36.550778 cloudify-common-7.0.0/ctx_wrappers/
--rw-r--r--   0 root         (0) root         (0)       71 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/ctx_wrappers/ctx-sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:53:36.554777 cloudify-common-7.0.0/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)      637 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4856 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/constants.py
--rw-r--r--   0 root         (0) root         (0)    19171 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/constraints.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:53:36.554777 cloudify-common-7.0.0/dsl_parser/elements/
--rw-r--r--   0 root         (0) root         (0)      712 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/elements/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5669 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/elements/blueprint.py
--rw-r--r--   0 root         (0) root         (0)    10177 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/elements/data_types.py
--rw-r--r--   0 root         (0) root         (0)     4985 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/elements/deployment_schedules.py
--rw-r--r--   0 root         (0) root         (0)    31837 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/elements/imports.py
--rw-r--r--   0 root         (0) root         (0)     6358 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/elements/inputs.py
--rw-r--r--   0 root         (0) root         (0)     6044 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/elements/misc.py
--rw-r--r--   0 root         (0) root         (0)    25808 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/elements/node_templates.py
--rw-r--r--   0 root         (0) root         (0)     3767 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/elements/node_types.py
--rw-r--r--   0 root         (0) root         (0)    16633 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/elements/operation.py
--rw-r--r--   0 root         (0) root         (0)     5413 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/elements/plugins.py
--rw-r--r--   0 root         (0) root         (0)    19699 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/elements/policies.py
--rw-r--r--   0 root         (0) root         (0)     4018 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/elements/relationships.py
--rw-r--r--   0 root         (0) root         (0)     6098 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/elements/scalable.py
--rw-r--r--   0 root         (0) root         (0)     2359 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/elements/types.py
--rw-r--r--   0 root         (0) root         (0)     1485 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/elements/version.py
--rw-r--r--   0 root         (0) root         (0)     8400 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/elements/workflows.py
--rw-r--r--   0 root         (0) root         (0)     5578 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:53:36.554777 cloudify-common-7.0.0/dsl_parser/framework/
--rw-r--r--   0 root         (0) root         (0)      637 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/framework/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7859 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/framework/elements.py
--rw-r--r--   0 root         (0) root         (0)    31720 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/framework/parser.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/framework/requirements.py
--rw-r--r--   0 root         (0) root         (0)    71265 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/functions.py
--rw-r--r--   0 root         (0) root         (0)     5031 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/holder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:53:36.554777 cloudify-common-7.0.0/dsl_parser/import_resolver/
--rw-r--r--   0 root         (0) root         (0)      637 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/import_resolver/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5209 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/import_resolver/abstract_import_resolver.py
--rw-r--r--   0 root         (0) root         (0)     7670 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/import_resolver/default_import_resolver.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:53:36.558777 cloudify-common-7.0.0/dsl_parser/interfaces/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/interfaces/__init__.py
--rw-r--r--   0 root         (0) root         (0)      813 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/interfaces/constants.py
--rw-r--r--   0 root         (0) root         (0)     3932 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/interfaces/interfaces_merger.py
--rw-r--r--   0 root         (0) root         (0)     2339 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/interfaces/interfaces_parser.py
--rw-r--r--   0 root         (0) root         (0)    10119 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/interfaces/operation_merger.py
--rw-r--r--   0 root         (0) root         (0)     3934 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/interfaces/utils.py
--rw-r--r--   0 root         (0) root         (0)     1710 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/models.py
--rw-r--r--   0 root         (0) root         (0)     4636 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/multi_instance.py
--rw-r--r--   0 root         (0) root         (0)     5833 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/parser.py
--rw-r--r--   0 root         (0) root         (0)    43420 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/rel_graph.py
--rw-r--r--   0 root         (0) root         (0)     8644 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/scan.py
--rw-r--r--   0 root         (0) root         (0)    12187 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/tasks.py
--rw-r--r--   0 root         (0) root         (0)    18600 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/utils.py
--rw-r--r--   0 root         (0) root         (0)     4288 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/version.py
--rw-r--r--   0 root         (0) root         (0)     5530 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/dsl_parser/yaml_loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:53:36.558777 cloudify-common-7.0.0/script_runner/
--rw-r--r--   0 root         (0) root         (0)      637 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/script_runner/__init__.py
--rw-r--r--   0 root         (0) root         (0)      124 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/script_runner/constants.py
--rw-r--r--   0 root         (0) root         (0)      984 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/script_runner/eval_env.py
--rw-r--r--   0 root         (0) root         (0)    16145 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/script_runner/tasks.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 11:53:36.558777 cloudify-common-7.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1381 2023-04-25 11:53:17.000000 cloudify-common-7.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:13:39.878526 cloudify-common-7.0.1/
+-rw-r--r--   0 root         (0) root         (0)    10273 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       39 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      226 2023-06-23 15:13:39.878526 cloudify-common-7.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3034 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:13:39.858527 cloudify-common-7.0.1/cloudify/
+-rw-r--r--   0 root         (0) root         (0)     2286 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5056 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/agent_utils.py
+-rw-r--r--   0 root         (0) root         (0)    23830 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/amqp_client.py
+-rw-r--r--   0 root         (0) root         (0)     4028 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/cluster.py
+-rw-r--r--   0 root         (0) root         (0)     1335 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/cluster_status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:13:39.858527 cloudify-common-7.0.1/cloudify/compute/
+-rw-r--r--   0 root         (0) root         (0)     4460 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/compute/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1302 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/conflict_handlers.py
+-rw-r--r--   0 root         (0) root         (0)     4385 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/constants.py
+-rw-r--r--   0 root         (0) root         (0)    47193 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/context.py
+-rw-r--r--   0 root         (0) root         (0)     3855 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/cryptography_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:13:39.858527 cloudify-common-7.0.1/cloudify/ctx_wrappers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/ctx_wrappers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8328 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/ctx_wrappers/ctx-py.py
+-rw-r--r--   0 root         (0) root         (0)     4271 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/decorators.py
+-rw-r--r--   0 root         (0) root         (0)     3394 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/deployment_dependencies.py
+-rw-r--r--   0 root         (0) root         (0)    18954 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/dispatch.py
+-rw-r--r--   0 root         (0) root         (0)    19168 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/endpoint.py
+-rw-r--r--   0 root         (0) root         (0)     3741 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/error_handling.py
+-rw-r--r--   0 root         (0) root         (0)     4872 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/event.py
+-rw-r--r--   0 root         (0) root         (0)     5918 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    15865 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/logs.py
+-rw-r--r--   0 root         (0) root         (0)    18303 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/manager.py
+-rw-r--r--   0 root         (0) root         (0)     7829 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/mocks.py
+-rw-r--r--   0 root         (0) root         (0)     4914 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/models_states.py
+-rw-r--r--   0 root         (0) root         (0)    20337 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/plugin_installer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:13:39.862527 cloudify-common-7.0.1/cloudify/plugins/
+-rw-r--r--   0 root         (0) root         (0)      643 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1213 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/plugins/install_utils.py
+-rw-r--r--   0 root         (0) root         (0)    53945 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/plugins/lifecycle.py
+-rw-r--r--   0 root         (0) root         (0)    59556 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/plugins/workflows.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:13:39.862527 cloudify-common-7.0.1/cloudify/proxy/
+-rw-r--r--   0 root         (0) root         (0)      637 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/proxy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3965 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/proxy/client.py
+-rw-r--r--   0 root         (0) root         (0)     8157 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/proxy/server.py
+-rw-r--r--   0 root         (0) root         (0)     6223 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/rabbitmq_client.py
+-rw-r--r--   0 root         (0) root         (0)      832 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/snapshots.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:13:39.862527 cloudify-common-7.0.1/cloudify/snmp/
+-rw-r--r--   0 root         (0) root         (0)     5393 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/snmp/CLOUDIFY-MIB.mib
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/snmp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4934 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/snmp/snmp_trap.py
+-rw-r--r--   0 root         (0) root         (0)     3054 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/state.py
+-rw-r--r--   0 root         (0) root         (0)     2330 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/systemddbus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:13:39.862527 cloudify-common-7.0.1/cloudify/test_utils/
+-rw-r--r--   0 root         (0) root         (0)      751 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/test_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      999 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/test_utils/dispatch_helper.py
+-rw-r--r--   0 root         (0) root         (0)    11243 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/test_utils/local_workflow_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     3892 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/test_utils/mock_rest_client.py
+-rw-r--r--   0 root         (0) root         (0)    37803 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:13:39.862527 cloudify-common-7.0.1/cloudify/workflows/
+-rw-r--r--   0 root         (0) root         (0)      848 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/workflows/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8618 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/workflows/amqp_dispatcher.py
+-rw-r--r--   0 root         (0) root         (0)     5562 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/workflows/events.py
+-rw-r--r--   0 root         (0) root         (0)    36444 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/workflows/local.py
+-rw-r--r--   0 root         (0) root         (0)    40724 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/workflows/tasks.py
+-rw-r--r--   0 root         (0) root         (0)    26098 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/workflows/tasks_graph.py
+-rw-r--r--   0 root         (0) root         (0)     2782 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/workflows/workflow_api.py
+-rw-r--r--   0 root         (0) root         (0)    80337 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/workflows/workflow_context.py
+-rw-r--r--   0 root         (0) root         (0)     1746 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify/zip_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:13:39.862527 cloudify-common-7.0.1/cloudify_async_client/
+-rw-r--r--   0 root         (0) root         (0)       69 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_async_client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1258 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_async_client/audit_log.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_async_client/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:13:39.866527 cloudify-common-7.0.1/cloudify_common.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      226 2023-06-23 15:13:39.000000 cloudify-common-7.0.1/cloudify_common.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4997 2023-06-23 15:13:39.000000 cloudify-common-7.0.1/cloudify_common.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 15:13:39.000000 cloudify-common-7.0.1/cloudify_common.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2023-06-23 15:13:39.000000 cloudify-common-7.0.1/cloudify_common.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 15:13:39.000000 cloudify-common-7.0.1/cloudify_common.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      242 2023-06-23 15:13:39.000000 cloudify-common-7.0.1/cloudify_common.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       77 2023-06-23 15:13:39.000000 cloudify-common-7.0.1/cloudify_common.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:13:39.870526 cloudify-common-7.0.1/cloudify_rest_client/
+-rw-r--r--   0 root         (0) root         (0)      731 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4122 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/_datetime_compat.py
+-rw-r--r--   0 root         (0) root         (0)     8814 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/agents.py
+-rw-r--r--   0 root         (0) root         (0)     3565 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/audit_log.py
+-rw-r--r--   0 root         (0) root         (0)    25807 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/blueprints.py
+-rw-r--r--   0 root         (0) root         (0)     3766 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/bytes_stream_utils.py
+-rw-r--r--   0 root         (0) root         (0)    22799 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/client.py
+-rw-r--r--   0 root         (0) root         (0)     1009 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/cluster.py
+-rw-r--r--   0 root         (0) root         (0)     1205 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/community_contacts.py
+-rw-r--r--   0 root         (0) root         (0)      435 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/constants.py
+-rw-r--r--   0 root         (0) root         (0)     6367 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/deployment_modifications.py
+-rw-r--r--   0 root         (0) root         (0)    10221 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/deployment_updates.py
+-rw-r--r--   0 root         (0) root         (0)    38732 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/deployments.py
+-rw-r--r--   0 root         (0) root         (0)     1963 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/evaluate.py
+-rw-r--r--   0 root         (0) root         (0)    11374 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/events.py
+-rw-r--r--   0 root         (0) root         (0)    10493 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    12947 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/execution_schedules.py
+-rw-r--r--   0 root         (0) root         (0)    22132 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/executions.py
+-rw-r--r--   0 root         (0) root         (0)     6266 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/filters.py
+-rw-r--r--   0 root         (0) root         (0)      284 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/idp.py
+-rw-r--r--   0 root         (0) root         (0)    10537 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/inter_deployment_dependencies.py
+-rw-r--r--   0 root         (0) root         (0)     1852 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/labels.py
+-rw-r--r--   0 root         (0) root         (0)     3760 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/ldap.py
+-rw-r--r--   0 root         (0) root         (0)     2886 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/license.py
+-rw-r--r--   0 root         (0) root         (0)     4568 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/log_bundles.py
+-rw-r--r--   0 root         (0) root         (0)     2947 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/maintenance.py
+-rw-r--r--   0 root         (0) root         (0)    15074 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/manager.py
+-rw-r--r--   0 root         (0) root         (0)    13494 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/node_instances.py
+-rw-r--r--   0 root         (0) root         (0)    13368 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/nodes.py
+-rw-r--r--   0 root         (0) root         (0)    10417 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/operations.py
+-rw-r--r--   0 root         (0) root         (0)     2489 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/permissions.py
+-rw-r--r--   0 root         (0) root         (0)    17819 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/plugins.py
+-rw-r--r--   0 root         (0) root         (0)     8930 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/plugins_update.py
+-rw-r--r--   0 root         (0) root         (0)    11395 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/resources.py
+-rw-r--r--   0 root         (0) root         (0)     2800 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/responses.py
+-rw-r--r--   0 root         (0) root         (0)     9516 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/secrets.py
+-rw-r--r--   0 root         (0) root         (0)     7514 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/secrets_providers.py
+-rw-r--r--   0 root         (0) root         (0)     5680 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/sites.py
+-rw-r--r--   0 root         (0) root         (0)     8391 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/snapshots.py
+-rw-r--r--   0 root         (0) root         (0)     1708 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/summary.py
+-rw-r--r--   0 root         (0) root         (0)     7510 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/tenants.py
+-rw-r--r--   0 root         (0) root         (0)     2891 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/tokens.py
+-rw-r--r--   0 root         (0) root         (0)     4578 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/user_groups.py
+-rw-r--r--   0 root         (0) root         (0)     6921 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/users.py
+-rw-r--r--   0 root         (0) root         (0)     4706 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1851 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/cloudify_rest_client/workflows.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:13:39.870526 cloudify-common-7.0.1/ctx_wrappers/
+-rw-r--r--   0 root         (0) root         (0)       71 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/ctx_wrappers/ctx-sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:13:39.870526 cloudify-common-7.0.1/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)      637 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4856 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/constants.py
+-rw-r--r--   0 root         (0) root         (0)    19171 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/constraints.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:13:39.874526 cloudify-common-7.0.1/dsl_parser/elements/
+-rw-r--r--   0 root         (0) root         (0)      712 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/elements/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5669 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/elements/blueprint.py
+-rw-r--r--   0 root         (0) root         (0)    10177 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/elements/data_types.py
+-rw-r--r--   0 root         (0) root         (0)     4985 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/elements/deployment_schedules.py
+-rw-r--r--   0 root         (0) root         (0)    31837 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/elements/imports.py
+-rw-r--r--   0 root         (0) root         (0)     6358 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/elements/inputs.py
+-rw-r--r--   0 root         (0) root         (0)     6044 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/elements/misc.py
+-rw-r--r--   0 root         (0) root         (0)    25808 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/elements/node_templates.py
+-rw-r--r--   0 root         (0) root         (0)     3767 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/elements/node_types.py
+-rw-r--r--   0 root         (0) root         (0)    15763 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/elements/operation.py
+-rw-r--r--   0 root         (0) root         (0)     5413 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/elements/plugins.py
+-rw-r--r--   0 root         (0) root         (0)    19699 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/elements/policies.py
+-rw-r--r--   0 root         (0) root         (0)     4018 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/elements/relationships.py
+-rw-r--r--   0 root         (0) root         (0)     6098 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/elements/scalable.py
+-rw-r--r--   0 root         (0) root         (0)     2359 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/elements/types.py
+-rw-r--r--   0 root         (0) root         (0)     1485 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/elements/version.py
+-rw-r--r--   0 root         (0) root         (0)     8400 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/elements/workflows.py
+-rw-r--r--   0 root         (0) root         (0)     5578 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:13:39.874526 cloudify-common-7.0.1/dsl_parser/framework/
+-rw-r--r--   0 root         (0) root         (0)      637 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/framework/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7859 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/framework/elements.py
+-rw-r--r--   0 root         (0) root         (0)    31720 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/framework/parser.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/framework/requirements.py
+-rw-r--r--   0 root         (0) root         (0)    71949 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/functions.py
+-rw-r--r--   0 root         (0) root         (0)     5031 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/holder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:13:39.874526 cloudify-common-7.0.1/dsl_parser/import_resolver/
+-rw-r--r--   0 root         (0) root         (0)      637 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/import_resolver/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5209 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/import_resolver/abstract_import_resolver.py
+-rw-r--r--   0 root         (0) root         (0)     7670 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/import_resolver/default_import_resolver.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:13:39.874526 cloudify-common-7.0.1/dsl_parser/interfaces/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/interfaces/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      813 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/interfaces/constants.py
+-rw-r--r--   0 root         (0) root         (0)     3932 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/interfaces/interfaces_merger.py
+-rw-r--r--   0 root         (0) root         (0)     2339 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/interfaces/interfaces_parser.py
+-rw-r--r--   0 root         (0) root         (0)    10119 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/interfaces/operation_merger.py
+-rw-r--r--   0 root         (0) root         (0)     3934 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/interfaces/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1710 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/models.py
+-rw-r--r--   0 root         (0) root         (0)     4636 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/multi_instance.py
+-rw-r--r--   0 root         (0) root         (0)     5833 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/parser.py
+-rw-r--r--   0 root         (0) root         (0)    43420 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/rel_graph.py
+-rw-r--r--   0 root         (0) root         (0)     8644 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/scan.py
+-rw-r--r--   0 root         (0) root         (0)    12442 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/tasks.py
+-rw-r--r--   0 root         (0) root         (0)    18600 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4288 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/version.py
+-rw-r--r--   0 root         (0) root         (0)     5530 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/dsl_parser/yaml_loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:13:39.878526 cloudify-common-7.0.1/script_runner/
+-rw-r--r--   0 root         (0) root         (0)      637 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/script_runner/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      124 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/script_runner/constants.py
+-rw-r--r--   0 root         (0) root         (0)      984 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/script_runner/eval_env.py
+-rw-r--r--   0 root         (0) root         (0)    16145 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/script_runner/tasks.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 15:13:39.878526 cloudify-common-7.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1381 2023-06-23 15:13:17.000000 cloudify-common-7.0.1/setup.py
```

### Comparing `cloudify-common-7.0.0/LICENSE` & `cloudify-common-7.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/README.md` & `cloudify-common-7.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/__init__.py` & `cloudify-common-7.0.1/cloudify/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/agent_utils.py` & `cloudify-common-7.0.1/cloudify/agent_utils.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/amqp_client.py` & `cloudify-common-7.0.1/cloudify/amqp_client.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/cluster.py` & `cloudify-common-7.0.1/cloudify/cluster.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/cluster_status.py` & `cloudify-common-7.0.1/cloudify/cluster_status.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/compute/__init__.py` & `cloudify-common-7.0.1/cloudify/compute/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/conflict_handlers.py` & `cloudify-common-7.0.1/cloudify/conflict_handlers.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/constants.py` & `cloudify-common-7.0.1/cloudify/constants.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/context.py` & `cloudify-common-7.0.1/cloudify/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -399,15 +399,18 @@
     def __init__(self, *args, **kwargs):
         super(NodeContext, self).__init__(*args, **kwargs)
         self._endpoint = kwargs['endpoint']
         self._node = None
 
     def _get_node_if_needed(self):
         if self._node is None:
-            self._node = self._endpoint.get_node(self.id)
+            self._node = self._endpoint.get_node(
+                self.id,
+                instance_context=self._context.get('node_id'),
+            )
             props = self._node.get('properties', {})
             self._node['properties'] = ImmutableProperties(props)
 
     @property
     def id(self):
         """The node's id"""
         return self.name
```

### Comparing `cloudify-common-7.0.0/cloudify/cryptography_utils.py` & `cloudify-common-7.0.1/cloudify/cryptography_utils.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/ctx_wrappers/ctx-py.py` & `cloudify-common-7.0.1/cloudify/ctx_wrappers/ctx-py.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/decorators.py` & `cloudify-common-7.0.1/cloudify/decorators.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/deployment_dependencies.py` & `cloudify-common-7.0.1/cloudify/deployment_dependencies.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/dispatch.py` & `cloudify-common-7.0.1/cloudify/dispatch.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/endpoint.py` & `cloudify-common-7.0.1/cloudify/endpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 
 class Endpoint(object):
 
     def __init__(self, ctx):
         self.ctx = ctx
 
-    def get_node(self, node_id):
+    def get_node(self, node_id, instance_context=None):
         raise NotImplementedError('Implemented by subclasses')
 
     def get_node_instance(self, node_instance_id):
         raise NotImplementedError('Implemented by subclasses')
 
     def update_node_instance(self, node_instance):
         raise NotImplementedError('Implemented by subclasses')
@@ -192,17 +192,21 @@
 
     @property
     def rest_client(self):
         if self._rest_client is None:
             self._rest_client = manager.get_rest_client(self.ctx.tenant_name)
         return self._rest_client
 
-    def get_node(self, node_id):
+    def get_node(self, node_id, instance_context=None):
         return self.rest_client.nodes.get(
-            self.ctx.deployment.id, node_id, evaluate_functions=True)
+            self.ctx.deployment.id,
+            node_id,
+            evaluate_functions=True,
+            instance_context=instance_context,
+        )
 
     def get_node_instance(self, node_instance_id):
         return manager.get_node_instance(node_instance_id,
                                          evaluate_functions=True,
                                          client=self.rest_client)
 
     def get_managers(self, network='default'):
@@ -369,15 +373,15 @@
 
 class LocalEndpoint(Endpoint):
 
     def __init__(self, ctx, storage):
         super(LocalEndpoint, self).__init__(ctx)
         self.storage = storage
 
-    def get_node(self, node_id):
+    def get_node(self, node_id, instance_context=None):
         return self.storage.get_node(node_id)
 
     def get_node_instance(self, node_instance_id):
         instance = self.storage.get_node_instance(node_instance_id)
         return manager.NodeInstance(
             node_instance_id,
             instance.node_id,
```

### Comparing `cloudify-common-7.0.0/cloudify/error_handling.py` & `cloudify-common-7.0.1/cloudify/error_handling.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/event.py` & `cloudify-common-7.0.1/cloudify/event.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/exceptions.py` & `cloudify-common-7.0.1/cloudify/exceptions.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/logs.py` & `cloudify-common-7.0.1/cloudify/logs.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/manager.py` & `cloudify-common-7.0.1/cloudify/manager.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/mocks.py` & `cloudify-common-7.0.1/cloudify/mocks.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/models_states.py` & `cloudify-common-7.0.1/cloudify/models_states.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/plugin_installer.py` & `cloudify-common-7.0.1/cloudify/plugin_installer.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/plugins/__init__.py` & `cloudify-common-7.0.1/cloudify/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/plugins/install_utils.py` & `cloudify-common-7.0.1/cloudify/plugins/install_utils.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/plugins/lifecycle.py` & `cloudify-common-7.0.1/cloudify/plugins/lifecycle.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/plugins/workflows.py` & `cloudify-common-7.0.1/cloudify/plugins/workflows.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,20 +11,24 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 #    * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    * See the License for the specific language governing permissions and
 #    * limitations under the License.
 
 import numbers
 import threading
+import time
 from itertools import chain
 from datetime import datetime
 
 from cloudify import constants, utils
 from cloudify.decorators import workflow
+from cloudify.manager import get_rest_client
+from cloudify.models_states import ExecutionState
 from cloudify.plugins import lifecycle
+from cloudify.workflows import api
 from cloudify.workflows.tasks_graph import make_or_get_graph
 from cloudify.workflows.tasks import HandlerResult, TASK_SUCCEEDED
 
 
 @workflow(resumable=True)
 def install(ctx, node_ids=None, node_instance_ids=None, type_names=None,
             **kwargs):
@@ -38,18 +42,106 @@
     lifecycle.install_node_instances(
         graph=ctx.graph_mode(),
         node_instances=filtered_node_instances,
         related_nodes=set(ctx.node_instances) - filtered_node_instances,
     )
 
 
+def _uninstall_contained_services(
+    ctx,
+    ignore_failure=False,
+    node_ids=None,
+    node_instance_ids=None,
+    type_names=None,
+    **kwargs,
+):
+    """Uninstall service deployments recursively
+
+    Service deployments are deployments that are using the current
+    deployment as an environment.
+    """
+    # this uses the rest-client directly, which is a bit ugly, and not
+    # going to be supported on cfy local (which environments aren't supported
+    # on either)
+    ctx.logger.info('Uninstalling service deployments recursively')
+    client = get_rest_client(tenant=ctx.tenant_name)
+
+    # create a deployment group containing the service deployments
+    # to be uninstalled
+    group_id = f'{ctx.deployment.id}_services_uninstall'
+    client.deployment_groups.put(group_id)
+    client.deployment_groups.add_deployments(
+        group_id,
+        filter_rules=[{
+            'key': 'csys-obj-parent',
+            'values': [ctx.deployment.id],
+            'operator': 'any_of',
+            'type': 'label',
+        }]
+    )
+
+    # uninstall all the service deployments, with the same arguments that
+    # we're using
+    uninstall_parameters = {
+        'ignore_failure': ignore_failure,
+        'node_ids': node_ids,
+        'node_instance_ids': node_instance_ids,
+        'type_names': type_names,
+        'recursive': True,
+    }
+    uninstall_parameters.update(kwargs)
+    exc_group = client.execution_groups.start(
+        group_id,
+        ctx.workflow_id,
+        default_parameters=uninstall_parameters,
+    )
+
+    last_log = time.time()
+    while not api.has_cancel_request():
+        # wait for the execution group to finish.
+        # I wish I was able to just poll excgroup.status, but that doesn't
+        # seem to work - to be fixed in RND-652.
+        # Instead, list the in-flight executions, and wait until there's
+        # none of them.
+        still_waiting = client.executions.list(
+            execution_group_id=exc_group.id,
+            status=(
+                ExecutionState.WAITING_STATES
+                + ExecutionState.IN_PROGRESS_STATES
+            ),
+        )
+        if len(still_waiting) == 0:
+            break
+        if time.time() - last_log > 600:
+            ctx.logger.info(
+                'Still waiting for %d service deployments to be uninstalled',
+                len(still_waiting),
+            )
+            last_log = time.time()
+
+        time.sleep(1)
+
+    client.deployment_groups.delete(group_id)
+    ctx.logger.info('Service deployments uninstalled')
+
+
 @workflow(resumable=True)
 def uninstall(ctx, ignore_failure=False, node_ids=None, node_instance_ids=None,
-              type_names=None, **kwargs):
+              type_names=None, recursive=False, **kwargs):
     """Default uninstall workflow"""
+    if recursive:
+        _uninstall_contained_services(
+            ctx,
+            ignore_failure=ignore_failure,
+            node_ids=node_ids,
+            node_instance_ids=node_instance_ids,
+            type_names=type_names,
+            **kwargs,
+        )
+
     filtered_node_instances = set(_filter_node_instances(
         ctx=ctx,
         node_ids=node_ids,
         node_instance_ids=node_instance_ids,
         type_names=type_names))
 
     lifecycle.uninstall_node_instances(
@@ -655,14 +747,15 @@
 
                 # Node instances denoted by these instance ids should
                 # be *removed* if possible.
                 # 'removed_ids_include_hint': []
             }
         })
     ctx.refresh_node_instances()
+    graph_name_prefix = scalable_entity_name + '_'
     graph = ctx.graph_mode()
     try:
         ctx.logger.info('Deployment modification started. '
                         '[modification_id={0}]'.format(modification.id))
         if delta > 0:
             added = {
                 ctx.get_node_instance(i.id)
@@ -674,15 +767,17 @@
                 for i in modification.added.node_instances
                 if i.modification != 'added'
             }
             try:
                 lifecycle.install_node_instances(
                     graph=graph,
                     node_instances=added,
-                    related_nodes=related)
+                    related_nodes=related,
+                    name_prefix=graph_name_prefix,
+                )
             except Exception:
                 if not rollback_if_failed:
                     ctx.logger.error('Scale out failed.')
                     raise
                 ctx.logger.error('Scale out failed, scaling back in.')
                 for task in graph.tasks:
                     graph.remove_task(task)
@@ -696,15 +791,17 @@
                     if i.modification == 'added'
                 }
 
                 lifecycle.rollback_node_instances(
                     graph=graph,
                     node_instances=added,
                     ignore_failure=ignore_failure,
-                    related_nodes=related)
+                    related_nodes=related,
+                    name_prefix=graph_name_prefix,
+                )
                 raise
         else:
             removed = {
                 ctx.get_node_instance(i.id)
                 for i in modification.removed.node_instances
                 if i.modification == 'removed'
             }
@@ -713,15 +810,17 @@
                 for i in modification.removed.node_instances
                 if i.modification != 'removed'
             }
             lifecycle.uninstall_node_instances(
                 graph=graph,
                 node_instances=removed,
                 ignore_failure=ignore_failure,
-                related_nodes=related)
+                related_nodes=related,
+                name_prefix=graph_name_prefix,
+            )
     except Exception:
         if not rollback_if_failed:
             raise
 
         ctx.logger.warn('Rolling back deployment modification. '
                         '[modification_id={0}]'.format(modification.id))
         try:
```

### Comparing `cloudify-common-7.0.0/cloudify/proxy/__init__.py` & `cloudify-common-7.0.1/cloudify/proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/proxy/client.py` & `cloudify-common-7.0.1/cloudify/proxy/client.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/proxy/server.py` & `cloudify-common-7.0.1/cloudify/proxy/server.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/rabbitmq_client.py` & `cloudify-common-7.0.1/cloudify/rabbitmq_client.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/snapshots.py` & `cloudify-common-7.0.1/cloudify/snapshots.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/snmp/CLOUDIFY-MIB.mib` & `cloudify-common-7.0.1/cloudify/snmp/CLOUDIFY-MIB.mib`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/snmp/snmp_trap.py` & `cloudify-common-7.0.1/cloudify/snmp/snmp_trap.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/state.py` & `cloudify-common-7.0.1/cloudify/state.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/systemddbus.py` & `cloudify-common-7.0.1/cloudify/systemddbus.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/test_utils/__init__.py` & `cloudify-common-7.0.1/cloudify/test_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/test_utils/dispatch_helper.py` & `cloudify-common-7.0.1/cloudify/test_utils/dispatch_helper.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/test_utils/local_workflow_decorator.py` & `cloudify-common-7.0.1/cloudify/test_utils/local_workflow_decorator.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/test_utils/mock_rest_client.py` & `cloudify-common-7.0.1/cloudify/test_utils/mock_rest_client.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/utils.py` & `cloudify-common-7.0.1/cloudify/utils.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/workflows/__init__.py` & `cloudify-common-7.0.1/cloudify/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/workflows/amqp_dispatcher.py` & `cloudify-common-7.0.1/cloudify/workflows/amqp_dispatcher.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/workflows/events.py` & `cloudify-common-7.0.1/cloudify/workflows/events.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/workflows/local.py` & `cloudify-common-7.0.1/cloudify/workflows/local.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/workflows/tasks.py` & `cloudify-common-7.0.1/cloudify/workflows/tasks.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/workflows/tasks_graph.py` & `cloudify-common-7.0.1/cloudify/workflows/tasks_graph.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/workflows/workflow_api.py` & `cloudify-common-7.0.1/cloudify/workflows/workflow_api.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify/workflows/workflow_context.py` & `cloudify-common-7.0.1/cloudify/workflows/workflow_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1646,35 +1646,40 @@
     def remove_operation(self, operation_id):
         self.rest_client.operations.delete(operation_id)
 
     def get_execution(self, execution_id):
         return self.rest_client.executions.get(execution_id)
 
     def get_nodes(self):
-        if self.workflow_ctx.workflow_id in ('create_deployment_environment',
-                                             'delete_deployment_environment'):
+        dep = self.workflow_ctx.deployment
+        if not dep.id or self.workflow_ctx.workflow_id in (
+            'upload_blueprint',
+            'create_deployment_environment',
+            'delete_deployment_environment',
+        ):
             # If creating a deployment environment, there are clearly
             # no nodes/instances yet.
             # If deleting it we don't care about the nodes/instances,
             # and trying to retrieve them might cause problems if
             # deployment environment creation had a really bad time.
             return []
-        dep = self.workflow_ctx.deployment
         return self.rest_client.nodes.list(
             deployment_id=dep.id,
             _get_all_results=True,
             evaluate_functions=dep.runtime_only_evaluation
         )
 
     def get_node_instances(self):
-        if self.workflow_ctx.workflow_id in ('upload_blueprint',
-                                             'create_deployment_environment',
-                                             'delete_deployment_environment'):
-            return []
         dep = self.workflow_ctx.deployment
+        if not dep.id or self.workflow_ctx.workflow_id in (
+            'upload_blueprint',
+            'create_deployment_environment',
+            'delete_deployment_environment',
+        ):
+            return []
         return self.rest_client.node_instances.list(
             deployment_id=dep.id,
             _get_all_results=True,
         )
 
     def get_plugin(self, plugin):
         key = (
```

### Comparing `cloudify-common-7.0.0/cloudify/zip_utils.py` & `cloudify-common-7.0.1/cloudify/zip_utils.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify_async_client/audit_log.py` & `cloudify-common-7.0.1/cloudify_async_client/audit_log.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify_async_client/client.py` & `cloudify-common-7.0.1/cloudify_async_client/client.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify_common.egg-info/SOURCES.txt` & `cloudify-common-7.0.1/cloudify_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify_rest_client/__init__.py` & `cloudify-common-7.0.1/cloudify_rest_client/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify_rest_client/_datetime_compat.py` & `cloudify-common-7.0.1/cloudify_rest_client/_datetime_compat.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify_rest_client/audit_log.py` & `cloudify-common-7.0.1/cloudify_rest_client/audit_log.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify_rest_client/blueprints.py` & `cloudify-common-7.0.1/cloudify_rest_client/blueprints.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 import tempfile
 import shutil
 import contextlib
 from urllib.parse import quote as urlquote, urlparse
 
 from requests_toolbelt import MultipartEncoder, MultipartEncoderMonitor
 
-from cloudify_rest_client import utils
-from cloudify_rest_client import bytes_stream_utils
-from cloudify_rest_client.constants import VisibilityState
+from cloudify_rest_client import bytes_stream_utils, constants, utils
 from cloudify_rest_client.exceptions import CloudifyClientError
 from cloudify_rest_client.responses import ListResponse
 
 from .labels import Label
 
 
 class Blueprint(dict):
@@ -184,15 +182,15 @@
         return data
 
     def _upload(
         self,
         archive_location,
         blueprint_id,
         application_file_name=None,
-        visibility=VisibilityState.TENANT,
+        visibility=constants.VisibilityState.TENANT,
         progress_callback=None,
         async_upload=False,
         labels=None,
         created_at=None,
         created_by=None,
         state=None,
         skip_execution=False,
@@ -256,15 +254,15 @@
             expected_status_code=expected_status,
         )
 
     def _validate(self,
                   archive_location,
                   blueprint_id,
                   application_file_name=None,
-                  visibility=VisibilityState.TENANT,
+                  visibility=constants.VisibilityState.TENANT,
                   progress_callback=None):
         return self._upload(archive_location, blueprint_id,
                             application_file_name=application_file_name,
                             visibility=visibility,
                             progress_callback=progress_callback,
                             async_upload=False,
                             validate=True)
@@ -344,15 +342,15 @@
         )
 
     def publish_archive(
         self,
         archive_location,
         blueprint_id,
         blueprint_filename=None,
-        visibility=VisibilityState.TENANT,
+        visibility=constants.VisibilityState.TENANT,
         progress_callback=None,
         async_upload=False,
         labels=None,
         created_at=None,
         created_by=None,
         skip_execution=False,
         requirements=None,
@@ -404,15 +402,15 @@
             shutil.rmtree(tempdir)
         return size
 
     def upload(
         self,
         path,
         entity_id,
-        visibility=VisibilityState.TENANT,
+        visibility=constants.VisibilityState.TENANT,
         progress_callback=None,
         skip_size_limit=True,
         async_upload=False,
         labels=None,
         created_at=None,
         created_by=None,
         state=None,
@@ -468,15 +466,15 @@
         finally:
             shutil.rmtree(tempdir)
 
     def validate(self,
                  path,
                  entity_id,
                  blueprint_filename=None,
-                 visibility=VisibilityState.TENANT,
+                 visibility=constants.VisibilityState.TENANT,
                  progress_callback=None,
                  skip_size_limit=True):
         """
         Validates a blueprint with Cloudify's manager.
 
         :param path: Main blueprint yaml file path.
         :param entity_id: Id of the uploaded blueprint.
@@ -568,15 +566,15 @@
     def set_global(self, blueprint_id):
         """
         Updates the blueprint's visibility to global
 
         :param blueprint_id: Blueprint's id to update.
         :return: The blueprint.
         """
-        data = {'visibility': VisibilityState.GLOBAL}
+        data = {'visibility': constants.VisibilityState.GLOBAL}
         return self.api.patch(
             '/{self._uri_prefix}/{id}/set-visibility'.format(
                 self=self, id=blueprint_id),
             data=data
         )
 
     def set_visibility(self, blueprint_id, visibility):
@@ -656,7 +654,63 @@
         Request removal of the icon for an existing a blueprint.
 
         :param blueprint_id: Blueprint's id to update.
         """
         self.api.patch('/{self._uri_prefix}/{id}/icon'.format(
             self=self, id=blueprint_id),
         )
+
+    def dump(self, blueprint_ids=None):
+        """Generate blueprints' attributes for a snapshot.
+
+        :param blueprint_ids: A list of blueprints identifiers, if not empty,
+         used to select specific blueprints to be dumped.
+        :returns: A generator of dictionaries, which describe blueprints'
+         attributes.
+        """
+        entities = utils.get_all(
+                self.api.get,
+                f'/{self._uri_prefix}',
+                params={'_get_data': True},
+                _include=['id', 'visibility', 'labels', 'created_at',
+                          'created_by', 'state', 'main_file_name', 'plan',
+                          'description', 'error', 'error_traceback',
+                          'is_hidden', 'requirements'],
+        )
+        if not blueprint_ids:
+            return entities
+        return (e for e in entities if e['id'] in blueprint_ids)
+
+    def restore(self, entities, logger, path_func=None):
+        """Restore blueprints from a snapshot.
+
+        :param entities: An iterable (e.g. a list) of dictionaries describing
+         blueprints to be restored.
+        :param logger: A logger instance.
+        :param path_func: A function used retrieve blueprint's path.
+        :returns: A generator of dictionaries, which describe additional data
+         used for snapshot restore entities post-processing.
+        """
+        for entity in entities:
+            if path_func:
+                entity['archive_location'] = path_func(entity['id'])
+            entity['skip_execution'] = True
+            entity['blueprint_id'] = entity.pop('id')
+            entity['blueprint_filename'] = entity.pop('main_file_name')
+            entity['async_upload'] = True
+            extra_details = {}
+            for detail_name in [
+                'plan', 'state', 'error', 'error_traceback',
+                'is_hidden', 'description', 'labels', 'requirements',
+            ]:
+                detail = entity.pop(detail_name, None)
+                if detail:
+                    extra_details[detail_name] = detail
+            try:
+                self.publish_archive(**entity)
+                yield {
+                    entity['blueprint_id']:
+                        (extra_details, entity['archive_location']),
+                }
+            except CloudifyClientError as exc:
+                logger.error("Error restoring blueprint "
+                             f"{entity['blueprint_id']}: {exc}")
```

### Comparing `cloudify-common-7.0.0/cloudify_rest_client/bytes_stream_utils.py` & `cloudify-common-7.0.1/cloudify_rest_client/bytes_stream_utils.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify_rest_client/client.py` & `cloudify-common-7.0.1/cloudify_rest_client/client.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify_rest_client/cluster.py` & `cloudify-common-7.0.1/cloudify_rest_client/cluster.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify_rest_client/community_contacts.py` & `cloudify-common-7.0.1/cloudify_rest_client/community_contacts.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify_rest_client/deployment_modifications.py` & `cloudify-common-7.0.1/cloudify_rest_client/deployment_modifications.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify_rest_client/deployment_updates.py` & `cloudify-common-7.0.1/cloudify_rest_client/plugins_update.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,270 +1,242 @@
-########
-# Copyright (c) 2016 GigaSpaces Technologies Ltd. All rights reserved
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#        http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-#    * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#    * See the License for the specific language governing permissions and
-#    * limitations under the License.
-
-import os
-import json
-import shutil
-import tempfile
-from urllib.parse import quote as urlquote, urlparse
-from urllib.request import pathname2url
-
-from mimetypes import MimeTypes
+import warnings
 
 from cloudify_rest_client import utils
+from cloudify_rest_client.exceptions import CloudifyClientError
 from cloudify_rest_client.responses import ListResponse
 
 
-class DeploymentUpdate(dict):
+class PluginsUpdate(dict):
 
     def __init__(self, update):
         self.update(update)
 
     @property
     def id(self):
         return self['id']
 
     @property
     def state(self):
         return self['state']
 
     @property
-    def deployment_id(self):
-        return self['deployment_id']
-
-    @property
-    def old_blueprint_id(self):
-        return self['old_blueprint_id']
+    def blueprint_id(self):
+        return self['blueprint_id']
 
     @property
-    def new_blueprint_id(self):
-        return self['new_blueprint_id']
+    def temp_blueprint_id(self):
+        return self['temp_blueprint_id']
 
     @property
-    def old_inputs(self):
-        return self['old_inputs']
-
-    @property
-    def new_inputs(self):
-        return self['new_inputs']
+    def execution_id(self):
+        return self['execution_id']
 
     @property
-    def steps(self):
-        return self['steps']
+    def deployments_to_update(self):
+        return self['deployments_to_update']
 
     @property
-    def execution_id(self):
-        return self['execution_id']
+    def deployments_per_tenant(self):
+        return self['deployments_per_tenant']
 
     @property
     def created_at(self):
         return self['created_at']
 
     @property
-    def runtime_only_evaluation(self):
-        return self['runtime_only_evaluation']
+    def forced(self):
+        return self['forced']
 
     @property
-    def deployment_plan(self):
-        return self['deployment_plan']
+    def tenant_name(self):
+        return self['tenant_name']
 
 
-class DeploymentUpdatesClient(object):
+class PluginsUpdateClient(object):
+    """
+    Cloudify's plugins update management client.
+    """
 
     def __init__(self, api):
         self.api = api
+        self._uri_prefix = 'plugins-updates'
+        self._wrapper_cls = PluginsUpdate
 
-    def create(self, update_id, deployment_id, **kwargs):
-        """Create a deployment-update object.
-
-        This is only useful from within the deployment-update workflow.
-        Do not use this otherwise.
+    def get(self, plugins_update_id, _include=None, **kwargs):
         """
-        url = '/deployment-updates/{0}'.format(update_id)
-        data = {
-            'deployment_id': deployment_id,
-        }
-        data.update(kwargs)
-        response = self.api.put(url, data=data)
-        return DeploymentUpdate(response)
-
-    def set_attributes(self, update_id, **kwargs):
-        """Update a deployment-update object with the given attributes.
+        Gets a plugins update by its id.
 
-        This is only useful from within the deployment-update workflow.
-        Do not use this otherwise.
+        :param plugins_update_id: PluginsUpdate's id to get.
+        :param _include: List of fields to include in response.
+        :return: The plugins update details.
         """
-        url = '/deployment-updates/{0}'.format(update_id)
-        self.api.patch(url, data=kwargs)
+        assert plugins_update_id
+        uri = '/{self._uri_prefix}/{id}'.format(
+            self=self, id=plugins_update_id)
+        response = self.api.get(uri, _include=_include, params=kwargs)
+        return self._wrapper_cls(response)
+
+    def _wrap_list(self, response):
+        return ListResponse(
+            [self._wrapper_cls(item) for item in response['items']],
+            response['metadata']
+        )
 
     def list(self, _include=None, sort=None, is_descending=False, **kwargs):
-        """List deployment updates
+        """
+        Returns a list of available plugins updates.
 
         :param _include: List of fields to include in response.
         :param sort: Key for sorting the list.
         :param is_descending: True for descending order, False for ascending.
-        :param kwargs: Optional filter fields. for a list of available fields
-               see the REST service's models.DeploymentUpdate.fields
+        :param kwargs: Optional filter fields. For a list of available fields
+               see the REST service's models.PluginsUpdate.fields
+        :return: Plugins list.
         """
-
-        uri = '/deployment-updates'
         params = kwargs
         if sort:
             params['_sort'] = '-' + sort if is_descending else sort
 
-        response = self.api.get(uri, params=params, _include=_include)
-        items = [DeploymentUpdate(item) for item in response['items']]
-        return ListResponse(items, response['metadata'])
-
-    def bulk_insert(self, updates):
-        """Bulk insert deployment updates. For internal use only."""
-        uri = '/deployment-updates'
-        self.api.post(uri, {'deployment_updates': updates},
-                      expected_status_code=[201, 204])
-
-    def _update_from_blueprint(self,
-                               deployment_id,
-                               blueprint_path,
-                               inputs=None):
-        """Create a deployment update transaction for blueprint app.
-
-        :param deployment_id: The deployment id
-        :param blueprint_path: the path of the blueprint to stage
-        """
-        assert deployment_id
-
-        tempdir = tempfile.mkdtemp()
-        try:
-            tar_path = utils.tar_blueprint(blueprint_path, tempdir)
-            application_filename = os.path.basename(blueprint_path)
-
-            return self._update_from_archive(deployment_id,
-                                             tar_path,
-                                             application_filename,
-                                             inputs=inputs)
-        finally:
-            shutil.rmtree(tempdir)
-
-    @staticmethod
-    def _update_from_archive(deployment_id,
-                             archive_path,
-                             application_file_name=None,
-                             inputs=None):
-        """Create a deployment update transaction for an archived app.
-
-        :param archive_path: the path for the archived app.
-        :param application_file_name: the main blueprint filename.
-        :param deployment_id: the deployment id to update.
-        :return: DeploymentUpdate dict
-        :rtype: DeploymentUpdate
-        """
-        assert deployment_id
-
-        mime_types = MimeTypes()
-
-        data_form = {}
-        params = {}
-        # all the inputs are passed through the query
-        if inputs:
-            data_form['inputs'] = ('inputs', json.dumps(inputs), 'text/plain')
-
-        if application_file_name:
-            params['application_file_name'] = urlquote(application_file_name)
-
-        # For a Windows path (e.g. "C:\aaa\bbb.zip") scheme is the
-        # drive letter and therefore the 2nd condition is present
-        if all([urlparse(archive_path).scheme,
-                not os.path.exists(archive_path)]):
-            # archive location is URL
-            params['blueprint_archive_url'] = archive_path
+        response = self.api.get('/{self._uri_prefix}'.format(self=self),
+                                _include=_include,
+                                params=params)
+        return self._wrap_list(response)
+
+    def inject(self, blueprint_id, force=False,
+               created_by=None, created_at=None,
+               execution_id=None, state=None,
+               update_id=None, affected_deployments=None,
+               deployments_per_tenant=None, all_tenants=None,
+               temp_blueprint_id=None):
+        return PluginsUpdate(self.api.post(
+            '/{self._uri_prefix}/{}/update/initiate'.format(blueprint_id,
+                                                            self=self),
+            data=_data_from_kwargs(
+                force=force,
+                created_by=created_by,
+                created_at=created_at,
+                execution_id=execution_id,
+                state=state,
+                update_id=update_id,
+                all_tenants=all_tenants,
+                affected_deployments=affected_deployments,
+                deployments_per_tenant=deployments_per_tenant,
+                temp_blueprint_id=temp_blueprint_id,
+            ),
+        ))
+
+    def update_plugins(self, blueprint_id, force=False, plugin_names=None,
+                       to_latest=None, all_to_latest=True,
+                       to_minor=None, all_to_minor=False,
+                       mapping=None, auto_correct_types=False,
+                       reevaluate_active_statuses=False,
+                       all_tenants=False):
+        """
+        Updates the plugins in all the deployments that use the given
+        blueprint.
+
+        :param blueprint_id: blueprint ID to perform the update with.
+        :param force: if to forcefully update when other non-active plugins
+         updates exists associated with this blueprint.
+        :param plugin_names: list of plugin names to update (only those).
+        :param to_latest: list of plugin names to be upgraded to the latest
+         installed version.
+        :param all_to_latest: update all (selected) plugins to the latest
+         installed version of a plugin.
+        :param to_minor: list of plugin names to be upgraded to the latest
+         installed minor version (i.e. major versions of the plugin in use and
+         the upgraded one will match)
+        :param all_to_minor: update all (selected) plugins to the latest
+         installed minor version
+        :param mapping: detailed information on required plugin update
+         (overrides all other arguments/settings concerning version
+         constraints)
+        :param auto_correct_types: auto_correct_types flag to run deployments
+         update with
+        :param reevaluate_active_statuses: reevaluate active plugin-updates'
+         and deployment-updates' states based on relevant executions statuses.
+        :param all_tenants: defines if plugin update process should update any
+         deployments based on blueprint_id (owned by any tenant)
+        :return: a PluginUpdate object.
+        """
+        if mapping and mapping.get('updates'):
+            warnings.warn("The 'mapping file' was used during the update; "
+                          "remember to update your blueprint files",
+                          RuntimeWarning)
         else:
-            data_form['blueprint_archive'] = (
-                os.path.basename(archive_path),
-                open(archive_path, 'rb'),
-                # Guess the archive mime type
-                mime_types.guess_type(pathname2url(archive_path)))
-
-        return data_form, params
-
-    def get(self, update_id, _include=None):
-        """Get deployment update
-
-        :param update_id: The update id
-        """
-        uri = '/deployment-updates/{0}'.format(update_id)
-        response = self.api.get(uri, _include=_include)
-        return DeploymentUpdate(response)
-
-    def update_with_existing_blueprint(
-        self,
-        deployment_id,
-        blueprint_id=None,
-        inputs=None,
-        skip_install=False,
-        skip_uninstall=False,
-        skip_reinstall=False,
-        skip_drift_check=False,
-        skip_heal=False,
-        force_reinstall=False,
-        workflow_id=None,
-        force=False,
-        ignore_failure=False,
-        install_first=False,
-        reinstall_list=None,
-        preview=False,
-        update_plugins=True,
-        runtime_only_evaluation=None,
-        auto_correct_types=None,
-        reevaluate_active_statuses=None
-    ):
-        data = {
-            'workflow_id': workflow_id,
-            'skip_install': skip_install,
-            'skip_uninstall': skip_uninstall,
-            'skip_reinstall': skip_reinstall,
-            'skip_drift_check': skip_drift_check,
-            'skip_heal': skip_heal,
-            'force_reinstall': force_reinstall,
-            'ignore_failure': ignore_failure,
-            'install_first': install_first,
-            'preview': preview,
-            'blueprint_id': blueprint_id,
-            'update_plugins': update_plugins,
-            'force': force,
-        }
-        if inputs:
-            data['inputs'] = inputs
-        if reinstall_list:
-            data['reinstall_list'] = reinstall_list
-        if runtime_only_evaluation is not None:
-            data['runtime_only_evaluation'] = runtime_only_evaluation
-        if auto_correct_types is not None:
-            data['auto_correct_types'] = auto_correct_types
-        if reevaluate_active_statuses is not None:
-            data['reevaluate_active_statuses'] = reevaluate_active_statuses
-        uri = '/deployment-updates/{0}/update/initiate'.format(deployment_id)
-        response = self.api.post(uri, data=data)
-        return DeploymentUpdate(response)
-
-    def finalize_commit(self, update_id):
-        """Finalize the committing process
-
-        :param update_id:
-        :return:
-        """
-        assert update_id
-
-        uri = '/deployment-updates/{0}/update/finalize'.format(update_id)
-        response = self.api.post(uri)
-        return DeploymentUpdate(response)
+            mapping = {}
+        response = self.api.post(
+            '/{self._uri_prefix}/{}/update/initiate'.format(blueprint_id,
+                                                            self=self),
+            data=_data_from_kwargs(
+                plugin_names=plugin_names,
+                to_latest=to_latest,
+                all_to_latest=all_to_latest,
+                to_minor=to_minor,
+                all_to_minor=all_to_minor,
+                mapping=mapping,
+                force=force,
+                auto_correct_types=auto_correct_types,
+                reevaluate_active_statuses=reevaluate_active_statuses,
+                all_tenants=all_tenants
+            )
+        )
+        return PluginsUpdate(response)
+
+    def finalize_plugins_update(self, plugins_update_id):
+        """
+        Finalize the plugins update (for internal use).
+
+        :return: a PluginUpdate object.
+        """
+        response = self.api.post(
+            '/{self._uri_prefix}/{}/update/finalize'.format(plugins_update_id,
+                                                            self=self)
+        )
+        return PluginsUpdate(response)
+
+    def dump(self, plugins_update_ids=None):
+        """Generate plugins updates' attributes for a snapshot.
+
+        :param plugins_update_ids: A list of plugins updates' identifiers,
+         if not empty, used to select specific plugins updates to be dumped.
+        :returns: A generator of dictionaries, which describe plugins
+         updates' attributes.
+        """
+        entities = utils.get_all(
+                self.api.get,
+                f'/{self._uri_prefix}',
+                params={'_get_data': True},
+                _include=['id', 'state', 'forced', 'all_tenants',
+                          'blueprint_id', 'execution_id', 'created_by',
+                          'created_at', 'deployments_to_update',
+                          'deployments_per_tenant', 'temp_blueprint_id'],
+        )
+        if not plugins_update_ids:
+            return entities
+        return (e for e in entities if e['id'] in plugins_update_ids)
+
+    def restore(self, entities, logger):
+        """Restore plugins updates from a snapshot.
+
+        :param entities: An iterable (e.g. a list) of dictionaries describing
+         plugins updates to be restored.
+        :param logger: A logger instance.
+        """
+        for entity in entities:
+            entity['update_id'] = entity.pop('id')
+            entity['affected_deployments'] = entity.pop(
+                    'deployments_to_update', None)
+            entity['force'] = entity.pop('forced', None)
+            try:
+                self.inject(**entity)
+            except CloudifyClientError as exc:
+                logger.error("Error restoring plugins update "
+                             f"{entity['update_id']}: {exc}")
+
+
+def _data_from_kwargs(**kwargs):
+    data = {}
+    for k, v in kwargs.items():
+        if v:
+            data[k] = v
+    return data or None
```

### Comparing `cloudify-common-7.0.0/cloudify_rest_client/deployments.py` & `cloudify-common-7.0.1/cloudify_rest_client/deployments.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,19 @@
+import os
 import warnings
 from copy import copy
 
+from cloudify_rest_client import constants, utils
+from cloudify_rest_client.exceptions import CloudifyClientError
 from cloudify_rest_client.responses import ListResponse
-from cloudify_rest_client.constants import VisibilityState
 
 from .labels import Label
 
+EMPTY_B64_ZIP = 'UEsFBgAAAAAAAAAAAAAAAAAAAAAAAA=='
+
 
 class Deployment(dict):
     """
     Cloudify deployment.
     """
 
     def __init__(self, deployment):
@@ -391,15 +395,15 @@
             response['metadata'])
 
     def get(self, group_id):
         """Get the specified deployment group."""
         response = self.api.get('/deployment-groups/{0}'.format(group_id))
         return DeploymentGroup(response)
 
-    def put(self, group_id, visibility=VisibilityState.TENANT,
+    def put(self, group_id, visibility=constants.VisibilityState.TENANT,
             description=None, blueprint_id=None, default_inputs=None,
             labels=None, filter_id=None, deployment_ids=None,
             new_deployments=None, deployments_from_group=None,
             created_by=None, created_at=None, creation_counter=None):
         """Create or update the specified deployment group.
 
         Setting group deployments using this method (via either filter_id
@@ -530,32 +534,72 @@
                     'deployments_from_group': deployments_from_group,
                 }
             }
         )
         return DeploymentGroup(response)
 
     def delete(self, group_id, delete_deployments=False,
-               force=False, with_logs=False):
+               force=False, with_logs=False, recursive=False):
         """Delete a deployment group. By default, keep the deployments.
 
         :param group_id: the group to remove
         :param delete_deployments: also delete all deployments belonging
             to this group
         :param force: same meaning as in deployments.delete
         :param with_logs: same meaning as in deployments.delete
+        :param recursive: same meaning as in deployments.delete
         """
-        self.api.delete(
+        return self.api.delete(
             '/deployment-groups/{0}'.format(group_id),
             params={
                 'delete_deployments': delete_deployments,
                 'force': force,
                 'delete_logs': with_logs,
+                'recursive': recursive,
             },
-            expected_status_code=204
+            expected_status_code=(200, 204),
+        )
+
+    def dump(self, deployment_groups_ids=None):
+        """Generate deployment groups' attributes for a snapshot.
+
+        :param deployment_groups_ids: A list of deployment groups'
+         identifiers, if not empty, used to select deployment groups
+         to be dumped.
+        :returns: A generator of dictionaries, which describe deployment
+         groups' attributes.
+        """
+        entities = utils.get_all(
+                self.api.get,
+                '/deployment-groups',
+                params={'_get_data': True},
+                _include=['id', 'visibility', 'description', 'labels',
+                          'default_blueprint_id', 'default_inputs',
+                          'deployment_ids', 'created_by', 'created_at',
+                          'creation_counter'],
         )
+        if not deployment_groups_ids:
+            return entities
+        return (e for e in entities if e['id'] in deployment_groups_ids)
+
+    def restore(self, entities, logger):
+        """Restore deployment groups from a snapshot.
+
+        :param entities: An iterable (e.g. a list) of dictionaries describing
+         deployment groups to be restored.
+        :param logger: A logger instance.
+        """
+        for entity in entities:
+            entity['group_id'] = entity.pop('id')
+            entity['blueprint_id'] = entity.pop('default_blueprint_id')
+            try:
+                self.put(**entity)
+            except CloudifyClientError as exc:
+                logger.error("Error restoring deployment group "
+                             f"{entity['group_id']}: {exc}")
 
 
 class DeploymentOutputsClient(object):
 
     def __init__(self, api):
         self.api = api
 
@@ -728,15 +772,15 @@
         )
         return Deployment(response)
 
     def create(self,
                blueprint_id,
                deployment_id,
                inputs=None,
-               visibility=VisibilityState.TENANT,
+               visibility=constants.VisibilityState.TENANT,
                skip_plugins_validation=False,
                site_name=None,
                runtime_only_evaluation=False,
                labels=None,
                display_name=None,
                async_create=None,
                created_at=None,
@@ -858,34 +902,44 @@
         if async_create is not None:
             # if it's None, we just keep the server's default behaviour
             params['async_create'] = async_create
         response = self.api.put(
             uri, data, params=params, expected_status_code=201)
         return Deployment(response)
 
-    def delete(self, deployment_id,
-               force=False,
-               delete_db_mode=False,
-               with_logs=False):
+    def delete(
+        self,
+        deployment_id,
+        force=False,
+        delete_db_mode=False,
+        with_logs=False,
+        recursive=False,
+    ):
         """
         Deletes the deployment whose id matches the provided deployment id.
         By default, deletion of a deployment with live nodes or installations
         which depend on it is not allowed. This behavior can be changed
         using the force argument.
 
         :param deployment_id: The deployment's to be deleted id.
         :param force: Delete deployment even if there are existing live nodes
                for it, or existing installations which depend on it.
         :param delete_db_mode: deprecated and does nothing
         :param with_logs: when set to true, the management workers' logs for
                the deployment are deleted as well.
+        :param recursive: also delete all service deployments contained in
+               this delployment.
         :return: The deleted deployment.
         """
         assert deployment_id
-        params = {'force': force, 'delete_logs': with_logs}
+        params = {
+            'force': force,
+            'delete_logs': with_logs,
+            'recursive': recursive,
+        }
         if delete_db_mode:
             warnings.warn('delete_db_mode is deprecated and does nothing',
                           DeprecationWarning)
 
         self.api.delete(
             '/deployments/{0}'.format(deployment_id), params=params)
 
@@ -947,7 +1001,63 @@
         instead.
 
         For internal use only.
         """
         updated_dep = self.api.patch(
             '/deployments/{0}'.format(deployment_id), data=kwargs)
         return Deployment(updated_dep)
+
+    def dump(self, deployment_ids=None):
+        """Generate deployments' attributes for a snapshot.
+
+        :param deployment_ids: A list of deployments' identifiers, if not
+         empty, used to select specific deployments to be dumped.
+        :returns: A generator of dictionaries, which describe deployments'
+         attributes.
+        """
+        entities = utils.get_all(
+                self.api.get,
+                '/deployments',
+                params={'_get_data': True},
+                _include=['id', 'blueprint_id', 'inputs', 'visibility',
+                          'labels', 'display_name', 'runtime_only_evaluation',
+                          'created_by', 'created_at', 'workflows', 'groups',
+                          'policy_triggers', 'policy_types', 'outputs',
+                          'capabilities', 'description', 'scaling_groups',
+                          'resource_tags', 'deployment_status',
+                          'installation_status', 'sub_services_status',
+                          'sub_environments_status', 'sub_services_count',
+                          'sub_environments_count'],
+        )
+        if not deployment_ids:
+            return entities
+        return (e for e in entities if e['id'] in deployment_ids)
+
+    def restore(self, entities, logger, path_func=None):
+        """Restore deployments from a snapshot.
+
+        :param entities: An iterable (e.g. a list) of dictionaries describing
+         deployments to be restored.
+        :param logger: A logger instance.
+        :param path_func: A function used retrieve deployment's path.
+        """
+        for entity in entities:
+            if path_func:
+                workdir_location = path_func(entity['id'])
+                if workdir_location and os.path.exists(workdir_location):
+                    with open(workdir_location) as workdir_handle:
+                        entity['_workdir_zip'] = workdir_handle.read()
+                    os.unlink(workdir_location)
+                else:
+                    entity['_workdir_zip'] = EMPTY_B64_ZIP
+                entity['deployment_id'] = entity.pop('id')
+                entity['async_create'] = False
+                if entity['workflows']:
+                    entity['workflows'] = {
+                        wf.pop('name'): wf
+                        for wf in entity.pop('workflows', {})
+                    }
+                try:
+                    self.create(**entity)
+                except CloudifyClientError as exc:
+                    logger.error("Error restoring deployment "
+                                 f"{entity['deployment_id']}: {exc}")
```

### Comparing `cloudify-common-7.0.0/cloudify_rest_client/evaluate.py` & `cloudify-common-7.0.1/cloudify_rest_client/evaluate.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify_rest_client/exceptions.py` & `cloudify-common-7.0.1/cloudify_rest_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify_rest_client/execution_schedules.py` & `cloudify-common-7.0.1/cloudify_rest_client/execution_schedules.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from datetime import datetime
 
+from cloudify_rest_client import utils
+from cloudify_rest_client.exceptions import CloudifyClientError
 from cloudify_rest_client.responses import ListResponse
 
 
 class ExecutionSchedule(dict):
     """
     Cloudify execution schedule.
     """
@@ -274,7 +276,44 @@
         :return: Execution.
         """
         assert schedule_id
         params = {'deployment_id': deployment_id}
         uri = '/{self._uri_prefix}/{id}'.format(self=self, id=schedule_id)
         response = self.api.get(uri, _include=_include, params=params)
         return ExecutionSchedule(response)
+
+    def dump(self, execution_schedule_ids=None):
+        """Generate execution schedules' attributes for a snapshot.
+
+        :param execution_schedule_ids: A list of execution schedules'
+         identifiers, if not empty, used to select specific execution
+         schedules to be dumped.
+        :returns: A generator of dictionaries, which describe execution
+         schedules' attributes.
+        """
+        entities = utils.get_all(
+                self.api.get,
+                f'/{self._uri_prefix}',
+                _include=['id', 'rule', 'deployment_id', 'workflow_id',
+                          'created_at', 'since', 'until', 'stop_on_fail',
+                          'parameters', 'execution_arguments', 'slip',
+                          'enabled', 'created_by'],
+        )
+        if not execution_schedule_ids:
+            return entities
+        return (e for e in entities if e['id'] in execution_schedule_ids)
+
+    def restore(self, entities, logger):
+        """Restore execution schedules from a snapshot.
+
+        :param entities: An iterable (e.g. a list) of dictionaries describing
+         execution schedules to be restored.
+        :param logger: A logger instance.
+        """
+        for entity in entities:
+            entity['schedule_id'] = entity.pop('id')
+            entity['rrule'] = entity.pop('rule', {}).pop('rrule')
+            try:
+                self.create(**entity)
+            except CloudifyClientError as exc:
+                logger.error("Error restoring execution schedule "
+                             f"{entity['schedule_id']}: {exc}")
```

### Comparing `cloudify-common-7.0.0/cloudify_rest_client/executions.py` & `cloudify-common-7.0.1/cloudify_rest_client/executions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import warnings
 
+from cloudify_rest_client import utils
+from cloudify_rest_client.exceptions import CloudifyClientError
 from cloudify_rest_client.responses import ListResponse
 
 
 class Execution(dict):
     """Cloudify workflow execution."""
     TERMINATED = 'terminated'
     FAILED = 'failed'
@@ -185,17 +187,19 @@
     def list(self, _include=None, **kwargs):
         response = self.api.get('/execution-groups', params=kwargs,
                                 _include=_include)
         return ListResponse(
             [ExecutionGroup(item) for item in response['items']],
             response['metadata'])
 
-    def get(self, execution_group_id):
+    def get(self, execution_group_id, _include=None):
         response = self.api.get(
-            '/execution-groups/{0}'.format(execution_group_id))
+            '/execution-groups/{0}'.format(execution_group_id),
+            _include=_include,
+        )
         return ExecutionGroup(response)
 
     def create(self, deployment_group_id, workflow_id, executions,
                force=False, default_parameters=None, parameters=None,
                concurrency=5, created_by=None, created_at=None,
                id=None):
         """Create an exec group without running it.
@@ -304,14 +308,48 @@
             '/execution-groups/{0}'.format(execution_group_id),
             data={
                 'concurrency': concurrency,
             },
         )
         return ExecutionGroup(response)
 
+    def dump(self, execution_group_ids=None):
+        """Generate execution groups' attributes for a snapshot.
+
+        :param execution_group_ids: A list of execution groups' identifiers,
+         if not empty, used to select specific execution groups to be dumped.
+        :returns: A generator of dictionaries, which describe execution
+         groups' attributes.
+        """
+        entities = utils.get_all(
+                self.api.get,
+                '/execution-groups',
+                params={'_get_data': True},
+                _include=['id', 'created_at', 'workflow_id', 'execution_ids',
+                          'concurrency', 'deployment_group_id', 'created_by'],
+        )
+        if not execution_group_ids:
+            return entities
+        return (e for e in entities if e['id'] in execution_group_ids)
+
+    def restore(self, entities, logger):
+        """Restore execution groups from a snapshot.
+
+        :param entities: An iterable (e.g. a list) of dictionaries describing
+         execution groups to be restored.
+        :param logger: A logger instance.
+        """
+        for entity in entities:
+            entity['executions'] = entity.pop('execution_ids')
+            try:
+                self.create(**entity)
+            except CloudifyClientError as exc:
+                logger.error("Error restoring execution group "
+                             f"{entity['id']}: {exc}")
+
 
 class ExecutionsClient(object):
 
     def __init__(self, api):
         self.api = api
         self._uri_prefix = 'executions'
         self._wrapper_cls = Execution
@@ -424,15 +462,15 @@
         return self.create(*args, **kwargs)
 
     def create(self, deployment_id, workflow_id, parameters=None,
                allow_custom_parameters=False, force=False, dry_run=False,
                queue=False, schedule=None, force_status=None,
                created_by=None, created_at=None, started_at=None,
                ended_at=None, execution_id=None, wait_after_fail=600,
-               error=None):
+               is_system_workflow=None, error=None):
         """Creates an execution on a deployment.
         If force_status is provided, the execution will not be started.
         Otherwise, parameters and return value are identical to 'start'.
         """
         if schedule:
             warnings.warn("The 'schedule' flag is deprecated. Please use "
                           "`cfy deployments schedule create instead`",
@@ -449,14 +487,15 @@
             'wait_after_fail': wait_after_fail,
             'force_status': force_status,
             'created_by': created_by,
             'created_at': created_at,
             'started_at': started_at,
             'ended_at': ended_at,
             'id': execution_id,
+            'is_system_workflow': is_system_workflow,
             'error': error,
         }
         uri = '/executions'
         response = self.api.post(uri,
                                  data=data,
                                  expected_status_code=201)
         return Execution(response)
@@ -522,7 +561,49 @@
         if keep_last:
             data['keep_last'] = keep_last
         response = self.api.delete('/{self._uri_prefix}'.format(self=self),
                                    data=data,
                                    params=kwargs,
                                    expected_status_code=200)
         return response['items'][0]['count']
+
+    def dump(self, execution_ids=None):
+        """Generate executions' attributes for a snapshot.
+
+        :param execution_ids: A list of executions' identifiers, if not
+         empty, used to select specific executions to be dumped.
+        :returns: A generator of dictionaries, which describe executions'
+         attributes.
+        """
+        entities = utils.get_all(
+                self.api.get,
+                f'/{self._uri_prefix}',
+                _include=['deployment_id', 'workflow_id', 'parameters',
+                          'is_dry_run', 'allow_custom_parameters', 'status',
+                          'created_by', 'created_at', 'id', 'started_at',
+                          'ended_at', 'error', 'is_system_workflow'],
+                params={
+                    '_get_data': True,
+                    '_include_system_workflows': True,
+                },
+        )
+        if not execution_ids:
+            return entities
+        return (e for e in entities if e['id'] in execution_ids)
+
+    def restore(self, entities, logger):
+        """Restore executions from a snapshot.
+
+        :param entities: An iterable (e.g. a list) of dictionaries describing
+         executions to be restored.
+        :param logger: A logger instance.
+        """
+        for entity in entities:
+            entity['execution_id'] = entity.pop('id')
+            entity['force_status'] = entity.pop('status')
+            entity['dry_run'] = entity.pop('is_dry_run')
+            entity['deployment_id'] = entity['deployment_id'] or ''
+            try:
+                self.create(**entity)
+            except CloudifyClientError as exc:
+                logger.error("Error restoring execution "
+                             f"{entity['execution_id']}: {exc}")
```

### Comparing `cloudify-common-7.0.0/cloudify_rest_client/filters.py` & `cloudify-common-7.0.1/cloudify_rest_client/filters.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from cloudify_rest_client import constants, utils
+from cloudify_rest_client.exceptions import CloudifyClientError
 from cloudify_rest_client.responses import ListResponse
-from cloudify_rest_client.constants import VisibilityState
 
 
 class Filter(dict):
     def __init__(self, filter_obj):
         super(Filter, self).__init__()
         self.update(filter_obj)
 
@@ -39,20 +40,21 @@
     def tenant_name(self):
         return self.get('tenant_name')
 
 
 class FiltersClient(object):
     def __init__(self, api, filtered_resource):
         self.api = api
+        self._filtered_resource = filtered_resource
         self.uri = '/filters/' + filtered_resource
 
     def create(self,
                filter_id,
                filter_rules,
-               visibility=VisibilityState.TENANT,
+               visibility=constants.VisibilityState.TENANT,
                created_at=None,
                created_by=None):
         """Creates a new filter.
 
         :param filter_id: The filter ID
         :param filter_rules: A list of filter rules. A filter rule is a
                dictionary of the form
@@ -131,14 +133,49 @@
         if new_filter_rules:
             data['filter_rules'] = new_filter_rules
 
         response = self.api.patch('{0}/{1}'.format(self.uri, filter_id),
                                   data=data)
         return Filter(response)
 
+    def dump(self, filter_ids=None):
+        """Generate filters' attributes for a snapshot.
+
+        :param filter_ids: A list of filter identifiers, if not empty,
+         used to select specific filters to be dumped.
+        :returns: A generator of dictionaries, which describe filters'
+         attributes.
+        """
+        for entity in utils.get_all(
+                self.api.get,
+                self.uri,
+                _include=['created_at', 'id', 'visibility', 'value',
+                          'created_by', 'is_system_filter'],
+        ):
+            if entity.pop('is_system_filter'):
+                continue
+            if not filter_ids or entity['id'] in filter_ids:
+                yield entity
+
+    def restore(self, entities, logger):
+        """Restore filters from a snapshot.
+
+        :param entities: An iterable (e.g. a list) of dictionaries describing
+         filters to be restored.
+        :param logger: A logger instance.
+        """
+        for entity in entities:
+            entity['filter_id'] = entity.pop('id')
+            entity['filter_rules'] = entity.pop('value')
+            try:
+                self.create(**entity)
+            except CloudifyClientError as exc:
+                logger.error("Error restoring filter "
+                             f"{entity['filter_id']}: {exc}")
+
 
 class BlueprintsFiltersClient(FiltersClient):
     def __init__(self, api):
         super(BlueprintsFiltersClient, self).__init__(api, 'blueprints')
 
 
 class DeploymentsFiltersClient(FiltersClient):
```

### Comparing `cloudify-common-7.0.0/cloudify_rest_client/inter_deployment_dependencies.py` & `cloudify-common-7.0.1/cloudify_rest_client/inter_deployment_dependencies.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,12 @@
-# Copyright (c) 2017-2019 Cloudify Platform Ltd. All rights reserved
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#        http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
 from cloudify.deployment_dependencies import (build_deployment_dependency,
                                               DEPENDENCY_CREATOR)
 
+from cloudify_rest_client import utils
+from cloudify_rest_client.exceptions import CloudifyClientError
 from cloudify_rest_client.responses import ListResponse
 
 
 class InterDeploymentDependency(dict):
 
     def __init__(self, dependency):
         self.update(dependency)
@@ -200,19 +188,63 @@
             params['_sort'] = '-' + sort if is_descending else sort
 
         response = self.api.get('/{self._uri_prefix}'.format(self=self),
                                 _include=_include,
                                 params=params)
         return self._wrap_list(response)
 
-    def restore(self, deployment_id, update_service_composition):
+    def legacy_restore(self, deployment_id, update_service_composition):
         """
         Updating the inter deployment dependencies table from the specified
         deployment during an upgrade
 
        """
         data = {
             'deployment_id': deployment_id,
             'update_service_composition': update_service_composition,
         }
         self.api.post('/{self._uri_prefix}/restore'.format(self=self),
                       data=data)
+
+    def dump(self, inter_deployment_dependency_ids=None):
+        """Generate inter-deployment dependencies' attributes for a snapshot.
+
+        :param inter_deployment_dependency_ids: A list of inter-deployment
+         dependencies' identifiers, if not empty, used to select specific
+         inter-deployment dependencies to be dumped.
+        :returns: A generator of dictionaries, which describe inter-deployment
+         dependencies' attributes.
+        """
+        entities = utils.get_all(
+                self.api.get,
+                f'/{self._uri_prefix}',
+                _include=['id', 'visibility', 'created_at', 'created_by',
+                          'dependency_creator', 'target_deployment_func',
+                          'source_deployment_id', 'target_deployment_id',
+                          'external_source', 'external_target'],
+        )
+        if not inter_deployment_dependency_ids:
+            return entities
+        return (e for e in entities
+                if e['id'] in inter_deployment_dependency_ids)
+
+    def restore(self, entities, logger):
+        """Restore inter-deployment dependencies from a snapshot.
+
+        :param entities: An iterable (e.g. a list) of dictionaries describing
+         inter-deployment dependencies to be restored.
+        :param logger: A logger instance.
+        """
+        for entity in entities:
+            entity['_id'] = entity.pop('id')
+            entity['_visibility'] = entity.pop('visibility')
+            entity['_created_at'] = entity.pop('created_at')
+            entity['_created_by'] = entity.pop('created_by')
+            entity['source_deployment'] = \
+                entity.pop('source_deployment_id')
+            entity['target_deployment'] = \
+                entity.pop('target_deployment_id')
+            try:
+                self.create(**entity)
+            except CloudifyClientError as exc:
+                logger.error("Error restoring inter-deployment dependency "
+                             f"{entity['_id']}: {exc}")
```

### Comparing `cloudify-common-7.0.0/cloudify_rest_client/labels.py` & `cloudify-common-7.0.1/cloudify_rest_client/labels.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify_rest_client/ldap.py` & `cloudify-common-7.0.1/cloudify_rest_client/ldap.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify_rest_client/license.py` & `cloudify-common-7.0.1/cloudify_rest_client/license.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify_rest_client/log_bundles.py` & `cloudify-common-7.0.1/cloudify_rest_client/log_bundles.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify_rest_client/maintenance.py` & `cloudify-common-7.0.1/cloudify_rest_client/maintenance.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify_rest_client/manager.py` & `cloudify-common-7.0.1/cloudify_rest_client/manager.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify_rest_client/node_instances.py` & `cloudify-common-7.0.1/cloudify_rest_client/node_instances.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,11 @@
-########
-# Copyright (c) 2014 GigaSpaces Technologies Ltd. All rights reserved
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#        http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-#    * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#    * See the License for the specific language governing permissions and
-#    * limitations under the License.
 import warnings
 
+from cloudify_rest_client import utils
+from cloudify_rest_client.exceptions import CloudifyClientError
 from cloudify_rest_client.responses import ListResponse
 
 
 class NodeInstance(dict):
     """
     Cloudify node instance.
     """
@@ -317,7 +305,67 @@
         :param instance_id: ID of the instance to be deleted
         """
         self.api.delete(
             '/{self._uri_prefix}/{instance_id}'
             .format(self=self, instance_id=instance_id),
             expected_status_code=204,
         )
+
+    def dump(self, deployment_ids=None, get_broker_conf=None,
+             node_instance_ids=None):
+        """Generate node instances' attributes for a snapshot.
+
+        :param deployment_ids: A list of deployments' identifiers used to
+         select node instances to be dumped, should not be empty.
+        :param get_broker_conf: A function used to retrieve broker
+         configuration.
+        :param node_instance_ids: A list of node instances' identifiers, if
+         not empty, used to select specific node instances to be dumped.
+        :returns: A generator of dictionaries, which describe node instances'
+         attributes.
+        """
+        if not deployment_ids:
+            return
+        for deployment_id in deployment_ids:
+            for entity in utils.get_all(
+                    self.api.get,
+                    f'/{self._uri_prefix}',
+                    params={'deployment_id': deployment_id},
+                    _include=['id', 'runtime_properties', 'state',
+                              'relationships', 'system_properties',
+                              'scaling_groups', 'host_id', 'index',
+                              'visibility', 'node_id', 'created_by',
+                              'has_configuration_drift', 'is_status_check_ok'],
+            ):
+                if get_broker_conf:
+                    # for "agent" node instances, store broker config in
+                    # runtime-props as well, so that during agent upgrade, we
+                    # can connect to the old rabbitmq. This is later analyzed
+                    # by snapshot_restore, _inject_broker_config, and by
+                    # several calls in cloudify-agent/operations.py (related
+                    # to creating the AMQP client there)
+                    rp = entity.get('runtime_properties') or {}
+                    if 'cloudify_agent' in rp:
+                        broker_conf = get_broker_conf(entity)
+                        rp['cloudify_agent'].update(broker_conf)
+                if not node_instance_ids or entity['id'] in node_instance_ids:
+                    yield {'__entity': entity, '__source_id': deployment_id}
+
+    def restore(self, entities, logger, deployment_id,
+                inject_broker_conf=None):
+        """Restore node instances from a snapshot.
+
+        :param entities: An iterable (e.g. a list) of dictionaries describing
+         node instances to be restored.
+        :param logger: A logger instance.
+        :param deployment_id: A deployment identifier for the entities.
+        :param inject_broker_conf: A function used to inject broker
+         configuration for given node_instance's runtime_properties.
+        """
+        for entity in entities:
+            entity['creator'] = entity.pop('created_by')
+            if inject_broker_conf:
+                inject_broker_conf(entity['runtime_properties'])
+        try:
+            self.create_many(deployment_id, entities)
+        except CloudifyClientError as exc:
+            logger.error(f'Error restoring node instances: {exc}')
```

### Comparing `cloudify-common-7.0.0/cloudify_rest_client/nodes.py` & `cloudify-common-7.0.1/cloudify_rest_client/nodes.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,11 @@
-########
-# Copyright (c) 2014 GigaSpaces Technologies Ltd. All rights reserved
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#        http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-#    * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#    * See the License for the specific language governing permissions and
-#    * limitations under the License.
 import warnings
 
+from cloudify_rest_client import utils
+from cloudify_rest_client.exceptions import CloudifyClientError
 from cloudify_rest_client.responses import ListResponse
 
 
 class Node(dict):
     """
     Cloudify node.
     """
@@ -250,37 +238,56 @@
                 _include=_include
             )
         return ListResponse(
             [self._wrapper_cls(item) for item in response['items']],
             response['metadata']
         )
 
-    def get(self, deployment_id, node_id, _include=None,
-            evaluate_functions=False):
+    def get(
+        self,
+        deployment_id,
+        node_id,
+        _include=None,
+        evaluate_functions=False,
+        instance_context=None,
+    ):
         """
         Returns the node which belongs to the deployment identified
         by the provided deployment id .
 
         :param deployment_id: The deployment's id of the node.
         :param node_id: The node id.
         :param _include: List of fields to include in response.
         :param evaluate_functions: Evaluate intrinsic functions
+        :param instance_context: When evaluating functions, do it in context
+            of this node instance id, i.e. get_attribute calls in node
+            properties can be treated as if they were on the node instance
+            with the given id.
         :return: Nodes.
         :rtype: Node
         """
         assert deployment_id
         assert node_id
-        result = self.list(deployment_id=deployment_id,
-                           id=node_id,
-                           _include=_include,
-                           evaluate_functions=evaluate_functions)
-        if not result:
+        params = {
+            'deployment_id': deployment_id,
+            'id': node_id,
+            '_evaluate_functions': evaluate_functions,
+            '_instance_context': instance_context,
+        }
+        if _include:
+            params['_include'] = ','.join(_include)
+        response = self.api.get(
+            '/{self._uri_prefix}'.format(self=self),
+            params=params,
+            _include=_include,
+        )
+        if not response.get('items'):
             return None
-        else:
-            return result[0]
+
+        return self._wrapper_cls(response['items'][0])
 
     def create_many(self, deployment_id, nodes):
         """Create multiple nodes.
 
         :param deployment_id: the new nodes belong to this deployment
         :param nodes: list of dicts representing the nodes to be created.
             Each node dict must contain at least the keys: id, type.
@@ -321,14 +328,58 @@
         """
         self.api.delete(
             '/{self._uri_prefix}/{deployment_id}/{node_id}'
             .format(self=self, deployment_id=deployment_id, node_id=node_id),
             expected_status_code=204,
         )
 
+    def dump(self, deployment_ids=None, node_ids=None):
+        """Generate nodes' attributes for a snapshot.
+
+        :param deployment_ids: A list of deployments' identifiers used to
+         select nodes to be dumped, should not be empty.
+        :param node_ids: A list of nodes' identifiers, if not empty, used to
+         select specific nodes to be dumped.
+        :returns: A generator of dictionaries, which describe nodes'
+         attributes.
+        """
+        if not deployment_ids:
+            return
+        for deployment_id in deployment_ids:
+            for entity in utils.get_all(
+                    self.api.get,
+                    '/nodes',
+                    params={'deployment_id': deployment_id},
+                    _include=['id', 'host_id', 'plugins', 'plugins_to_install',
+                              'properties', 'max_number_of_instances',
+                              'min_number_of_instances',
+                              'planned_number_of_instances',
+                              'deploy_number_of_instances', 'relationships',
+                              'operations', 'type', 'type_hierarchy',
+                              'visibility', 'created_by',
+                              'number_of_instances'],
+            ):
+                if not node_ids or entity['id'] in node_ids:
+                    yield {'__entity': entity, '__source_id': deployment_id}
+
+    def restore(self, entities, logger, deployment_id):
+        """Restore nodes from a snapshot.
+
+        :param entities: An iterable (e.g. a list) of dictionaries describing
+         nodes to be restored.
+        :param logger: A logger instance.
+        :param deployment_id: A deployment identifier for the entities.
+        """
+        for entity in entities:
+            entity['creator'] = entity.pop('created_by')
+        try:
+            self.create_many(deployment_id, entities)
+        except CloudifyClientError as exc:
+            logger.error(f"Error restoring nodes: {exc}")
+
 
 class NodeTypesClient(object):
 
     def __init__(self, api):
         self.api = api
 
     def list(self, node_type=None, constraints=None, **kwargs):
```

### Comparing `cloudify-common-7.0.0/cloudify_rest_client/operations.py` & `cloudify-common-7.0.1/cloudify_rest_client/sites.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,212 +1,177 @@
+from cloudify_rest_client import utils
+from cloudify_rest_client.exceptions import CloudifyClientError
 from cloudify_rest_client.responses import ListResponse
+from cloudify_rest_client.constants import VisibilityState
 
 
-class Operation(dict):
-    def __init__(self, operation):
-        self.update(operation)
+class Site(dict):
 
-    @property
-    def id(self):
-        return self.get('id')
-
-    @property
-    def state(self):
-        return self.get('state')
-
-    @property
-    def created_at(self):
-        return self.get('created_at')
-
-    @property
-    def dependencies(self):
-        return self.get('dependencies')
-
-    @property
-    def type(self):
-        return self.get('type')
-
-    @property
-    def parameters(self):
-        return self.get('parameters', {})
+    def __init__(self, site):
+        super(Site, self).__init__()
+        self.update(site)
 
     @property
     def name(self):
+        """
+        :return: The name of the site.
+        """
         return self.get('name')
 
     @property
-    def containing_subgraph(self):
-        return self.get('parameters', {}).get('containing_subgraph')
+    def location(self):
+        """
+        :return: The location of the site : latitude,longitude.
+        """
+        return self.get('location')
 
     @property
-    def info(self):
-        return self.get('parameters', {}).get('info')
+    def created_at(self):
+        """
+        :return: Site creation date.
+        """
+        return self.get('created_at')
 
     @property
-    def tasks_graph_id(self):
-        return self.get('tasks_graph_id')
+    def visibility(self):
+        """
+        :return: Site visibility.
+        """
+        return self.get('visibility')
 
 
-class OperationsClient(object):
+class SitesClient(object):
+
     def __init__(self, api):
         self.api = api
-        self._uri_prefix = 'operations'
-        self._wrapper_cls = Operation
+        self._uri_prefix = 'sites'
+        self._wrapper_cls = Site
 
-    def list(
-        self,
-        graph_id=None,
-        _offset=None,
-        _size=None,
-        execution_id=None,
-        state=None,
-        skip_internal=False,
-        _include=None,
-    ):
-        """List operations for the given graph or execution.
-
-        :param graph_id: list operations for this graph
-        :param execution_id: list operations for all graphs of this execution.
-            Mutually exclusive with graph_id.
-        :param state: only list operations in this state
-        :param skip_internal: skip "uninteresting" internal operations; this
-            will skip all local tasks and NOP tasks, and only return remote
-            and subgraph tasks
-        :param _offset: pagination offset
-        :param _size: pagination size
-        """
-        params = {}
-        if graph_id and execution_id:
-            raise RuntimeError(
-                'Pass either graph_id or execution_id, not both')
-        if graph_id:
-            params['graph_id'] = graph_id
-        if execution_id:
-            params['execution_id'] = execution_id
-        if state:
-            params['state'] = state
-        if skip_internal:
-            params['skip_internal'] = True
-        if _offset is not None:
-            params['_offset'] = _offset
-        if _size is not None:
-            params['_size'] = _size
-        response = self.api.get('/{self._uri_prefix}'.format(self=self),
-                                params=params, _include=_include)
-        return ListResponse(
-            [self._wrapper_cls(item) for item in response['items']],
-            response['metadata'])
+    def create(self, name, location=None, visibility=VisibilityState.TENANT,
+               created_by=None, created_at=None):
+        """
+        Create a new site.
 
-    def get(self, operation_id):
-        response = self.api.get('/{self._uri_prefix}/{id}'
-                                .format(self=self, id=operation_id))
-        return Operation(response)
+        :param name: The name of the site.
+        :param location: The location of the site : "latitude,longitude".
+        :param visibility: The visibility of the site, can be 'private',
+                           'tenant' or 'global'
+        :param created_by: Override the creator. Internal use only.
+        :param created_at: Override the creation timestamp. Internal use only.
+        :return: The created site.
+        """
+        data = {'visibility': visibility}
+        if location:
+            data['location'] = location
+        if created_by:
+            data['created_by'] = created_by
+        if created_at:
+            data['created_at'] = created_at
+        response = self.api.put(
+            '/{self._uri_prefix}/{name}'.format(self=self, name=name),
+            data=data
+        )
+        return self._wrapper_cls(response)
 
-    def create(self, operation_id, graph_id, name, type, parameters,
-               dependencies):
+    def update(self, name, location=None, visibility=VisibilityState.TENANT,
+               new_name=None):
+        """
+        Update an existing site.
+
+        :param name: The name of the site
+        :param location: The location of the site : "latitude,longitude".
+        :param visibility: The new visibility of the site, can be 'private',
+                           'tenant' or 'global'
+        :param new_name: The new name of the site
+        :return: The created site.
+        """
         data = {
-            'name': name,
-            'graph_id': graph_id,
-            'dependencies': dependencies,
-            'type': type,
-            'parameters': parameters
+            'location': location,
+            'visibility': visibility,
+            'new_name': new_name
         }
-        uri = '/operations/{0}'.format(operation_id)
-        response = self.api.put(uri, data=data, expected_status_code=201)
-        return Operation(response)
-
-    def update(self, operation_id, state, result=None,
-               exception=None, exception_causes=None,
-               manager_name=None, agent_name=None):
-        uri = '/operations/{0}'.format(operation_id)
-        self.api.patch(uri, data={
-            'state': state,
-            'result': result,
-            'exception': exception,
-            'exception_causes': exception_causes,
-            'manager_name': manager_name,
-            'agent_name': agent_name,
-        }, expected_status_code=(
-            200,  # compat with pre-6.2 managers
-            204
-        ))
-
-    def _update_operation_inputs(self, deployment_id=None, node_id=None,
-                                 operation=None, key=None, rel_index=None):
-        """Update stored operations' inputs
-
-        This is internal and is only called in deployment-update, to
-        update stored operations' inputs.
-
-        :param deployment_id: update operations of this deployment
-        :param node_id: update operations of this node
-        :param operation: the operation name
-        :param key: operations/source_operations/target_operations
-        :param rel_index: when updating relationship operations, look at
-            the relationship at this index
-        """
-        self.api.post('/operations', data={
-            'action': 'update-stored',
-            'deployment_id': deployment_id,
-            'node_id': node_id,
-            'operation': operation,
-            'key': key,
-            'rel_index': rel_index,
-        }, expected_status_code=(200, 204))
-
-    def delete(self, operation_id):
-        uri = '/operations/{0}'.format(operation_id)
-        self.api.delete(uri)
-
-
-class TasksGraph(dict):
-    def __init__(self, tasks_graph):
-        self.update(tasks_graph)
+        # Remove the keys with value None
+        data = dict((k, v) for k, v in data.items() if v is not None)
+        response = self.api.post(
+            '/{self._uri_prefix}/{name}'.format(self=self, name=name),
+            data=data
+        )
+        return self._wrapper_cls(response)
 
-    @property
-    def id(self):
-        return self.get('id')
+    def get(self, name):
+        """
+        Get a site from the manager.
 
-    @property
-    def execution(self):
-        return self.get('execution_id')
+        :param name: The name of the site
+        :return: The details of the site
+        """
+        response = self.api.get(
+            '/{self._uri_prefix}/{name}'.format(self=self, name=name)
+        )
+        return self._wrapper_cls(response)
 
-    @property
-    def name(self):
-        return self.get('name')
+    def list(self, _include=None, sort=None, is_descending=False, **kwargs):
+        """
+        Returns a list of currently stored sites.
 
+        :param _include: List of fields to include in response.
+        :param sort: Key for sorting the list.
+        :param is_descending: True for descending order, False for ascending.
+        :param kwargs: Optional filter fields. For a list of available fields
+               see the REST service's models.Site.fields
+        :return: Sites list.
+        """
 
-class TasksGraphClient(object):
-    def __init__(self, api):
-        self.api = api
-        self._uri_prefix = 'tasks_graphs'
-        self._wrapper_cls = TasksGraph
+        if sort:
+            kwargs['_sort'] = '-' + sort if is_descending else sort
 
-    def list(self, execution_id, name=None, _include=None):
-        params = {'execution_id': execution_id}
-        if name:
-            params['name'] = name
         response = self.api.get('/{self._uri_prefix}'.format(self=self),
-                                params=params, _include=_include)
+                                _include=_include,
+                                params=kwargs)
         return ListResponse(
             [self._wrapper_cls(item) for item in response['items']],
-            response['metadata'])
+            response['metadata']
+        )
 
-    def create(self, execution_id, name, operations=None, created_at=None,
-               graph_id=None):
-        params = {
-            'name': name,
-            'execution_id': execution_id,
-            'operations': operations
-        }
-        if created_at:
-            params['created_at'] = created_at
-        if graph_id:
-            params['graph_id'] = graph_id
-        uri = '/{self._uri_prefix}/tasks_graphs'.format(self=self)
-        response = self.api.post(uri, data=params, expected_status_code=201)
-        return TasksGraph(response)
-
-    def update(self, tasks_graph_id, state):
-        uri = '/tasks_graphs/{0}'.format(tasks_graph_id)
-        response = self.api.patch(uri, data={'state': state})
-        return TasksGraph(response)
+    def delete(self, name):
+        """
+        Deletes a site.
+
+        :param name: The name of the site to be deleted.
+        :return: Deleted site.
+        """
+        self.api.delete(
+            '/{self._uri_prefix}/{name}'.format(self=self, name=name)
+        )
+
+    def dump(self, site_ids=None):
+        """Generate sites' attributes for a snapshot.
+
+        :param site_ids: A list of site identifiers, if not empty,
+         used to select specific sites to be dumped.
+        :returns: A generator of dictionaries, which describe sites'
+         attributes.
+        """
+        entities = utils.get_all(
+                self.api.get,
+                f'/{self._uri_prefix}',
+                params={'_get_data': True},
+                _include=['name', 'location', 'visibility', 'created_by',
+                          'created_at']
+        )
+        if not site_ids:
+            return entities
+        return (e for e in entities if e['name'] in site_ids)
+
+    def restore(self, entities, logger):
+        """Restore sites from a snapshot.
+
+        :param entities: An iterable (e.g. a list) of dictionaries describing
+         sites to be restored.
+        :param logger: A logger instance.
+        """
+        for entity in entities:
+            try:
+                self.create(**entity)
+            except CloudifyClientError as exc:
+                logger.error("Error restoring site "
+                             f"{entity['name']}: {exc}")
```

### Comparing `cloudify-common-7.0.0/cloudify_rest_client/plugins.py` & `cloudify-common-7.0.1/cloudify_rest_client/plugins.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import contextlib
 import re
 import tempfile
 from urllib.parse import urlparse
 
-from cloudify_rest_client import bytes_stream_utils
+from cloudify_rest_client import bytes_stream_utils, utils
+from cloudify_rest_client.exceptions import CloudifyClientError
 from cloudify_rest_client.responses import ListResponse
 from cloudify_rest_client.constants import VisibilityState
 
 
 class Plugin(dict):
     """
     Cloudify plugin.
@@ -474,7 +475,50 @@
                                   data={'creator': creator})
         return Plugin(response)
 
     def update(self, plugin_id, **kwargs):
         response = self.api.patch('/plugins/{0}'.format(plugin_id),
                                   data=kwargs)
         return Plugin(response)
+
+    def dump(self, plugin_ids=None):
+        """Generate plugins' attributes for a snapshot.
+
+        :param plugin_ids: A list of plugin identifiers, if not empty,
+         used to select specific plugins to be dumped.
+        :returns: A generator of dictionaries, which describe plugins'
+         attributes.
+        """
+        entities = utils.get_all(
+                self.api.get,
+                '/plugins',
+                params={'_get_data': True},
+                _include=['id', 'title', 'visibility', 'uploaded_at',
+                          'created_by']
+        )
+        if not plugin_ids:
+            return entities
+        return (e for e in entities if e['id'] in plugin_ids)
+
+    def restore(self, entities, logger, path_func=None):
+        """Restore plugins from a snapshot.
+
+        :param entities: An iterable (e.g. a list) of dictionaries describing
+         plugins to be restored.
+        :param logger: A logger instance.
+        :param path_func: A function used retrieve plugin's path.
+        :returns: A generator of dictionaries, which describe additional data
+         used for snapshot restore entities post-processing.
+        """
+        for entity in entities:
+            if path_func:
+                entity['plugin_path'] = path_func(entity['id'])
+            entity['_plugin_id'] = entity.pop('id')
+            entity['_uploaded_at'] = entity.pop('uploaded_at')
+            entity['plugin_title'] = entity.pop('title')
+            entity['_created_by'] = entity.pop('created_by')
+            try:
+                self.upload(**entity)
+                yield {entity['_plugin_id']: entity['plugin_path']}
+            except CloudifyClientError as exc:
+                logger.error("Error restoring plugin "
+                             f"{entity['_plugin_id']}: {exc}")
```

### Comparing `cloudify-common-7.0.0/cloudify_rest_client/resources.py` & `cloudify-common-7.0.1/cloudify_rest_client/resources.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify_rest_client/responses.py` & `cloudify-common-7.0.1/cloudify_rest_client/responses.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify_rest_client/secrets.py` & `cloudify-common-7.0.1/cloudify_rest_client/secrets.py`

 * *Files 3% similar despite different names*

```diff
@@ -269,7 +269,35 @@
         :return: The secret.
         """
         data = {'visibility': visibility}
         return self.api.patch(
             '/secrets/{0}/set-visibility'.format(key),
             data=data
         )
+
+    def dump(self):
+        """Generate secrets' attributes for a snapshot.
+
+        :returns: A generator of dictionaries, which describe secrets'
+         attributes.
+        """
+        return self.export(
+                _include=['key', 'value', 'visibility', 'is_hidden_value',
+                          'encrypted', 'tenant_name', 'creator', 'created_at',
+                          'provider', 'provider_options'],
+                _include_metadata=True,
+        )
+
+    def restore(self, entities, logger):
+        """Restore secrets from a snapshot.
+
+        :param entities: An iterable (e.g. a list) of dictionaries describing
+         secrets to be restored.
+        :param logger: A logger instance.
+        """
+        response = self.import_secrets(secrets_list=entities)
+        collisions = response.get('colliding_secrets')
+        if collisions:
+            logger.warn('The following secrets existed: %s', collisions)
+        errors = response.get('secrets_errors')
+        if errors:
+            yield {'errors': errors}
```

### Comparing `cloudify-common-7.0.0/cloudify_rest_client/secrets_providers.py` & `cloudify-common-7.0.1/cloudify_rest_client/secrets_providers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from cloudify_rest_client import utils
+from cloudify_rest_client.exceptions import CloudifyClientError
 from cloudify_rest_client.responses import ListResponse
 from cloudify_rest_client.constants import VisibilityState
 
 
 class SecretsProvider(dict):
     def __init__(self, secrets_provider):
         super(SecretsProvider, self).__init__()
@@ -216,7 +218,40 @@
         response = self.api.put(
             '/secrets-providers',
             data=data,
             expected_status_code=204,
         )
 
         return response
+
+    def dump(self, secrets_provider_ids=None):
+        """Generate secrets' providers' attributes for a snapshot.
+
+        :param secrets_provider_ids: A list of secrets' provider identifiers,
+         if not empty, used to select specific secrets' providers to be dumped.
+        :returns: A generator of dictionaries, which describe secrets'
+         providers' attributes.
+        """
+        for entity in utils.get_all(
+                self.api.get,
+                '/secrets-providers',
+                _include=['id', 'created_at', 'name', 'visibility', 'type',
+                          'connection_parameters', 'created_by', 'created_at'],
+        ):
+            entity_id = entity.pop('id')
+            if not secrets_provider_ids or entity_id in secrets_provider_ids:
+                yield entity
+
+    def restore(self, entities, logger):
+        """Restore secrets' providers from a snapshot.
+
+        :param entities: An iterable (e.g. a list) of dictionaries describing
+         secrets' providers to be restored.
+        :param logger: A logger instance.
+        """
+        for entity in entities:
+            entity['_type'] = entity.pop('type', None)
+            try:
+                self.create(**entity)
+            except CloudifyClientError as exc:
+                logger.error("Error restoring secrets provider "
+                             f"{entity['id']}: {exc}")
```

### Comparing `cloudify-common-7.0.0/cloudify_rest_client/sites.py` & `cloudify-common-7.0.1/cloudify_rest_client/user_groups.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,157 +1,141 @@
-########
-# Copyright (c) 2013-2019 Cloudify Technologies Ltd. All rights reserved
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#        http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-#    * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#    * See the License for the specific language governing permissions and
-#    * limitations under the License.
-
+from cloudify_rest_client import utils
+from cloudify_rest_client.exceptions import CloudifyClientError
 from cloudify_rest_client.responses import ListResponse
-from cloudify_rest_client.constants import VisibilityState
 
 
-class Site(dict):
+class Group(dict):
 
-    def __init__(self, site):
-        super(Site, self).__init__()
-        self.update(site)
+    def __init__(self, group):
+        super(Group, self).__init__()
+        self.update(group)
 
     @property
     def name(self):
         """
-        :return: The name of the site.
+        :return: The name of the group.
         """
         return self.get('name')
 
     @property
-    def location(self):
+    def users(self):
         """
-        :return: The location of the site : latitude,longitude.
+        :return: The list of users connected to the group.
         """
-        return self.get('location')
+        return self.get('users')
 
     @property
-    def created_at(self):
+    def role(self):
         """
-        :return: Site creation date.
+        :return: The role of the group.
         """
-        return self.get('created_at')
+        return self.get('role')
 
     @property
-    def visibility(self):
+    def tenants(self):
         """
-        :return: Site visibility.
+        :return: The list of tenants to which the group is connected.
         """
-        return self.get('visibility')
-
-
-class SitesClient(object):
-
-    def __init__(self, api):
-        self.api = api
-        self._uri_prefix = 'sites'
-        self._wrapper_cls = Site
+        return self.get('tenants')
 
-    def create(self, name, location=None, visibility=VisibilityState.TENANT,
-               created_by=None, created_at=None):
+    @property
+    def ldap_dn(self):
         """
-        Create a new site.
-
-        :param name: The name of the site.
-        :param location: The location of the site : "latitude,longitude".
-        :param visibility: The visibility of the site, can be 'private',
-                           'tenant' or 'global'
-        :param created_by: Override the creator. Internal use only.
-        :param created_at: Override the creation timestamp. Internal use only.
-        :return: The created site.
-        """
-        data = {'visibility': visibility}
-        if location:
-            data['location'] = location
-        if created_by:
-            data['created_by'] = created_by
-        if created_at:
-            data['created_at'] = created_at
-        response = self.api.put(
-            '/{self._uri_prefix}/{name}'.format(self=self, name=name),
-            data=data
-        )
-        return self._wrapper_cls(response)
-
-    def update(self, name, location=None, visibility=VisibilityState.TENANT,
-               new_name=None):
+        :return: If using ldap, will return the group's distinguished name.
         """
-        Update an existing site.
+        return self.get('ldap_dn')
 
-        :param name: The name of the site
-        :param location: The location of the site : "latitude,longitude".
-        :param visibility: The new visibility of the site, can be 'private',
-                           'tenant' or 'global'
-        :param new_name: The new name of the site
-        :return: The created site.
-        """
-        data = {
-            'location': location,
-            'visibility': visibility,
-            'new_name': new_name
-        }
-        # Remove the keys with value None
-        data = dict((k, v) for k, v in data.items() if v is not None)
-        response = self.api.post(
-            '/{self._uri_prefix}/{name}'.format(self=self, name=name),
-            data=data
-        )
-        return self._wrapper_cls(response)
 
-    def get(self, name):
-        """
-        Get a site from the manager.
+class UserGroupsClient(object):
 
-        :param name: The name of the site
-        :return: The details of the site
-        """
-        response = self.api.get(
-            '/{self._uri_prefix}/{name}'.format(self=self, name=name)
-        )
-        return self._wrapper_cls(response)
+    def __init__(self, api):
+        self.api = api
 
     def list(self, _include=None, sort=None, is_descending=False, **kwargs):
         """
-        Returns a list of currently stored sites.
+        Returns a list of currently stored user groups.
 
         :param _include: List of fields to include in response.
         :param sort: Key for sorting the list.
         :param is_descending: True for descending order, False for ascending.
         :param kwargs: Optional filter fields. For a list of available fields
-               see the REST service's models.Site.fields
-        :return: Sites list.
+               see the REST service's models.BlueprintState.fields
+        :return: Blueprints list.
         """
-
+        params = kwargs
         if sort:
-            kwargs['_sort'] = '-' + sort if is_descending else sort
+            params['_sort'] = '-' + sort if is_descending else sort
 
-        response = self.api.get('/{self._uri_prefix}'.format(self=self),
+        response = self.api.get('/user-groups',
                                 _include=_include,
-                                params=kwargs)
-        return ListResponse(
-            [self._wrapper_cls(item) for item in response['items']],
-            response['metadata']
+                                params=params)
+        return ListResponse([Group(item) for item in response['items']],
+                            response['metadata'])
+
+    def create(self, group_name, role, ldap_group_dn=None):
+        data = {
+            'group_name': group_name,
+            'ldap_group_dn': ldap_group_dn,
+            'role': role
+        }
+        response = self.api.post('/user-groups',
+                                 data=data,
+                                 expected_status_code=201)
+        return Group(response)
+
+    def get(self, group_name, **kwargs):
+        response = self.api.get(
+            '/user-groups/{0}'.format(group_name),
+            params=kwargs
         )
+        return Group(response)
 
-    def delete(self, name):
-        """
-        Deletes a site.
+    def delete(self, group_name):
+        self.api.delete('/user-groups/{0}'.format(group_name))
 
-        :param name: The name of the site to be deleted.
-        :return: Deleted site.
-        """
-        self.api.delete(
-            '/{self._uri_prefix}/{name}'.format(self=self, name=name)
+    def set_role(self, group_name, new_role):
+        data = {'role': new_role}
+        response = self.api.post('/user-groups/{0}'.format(group_name),
+                                 data=data)
+        return Group(response)
+
+    def add_user(self, username, group_name):
+        data = {'username': username, 'group_name': group_name}
+        response = self.api.put('/user-groups/users', data=data)
+        return Group(response)
+
+    def remove_user(self, username, group_name):
+        data = {'username': username, 'group_name': group_name}
+        self.api.delete('/user-groups/users', data=data)
+
+    def dump(self):
+        """Generate user groups' attributes for a snapshot.
+
+        :returns: A generator of dictionaries, which describe user groups'
+         attributes.
+        """
+        return utils.get_all(
+                self.api.get,
+                '/user-groups',
+                params={'_get_data': True},
+                _include=['name', 'ldap_dn', 'tenants', 'role']
         )
+
+    def restore(self, entities, logger):
+        """Restore user_groups from a snapshot.
+
+        :param entities: An iterable (e.g. a list) of dictionaries describing
+         user_groups to be restored.
+        :param logger: A logger instance.
+        :returns: A generator of dictionaries, which describe additional data
+         used for snapshot restore entities post-processing.
+        """
+        for entity in entities:
+            entity['group_name'] = entity.pop('name')
+            entity['ldap_group_dn'] = entity.pop('ldap_dn')
+            group_tenants = entity.pop('tenants')
+            try:
+                self.create(**entity)
+                yield {entity['group_name']: group_tenants}
+            except CloudifyClientError as exc:
+                logger.error("Error restoring user group "
+                             f"{entity['group_name']}: {exc}")
```

### Comparing `cloudify-common-7.0.0/cloudify_rest_client/snapshots.py` & `cloudify-common-7.0.1/cloudify_rest_client/snapshots.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify_rest_client/summary.py` & `cloudify-common-7.0.1/cloudify_rest_client/summary.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify_rest_client/tenants.py` & `cloudify-common-7.0.1/cloudify_rest_client/tenants.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,9 @@
-########
-# Copyright (c) 2014 GigaSpaces Technologies Ltd. All rights reserved
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#        http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-#    * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#    * See the License for the specific language governing permissions and
-#    * limitations under the License.
-
+from cloudify_rest_client import utils
+from cloudify_rest_client.exceptions import CloudifyClientError
 from cloudify_rest_client.responses import ListResponse
 
 DEFAULT_TENANT_ROLE = 'user'
 
 
 class Tenant(dict):
 
@@ -208,7 +195,40 @@
             '/tenants/{0}'.format(tenant_name),
             params=kwargs
         )
         return Tenant(response)
 
     def delete(self, tenant_name):
         self.api.delete('/tenants/{0}'.format(tenant_name))
+
+    def dump(self):
+        """Generate tenants' attributes for a snapshot.
+
+        :returns: A generator of dictionaries, which describe tenants'
+         attributes.
+        """
+        return utils.get_all(
+                self.api.get,
+                '/tenants',
+                _include=['name', 'rabbitmq_password'],
+        )
+
+    def restore(self, entities, logger):
+        """Restore tenants from a snapshot.
+
+        :param entities: An iterable (e.g. a list) of dictionaries describing
+         tenants to be restored.
+        :param logger: A logger instance.
+        :returns: A generator of dictionaries, which describe additional data
+         used for snapshot restore entities post-processing.
+        """
+        for entity in entities:
+            if entity['name'] == 'default_tenant':
+                if logger:
+                    logger.debug('Skipping creation of default tenant')
+                continue
+            entity['tenant_name'] = entity.pop('name')
+            try:
+                self.create(**entity)
+            except CloudifyClientError as exc:
+                logger.error("Error restoring tenant "
+                             f"{entity['tenant_name']}: {exc}")
```

### Comparing `cloudify-common-7.0.0/cloudify_rest_client/tokens.py` & `cloudify-common-7.0.1/cloudify_rest_client/tokens.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/cloudify_rest_client/users.py` & `cloudify-common-7.0.1/cloudify_rest_client/users.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from cloudify_rest_client import utils
+from cloudify_rest_client.exceptions import CloudifyClientError
 from cloudify_rest_client.responses import ListResponse
 
 
 class User(dict):
 
     def __init__(self, user):
         super(User, self).__init__()
@@ -178,7 +180,45 @@
 
     def unlock(self, username, **kwargs):
         response = self.api.post(
             '/users/unlock/{0}'.format(username),
             params=kwargs
         )
         return User(response)
+
+    def dump(self):
+        """Generate users' attributes for a snapshot.
+
+        :returns: A generator of dictionaries, which describe users'
+         attributes.
+        """
+        return utils.get_all(
+                self.api.get,
+                '/users',
+                params={'_get_data': True, '_include_hash': True},
+                _include=['username', 'role', 'tenant_roles',
+                          'first_login_at', 'last_login_at', 'created_at'],
+        )
+
+    def restore(self, entities, logger):
+        """Restore users from a snapshot.
+
+        :param entities: An iterable (e.g. a list) of dictionaries describing
+         users to be restored.
+        :param logger: A logger instance.
+        :returns: A generator of dictionaries, which describe additional data
+         used for snapshot restore entities post-processing.
+        """
+        for entity in entities:
+            if entity['username'] == 'admin':
+                if logger:
+                    logger.debug('Skipping creation of admin user')
+                continue
+            entity['password'] = entity.pop('password_hash')
+            entity['is_prehashed'] = True
+            tenant_roles = entity.pop('tenant_roles')
+            try:
+                self.create(**entity)
+                yield {entity['username']: tenant_roles}
+            except CloudifyClientError as exc:
+                logger.error("Error restoring user "
+                             f"{entity['username']}: {exc}")
```

### Comparing `cloudify-common-7.0.0/cloudify_rest_client/utils.py` & `cloudify-common-7.0.1/cloudify_rest_client/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     app_name = os.path.basename(os.path.splitext(blueprint_path)[0])
     blueprint_directory = os.path.dirname(blueprint_path) or os.getcwd()
     return tar_file(blueprint_directory, dest_dir, app_name)
 
 
 def tar_file(file_to_tar, destination_dir, tar_name=''):
     """
-    tar a file into a desintation dir.
+    tar a file into a destination dir.
     :param file_to_tar:
     :param destination_dir:
     :param tar_name: optional tar name.
     :return:
     """
     def _reset_tarinfo(tarinfo):
         """Set all tar'd files to be world-readable, so that other services
@@ -104,14 +104,31 @@
                 # the file exists, we have a shot at spawn working
                 return f
         return None
     else:
         return executable
 
 
+def get_all(method, *args, **kwargs):
+    """Generator of entities retrieved by a method called with args/kwargs."""
+    include = kwargs.get('_include')
+    if kwargs.get('params', {}).get('_include_hash'):
+        include.append('password_hash')
+    more_data = True
+    entities_yielded = 0
+    while more_data:
+        result = method(*args, **kwargs)
+        for item in result['items']:
+            yield {k: v for k, v in item.items()
+                   if include is None or k in include}
+            entities_yielded += 1
+        more_data = \
+            (entities_yielded < result['metadata']['pagination']['total'])
+
+
 class StreamedResponse(object):
 
     def __init__(self, response):
         self._response = response
 
     @property
     def headers(self):
```

### Comparing `cloudify-common-7.0.0/cloudify_rest_client/workflows.py` & `cloudify-common-7.0.1/cloudify_rest_client/workflows.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/dsl_parser/__init__.py` & `cloudify-common-7.0.1/dsl_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/dsl_parser/constants.py` & `cloudify-common-7.0.1/dsl_parser/constants.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/dsl_parser/constraints.py` & `cloudify-common-7.0.1/dsl_parser/constraints.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/dsl_parser/elements/__init__.py` & `cloudify-common-7.0.1/dsl_parser/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/dsl_parser/elements/blueprint.py` & `cloudify-common-7.0.1/dsl_parser/elements/blueprint.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/dsl_parser/elements/data_types.py` & `cloudify-common-7.0.1/dsl_parser/elements/data_types.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/dsl_parser/elements/deployment_schedules.py` & `cloudify-common-7.0.1/dsl_parser/elements/deployment_schedules.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/dsl_parser/elements/imports.py` & `cloudify-common-7.0.1/dsl_parser/elements/imports.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/dsl_parser/elements/inputs.py` & `cloudify-common-7.0.1/dsl_parser/elements/inputs.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/dsl_parser/elements/misc.py` & `cloudify-common-7.0.1/dsl_parser/elements/misc.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/dsl_parser/elements/node_templates.py` & `cloudify-common-7.0.1/dsl_parser/elements/node_templates.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/dsl_parser/elements/node_types.py` & `cloudify-common-7.0.1/dsl_parser/elements/node_types.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/dsl_parser/elements/operation.py` & `cloudify-common-7.0.1/dsl_parser/elements/operation.py`

 * *Files 6% similar despite different names*

```diff
@@ -441,36 +441,10 @@
 def _is_inline_script(script):
     """Check if the string `script` contains a script.
 
     The string, which is coming from an operation mapping in the blueprint,
     can contain either an operation dotted import path, or a script written
     right there in the blueprint.
     """
-    script = script.strip()
-    if script.count('\n') > 1:
-        # multiple lines? this for sure isn't a dotted path
-        return True
-
-    if utils.NAMESPACE_DELIMITER in script:
-        ns, _, _rest = script.partition(utils.NAMESPACE_DELIMITER)
-        if ns.isidentifier():
-            # a namespace delimiter, separating a single identifier? this
-            # for sure is not a script!
-            return False
-
-    if '/' in script or '\\' in script:
-        # script is one line and contains a slash/backslash - interpret
-        # this as a path (posix or windows).
-        # This means it's impossible to have 1-line scripts containing
-        # slashes, but this stays backwards-compatible
-        return False
-
-    if (
-        '.' in script and
-        all(part.isidentifier() for part in script.split('.'))
-    ):
-        # this looks like a dotted path - identifiers separated by dots
-        return False
-
-    # it doesn't look like a file path, or a dotted path - it must be a
-    # one-liner script!
-    return True
+    # a very simple heuristic: if it's multiple lines, then it's an inline
+    # script. Otherwise it's a filename or a plugin path.
+    return '\n' in script.strip()
```

### Comparing `cloudify-common-7.0.0/dsl_parser/elements/plugins.py` & `cloudify-common-7.0.1/dsl_parser/elements/plugins.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/dsl_parser/elements/policies.py` & `cloudify-common-7.0.1/dsl_parser/elements/policies.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/dsl_parser/elements/relationships.py` & `cloudify-common-7.0.1/dsl_parser/elements/relationships.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/dsl_parser/elements/scalable.py` & `cloudify-common-7.0.1/dsl_parser/elements/scalable.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/dsl_parser/elements/types.py` & `cloudify-common-7.0.1/dsl_parser/elements/types.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/dsl_parser/elements/version.py` & `cloudify-common-7.0.1/dsl_parser/elements/version.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/dsl_parser/elements/workflows.py` & `cloudify-common-7.0.1/dsl_parser/elements/workflows.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/dsl_parser/exceptions.py` & `cloudify-common-7.0.1/dsl_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/dsl_parser/framework/__init__.py` & `cloudify-common-7.0.1/dsl_parser/framework/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/dsl_parser/framework/elements.py` & `cloudify-common-7.0.1/dsl_parser/framework/elements.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/dsl_parser/framework/parser.py` & `cloudify-common-7.0.1/dsl_parser/framework/parser.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/dsl_parser/framework/requirements.py` & `cloudify-common-7.0.1/dsl_parser/framework/requirements.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/dsl_parser/functions.py` & `cloudify-common-7.0.1/dsl_parser/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -459,15 +459,20 @@
         self.attribute_path = args[1:]
 
     def validate(self, plan):
         _validate_no_functions_in_args(self.node_name, self.attribute_path,
                                        self.path, self.name, self.scope, plan)
 
     def evaluate(self, handler):
-        if self.node_name in [SELF, SOURCE, TARGET]:
+        if 'instance_id_hint' in self.context:
+            # we're evaluating a node in the context of a specific instance,
+            # and we were told exactly which instance is it
+            node_instance = handler.get_node_instance(
+                self.context['instance_id_hint'])
+        elif self.node_name in [SELF, SOURCE, TARGET]:
             node_instance_id = self._resolve_available_node_targets(handler)
             _validate_ref(node_instance_id, self.node_name, self.name,
                           self.path, self.attribute_path)
             node_instance = handler.get_node_instance(node_instance_id)
         else:
             try:
                 node_instance = self._resolve_node_instance_by_name(handler)
@@ -1372,16 +1377,22 @@
                     context=context,
                     path=path,
                     raw=raw_function,
                     return_type=return_type)
     return raw_function
 
 
-def evaluate_node_functions(node, storage):
+def evaluate_node_functions(node, storage, instance_context=None):
     handler = runtime_evaluation_handler(storage)
+    if instance_context:
+        # instance_context means we're evaluating node functions in the
+        # context of a specific node instance - the ID of that instance is
+        # given as this "context". Let's pass it through to the functions,
+        # so that e.g. get_attribute can decide which instance to use.
+        node['instance_id_hint'] = instance_context
     scan.scan_node_template(node, handler, replace=True)
     return node
 
 
 def evaluate_node_instance_functions(instance, storage):
     handler = runtime_evaluation_handler(storage)
     scan.scan_properties(
```

### Comparing `cloudify-common-7.0.0/dsl_parser/holder.py` & `cloudify-common-7.0.1/dsl_parser/holder.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/dsl_parser/import_resolver/__init__.py` & `cloudify-common-7.0.1/dsl_parser/import_resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/dsl_parser/import_resolver/abstract_import_resolver.py` & `cloudify-common-7.0.1/dsl_parser/import_resolver/abstract_import_resolver.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/dsl_parser/import_resolver/default_import_resolver.py` & `cloudify-common-7.0.1/dsl_parser/import_resolver/default_import_resolver.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/dsl_parser/interfaces/constants.py` & `cloudify-common-7.0.1/dsl_parser/interfaces/constants.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/dsl_parser/interfaces/interfaces_merger.py` & `cloudify-common-7.0.1/dsl_parser/interfaces/interfaces_merger.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/dsl_parser/interfaces/interfaces_parser.py` & `cloudify-common-7.0.1/dsl_parser/interfaces/interfaces_parser.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/dsl_parser/interfaces/operation_merger.py` & `cloudify-common-7.0.1/dsl_parser/interfaces/operation_merger.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/dsl_parser/interfaces/utils.py` & `cloudify-common-7.0.1/dsl_parser/interfaces/utils.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/dsl_parser/models.py` & `cloudify-common-7.0.1/dsl_parser/models.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/dsl_parser/multi_instance.py` & `cloudify-common-7.0.1/dsl_parser/multi_instance.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/dsl_parser/parser.py` & `cloudify-common-7.0.1/dsl_parser/parser.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/dsl_parser/rel_graph.py` & `cloudify-common-7.0.1/dsl_parser/rel_graph.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/dsl_parser/scan.py` & `cloudify-common-7.0.1/dsl_parser/scan.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/dsl_parser/tasks.py` & `cloudify-common-7.0.1/dsl_parser/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,27 +212,32 @@
             'target_deployment': idd_spec.target_deployment,
         }
 
         if idd_spec.scope == 'node_template':
             # the IDDSpec is a node one (e.g. in node properties):
             # create an instance of IDD, for every node-instance of the node
             node_name = idd_spec.context['node_name']
+            if not nis_by_node.get(node_name):
+                # node with 0 instances - nothing to do
+                continue
             for ni in nis_by_node[node_name]:
                 idd = idd_base.copy()
                 idd['context'] = {
                     'self': ni['id'],
                 }
                 idds.append(idd)
 
         elif idd_spec.scope == 'node_template_relationship':
             # the IDDSpec is a relationship one (e.g. in relationship operation
             # inputs) - create an instance of IDD for every node-instance of
             # the source node
             node_name = idd_spec.context['source_node_name']
-
+            if not nis_by_node.get(node_name):
+                # node with 0 instances - nothing to do
+                continue
             for ni in nis_by_node[node_name]:
                 target_id = _find_rel_target_by_iddspec(
                     ni.get('relationships', []),
                     idd_spec,
                 )
                 idd = idd_base.copy()
                 idd['context'] = {
```

### Comparing `cloudify-common-7.0.0/dsl_parser/utils.py` & `cloudify-common-7.0.1/dsl_parser/utils.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/dsl_parser/version.py` & `cloudify-common-7.0.1/dsl_parser/version.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/dsl_parser/yaml_loader.py` & `cloudify-common-7.0.1/dsl_parser/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/script_runner/__init__.py` & `cloudify-common-7.0.1/script_runner/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/script_runner/eval_env.py` & `cloudify-common-7.0.1/script_runner/eval_env.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/script_runner/tasks.py` & `cloudify-common-7.0.1/script_runner/tasks.py`

 * *Files identical despite different names*

### Comparing `cloudify-common-7.0.0/setup.py` & `cloudify-common-7.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cloudify-common',
-    version='7.0.0',
+    version='7.0.1',
     author='Cloudify',
     author_email='cosmo-admin@cloudify.co',
     packages=find_packages(exclude=('cloudify.tests*',
                                     'cloudify_rest_client.tests*',
                                     'dsl_parser.tests*',
                                     'script_runner.tests*',)),
     include_package_data=True,
```

